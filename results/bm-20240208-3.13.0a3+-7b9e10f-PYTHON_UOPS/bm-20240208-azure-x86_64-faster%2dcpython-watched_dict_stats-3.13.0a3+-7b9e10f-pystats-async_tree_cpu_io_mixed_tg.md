
# Pystats results

- benchmark: async_tree_cpu_io_mixed_tg
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 397,705,080 | 19.7% | 19.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 126,218,460 | 6.3% | 26.0% |  |
| POP_JUMP_IF_FALSE | 112,113,500 | 5.6% | 31.5% |  |
| RESUME_CHECK | 107,990,220 | 5.4% | 36.9% | 0.0% |
| LOAD_FAST_LOAD_FAST | 96,951,300 | 4.8% | 41.7% |  |
| POP_TOP | 90,941,420 | 4.5% | 46.2% |  |
| LOAD_CONST | 86,489,260 | 4.3% | 50.5% |  |
| STORE_ATTR_SLOT | 71,764,340 | 3.6% | 54.1% | 3.5% |
| STORE_FAST | 66,549,820 | 3.3% | 57.4% |  |
| TO_BOOL_BOOL | 64,643,280 | 3.2% | 60.6% | 0.0% |
| RETURN_VALUE | 60,911,540 | 3.0% | 63.6% |  |
| RETURN_CONST | 55,279,340 | 2.7% | 66.3% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 49,870,140 | 2.5% | 68.8% |  |
| LOAD_GLOBAL_MODULE | 48,968,400 | 2.4% | 71.2% |  |
| INTERPRETER_EXIT | 48,196,060 | 2.4% | 73.6% |  |
| CALL_PY_EXACT_ARGS | 45,215,940 | 2.2% | 75.9% |  |
| CALL | 38,673,120 | 1.9% | 77.8% |  |
| LOAD_ATTR_SLOT | 36,319,240 | 1.8% | 79.6% | 1.0% |
| PUSH_NULL | 33,480,200 | 1.7% | 81.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 31,744,900 | 1.6% | 82.8% | 0.0% |
| LOAD_ATTR | 31,017,120 | 1.5% | 84.4% |  |
| POP_JUMP_IF_NOT_NONE | 28,008,680 | 1.4% | 85.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 27,809,840 | 1.4% | 87.1% | 0.0% |
| LOAD_ATTR_MODULE | 26,530,820 | 1.3% | 88.5% |  |
| TO_BOOL_NONE | 24,836,040 | 1.2% | 89.7% | 0.0% |
| ENTER_EXECUTOR | 14,677,460 | 0.7% | 90.4% |  |
| POP_JUMP_IF_NONE | 13,437,680 | 0.7% | 91.1% |  |
| COMPARE_OP_INT | 12,366,200 | 0.6% | 91.7% |  |
| RETURN_GENERATOR | 11,951,360 | 0.6% | 92.3% |  |
| STORE_ATTR_INSTANCE_VALUE | 11,946,640 | 0.6% | 92.9% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 11,764,760 | 0.6% | 93.5% | 0.0% |
| TO_BOOL | 11,205,700 | 0.6% | 94.0% |  |
| CALL_FUNCTION_EX | 10,272,360 | 0.5% | 94.5% |  |
| POP_JUMP_IF_TRUE | 10,087,300 | 0.5% | 95.0% |  |
| CALL_BUILTIN_O | 9,937,060 | 0.5% | 95.5% |  |
| CALL_KW | 9,893,720 | 0.5% | 96.0% |  |
| SEND_GEN | 8,975,840 | 0.4% | 96.5% |  |
| END_SEND | 8,408,120 | 0.4% | 96.9% |  |
| GET_AWAITABLE | 8,408,120 | 0.4% | 97.3% |  |
| COMPARE_OP_FLOAT | 5,813,920 | 0.3% | 97.6% |  |
| TO_BOOL_LIST | 5,229,600 | 0.3% | 97.8% |  |
| JUMP_FORWARD | 4,483,220 | 0.2% | 98.1% |  |
| LOAD_GLOBAL_BUILTIN | 3,962,420 | 0.2% | 98.3% | 0.0% |
| BINARY_OP_ADD_INT | 3,736,660 | 0.2% | 98.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 2,629,160 | 0.1% | 98.6% | 28.9% |
| BINARY_OP_SUBTRACT_INT | 2,615,100 | 0.1% | 98.7% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 2,439,320 | 0.1% | 98.8% |  |
| YIELD_VALUE | 2,439,320 | 0.1% | 98.9% |  |
| CALL_ISINSTANCE | 2,081,380 | 0.1% | 99.0% |  |
| CALL_PY_WITH_DEFAULTS | 2,057,900 | 0.1% | 99.2% |  |
| SEND | 1,872,600 | 0.1% | 99.2% |  |
| LOAD_ATTR_CLASS | 1,868,440 | 0.1% | 99.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,681,060 | 0.1% | 99.4% |  |
| FOR_ITER_RANGE | 1,497,160 | 0.1% | 99.5% |  |
| CALL_BUILTIN_CLASS | 1,495,460 | 0.1% | 99.6% |  |
| NOP | 1,130,440 | 0.1% | 99.6% |  |
| BUILD_LIST | 1,129,160 | 0.1% | 99.7% |  |
| GET_ITER | 752,260 | 0.0% | 99.7% |  |
| BEFORE_ASYNC_WITH | 746,480 | 0.0% | 99.8% |  |
| EXIT_INIT_CHECK | 746,460 | 0.0% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 746,460 | 0.0% | 99.8% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 746,460 | 0.0% | 99.9% |  |
| CALL_INTRINSIC_1 | 380,600 | 0.0% | 99.9% |  |
| LIST_EXTEND | 380,600 | 0.0% | 99.9% |  |
| LOAD_DEREF | 379,700 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 379,540 | 0.0% | 99.9% |  |
| LOAD_SUPER_ATTR_METHOD | 379,060 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 191,040 | 0.0% | 100.0% |  |
| COMPARE_OP | 190,340 | 0.0% | 100.0% |  |
| BUILD_MAP | 189,640 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 189,460 | 0.0% | 100.0% |  |
| CALL_LEN | 5,460 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,820 | 0.0% | 100.0% |  |
| STORE_ATTR | 3,700 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 3,700 | 0.0% | 100.0% |  |
| COPY | 2,580 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 2,200 | 0.0% | 100.0% |  |
| RESUME | 2,080 | 0.0% | 100.0% | 1,361.5% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 2,020 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 1,840 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 1,720 | 0.0% | 100.0% |  |
| BINARY_OP | 1,160 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 640 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 600 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 121,737,160 | 6.0% | 6.0% |
| RESUME_CHECK LOAD_FAST | 82,912,820 | 4.1% | 10.2% |
| POP_JUMP_IF_FALSE LOAD_FAST | 78,948,000 | 3.9% | 14.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 59,038,780 | 2.9% | 17.0% |
| STORE_FAST LOAD_FAST | 44,834,960 | 2.2% | 19.2% |
| CACHE RESUME_CHECK | 42,034,380 | 2.1% | 21.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 40,520,880 | 2.0% | 23.3% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 39,767,520 | 2.0% | 25.3% |
| LOAD_CONST LOAD_FAST | 39,600,940 | 2.0% | 27.2% |
| POP_TOP LOAD_FAST | 39,021,280 | 1.9% | 29.2% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 38,489,300 | 1.9% | 31.1% |
| LOAD_FAST LOAD_ATTR_SLOT | 36,122,320 | 1.8% | 32.9% |
| LOAD_FAST RETURN_VALUE | 33,519,620 | 1.7% | 34.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 32,311,440 | 1.6% | 36.2% |
| LOAD_FAST STORE_ATTR_SLOT | 31,195,800 | 1.5% | 37.7% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 30,248,820 | 1.5% | 39.2% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 29,883,560 | 1.5% | 40.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 29,494,980 | 1.5% | 42.1% |
| LOAD_FAST LOAD_ATTR | 29,317,740 | 1.5% | 43.6% |
| RETURN_CONST INTERPRETER_EXIT | 28,188,720 | 1.4% | 45.0% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 27,809,820 | 1.4% | 46.4% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 26,529,680 | 1.3% | 47.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 26,340,920 | 1.3% | 49.0% |
| RETURN_CONST POP_TOP | 25,408,200 | 1.3% | 50.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 25,011,780 | 1.2% | 51.5% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 24,836,020 | 1.2% | 52.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 23,330,640 | 1.2% | 53.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 21,289,920 | 1.1% | 54.9% |
| STORE_ATTR_SLOT LOAD_CONST | 20,544,540 | 1.0% | 56.0% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 20,354,800 | 1.0% | 57.0% |
| CALL STORE_FAST | 19,420,080 | 1.0% | 57.9% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 18,679,140 | 0.9% | 58.9% |
| RETURN_VALUE INTERPRETER_EXIT | 17,578,660 | 0.9% | 59.7% |
| RETURN_VALUE STORE_FAST | 16,621,880 | 0.8% | 60.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 16,240,780 | 0.8% | 61.4% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 15,687,300 | 0.8% | 62.1% |
| POP_JUMP_IF_FALSE RETURN_CONST | 15,498,180 | 0.8% | 62.9% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 14,751,480 | 0.7% | 63.6% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 14,562,080 | 0.7% | 64.4% |
| POP_TOP ENTER_EXECUTOR | 14,561,080 | 0.7% | 65.1% |
| POP_TOP RETURN_CONST | 14,005,760 | 0.7% | 65.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 13,824,120 | 0.7% | 66.5% |
| POP_JUMP_IF_NONE LOAD_FAST | 12,690,400 | 0.6% | 67.1% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 12,366,200 | 0.6% | 67.7% |
| POP_TOP RESUME_CHECK | 11,951,180 | 0.6% | 68.3% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 11,945,020 | 0.6% | 68.9% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL | 11,199,400 | 0.6% | 69.5% |
| POP_TOP LOAD_CONST | 11,021,180 | 0.5% | 70.0% |
| LOAD_CONST STORE_FAST | 10,838,640 | 0.5% | 70.5% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 10,826,240 | 0.5% | 71.1% |
| STORE_ATTR_SLOT LOAD_FAST | 10,462,060 | 0.5% | 71.6% |
| STORE_ATTR_SLOT RETURN_CONST | 10,461,600 | 0.5% | 72.1% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_WITH_VALUES | 10,461,400 | 0.5% | 72.6% |
| POP_JUMP_IF_FALSE LOAD_CONST | 10,278,000 | 0.5% | 73.1% |
| RETURN_VALUE TO_BOOL_BOOL | 10,272,680 | 0.5% | 73.6% |
| LOAD_FAST LOAD_CONST | 10,089,740 | 0.5% | 74.1% |
| STORE_FAST RETURN_CONST | 10,084,720 | 0.5% | 74.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 10,083,360 | 0.5% | 75.1% |
| LOAD_FAST_LOAD_FAST CALL | 10,083,080 | 0.5% | 75.6% |
| CALL_FUNCTION_EX POP_TOP | 10,083,040 | 0.5% | 76.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 9,893,900 | 0.5% | 76.6% |
| LOAD_CONST CALL_KW | 9,893,720 | 0.5% | 77.1% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 9,893,640 | 0.5% | 77.6% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 9,893,440 | 0.5% | 78.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 9,893,400 | 0.5% | 78.6% |
| ENTER_EXECUTOR CALL_FUNCTION_EX | 9,891,520 | 0.5% | 79.1% |
| PUSH_NULL CALL | 9,528,820 | 0.5% | 79.6% |
| LOAD_ATTR CALL | 8,959,720 | 0.4% | 80.0% |
| GET_AWAITABLE LOAD_CONST | 8,408,120 | 0.4% | 80.4% |
| LOAD_CONST COMPARE_OP_INT | 8,217,720 | 0.4% | 80.8% |
| LOAD_FAST POP_JUMP_IF_NONE | 8,211,840 | 0.4% | 81.2% |
| LOAD_FAST CALL_BUILTIN_O | 8,072,260 | 0.4% | 81.6% |
| CALL_BUILTIN_O STORE_FAST | 7,883,580 | 0.4% | 82.0% |
| SEND_GEN POP_TOP | 7,472,240 | 0.4% | 82.4% |
| LOAD_CONST SEND_GEN | 7,472,120 | 0.4% | 82.8% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_MODULE | 7,283,280 | 0.4% | 83.1% |
| LOAD_FAST PUSH_NULL | 6,757,640 | 0.3% | 83.5% |
| TO_BOOL POP_JUMP_IF_FALSE | 6,719,500 | 0.3% | 83.8% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NOT_NONE | 6,718,340 | 0.3% | 84.1% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 6,536,780 | 0.3% | 84.5% |
| RETURN_VALUE END_SEND | 6,536,520 | 0.3% | 84.8% |
| RETURN_GENERATOR GET_AWAITABLE | 5,979,440 | 0.3% | 85.1% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 5,605,940 | 0.3% | 85.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 5,605,420 | 0.3% | 85.6% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 5,604,440 | 0.3% | 85.9% |
| END_SEND POP_TOP | 5,604,080 | 0.3% | 86.2% |
| CALL POP_TOP | 5,415,400 | 0.3% | 86.5% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 5,236,280 | 0.3% | 86.7% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 5,229,600 | 0.3% | 87.0% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_LIST | 5,229,500 | 0.3% | 87.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 5,227,400 | 0.3% | 87.5% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 5,226,060 | 0.3% | 87.8% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 5,225,580 | 0.3% | 88.0% |
| PUSH_NULL LOAD_FAST | 4,720,740 | 0.2% | 88.3% |
| LOAD_ATTR LOAD_FAST | 4,669,380 | 0.2% | 88.5% |
| CALL RESUME_CHECK | 4,668,780 | 0.2% | 88.7% |
| STORE_FAST JUMP_FORWARD | 4,482,960 | 0.2% | 88.9% |
| JUMP_FORWARD LOAD_FAST | 4,481,280 | 0.2% | 89.2% |
| TO_BOOL POP_JUMP_IF_TRUE | 4,480,980 | 0.2% | 89.4% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 4,479,200 | 0.2% | 89.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 42,034,380 | 87.2% |
| POP_TOP | 4,478,960 | 9.3% |
| RETURN_GENERATOR | 1,492,960 | 3.1% |
| COPY_FREE_VARS | 189,420 | 0.4% |
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
| RETURN_VALUE | 6,536,520 | 77.7% |
| RETURN_CONST | 935,880 | 11.1% |
| SEND | 935,720 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 5,604,080 | 66.7% |
| RETURN_VALUE | 1,868,320 | 22.2% |
| STORE_FAST | 746,480 | 8.9% |
| LOAD_FAST | 189,240 | 2.3% |


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
| CALL_BUILTIN_CLASS | 748,340 | 99.5% |
| LOAD_FAST | 3,700 | 0.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 160 | 0.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 748,280 | 99.5% |
| FOR_ITER_LIST | 3,640 | 0.5% |
| FOR_ITER | 320 | 0.0% |
| FOR_ITER_TUPLE | 20 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 28,188,720 | 58.5% |
| RETURN_VALUE | 17,578,660 | 36.5% |
| RETURN_GENERATOR | 1,492,960 | 3.1% |
| YIELD_VALUE | 935,720 | 1.9% |


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
| STORE_ATTR_INSTANCE_VALUE | 746,460 | 66.0% |
| RESUME_CHECK | 191,980 | 17.0% |
| STORE_FAST | 191,240 | 16.9% |
| POP_TOP | 400 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,129,880 | 100.0% |
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
| CALL_METHOD_DESCRIPTOR_O | 27,809,820 | 30.6% |
| RETURN_CONST | 25,408,200 | 27.9% |
| CALL_FUNCTION_EX | 10,083,040 | 11.1% |
| SEND_GEN | 7,472,240 | 8.2% |
| END_SEND | 5,604,080 | 6.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,021,280 | 42.9% |
| ENTER_EXECUTOR | 14,561,080 | 16.0% |
| RETURN_CONST | 14,005,760 | 15.4% |
| RESUME_CHECK | 11,951,180 | 13.1% |
| LOAD_CONST | 11,021,180 | 12.1% |


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
| LOAD_ATTR_MODULE | 26,340,920 | 78.7% |
| LOAD_FAST | 6,757,640 | 20.2% |
| LOAD_ATTR | 381,560 | 1.1% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 14,562,080 | 43.5% |
| CALL | 9,528,820 | 28.5% |
| LOAD_FAST | 4,720,740 | 14.1% |
| LOAD_GLOBAL_MODULE | 2,053,320 | 6.1% |
| LOAD_CONST | 1,868,560 | 5.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 6,536,780 | 54.7% |
| ENTER_EXECUTOR | 3,732,120 | 31.2% |
| CACHE | 1,492,960 | 12.5% |
| CALL_PY_WITH_DEFAULTS | 189,220 | 1.6% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 5,979,440 | 50.0% |
| CALL | 4,478,920 | 37.5% |
| INTERPRETER_EXIT | 1,492,960 | 12.5% |
| CALL_PY_EXACT_ARGS | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,519,620 | 55.0% |
| LOAD_ATTR_INSTANCE_VALUE | 15,687,300 | 25.8% |
| COMPARE_OP_FLOAT | 2,080,860 | 3.4% |
| RETURN_VALUE | 1,868,800 | 3.1% |
| END_SEND | 1,868,320 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 17,578,660 | 28.9% |
| STORE_FAST | 16,621,880 | 27.3% |
| TO_BOOL_BOOL | 10,272,680 | 16.9% |
| END_SEND | 6,536,520 | 10.7% |
| POP_TOP | 4,479,120 | 7.4% |


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
| LOAD_ATTR_INSTANCE_VALUE | 11,199,400 | 99.9% |
| TO_BOOL | 3,800 | 0.0% |
| LOAD_ATTR | 760 | 0.0% |
| RETURN_VALUE | 480 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,719,500 | 60.0% |
| POP_JUMP_IF_TRUE | 4,480,980 | 40.0% |
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
| LOAD_FAST | 240 | 20.7% |
| LOAD_GLOBAL_MODULE | 180 | 15.5% |
| UNARY_INVERT | 160 | 13.8% |
| BINARY_OP | 160 | 13.8% |
| LOAD_CONST | 160 | 13.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 220 | 19.0% |
| BINARY_OP | 160 | 13.8% |
| COPY | 160 | 13.8% |
| LOAD_GLOBAL_MODULE | 120 | 10.3% |
| UNARY_INVERT | 80 | 6.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 746,680 | 66.1% |
| LOAD_ATTR_SLOT | 191,340 | 16.9% |
| LOAD_FAST | 189,240 | 16.8% |
| STORE_FAST | 1,840 | 0.2% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,127,320 | 99.8% |
| STORE_FAST | 1,840 | 0.2% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 189,240 | 99.8% |
| STORE_ATTR_INSTANCE_VALUE | 140 | 0.1% |
| POP_TOP | 80 | 0.0% |
| BUILD_TUPLE | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 189,240 | 99.8% |
| LOAD_FAST | 400 | 0.2% |


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
| LOAD_FAST_LOAD_FAST | 10,083,080 | 26.1% |
| PUSH_NULL | 9,528,820 | 24.6% |
| LOAD_ATTR | 8,959,720 | 23.2% |
| LOAD_ATTR_INSTANCE_VALUE | 4,479,120 | 11.6% |
| RETURN_GENERATOR | 4,478,920 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 19,420,080 | 50.2% |
| POP_TOP | 5,415,400 | 14.0% |
| RESUME_CHECK | 4,668,780 | 12.1% |
| CALL_METHOD_DESCRIPTOR_O | 4,479,100 | 11.6% |
| LOAD_GLOBAL_MODULE | 3,732,500 | 9.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,891,520 | 96.3% |
| CALL_INTRINSIC_1 | 191,360 | 1.9% |
| BUILD_MAP | 189,240 | 1.8% |
| DICT_MERGE | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,083,040 | 98.2% |
| STORE_FAST | 189,240 | 1.8% |
| COPY_FREE_VARS | 80 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 380,600 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 191,360 | 50.3% |
| LOAD_CONST | 189,240 | 49.7% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,893,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,478,960 | 45.3% |
| RESUME_CHECK | 4,478,940 | 45.3% |
| RETURN_VALUE | 935,720 | 9.5% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 189,540 | 99.6% |
| COMPARE_OP | 280 | 0.1% |
| CALL_BUILTIN_CLASS | 140 | 0.1% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 189,720 | 99.7% |
| COMPARE_OP | 280 | 0.1% |
| COMPARE_OP_INT | 220 | 0.1% |
| COMPARE_OP_FLOAT | 80 | 0.0% |
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
| CALL_LEN | 1,820 | 70.5% |
| BINARY_OP | 160 | 6.2% |
| LOAD_FAST | 160 | 6.2% |
| CALL_BUILTIN_FAST | 140 | 5.4% |
| UNARY_NOT | 80 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 1,880 | 72.9% |
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
| CALL_PY_EXACT_ARGS | 189,860 | 50.0% |
| CACHE | 189,420 | 49.9% |
| CALL | 180 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 379,140 | 99.9% |
| RESUME | 240 | 0.1% |
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
| POP_TOP | 14,561,080 | 99.2% |
| POP_JUMP_IF_FALSE | 91,400 | 0.6% |
| ENTER_EXECUTOR | 24,880 | 0.2% |
| JUMP_BACKWARD | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 9,891,520 | 67.4% |
| RETURN_GENERATOR | 3,732,120 | 25.4% |
| FOR_ITER_RANGE | 748,240 | 5.1% |
| LOAD_ATTR_SLOT | 189,240 | 1.3% |
| RETURN_VALUE | 89,840 | 0.6% |


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
| RETURN_GENERATOR | 5,979,440 | 71.1% |
| BEFORE_ASYNC_WITH | 746,480 | 8.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 746,460 | 8.9% |
| LOAD_ATTR_INSTANCE_VALUE | 746,460 | 8.9% |
| LOAD_FAST | 189,240 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,408,120 | 100.0% |


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
| POP_JUMP_IF_FALSE | 1,040 | 60.5% |
| POP_TOP | 680 | 39.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 57.0% |
| FOR_ITER_RANGE | 600 | 34.9% |
| ENTER_EXECUTOR | 100 | 5.8% |
| FOR_ITER | 40 | 2.3% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,439,140 | 100.0% |
| RESUME | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 1,503,560 | 61.6% |
| SEND | 935,760 | 38.4% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,482,960 | 100.0% |
| POP_TOP | 100 | 0.0% |
| ENTER_EXECUTOR | 80 | 0.0% |
| POP_JUMP_IF_FALSE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,481,280 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 1,880 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_FAST_CHECK | 20 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 191,340 | 50.3% |
| LOAD_FAST | 189,240 | 49.7% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 380,600 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,317,740 | 94.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,493,560 | 4.8% |
| LOAD_ATTR_SLOT | 191,460 | 0.6% |
| LOAD_ATTR | 11,420 | 0.0% |
| LOAD_GLOBAL_MODULE | 1,040 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,893,440 | 31.9% |
| CALL | 8,959,720 | 28.9% |
| LOAD_FAST | 4,669,380 | 15.1% |
| TO_BOOL_NONE | 4,478,920 | 14.4% |
| STORE_FAST | 1,868,480 | 6.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 20,544,540 | 23.8% |
| POP_TOP | 11,021,180 | 12.7% |
| LOAD_FAST_LOAD_FAST | 10,826,240 | 12.5% |
| POP_JUMP_IF_FALSE | 10,278,000 | 11.9% |
| LOAD_FAST | 10,089,740 | 11.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,600,940 | 45.8% |
| STORE_FAST | 10,838,640 | 12.5% |
| CALL_KW | 9,893,720 | 11.4% |
| COMPARE_OP_INT | 8,217,720 | 9.5% |
| SEND_GEN | 7,472,120 | 8.6% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 379,060 | 99.8% |
| LOAD_GLOBAL | 240 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 379,300 | 99.9% |
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
| RESUME_CHECK | 82,912,820 | 20.8% |
| POP_JUMP_IF_FALSE | 78,948,000 | 19.9% |
| STORE_FAST | 44,834,960 | 11.3% |
| LOAD_CONST | 39,600,940 | 10.0% |
| POP_TOP | 39,021,280 | 9.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 121,737,160 | 30.6% |
| LOAD_ATTR_SLOT | 36,122,320 | 9.1% |
| RETURN_VALUE | 33,519,620 | 8.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 32,311,440 | 8.1% |
| STORE_ATTR_SLOT | 31,195,800 | 7.8% |


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
| STORE_ATTR_SLOT | 30,248,820 | 31.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 16,240,780 | 16.8% |
| LOAD_FAST_LOAD_FAST | 14,751,480 | 15.2% |
| PUSH_NULL | 14,562,080 | 15.0% |
| POP_JUMP_IF_NOT_NONE | 9,893,640 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 40,520,880 | 41.8% |
| LOAD_FAST_LOAD_FAST | 14,751,480 | 15.2% |
| LOAD_CONST | 10,826,240 | 11.2% |
| LOAD_FAST | 10,083,360 | 10.4% |
| CALL | 10,083,080 | 10.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME | 620 | 12.9% |
| RESUME_CHECK | 600 | 12.4% |
| POP_JUMP_IF_FALSE | 540 | 11.2% |
| POP_TOP | 500 | 10.4% |
| LOAD_FAST | 500 | 10.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,680 | 34.9% |
| LOAD_ATTR | 1,020 | 21.2% |
| LOAD_GLOBAL_BUILTIN | 660 | 13.7% |
| LOAD_FAST | 400 | 8.3% |
| CALL | 320 | 6.6% |


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
| TO_BOOL_BOOL | 59,038,780 | 52.7% |
| TO_BOOL_NONE | 24,836,020 | 22.2% |
| COMPARE_OP_INT | 12,366,200 | 11.0% |
| TO_BOOL | 6,719,500 | 6.0% |
| TO_BOOL_LIST | 5,229,600 | 4.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 78,948,000 | 70.4% |
| RETURN_CONST | 15,498,180 | 13.8% |
| LOAD_CONST | 10,278,000 | 9.2% |
| LOAD_GLOBAL_MODULE | 5,236,280 | 4.7% |
| LOAD_FAST_LOAD_FAST | 2,057,660 | 1.8% |


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
| LOAD_FAST | 21,289,920 | 76.0% |
| LOAD_ATTR_INSTANCE_VALUE | 6,718,340 | 24.0% |
| LOAD_GLOBAL_MODULE | 220 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 9,893,640 | 35.3% |
| LOAD_GLOBAL_MODULE | 7,283,280 | 26.0% |
| LOAD_FAST | 5,605,940 | 20.0% |
| RETURN_CONST | 4,478,880 | 16.0% |
| LOAD_CONST | 746,500 | 2.7% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 5,604,440 | 55.6% |
| TO_BOOL | 4,480,980 | 44.4% |
| TO_BOOL_INT | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,893,900 | 98.1% |
| LOAD_CONST | 191,160 | 1.9% |
| STORE_FAST | 1,840 | 0.0% |
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
| POP_JUMP_IF_FALSE | 15,498,180 | 28.0% |
| POP_TOP | 14,005,760 | 25.3% |
| STORE_ATTR_SLOT | 10,461,600 | 18.9% |
| STORE_FAST | 10,084,720 | 18.2% |
| POP_JUMP_IF_NOT_NONE | 4,478,880 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 28,188,720 | 51.0% |
| POP_TOP | 25,408,200 | 46.0% |
| END_SEND | 935,880 | 1.7% |
| EXIT_INIT_CHECK | 746,460 | 1.4% |
| TO_BOOL | 40 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 936,000 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 935,760 | 50.0% |
| SEND | 840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 935,720 | 50.0% |
| YIELD_VALUE | 935,720 | 50.0% |
| SEND | 840 | 0.0% |
| POP_TOP | 160 | 0.0% |
| SEND_GEN | 160 | 0.0% |


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
| CALL | 19,420,080 | 29.2% |
| RETURN_VALUE | 16,621,880 | 25.0% |
| LOAD_CONST | 10,838,640 | 16.3% |
| CALL_BUILTIN_O | 7,883,580 | 11.8% |
| CALL_KW | 4,478,960 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,834,960 | 67.4% |
| RETURN_CONST | 10,084,720 | 15.2% |
| JUMP_FORWARD | 4,482,960 | 6.7% |
| LOAD_FAST_LOAD_FAST | 4,336,140 | 6.5% |
| LOAD_GLOBAL_MODULE | 1,868,480 | 2.8% |


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
| YIELD_VALUE | 1,503,600 | 61.6% |
| SEND | 935,720 | 38.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 1,503,600 | 61.6% |
| INTERPRETER_EXIT | 935,720 | 38.4% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,160 | 55.8% |
| CACHE | 340 | 16.3% |
| COPY_FREE_VARS | 240 | 11.5% |
| POP_TOP | 180 | 8.7% |
| SEND_GEN | 120 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 46.2% |
| LOAD_GLOBAL | 620 | 29.8% |
| JUMP_BACKWARD_NO_INTERRUPT | 180 | 8.7% |
| LOAD_CONST | 140 | 6.7% |
| NOP | 100 | 4.8% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 189,200 | 99.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,800 | 0.9% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 189,220 | 99.0% |
| STORE_FAST | 1,820 | 1.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,868,320 | 50.0% |
| RETURN_VALUE | 1,868,280 | 50.0% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,868,300 | 50.0% |
| CALL_PY_WITH_DEFAULTS | 1,868,280 | 50.0% |
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
| LOAD_FAST_LOAD_FAST | 1,868,280 | 71.4% |
| LOAD_CONST | 746,760 | 28.6% |
| BINARY_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,868,300 | 71.4% |
| CALL_PY_EXACT_ARGS | 746,720 | 28.6% |
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
| LOAD_CONST | 560 | 93.3% |
| BINARY_SUBSCR | 40 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 460 | 76.7% |
| LOAD_ATTR_SLOT | 120 | 20.0% |
| LOAD_ATTR | 20 | 3.3% |


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
| LOAD_CONST | 2,614,720 | 99.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 0.5% |
| CALL | 60 | 0.0% |
| PUSH_NULL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,868,300 | 71.1% |
| GET_AWAITABLE | 746,460 | 28.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 0.5% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 746,660 | 49.9% |
| LOAD_GLOBAL_MODULE | 746,440 | 49.9% |
| LOAD_FAST | 1,980 | 0.1% |
| CALL | 180 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 748,340 | 50.0% |
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
| LOAD_FAST | 189,200 | 99.9% |
| LOAD_CONST | 180 | 0.1% |
| CALL | 60 | 0.0% |
| LOAD_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 189,220 | 99.9% |
| COPY | 140 | 0.1% |
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
| LOAD_FAST | 8,072,260 | 81.2% |
| LOAD_GLOBAL_MODULE | 1,864,120 | 18.8% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.0% |
| CALL | 200 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,883,580 | 79.3% |
| RETURN_VALUE | 1,864,140 | 18.8% |
| TO_BOOL_BOOL | 189,200 | 1.9% |
| POP_TOP | 120 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,080,880 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 380 | 0.0% |
| CALL | 80 | 0.0% |
| BUILD_TUPLE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,081,300 | 100.0% |
| TO_BOOL | 80 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,400 | 98.9% |
| CALL | 60 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,640 | 66.7% |
| COPY | 1,820 | 33.3% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,680,840 | 100.0% |
| LOAD_FAST_LOAD_FAST | 120 | 0.0% |
| CALL | 60 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,678,660 | 99.9% |
| TO_BOOL_NONE | 2,180 | 0.1% |
| RETURN_VALUE | 140 | 0.0% |
| STORE_FAST | 60 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,800 | 89.1% |
| LOAD_CONST | 80 | 4.0% |
| CALL | 60 | 3.0% |
| LOAD_ATTR | 40 | 2.0% |
| LOAD_FAST | 40 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,820 | 90.1% |
| POP_TOP | 120 | 5.9% |
| RETURN_VALUE | 80 | 4.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 9,893,440 | 84.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,870,800 | 15.9% |
| CALL | 400 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 9,893,400 | 84.1% |
| STORE_FAST | 1,870,400 | 15.9% |
| POP_TOP | 380 | 0.0% |
| GET_ITER | 160 | 0.0% |
| CALL | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,330,640 | 83.9% |
| CALL | 4,479,100 | 16.1% |
| LOAD_CONST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 27,809,820 | 100.0% |
| LOAD_CONST | 20 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 29,883,560 | 66.1% |
| LOAD_FAST | 13,824,120 | 30.6% |
| BINARY_OP_SUBTRACT_INT | 746,720 | 1.7% |
| LOAD_ATTR_METHOD_NO_DICT | 380,640 | 0.8% |
| LOAD_SUPER_ATTR_METHOD | 189,400 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 38,489,300 | 85.1% |
| RETURN_GENERATOR | 6,536,780 | 14.5% |
| COPY_FREE_VARS | 189,860 | 0.4% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 1,868,280 | 90.8% |
| LOAD_GLOBAL_MODULE | 189,200 | 9.2% |
| CALL | 140 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,868,680 | 90.8% |
| RETURN_GENERATOR | 189,220 | 9.2% |


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
| LOAD_GLOBAL_MODULE | 3,732,560 | 64.2% |
| LOAD_ATTR_SLOT | 2,080,840 | 35.8% |
| LOAD_FAST | 440 | 0.0% |
| COMPARE_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,733,060 | 64.2% |
| RETURN_VALUE | 2,080,860 | 35.8% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,217,720 | 66.5% |
| LOAD_FAST_LOAD_FAST | 2,278,180 | 18.4% |
| LOAD_GLOBAL_MODULE | 1,870,080 | 15.1% |
| COMPARE_OP | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,366,200 | 100.0% |


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
| GET_ITER | 3,640 | 98.4% |
| FOR_ITER | 60 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,880 | 50.8% |
| LOAD_FAST | 1,820 | 49.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 748,280 | 50.0% |
| ENTER_EXECUTOR | 748,240 | 50.0% |
| JUMP_BACKWARD | 600 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 748,840 | 50.0% |
| LOAD_CONST | 748,320 | 50.0% |


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
| LOAD_GLOBAL_MODULE | 1,868,280 | 100.0% |
| LOAD_FAST | 120 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,868,440 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 121,737,160 | 96.4% |
| LOAD_FAST_LOAD_FAST | 4,479,120 | 3.5% |
| LOAD_ATTR | 1,980 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| COPY | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 39,767,520 | 31.5% |
| LOAD_ATTR_METHOD_NO_DICT | 29,494,980 | 23.4% |
| RETURN_VALUE | 15,687,300 | 12.4% |
| TO_BOOL | 11,199,400 | 8.9% |
| POP_JUMP_IF_NOT_NONE | 6,718,340 | 5.3% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 29,494,980 | 92.9% |
| LOAD_FAST | 2,249,160 | 7.1% |
| LOAD_ATTR | 620 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,011,780 | 78.8% |
| LOAD_GLOBAL_MODULE | 4,478,960 | 14.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,870,800 | 5.9% |
| CALL_PY_EXACT_ARGS | 380,640 | 1.2% |
| LOAD_FAST_LOAD_FAST | 1,960 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,311,440 | 64.8% |
| LOAD_ATTR_SLOT | 10,461,400 | 21.0% |
| LOAD_ATTR_INSTANCE_VALUE | 5,227,400 | 10.5% |
| LOAD_FAST_LOAD_FAST | 1,868,320 | 3.7% |
| LOAD_ATTR | 1,260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 29,883,560 | 59.9% |
| LOAD_FAST_LOAD_FAST | 16,240,780 | 32.6% |
| LOAD_FAST | 3,744,800 | 7.5% |
| CALL | 700 | 0.0% |
| LOAD_CONST | 120 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 26,529,680 | 100.0% |
| LOAD_ATTR | 1,020 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 26,340,920 | 99.3% |
| LOAD_FAST_LOAD_FAST | 189,220 | 0.7% |
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
| LOAD_FAST | 36,122,320 | 99.5% |
| ENTER_EXECUTOR | 189,240 | 0.5% |
| LOAD_ATTR_SLOT | 7,000 | 0.0% |
| LOAD_ATTR | 480 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 20,354,800 | 56.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,461,400 | 28.8% |
| LOAD_FAST | 2,081,320 | 5.7% |
| COMPARE_OP_FLOAT | 2,080,840 | 5.7% |
| TO_BOOL_BOOL | 759,120 | 2.1% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,272,920 | 57.4% |
| STORE_FAST | 748,300 | 18.9% |
| STORE_ATTR_INSTANCE_VALUE | 746,580 | 18.8% |
| POP_TOP | 189,400 | 4.8% |
| JUMP_FORWARD | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,089,440 | 52.7% |
| CALL_BUILTIN_CLASS | 746,660 | 18.8% |
| LOAD_GLOBAL_MODULE | 746,480 | 18.8% |
| LOAD_DEREF | 379,060 | 9.6% |
| CALL_ISINSTANCE | 380 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,679,140 | 38.1% |
| POP_JUMP_IF_NOT_NONE | 7,283,280 | 14.9% |
| POP_JUMP_IF_FALSE | 5,236,280 | 10.7% |
| LOAD_ATTR_METHOD_NO_DICT | 4,478,960 | 9.1% |
| LOAD_FAST | 4,140,360 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 26,529,680 | 54.2% |
| LOAD_FAST | 5,605,420 | 11.4% |
| LOAD_FAST_LOAD_FAST | 4,479,200 | 9.1% |
| COMPARE_OP_FLOAT | 3,732,560 | 7.6% |
| CALL_ISINSTANCE | 2,080,880 | 4.2% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 378,840 | 99.9% |
| LOAD_SUPER_ATTR | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 189,400 | 50.0% |
| LOAD_FAST_LOAD_FAST | 189,280 | 49.9% |
| LOAD_FAST | 260 | 0.1% |
| CALL | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 42,034,380 | 38.9% |
| CALL_PY_EXACT_ARGS | 38,489,300 | 35.6% |
| POP_TOP | 11,951,180 | 11.1% |
| CALL | 4,668,780 | 4.3% |
| CALL_KW | 4,478,940 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,912,820 | 76.8% |
| LOAD_GLOBAL_MODULE | 18,679,140 | 17.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 2,439,140 | 2.3% |
| LOAD_GLOBAL_BUILTIN | 2,272,920 | 2.1% |
| LOAD_CONST | 1,493,380 | 1.4% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,472,120 | 83.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,503,560 | 16.8% |
| SEND | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 7,472,240 | 83.2% |
| RESUME_CHECK | 1,503,480 | 16.8% |
| RESUME | 120 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 40,520,880 | 56.5% |
| LOAD_FAST | 31,195,800 | 43.5% |
| STORE_ATTR_SLOT | 47,320 | 0.1% |
| STORE_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 30,248,820 | 42.2% |
| LOAD_CONST | 20,544,540 | 28.6% |
| LOAD_FAST | 10,462,060 | 14.6% |
| RETURN_CONST | 10,461,600 | 14.6% |
| STORE_ATTR_SLOT | 47,320 | 0.1% |


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
| LOAD_ATTR_INSTANCE_VALUE | 39,767,520 | 61.5% |
| RETURN_VALUE | 10,272,680 | 15.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 9,893,400 | 15.3% |
| CALL_ISINSTANCE | 2,081,300 | 3.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,678,660 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 59,038,780 | 91.3% |
| POP_JUMP_IF_TRUE | 5,604,440 | 8.7% |
| UNARY_NOT | 60 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,880 | 85.5% |
| TO_BOOL | 160 | 7.3% |
| LOAD_FAST | 80 | 3.6% |
| BINARY_OP | 40 | 1.8% |
| LOAD_ATTR_SLOT | 40 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,880 | 85.5% |
| POP_JUMP_IF_FALSE | 260 | 11.8% |
| UNARY_NOT | 60 | 2.7% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,229,500 | 100.0% |
| TO_BOOL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,229,600 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 20,354,800 | 82.0% |
| LOAD_ATTR | 4,478,920 | 18.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,180 | 0.0% |
| TO_BOOL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 24,836,020 | 100.0% |
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
|     deferred | 820 | 0.0% |
|          hit | 6,542,860 | 100.0% |

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
|     deferred | 60 | 6.2% |
|          hit | 840 | 87.5% |

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
|     deferred | 39,403,840 | 26.8% |
|          hit | 107,469,660 | 73.2% |
|         miss | 761,180 | 0.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 17,500 | 57.5% |
| Failure | 12,960 | 42.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr method fastcall keywords | 3,240 | 25.0% |
| no dict | 2,860 | 22.1% |
| cfunc noargs | 2,360 | 18.2% |
| code complex parameters | 1,580 | 12.2% |
| class no vectorcall | 1,340 | 10.3% |
| other | 1,280 | 9.9% |
| class mutable | 80 | 0.6% |
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
|     deferred | 189,760 | 1.0% |
|          hit | 18,180,140 | 99.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 51.7% |
| Failure | 280 | 48.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 240 | 85.7% |
| bool | 40 | 14.3% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 1,500,900 | 100.0% |

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
|     deferred | 31,370,120 | 10.3% |
|          hit | 272,176,040 | 89.7% |
|         miss | 376,020 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,480 | 54.2% |
| Failure | 10,540 | 45.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 6,480 | 61.5% |
| method | 2,540 | 24.1% |
| class attr descriptor | 1,280 | 12.1% |
| not managed dict | 140 | 1.3% |
| metaclass attribute | 60 | 0.6% |
| class attr simple | 40 | 0.4% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,560 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 52,930,740 | 100.0% |
|         miss | 80 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,340 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.1% |
|          hit | 379,060 | 99.9% |

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
|     deferred | 1,871,600 | 17.3% |
|          hit | 8,975,840 | 82.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 16.0% |
| Failure | 840 | 84.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 840 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,464,120 | 2.9% |
|          hit | 81,201,520 | 97.0% |
|         miss | 2,509,460 | 3.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 48,940 | 99.8% |
| Failure | 100 | 0.2% |

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
|     deferred | 11,202,200 | 10.6% |
|          hit | 94,709,420 | 89.4% |
|         miss | 1,700 | 0.0% |

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
| Basic | 1,015,701,860 | 50.4% |
| Not specialized | 246,616,960 | 12.2% |
| Specialized hits | 750,162,580 | 37.2% |
| Specialized misses | 3,676,760 | 0.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 39,403,840 | 45.6% |
| LOAD_ATTR | 31,370,120 | 36.3% |
| TO_BOOL | 11,202,200 | 12.9% |
| STORE_ATTR | 2,464,120 | 2.8% |
| SEND | 1,871,600 | 2.2% |
| COMPARE_OP | 189,760 | 0.2% |
| LOAD_GLOBAL | 2,560 | 0.0% |
| BINARY_OP | 820 | 0.0% |
| FOR_ITER | 260 | 0.0% |
| LOAD_SUPER_ATTR | 240 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,509,460 | 67.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 760,800 | 20.5% |
| LOAD_ATTR_SLOT | 372,540 | 10.1% |
| RESUME | 28,320 | 0.8% |
| RESUME_CHECK | 28,320 | 0.8% |
| LOAD_ATTR_METHOD_NO_DICT | 3,480 | 0.1% |
| TO_BOOL_NONE | 1,060 | 0.0% |
| TO_BOOL_BOOL | 640 | 0.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 260 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 48,196,060 | 41.5% |
| Calls to Python functions inlined | 68,014,040 | 58.5% |
| Calls via PyEval_EvalFrame (total) | 48,196,060 | 41.5% |
| Calls via PyEval_EvalFrame (vector) | 42,781,380 | 36.8% |
| Calls via PyEval_EvalFrame (generator) | 5,414,680 | 4.7% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 42,781,380 | 36.8% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 2,080,880 | 1.8% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 4,479,100 | 3.9% |
| Calls via PyEval_EvalFrame (method) | 19,787,280 | 17.0% |
| Frame objects created | 180 | 0.0% |
| Frames pushed | 64,260,280 | 55.3% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 57,521,240 | 16.8% |
| Frees to freelist | 57,856,680 |  |
| Allocations | 284,515,366 | 83.2% |
| Allocations to 512 bytes | 281,844,650 | 82.4% |
| Allocations to 4 kbytes | 2,670,590 | 0.8% |
| Allocations over 4 kbytes | 126 | 0.0% |
| Frees | 284,430,302 |  |
| New values | 440 |  |
| Interpreter increfs | 1,211,263,920 | 79.9% |
| Interpreter decrefs | 1,282,820,610 | 69.7% |
| Increfs | 305,373,825 | 20.1% |
| Decrefs | 556,976,616 | 30.3% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 63,580,105 |  |
| Method cache misses | 4,255 |  |
| Method cache collisions | 3,957 |  |
| Method cache dunder hits | 13,658,106 |  |
| Method cache dunder misses | 514 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 53,420 | 2,040 | 356,178,800 |
| 1 | 4,860 | 0 | 367,218,200 |
| 2 | 440 | 0 | 951,535,680 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 100 |  |
| Traces created | 100 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 20 | 20.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 20 | 20.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 14,677,460 |  |
| Uops executed | 780,291,560 | 53.16 |

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
| <= 32 | 20 | 20.0% |
| <= 64 | 40 | 40.0% |
| <= 128 | 40 | 40.0% |


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
| <= 16 | 40 | 40.0% |
| <= 32 | 20 | 20.0% |
| <= 64 | 20 | 20.0% |
| <= 128 | 20 | 20.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 20 | 0.0% |
| <= 4 | 748,240 | 5.1% |
| <= 8 | 0 | 0.0% |
| <= 16 | 116,160 | 0.8% |
| <= 32 | 3,921,360 | 26.7% |
| <= 64 | 0 | 0.0% |
| <= 128 | 9,891,520 | 67.4% |
| <= 256 | 0 | 0.0% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 0 | 0.0% |
| <= 2,048 | 0 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 0 | 0.0% |
| <= 16,384 | 80 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 0 | 0.0% |
| <= 131,072 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 110,176,440 | 14.1% | 14.1% |  |
| _CHECK_VALIDITY | 101,962,520 | 13.1% | 27.2% |  |
| _GUARD_TYPE_VERSION | 88,487,040 | 11.3% | 38.5% | 0.2% |
| LOAD_FAST | 82,875,960 | 10.6% | 49.1% |  |
| _LOAD_ATTR_SLOT | 39,754,920 | 5.1% | 54.2% |  |
| STORE_FAST | 24,385,960 | 3.1% | 57.4% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 20,727,400 | 2.7% | 60.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 20,727,400 | 2.7% | 62.7% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 20,161,040 | 2.6% | 65.3% |  |
| _GUARD_IS_FALSE_POP | 20,086,600 | 2.6% | 67.8% | 0.1% |
| TO_BOOL_BOOL | 19,783,040 | 2.5% | 70.4% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 14,561,120 | 1.9% | 72.2% | 5.1% |
| _ITER_CHECK_RANGE | 14,561,120 | 1.9% | 74.1% |  |
| _ITER_NEXT_RANGE | 13,812,880 | 1.8% | 75.9% |  |
| _EXIT_TRACE | 13,714,920 | 1.8% | 77.6% | 100.0% |
| _CHECK_FUNCTION_EXACT_ARGS | 13,625,080 | 1.7% | 79.4% |  |
| _CHECK_STACK_SPACE | 13,625,080 | 1.7% | 81.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 13,625,080 | 1.7% | 82.9% |  |
| _PUSH_FRAME | 13,625,080 | 1.7% | 84.6% |  |
| _SAVE_RETURN_OFFSET | 13,625,080 | 1.7% | 86.4% |  |
| PUSH_NULL | 10,195,000 | 1.3% | 87.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,080,760 | 1.3% | 89.0% |  |
| BUILD_LIST | 9,891,520 | 1.3% | 90.2% |  |
| CALL_INTRINSIC_1 | 9,891,520 | 1.3% | 91.5% |  |
| LIST_EXTEND | 9,891,520 | 1.3% | 92.8% |  |
| RESUME_CHECK | 9,891,520 | 1.3% | 94.0% |  |
| _LOAD_ATTR | 9,891,520 | 1.3% | 95.3% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 7,465,680 | 1.0% | 96.3% |  |
| _GUARD_KEYS_VERSION | 7,465,680 | 1.0% | 97.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 7,465,680 | 1.0% | 98.2% |  |
| _LOAD_CONST_INLINE_BORROW | 4,109,720 | 0.5% | 98.7% |  |
| _GUARD_BOTH_INT | 3,732,120 | 0.5% | 99.2% |  |
| _BINARY_OP_SUBTRACT_INT | 3,732,120 | 0.5% | 99.7% |  |
| CALL_BUILTIN_O | 303,480 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_LIST_INT | 188,840 | 0.0% | 99.7% |  |
| COMPARE_OP_FLOAT | 188,840 | 0.0% | 99.7% |  |
| _GUARD_IS_TRUE_POP | 188,760 | 0.0% | 99.8% | 0.0% |
| POP_TOP | 188,760 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 188,760 | 0.0% | 99.8% |  |
| TO_BOOL_LIST | 188,760 | 0.0% | 99.8% |  |
| _CHECK_ATTR_MODULE | 188,760 | 0.0% | 99.9% |  |
| _LOAD_ATTR_MODULE | 188,760 | 0.0% | 99.9% |  |
| _STORE_ATTR_SLOT | 188,760 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE | 188,760 | 0.0% | 99.9% |  |
| _CHECK_GLOBALS | 188,760 | 0.0% | 100.0% |  |
| _JUMP_TO_TOP | 188,680 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 114,720 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 20 | 0.0% | 100.0% | 100.0% |
| _ITER_CHECK_TUPLE | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_FUNCTION_EX | 20 |


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


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-08
