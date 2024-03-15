
# Pystats results

- benchmark: async_tree_io_tg
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 783,754,780 | 19.7% | 19.7% |  |
| RESUME_CHECK | 243,821,120 | 6.1% | 25.8% | 0.0% |
| POP_JUMP_IF_FALSE | 210,230,400 | 5.3% | 31.1% |  |
| LOAD_ATTR_SLOT | 188,276,420 | 4.7% | 35.9% | 0.0% |
| TO_BOOL_BOOL | 160,204,860 | 4.0% | 39.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 159,777,780 | 4.0% | 43.9% |  |
| POP_TOP | 149,308,180 | 3.8% | 47.7% |  |
| LOAD_FAST_LOAD_FAST | 149,303,160 | 3.8% | 51.4% |  |
| LOAD_CONST | 146,331,380 | 3.7% | 55.1% |  |
| RETURN_VALUE | 143,784,060 | 3.6% | 58.7% |  |
| STORE_ATTR_SLOT | 142,582,940 | 3.6% | 62.3% | 0.0% |
| INTERPRETER_EXIT | 128,101,300 | 3.2% | 65.5% |  |
| LOAD_GLOBAL_MODULE | 120,643,740 | 3.0% | 68.6% |  |
| RETURN_CONST | 101,530,700 | 2.6% | 71.1% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 92,574,920 | 2.3% | 73.4% |  |
| CALL_PY_EXACT_ARGS | 91,084,760 | 2.3% | 75.7% |  |
| STORE_FAST | 90,357,920 | 2.3% | 78.0% |  |
| LOAD_GLOBAL_BUILTIN | 66,151,460 | 1.7% | 79.7% | 0.0% |
| CALL | 59,747,900 | 1.5% | 81.2% |  |
| PUSH_NULL | 58,979,440 | 1.5% | 82.6% |  |
| COMPARE_OP_FLOAT | 57,184,020 | 1.4% | 84.1% |  |
| CALL_ISINSTANCE | 57,183,940 | 1.4% | 85.5% |  |
| LOAD_ATTR_MODULE | 54,498,400 | 1.4% | 86.9% |  |
| TO_BOOL_NONE | 42,550,040 | 1.1% | 88.0% |  |
| POP_JUMP_IF_NOT_NONE | 40,313,320 | 1.0% | 89.0% |  |
| LOAD_ATTR | 39,590,100 | 1.0% | 90.0% |  |
| LOAD_ATTR_METHOD_NO_DICT | 35,091,840 | 0.9% | 90.9% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 31,353,080 | 0.8% | 91.6% | 0.0% |
| SEND_GEN | 24,634,500 | 0.6% | 92.3% |  |
| CALL_FUNCTION_EX | 20,902,080 | 0.5% | 92.8% |  |
| POP_JUMP_IF_TRUE | 17,173,780 | 0.4% | 93.2% |  |
| ENTER_EXECUTOR | 17,170,860 | 0.4% | 93.7% |  |
| END_SEND | 17,169,520 | 0.4% | 94.1% |  |
| RETURN_GENERATOR | 17,169,520 | 0.4% | 94.5% |  |
| GET_AWAITABLE | 17,169,520 | 0.4% | 94.9% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 16,423,040 | 0.4% | 95.4% |  |
| YIELD_VALUE | 16,423,040 | 0.4% | 95.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 13,439,700 | 0.3% | 96.1% | 0.0% |
| POP_JUMP_IF_NONE | 13,437,680 | 0.3% | 96.4% |  |
| CALL_KW | 13,436,960 | 0.3% | 96.8% |  |
| STORE_ATTR_INSTANCE_VALUE | 11,946,640 | 0.3% | 97.1% |  |
| TO_BOOL | 11,205,740 | 0.3% | 97.4% |  |
| SEND | 8,960,780 | 0.2% | 97.6% |  |
| LOAD_DEREF | 7,466,180 | 0.2% | 97.8% |  |
| COPY_FREE_VARS | 7,466,020 | 0.2% | 98.0% |  |
| LOAD_SUPER_ATTR_METHOD | 7,465,540 | 0.2% | 98.2% |  |
| TO_BOOL_LIST | 5,229,660 | 0.1% | 98.3% |  |
| FOR_ITER_RANGE | 5,229,280 | 0.1% | 98.4% |  |
| NOP | 4,483,360 | 0.1% | 98.5% |  |
| JUMP_FORWARD | 4,483,140 | 0.1% | 98.6% |  |
| COMPARE_OP_INT | 4,483,080 | 0.1% | 98.8% |  |
| BUILD_LIST | 4,482,680 | 0.1% | 98.9% |  |
| JUMP_BACKWARD | 4,481,340 | 0.1% | 99.0% |  |
| BINARY_OP_SUBTRACT_INT | 4,478,920 | 0.1% | 99.1% |  |
| COMPARE_OP | 3,734,400 | 0.1% | 99.2% |  |
| BINARY_OP_ADD_FLOAT | 3,734,280 | 0.1% | 99.3% |  |
| CALL_INTRINSIC_1 | 3,734,120 | 0.1% | 99.4% |  |
| LIST_EXTEND | 3,734,120 | 0.1% | 99.5% |  |
| CALL_BUILTIN_O | 3,733,040 | 0.1% | 99.6% |  |
| BUILD_MAP | 3,732,880 | 0.1% | 99.7% |  |
| CALL_PY_WITH_DEFAULTS | 3,732,840 | 0.1% | 99.8% |  |
| CALL_BUILTIN_FAST | 3,732,700 | 0.1% | 99.8% |  |
| CALL_BUILTIN_CLASS | 1,495,460 | 0.0% | 99.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 760,860 | 0.0% | 99.9% | 100.0% |
| GET_ITER | 752,260 | 0.0% | 99.9% |  |
| BEFORE_ASYNC_WITH | 746,480 | 0.0% | 99.9% |  |
| EXIT_INIT_CHECK | 746,460 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 746,460 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 746,460 | 0.0% | 100.0% |  |
| CALL_LEN | 5,460 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,460 | 0.0% | 100.0% |  |
| STORE_ATTR | 3,700 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 3,700 | 0.0% | 100.0% |  |
| COPY | 2,580 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 2,200 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 2,020 | 0.0% | 100.0% |  |
| RESUME | 1,980 | 0.0% | 100.0% | 3,751.5% |
| BINARY_OP | 1,080 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 660 | 0.0% | 100.0% |  |
| BUILD_TUPLE | 640 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 460 | 0.0% | 100.0% |  |
| FOR_ITER | 440 | 0.0% | 100.0% |  |
| IS_OP | 400 | 0.0% | 100.0% |  |
| SWAP | 340 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 240 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 240 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 200 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 180 | 0.0% | 100.0% |  |
| POP_EXCEPT | 180 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 180 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 160 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| UNARY_NOT | 160 | 0.0% | 100.0% |  |
| CONTAINS_OP | 160 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 160 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 140 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 140 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 120 | 0.0% | 100.0% |  |
| IMPORT_NAME | 100 | 0.0% | 100.0% |  |
| DICT_MERGE | 80 | 0.0% | 100.0% |  |
| MAKE_CELL | 80 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 80 | 0.0% | 100.0% |  |
| RERAISE | 80 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 80 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 60 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_INT | 60 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 60 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 60 | 0.0% | 100.0% |  |
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
| LOAD_FAST LOAD_ATTR_SLOT | 188,274,580 | 4.7% | 4.7% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 155,296,460 | 3.9% | 8.6% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 147,513,880 | 3.7% | 12.3% |
| POP_JUMP_IF_FALSE LOAD_FAST | 143,781,940 | 3.6% | 16.0% |
| RESUME_CHECK LOAD_FAST | 139,600,520 | 3.5% | 19.5% |
| CACHE RESUME_CHECK | 118,396,380 | 3.0% | 22.5% |
| RETURN_VALUE INTERPRETER_EXIT | 83,310,940 | 2.1% | 24.5% |
| LOAD_CONST LOAD_FAST | 82,118,020 | 2.1% | 26.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 75,407,820 | 1.9% | 28.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 72,410,040 | 1.8% | 30.3% |
| LOAD_FAST STORE_ATTR_SLOT | 70,171,440 | 1.8% | 32.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 62,711,560 | 1.6% | 33.7% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 60,918,720 | 1.5% | 35.2% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 60,917,920 | 1.5% | 36.7% |
| STORE_FAST LOAD_FAST | 60,485,080 | 1.5% | 38.3% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 58,230,960 | 1.5% | 39.7% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 57,192,000 | 1.4% | 41.2% |
| LOAD_ATTR_SLOT LOAD_FAST | 57,183,940 | 1.4% | 42.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 57,183,860 | 1.4% | 44.0% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 57,183,440 | 1.4% | 45.5% |
| COMPARE_OP_FLOAT RETURN_VALUE | 57,183,420 | 1.4% | 46.9% |
| LOAD_ATTR_SLOT COMPARE_OP_FLOAT | 57,183,400 | 1.4% | 48.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 54,497,320 | 1.4% | 49.7% |
| RETURN_CONST POP_TOP | 53,754,120 | 1.4% | 51.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 53,749,900 | 1.4% | 52.4% |
| POP_TOP LOAD_FAST | 53,005,000 | 1.3% | 53.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 51,508,260 | 1.3% | 55.1% |
| LOAD_ATTR_MODULE PUSH_NULL | 50,765,260 | 1.3% | 56.3% |
| LOAD_FAST RETURN_VALUE | 44,045,780 | 1.1% | 57.4% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 42,550,040 | 1.1% | 58.5% |
| STORE_ATTR_SLOT LOAD_CONST | 41,803,980 | 1.1% | 59.6% |
| RETURN_CONST INTERPRETER_EXIT | 38,818,440 | 1.0% | 60.5% |
| LOAD_FAST LOAD_ATTR | 38,079,140 | 1.0% | 61.5% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 38,071,000 | 1.0% | 62.4% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 33,594,560 | 0.8% | 63.3% |
| CALL STORE_FAST | 33,592,920 | 0.8% | 64.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 31,357,380 | 0.8% | 64.9% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 31,353,060 | 0.8% | 65.7% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 29,860,260 | 0.8% | 66.5% |
| POP_TOP RETURN_CONST | 28,367,960 | 0.7% | 67.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 26,874,160 | 0.7% | 67.9% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 26,873,880 | 0.7% | 68.5% |
| POP_JUMP_IF_FALSE RETURN_CONST | 26,127,900 | 0.7% | 69.2% |
| RETURN_VALUE STORE_FAST | 25,383,280 | 0.6% | 69.8% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 25,383,180 | 0.6% | 70.5% |
| LOAD_FAST_LOAD_FAST LOAD_FAST_LOAD_FAST | 25,381,200 | 0.6% | 71.1% |
| STORE_ATTR_SLOT LOAD_FAST | 24,635,020 | 0.6% | 71.7% |
| STORE_ATTR_SLOT RETURN_CONST | 24,634,560 | 0.6% | 72.3% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_WITH_VALUES | 24,634,360 | 0.6% | 73.0% |
| POP_TOP LOAD_CONST | 21,650,900 | 0.5% | 73.5% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 21,648,560 | 0.5% | 74.0% |
| POP_JUMP_IF_FALSE LOAD_CONST | 20,906,000 | 0.5% | 74.6% |
| RETURN_VALUE TO_BOOL_BOOL | 20,902,400 | 0.5% | 75.1% |
| LOAD_CONST STORE_FAST | 17,925,120 | 0.5% | 75.6% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 17,915,720 | 0.5% | 76.0% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 17,174,040 | 0.4% | 76.4% |
| LOAD_FAST LOAD_CONST | 17,171,780 | 0.4% | 76.9% |
| STORE_FAST RETURN_CONST | 17,171,200 | 0.4% | 77.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 17,169,840 | 0.4% | 77.7% |
| LOAD_FAST_LOAD_FAST CALL | 17,169,560 | 0.4% | 78.2% |
| CALL_FUNCTION_EX POP_TOP | 17,169,520 | 0.4% | 78.6% |
| GET_AWAITABLE LOAD_CONST | 17,169,520 | 0.4% | 79.0% |
| POP_TOP RESUME_CHECK | 17,169,360 | 0.4% | 79.5% |
| POP_TOP ENTER_EXECUTOR | 17,169,020 | 0.4% | 79.9% |
| ENTER_EXECUTOR CALL_FUNCTION_EX | 17,167,700 | 0.4% | 80.3% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 16,427,220 | 0.4% | 80.7% |
| PUSH_NULL CALL | 16,426,140 | 0.4% | 81.1% |
| PUSH_NULL LOAD_FAST | 16,425,420 | 0.4% | 81.6% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 16,422,880 | 0.4% | 82.0% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 15,676,840 | 0.4% | 82.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 13,437,220 | 0.3% | 82.7% |
| LOAD_CONST CALL_KW | 13,436,960 | 0.3% | 83.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST_LOAD_FAST | 13,436,880 | 0.3% | 83.4% |
| LOAD_ATTR CALL_METHOD_DESCRIPTOR_NOARGS | 13,436,680 | 0.3% | 83.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS TO_BOOL_BOOL | 13,436,640 | 0.3% | 84.1% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 12,692,420 | 0.3% | 84.4% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 12,690,920 | 0.3% | 84.7% |
| END_SEND POP_TOP | 12,690,560 | 0.3% | 85.0% |
| SEND_GEN POP_TOP | 12,690,420 | 0.3% | 85.3% |
| POP_JUMP_IF_NONE LOAD_FAST | 12,690,400 | 0.3% | 85.7% |
| LOAD_CONST SEND_GEN | 12,690,320 | 0.3% | 86.0% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 11,945,020 | 0.3% | 86.3% |
| YIELD_VALUE YIELD_VALUE | 11,944,080 | 0.3% | 86.6% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 11,944,040 | 0.3% | 86.9% |
| SEND_GEN RESUME_CHECK | 11,943,980 | 0.3% | 87.2% |
| CALL_PY_EXACT_ARGS RETURN_GENERATOR | 11,943,840 | 0.3% | 87.5% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL | 11,199,440 | 0.3% | 87.8% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 11,198,220 | 0.3% | 88.0% |
| RETURN_GENERATOR GET_AWAITABLE | 11,197,600 | 0.3% | 88.3% |
| LOAD_ATTR CALL | 8,959,720 | 0.2% | 88.5% |
| CALL POP_TOP | 8,958,640 | 0.2% | 88.8% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_MODULE | 8,958,240 | 0.2% | 89.0% |
| LOAD_FAST_LOAD_FAST LOAD_CONST | 8,957,920 | 0.2% | 89.2% |
| LOAD_ATTR LOAD_FAST | 8,212,560 | 0.2% | 89.4% |
| CALL RESUME_CHECK | 8,212,040 | 0.2% | 89.6% |
| LOAD_FAST POP_JUMP_IF_NONE | 8,211,840 | 0.2% | 89.8% |
| RETURN_CONST END_SEND | 8,211,600 | 0.2% | 90.0% |
| LOAD_FAST CALL | 7,467,000 | 0.2% | 90.2% |
| LOAD_DEREF LOAD_FAST | 7,465,780 | 0.2% | 90.4% |
| COPY_FREE_VARS RESUME_CHECK | 7,465,620 | 0.2% | 90.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 118,396,380 | 92.4% |
| POP_TOP | 4,478,960 | 3.5% |
| COPY_FREE_VARS | 3,732,660 | 2.9% |
| RETURN_GENERATOR | 1,492,960 | 1.2% |
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
| LOAD_CONST | 120 | 75.0% |
| LOAD_FAST | 40 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 60 | 37.5% |
| LOAD_ATTR | 40 | 25.0% |
| PUSH_EXC_INFO | 20 | 12.5% |
| STORE_FAST | 20 | 12.5% |
| BINARY_SUBSCR_DICT | 20 | 12.5% |


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
| RETURN_CONST | 8,211,600 | 47.8% |
| RETURN_VALUE | 4,478,960 | 26.1% |
| SEND | 4,478,960 | 26.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,690,560 | 73.9% |
| LOAD_FAST | 3,732,480 | 21.7% |
| STORE_FAST | 746,480 | 4.3% |


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
| RETURN_VALUE | 83,310,940 | 65.0% |
| RETURN_CONST | 38,818,440 | 30.3% |
| YIELD_VALUE | 4,478,960 | 3.5% |
| RETURN_GENERATOR | 1,492,960 | 1.2% |


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
| STORE_FAST | 3,734,480 | 83.3% |
| STORE_ATTR_INSTANCE_VALUE | 746,460 | 16.6% |
| RESUME_CHECK | 1,660 | 0.0% |
| POP_TOP | 400 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,482,800 | 100.0% |
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
| RETURN_CONST | 53,754,120 | 36.0% |
| CALL_METHOD_DESCRIPTOR_O | 31,353,060 | 21.0% |
| CALL_FUNCTION_EX | 17,169,520 | 11.5% |
| END_SEND | 12,690,560 | 8.5% |
| SEND_GEN | 12,690,420 | 8.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,005,000 | 35.5% |
| RETURN_CONST | 28,367,960 | 19.0% |
| LOAD_CONST | 21,650,900 | 14.5% |
| RESUME_CHECK | 17,169,360 | 11.5% |
| ENTER_EXECUTOR | 17,169,020 | 11.5% |


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
| LOAD_ATTR_MODULE | 50,765,260 | 86.1% |
| LOAD_FAST | 4,479,380 | 7.6% |
| LOAD_ATTR | 3,734,720 | 6.3% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 21,648,560 | 36.7% |
| CALL | 16,426,140 | 27.9% |
| LOAD_FAST | 16,425,420 | 27.8% |
| LOAD_GLOBAL_MODULE | 3,732,440 | 6.3% |
| CALL_ALLOC_AND_ENTER_INIT | 746,440 | 1.3% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 11,943,840 | 69.6% |
| CALL_PY_WITH_DEFAULTS | 3,732,460 | 21.7% |
| CACHE | 1,492,960 | 8.7% |
| CALL | 120 | 0.0% |
| COPY_FREE_VARS | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 11,197,600 | 65.2% |
| CALL | 4,478,920 | 26.1% |
| INTERPRETER_EXIT | 1,492,960 | 8.7% |
| CALL_PY_EXACT_ARGS | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_FLOAT | 57,183,420 | 39.8% |
| LOAD_FAST | 44,045,780 | 30.6% |
| LOAD_ATTR_INSTANCE_VALUE | 29,860,260 | 20.8% |
| CALL_KW | 4,478,960 | 3.1% |
| CALL | 3,734,700 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 83,310,940 | 57.9% |
| STORE_FAST | 25,383,280 | 17.7% |
| TO_BOOL_BOOL | 20,902,400 | 14.5% |
| LOAD_FAST | 4,480,800 | 3.1% |
| POP_TOP | 4,479,120 | 3.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 66.7% |
| LOAD_FAST | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20 | 33.3% |
| LOAD_FAST | 20 | 33.3% |
| STORE_SUBSCR_DICT | 20 | 33.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 11,199,440 | 99.9% |
| TO_BOOL | 3,800 | 0.0% |
| LOAD_ATTR | 800 | 0.0% |
| RETURN_VALUE | 480 | 0.0% |
| CALL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,719,520 | 60.0% |
| POP_JUMP_IF_TRUE | 4,480,980 | 40.0% |
| TO_BOOL | 3,800 | 0.0% |
| TO_BOOL_BOOL | 1,000 | 0.0% |
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
| LOAD_FAST | 240 | 22.2% |
| LOAD_GLOBAL_MODULE | 180 | 16.7% |
| UNARY_INVERT | 160 | 14.8% |
| BINARY_OP | 160 | 14.8% |
| LOAD_CONST | 120 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 220 | 20.4% |
| BINARY_OP | 160 | 14.8% |
| COPY | 160 | 14.8% |
| LOAD_GLOBAL_MODULE | 120 | 11.1% |
| UNARY_INVERT | 80 | 7.4% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,732,480 | 83.3% |
| STORE_ATTR_INSTANCE_VALUE | 746,680 | 16.7% |
| STORE_FAST | 1,840 | 0.0% |
| LOAD_ATTR_SLOT | 1,620 | 0.0% |
| STORE_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,480,840 | 100.0% |
| STORE_FAST | 1,840 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,732,480 | 100.0% |
| STORE_ATTR_INSTANCE_VALUE | 140 | 0.0% |
| POP_TOP | 80 | 0.0% |
| BUILD_TUPLE | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 3,732,480 | 100.0% |
| LOAD_FAST | 400 | 0.0% |


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
| LOAD_FAST_LOAD_FAST | 17,169,560 | 28.7% |
| PUSH_NULL | 16,426,140 | 27.5% |
| LOAD_ATTR | 8,959,720 | 15.0% |
| LOAD_FAST | 7,467,000 | 12.5% |
| LOAD_ATTR_INSTANCE_VALUE | 4,479,120 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 33,592,920 | 56.2% |
| POP_TOP | 8,958,640 | 15.0% |
| RESUME_CHECK | 8,212,040 | 13.7% |
| CALL_METHOD_DESCRIPTOR_O | 4,479,100 | 7.5% |
| RETURN_VALUE | 3,734,700 | 6.3% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,167,700 | 82.1% |
| BUILD_MAP | 3,732,480 | 17.9% |
| CALL_INTRINSIC_1 | 1,640 | 0.0% |
| DICT_MERGE | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 17,169,520 | 82.1% |
| STORE_FAST | 3,732,480 | 17.9% |
| COPY_FREE_VARS | 80 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 3,734,120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,732,480 | 100.0% |
| CALL_FUNCTION_EX | 1,640 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,436,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,478,960 | 33.3% |
| STORE_FAST | 4,478,960 | 33.3% |
| RESUME_CHECK | 4,478,940 | 33.3% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,732,780 | 100.0% |
| COMPARE_OP | 1,180 | 0.0% |
| CALL_BUILTIN_CLASS | 140 | 0.0% |
| LOAD_GLOBAL_MODULE | 100 | 0.0% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,733,000 | 100.0% |
| COMPARE_OP | 1,180 | 0.0% |
| COMPARE_OP_INT | 120 | 0.0% |
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
| CALL_PY_EXACT_ARGS | 3,733,100 | 50.0% |
| CACHE | 3,732,660 | 50.0% |
| CALL | 180 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 7,465,620 | 100.0% |
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
| POP_TOP | 17,169,020 | 100.0% |
| LOAD_FAST | 1,680 | 0.0% |
| POP_JUMP_IF_FALSE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 17,167,700 | 100.0% |
| FOR_ITER_RANGE | 1,800 | 0.0% |
| LOAD_ATTR_SLOT | 900 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 300 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 0.0% |


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
| RETURN_GENERATOR | 11,197,600 | 65.2% |
| LOAD_FAST | 3,732,480 | 21.7% |
| BEFORE_ASYNC_WITH | 746,480 | 4.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 746,460 | 4.3% |
| LOAD_ATTR_INSTANCE_VALUE | 746,460 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 17,169,520 | 100.0% |


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
| POP_TOP | 4,479,220 | 100.0% |
| POP_JUMP_IF_FALSE | 2,120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 4,479,160 | 100.0% |
| LOAD_FAST | 2,100 | 0.0% |
| FOR_ITER | 40 | 0.0% |
| CALL_FUNCTION_EX | 20 | 0.0% |
| JUMP_FORWARD | 20 | 0.0% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 16,422,880 | 100.0% |
| RESUME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 11,944,040 | 72.7% |
| SEND | 4,479,000 | 27.3% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,482,880 | 100.0% |
| POP_TOP | 100 | 0.0% |
| POP_JUMP_IF_FALSE | 80 | 0.0% |
| ENTER_EXECUTOR | 60 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,481,200 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 1,880 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_FAST_CHECK | 20 | 0.0% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,732,480 | 100.0% |
| LOAD_ATTR_SLOT | 1,620 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 3,734,120 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 38,079,140 | 96.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,493,540 | 3.8% |
| LOAD_ATTR | 13,200 | 0.0% |
| LOAD_ATTR_SLOT | 1,440 | 0.0% |
| LOAD_GLOBAL_MODULE | 960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 13,436,680 | 33.9% |
| CALL | 8,959,720 | 22.6% |
| LOAD_FAST | 8,212,560 | 20.7% |
| TO_BOOL_NONE | 4,478,920 | 11.3% |
| PUSH_NULL | 3,734,720 | 9.4% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 41,803,980 | 28.6% |
| POP_TOP | 21,650,900 | 14.8% |
| POP_JUMP_IF_FALSE | 20,906,000 | 14.3% |
| LOAD_FAST | 17,171,780 | 11.7% |
| GET_AWAITABLE | 17,169,520 | 11.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,118,020 | 56.1% |
| STORE_FAST | 17,925,120 | 12.2% |
| CALL_KW | 13,436,960 | 9.2% |
| SEND_GEN | 12,690,320 | 8.7% |
| COMPARE_OP_INT | 4,481,160 | 3.1% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 7,465,540 | 100.0% |
| LOAD_GLOBAL | 240 | 0.0% |
| STORE_FAST | 160 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,465,780 | 100.0% |
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
| POP_JUMP_IF_FALSE | 143,781,940 | 18.3% |
| RESUME_CHECK | 139,600,520 | 17.8% |
| LOAD_CONST | 82,118,020 | 10.5% |
| STORE_FAST | 60,485,080 | 7.7% |
| LOAD_GLOBAL_BUILTIN | 57,192,000 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 188,274,580 | 24.0% |
| LOAD_ATTR_INSTANCE_VALUE | 155,296,460 | 19.8% |
| STORE_ATTR_SLOT | 70,171,440 | 9.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 62,711,560 | 8.0% |
| LOAD_GLOBAL_MODULE | 60,917,920 | 7.8% |


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
| STORE_ATTR_SLOT | 51,508,260 | 34.5% |
| LOAD_FAST_LOAD_FAST | 25,381,200 | 17.0% |
| PUSH_NULL | 21,648,560 | 14.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 17,915,720 | 12.0% |
| POP_JUMP_IF_NOT_NONE | 13,436,880 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 72,410,040 | 48.5% |
| LOAD_FAST_LOAD_FAST | 25,381,200 | 17.0% |
| LOAD_FAST | 17,169,840 | 11.5% |
| CALL | 17,169,560 | 11.5% |
| LOAD_CONST | 8,957,920 | 6.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME | 560 | 12.6% |
| RESUME_CHECK | 540 | 12.1% |
| POP_TOP | 500 | 11.2% |
| LOAD_FAST | 500 | 11.2% |
| POP_JUMP_IF_FALSE | 460 | 10.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,500 | 33.6% |
| LOAD_ATTR | 940 | 21.1% |
| LOAD_GLOBAL_BUILTIN | 660 | 14.8% |
| LOAD_FAST | 340 | 7.6% |
| CALL | 300 | 6.7% |


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
| TO_BOOL_BOOL | 147,513,880 | 70.2% |
| TO_BOOL_NONE | 42,550,040 | 20.2% |
| TO_BOOL | 6,719,520 | 3.2% |
| TO_BOOL_LIST | 5,229,660 | 2.5% |
| COMPARE_OP_INT | 4,483,080 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 143,781,940 | 68.4% |
| RETURN_CONST | 26,127,900 | 12.4% |
| LOAD_CONST | 20,906,000 | 9.9% |
| LOAD_GLOBAL_MODULE | 15,676,840 | 7.5% |
| LOAD_FAST_LOAD_FAST | 3,732,580 | 1.8% |


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
| LOAD_FAST | 33,594,560 | 83.3% |
| LOAD_ATTR_INSTANCE_VALUE | 6,718,340 | 16.7% |
| LOAD_GLOBAL_MODULE | 220 | 0.0% |
| LOAD_ATTR | 80 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 13,436,880 | 33.3% |
| LOAD_FAST | 12,692,420 | 31.5% |
| LOAD_GLOBAL_MODULE | 8,958,240 | 22.2% |
| RETURN_CONST | 4,478,880 | 11.1% |
| LOAD_CONST | 746,500 | 1.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 12,690,920 | 73.9% |
| TO_BOOL | 4,480,980 | 26.1% |
| TO_BOOL_INT | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,437,220 | 78.2% |
| LOAD_CONST | 3,734,320 | 21.7% |
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
| POP_TOP | 28,367,960 | 27.9% |
| POP_JUMP_IF_FALSE | 26,127,900 | 25.7% |
| STORE_ATTR_SLOT | 24,634,560 | 24.3% |
| STORE_FAST | 17,171,200 | 16.9% |
| POP_JUMP_IF_NOT_NONE | 4,478,880 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 53,754,120 | 52.9% |
| INTERPRETER_EXIT | 38,818,440 | 38.2% |
| END_SEND | 8,211,600 | 8.1% |
| EXIT_INIT_CHECK | 746,460 | 0.7% |
| TO_BOOL | 40 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,479,200 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 4,479,000 | 50.0% |
| SEND | 2,580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 4,478,960 | 50.0% |
| YIELD_VALUE | 4,478,960 | 50.0% |
| SEND | 2,580 | 0.0% |
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
| CALL | 33,592,920 | 37.2% |
| RETURN_VALUE | 25,383,280 | 28.1% |
| LOAD_CONST | 17,925,120 | 19.8% |
| FOR_ITER_RANGE | 4,480,960 | 5.0% |
| CALL_KW | 4,478,960 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,485,080 | 66.9% |
| RETURN_CONST | 17,171,200 | 19.0% |
| JUMP_FORWARD | 4,482,880 | 5.0% |
| NOP | 3,734,480 | 4.1% |
| LOAD_FAST_LOAD_FAST | 3,732,800 | 4.1% |


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
| YIELD_VALUE | 11,944,080 | 72.7% |
| SEND | 4,478,960 | 27.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 11,944,080 | 72.7% |
| INTERPRETER_EXIT | 4,478,960 | 27.3% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,100 | 55.6% |
| CACHE | 340 | 17.2% |
| COPY_FREE_VARS | 240 | 12.1% |
| POP_TOP | 160 | 8.1% |
| SEND_GEN | 100 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 940 | 47.5% |
| LOAD_GLOBAL | 560 | 28.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 160 | 8.1% |
| LOAD_CONST | 140 | 7.1% |
| NOP | 100 | 5.1% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,732,440 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 1,800 | 0.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,732,460 | 100.0% |
| STORE_FAST | 1,820 | 0.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 66.7% |
| BINARY_OP | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 33.3% |
| BINARY_OP | 40 | 33.3% |
| LOAD_FAST | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 120 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,478,880 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,478,840 | 100.0% |
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
| LOAD_CONST | 600 | 90.9% |
| BINARY_SUBSCR | 60 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 460 | 69.7% |
| LOAD_ATTR_SLOT | 160 | 24.2% |
| LOAD_ATTR | 40 | 6.1% |


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
| LOAD_CONST | 746,440 | 98.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 1.9% |
| PUSH_NULL | 40 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 746,460 | 98.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 14,340 | 1.9% |
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
| LOAD_FAST | 3,732,440 | 100.0% |
| LOAD_CONST | 180 | 0.0% |
| CALL | 60 | 0.0% |
| LOAD_FAST_LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,732,460 | 100.0% |
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
| LOAD_FAST | 3,732,480 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.0% |
| CALL | 80 | 0.0% |
| LOAD_CONST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,732,440 | 100.0% |
| STORE_FAST | 460 | 0.0% |
| POP_TOP | 120 | 0.0% |
| TO_BOOL | 20 | 0.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 57,183,440 | 100.0% |
| LOAD_GLOBAL_BUILTIN | 380 | 0.0% |
| CALL | 80 | 0.0% |
| BUILD_TUPLE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 57,183,860 | 100.0% |
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
| LOAD_FAST_LOAD_FAST | 120 | 60.0% |
| RETURN_VALUE | 40 | 20.0% |
| CALL | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 140 | 70.0% |
| STORE_FAST | 60 | 30.0% |


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
| LOAD_ATTR | 13,436,680 | 100.0% |
| LOAD_ATTR_METHOD_NO_DICT | 2,520 | 0.0% |
| CALL | 380 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 13,436,640 | 100.0% |
| STORE_FAST | 2,100 | 0.0% |
| POP_TOP | 380 | 0.0% |
| GET_ITER | 160 | 0.0% |
| CALL | 140 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,873,880 | 85.7% |
| CALL | 4,479,100 | 14.3% |
| LOAD_CONST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 31,353,060 | 100.0% |
| LOAD_CONST | 20 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 58,230,960 | 63.9% |
| LOAD_FAST | 17,174,040 | 18.9% |
| BINARY_OP_SUBTRACT_INT | 4,478,840 | 4.9% |
| LOAD_ATTR_METHOD_NO_DICT | 3,733,560 | 4.1% |
| LOAD_SUPER_ATTR_METHOD | 3,732,640 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 75,407,820 | 82.8% |
| RETURN_GENERATOR | 11,943,840 | 13.1% |
| COPY_FREE_VARS | 3,733,100 | 4.1% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,732,440 | 100.0% |
| CALL | 120 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 0.0% |
| LOAD_FAST | 80 | 0.0% |
| PUSH_NULL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 3,732,460 | 100.0% |
| RESUME_CHECK | 380 | 0.0% |


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
| LOAD_ATTR_SLOT | 57,183,400 | 100.0% |
| LOAD_FAST | 440 | 0.0% |
| LOAD_GLOBAL_MODULE | 120 | 0.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 57,183,420 | 100.0% |
| POP_JUMP_IF_FALSE | 600 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,481,160 | 100.0% |
| LOAD_GLOBAL_MODULE | 1,800 | 0.0% |
| COMPARE_OP | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,483,080 | 100.0% |


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
| JUMP_BACKWARD | 4,479,160 | 85.7% |
| GET_ITER | 748,280 | 14.3% |
| ENTER_EXECUTOR | 1,800 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,480,960 | 85.7% |
| LOAD_CONST | 748,320 | 14.3% |


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
| LOAD_FAST | 155,296,460 | 97.2% |
| LOAD_FAST_LOAD_FAST | 4,479,120 | 2.8% |
| LOAD_ATTR | 2,000 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| COPY | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 53,749,900 | 33.6% |
| LOAD_ATTR_METHOD_NO_DICT | 31,357,380 | 19.6% |
| RETURN_VALUE | 29,860,260 | 18.7% |
| TO_BOOL | 11,199,440 | 7.0% |
| POP_JUMP_IF_NOT_NONE | 6,718,340 | 4.2% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 31,357,380 | 89.4% |
| LOAD_FAST | 3,733,500 | 10.6% |
| LOAD_ATTR | 580 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,874,160 | 76.6% |
| LOAD_GLOBAL_MODULE | 4,478,960 | 12.8% |
| CALL_PY_EXACT_ARGS | 3,733,560 | 10.6% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,520 | 0.0% |
| LOAD_FAST_LOAD_FAST | 1,960 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,711,560 | 67.7% |
| LOAD_ATTR_SLOT | 24,634,360 | 26.6% |
| LOAD_ATTR_INSTANCE_VALUE | 5,227,400 | 5.6% |
| LOAD_ATTR | 1,240 | 0.0% |
| RETURN_VALUE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 58,230,960 | 62.9% |
| LOAD_FAST_LOAD_FAST | 17,915,720 | 19.4% |
| LOAD_FAST | 16,427,220 | 17.7% |
| CALL | 720 | 0.0% |
| LOAD_CONST | 120 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 54,497,320 | 100.0% |
| LOAD_ATTR | 960 | 0.0% |
| LOAD_FAST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 50,765,260 | 93.2% |
| LOAD_FAST_LOAD_FAST | 3,732,460 | 6.8% |
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
| LOAD_FAST | 188,274,580 | 100.0% |
| ENTER_EXECUTOR | 900 | 0.0% |
| LOAD_ATTR | 500 | 0.0% |
| LOAD_ATTR_SLOT | 200 | 0.0% |
| BINARY_SUBSCR_LIST_INT | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,183,940 | 30.4% |
| COMPARE_OP_FLOAT | 57,183,400 | 30.4% |
| TO_BOOL_NONE | 38,071,000 | 20.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 24,634,360 | 13.1% |
| TO_BOOL_BOOL | 11,198,220 | 5.9% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60,918,720 | 92.1% |
| POP_TOP | 3,732,640 | 5.6% |
| STORE_FAST | 748,300 | 1.1% |
| STORE_ATTR_INSTANCE_VALUE | 746,580 | 1.1% |
| JUMP_FORWARD | 1,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,192,000 | 86.5% |
| LOAD_DEREF | 7,465,540 | 11.3% |
| CALL_BUILTIN_CLASS | 746,660 | 1.1% |
| LOAD_GLOBAL_MODULE | 746,480 | 1.1% |
| CALL_ISINSTANCE | 380 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,917,920 | 50.5% |
| RESUME_CHECK | 25,383,180 | 21.0% |
| POP_JUMP_IF_FALSE | 15,676,840 | 13.0% |
| POP_JUMP_IF_NOT_NONE | 8,958,240 | 7.4% |
| LOAD_ATTR_METHOD_NO_DICT | 4,478,960 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 57,183,440 | 47.4% |
| LOAD_ATTR_MODULE | 54,497,320 | 45.2% |
| LOAD_FAST_LOAD_FAST | 4,479,200 | 3.7% |
| CALL_PY_WITH_DEFAULTS | 3,732,440 | 3.1% |
| CALL_BUILTIN_CLASS | 746,440 | 0.6% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,465,320 | 100.0% |
| LOAD_SUPER_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,732,640 | 50.0% |
| LOAD_FAST_LOAD_FAST | 3,732,520 | 50.0% |
| LOAD_FAST | 260 | 0.0% |
| CALL | 120 | 0.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 118,396,380 | 48.6% |
| CALL_PY_EXACT_ARGS | 75,407,820 | 30.9% |
| POP_TOP | 17,169,360 | 7.0% |
| SEND_GEN | 11,943,980 | 4.9% |
| CALL | 8,212,040 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 139,600,520 | 57.3% |
| LOAD_GLOBAL_BUILTIN | 60,918,720 | 25.0% |
| LOAD_GLOBAL_MODULE | 25,383,180 | 10.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 16,422,880 | 6.7% |
| LOAD_CONST | 1,493,380 | 0.6% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,690,320 | 51.5% |
| JUMP_BACKWARD_NO_INTERRUPT | 11,944,040 | 48.5% |
| SEND | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 12,690,420 | 51.5% |
| RESUME_CHECK | 11,943,980 | 48.5% |
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
| LOAD_FAST_LOAD_FAST | 72,410,040 | 50.8% |
| LOAD_FAST | 70,171,440 | 49.2% |
| STORE_ATTR_SLOT | 1,120 | 0.0% |
| STORE_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 51,508,260 | 36.1% |
| LOAD_CONST | 41,803,980 | 29.3% |
| LOAD_FAST | 24,635,020 | 17.3% |
| RETURN_CONST | 24,634,560 | 17.3% |
| STORE_ATTR_SLOT | 1,120 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 66.7% |
| STORE_SUBSCR | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 57,183,860 | 35.7% |
| LOAD_ATTR_INSTANCE_VALUE | 53,749,900 | 33.6% |
| RETURN_VALUE | 20,902,400 | 13.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 13,436,640 | 8.4% |
| LOAD_ATTR_SLOT | 11,198,220 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 147,513,880 | 92.1% |
| POP_JUMP_IF_TRUE | 12,690,920 | 7.9% |
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
| LOAD_ATTR_INSTANCE_VALUE | 5,229,540 | 100.0% |
| TO_BOOL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,229,660 | 100.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 38,071,000 | 89.5% |
| LOAD_ATTR | 4,478,920 | 10.5% |
| TO_BOOL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 42,550,040 | 100.0% |


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
|     deferred | 780 | 0.0% |
|          hit | 8,213,380 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 46.7% |
| Failure | 160 | 53.3% |

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
|     deferred | 80 | 7.5% |
|          hit | 900 | 84.9% |

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
|     deferred | 60,473,900 | 22.6% |
|          hit | 207,255,920 | 77.4% |
|         miss | 761,180 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 17,280 | 49.1% |
| Failure | 17,900 | 50.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 4,600 | 25.7% |
| meth descr method fastcall keywords | 4,100 | 22.9% |
| cfunc noargs | 3,840 | 21.5% |
| code complex parameters | 2,440 | 13.6% |
| class no vectorcall | 1,340 | 7.5% |
| other | 1,280 | 7.2% |
| class mutable | 80 | 0.4% |
| metaclass | 60 | 0.3% |
| wrong number arguments | 40 | 0.2% |
| cfunc varargs | 40 | 0.2% |
| operator wrapper | 40 | 0.2% |
| cmethod | 20 | 0.1% |
| cfunc varargs keywords | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,733,040 | 5.7% |
|          hit | 61,667,120 | 94.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 13.2% |
| Failure | 1,180 | 86.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| float long | 1,140 | 96.6% |
| bool | 40 | 3.4% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 260 | 0.0% |
|          hit | 5,233,020 | 100.0% |

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
|     deferred | 39,584,860 | 6.9% |
|          hit | 530,206,940 | 93.0% |
|         miss | 12,620 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,520 | 30.9% |
| Failure | 12,340 | 69.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 8,200 | 66.5% |
| method | 2,620 | 21.2% |
| class attr descriptor | 1,280 | 10.4% |
| not managed dict | 140 | 1.1% |
| metaclass attribute | 60 | 0.5% |
| class attr simple | 40 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,380 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 186,795,120 | 100.0% |
|         miss | 80 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,160 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 240 | 0.0% |
|          hit | 7,465,540 | 100.0% |

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
|     deferred | 8,958,060 | 26.7% |
|          hit | 24,634,500 | 73.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 140 | 5.1% |
| Failure | 2,580 | 94.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 2,580 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60,460 | 0.0% |
|          hit | 154,469,980 | 100.0% |
|         miss | 59,600 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,740 | 96.5% |
| Failure | 100 | 3.5% |

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
|     deferred | 40 | 33.3% |
|          hit | 60 | 50.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,200,540 | 5.1% |
|          hit | 207,986,760 | 94.9% |

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
| Basic | 1,933,632,640 | 48.6% |
| Not specialized | 404,404,580 | 10.2% |
| Specialized hits | 1,637,676,200 | 41.2% |
| Specialized misses | 907,760 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 60,473,900 | 48.8% |
| LOAD_ATTR | 39,584,860 | 31.9% |
| TO_BOOL | 11,200,540 | 9.0% |
| SEND | 8,958,060 | 7.2% |
| COMPARE_OP | 3,733,040 | 3.0% |
| STORE_ATTR | 60,460 | 0.0% |
| LOAD_GLOBAL | 2,380 | 0.0% |
| BINARY_OP | 780 | 0.0% |
| FOR_ITER | 260 | 0.0% |
| LOAD_SUPER_ATTR | 240 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 760,800 | 77.5% |
| RESUME | 74,280 | 7.6% |
| RESUME_CHECK | 74,280 | 7.6% |
| STORE_ATTR_SLOT | 59,600 | 6.1% |
| LOAD_ATTR_SLOT | 12,000 | 1.2% |
| LOAD_ATTR_METHOD_NO_DICT | 620 | 0.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 260 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 120 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 80 | 0.0% |
| CACHE | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 128,101,300 | 49.1% |
| Calls to Python functions inlined | 132,891,320 | 50.9% |
| Calls via PyEval_EvalFrame (total) | 128,101,300 | 49.1% |
| Calls via PyEval_EvalFrame (vector) | 119,143,380 | 45.7% |
| Calls via PyEval_EvalFrame (generator) | 8,957,920 | 3.4% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 119,143,380 | 45.7% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 57,183,440 | 21.9% |
| Calls via PyEval_EvalFrame (function ex) | 80 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 4,479,100 | 1.7% |
| Calls via PyEval_EvalFrame (method) | 26,873,760 | 10.3% |
| Frame objects created | 180 | 0.0% |
| Frames pushed | 113,478,980 | 43.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 106,777,294 | 38.1% |
| Frees to freelist | 107,301,360 |  |
| Allocations | 173,513,964 | 61.9% |
| Allocations to 512 bytes | 172,651,801 | 61.6% |
| Allocations to 4 kbytes | 862,060 | 0.3% |
| Allocations over 4 kbytes | 103 | 0.0% |
| Frees | 173,428,994 |  |
| New values | 440 |  |
| Interpreter increfs | 2,598,387,780 | 78.6% |
| Interpreter decrefs | 2,730,313,711 | 77.1% |
| Increfs | 709,215,697 | 21.4% |
| Decrefs | 813,136,947 | 22.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 98,631,245 |  |
| Method cache misses | 4,295 |  |
| Method cache collisions | 4,044 |  |
| Method cache dunder hits | 75,847,191 |  |
| Method cache dunder misses | 469 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 94,972 | 2,040 | 678,346,162 |
| 1 | 8,640 | 0 | 731,769,932 |
| 2 | 660 | 0 | 2,417,370,454 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 2,380 |  |
| Traces created | 2,460 | 103.4% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 536,500 | 22,542.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 2,300 | 96.6% |
| Low confidence | 0 | 0.0% |
| Traces executed | 49,266,840 |  |
| Uops executed | 1,333,872,660 | 27.07 |

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
| <= 32 | 60 | 2.4% |
| <= 64 | 2,340 | 95.1% |
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
| <= 512 | 40 | 1.6% |
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
| <= 4 | 1,820 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 14,926,840 | 30.3% |
| <= 32 | 3,732,400 | 7.6% |
| <= 64 | 13,436,460 | 27.3% |
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
| <= 131,072 | 0 | 0.0% |
| <= 262,144 | 0 | 0.0% |
| <= 524,288 | 80 | 0.0% |
| <= 1,048,576 | 0 | 0.0% |
| <= 2,097,152 | 2 | 0.0% |
| <= 4,194,304 | 78 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _GUARD_TYPE_VERSION | 163,467,180 | 12.3% | 12.3% | 9.1% |
| LOAD_FAST | 150,032,020 | 11.2% | 23.5% |  |
| _SET_IP | 129,134,080 | 9.7% | 33.2% |  |
| _CHECK_VALIDITY | 125,400,120 | 9.4% | 42.6% |  |
| _LOAD_ATTR_SLOT | 61,207,560 | 4.6% | 47.2% |  |
| _CHECK_VALIDITY_AND_SET_IP | 58,966,100 | 4.4% | 51.6% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 49,263,940 | 3.7% | 55.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 49,263,940 | 3.7% | 59.0% |  |
| STORE_FAST | 41,798,560 | 3.1% | 62.1% |  |
| _GUARD_IS_FALSE_POP | 38,069,320 | 2.9% | 65.0% | 0.0% |
| TO_BOOL_BOOL | 34,337,240 | 2.6% | 67.5% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 34,335,700 | 2.6% | 70.1% |  |
| _START_EXECUTOR | 32,097,680 | 2.4% | 72.5% |  |
| _LOAD_ATTR | 32,096,480 | 2.4% | 74.9% |  |
| PUSH_NULL | 20,900,020 | 1.6% | 76.5% |  |
| _COLD_EXIT | 17,169,160 | 1.3% | 77.8% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 17,169,040 | 1.3% | 79.1% | 0.0% |
| _ITER_CHECK_RANGE | 17,169,040 | 1.3% | 80.4% |  |
| RESUME_CHECK | 17,168,320 | 1.3% | 81.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 17,168,320 | 1.3% | 82.9% |  |
| _CHECK_STACK_SPACE | 17,168,320 | 1.3% | 84.2% |  |
| _INIT_CALL_PY_EXACT_ARGS | 17,168,320 | 1.3% | 85.5% |  |
| _PUSH_FRAME | 17,168,320 | 1.3% | 86.8% |  |
| _SAVE_RETURN_OFFSET | 17,168,320 | 1.3% | 88.1% |  |
| _EXIT_TRACE | 17,167,720 | 1.3% | 89.4% | 100.0% |
| BUILD_LIST | 17,167,720 | 1.3% | 90.7% |  |
| CALL_INTRINSIC_1 | 17,167,720 | 1.3% | 91.9% |  |
| LIST_EXTEND | 17,167,720 | 1.3% | 93.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 17,167,240 | 1.3% | 94.5% |  |
| _ITER_NEXT_RANGE | 17,167,240 | 1.3% | 95.8% |  |
| _LOAD_CONST_INLINE_BORROW | 7,464,080 | 0.6% | 96.4% |  |
| BINARY_SUBSCR_LIST_INT | 3,732,080 | 0.3% | 96.6% |  |
| COMPARE_OP_FLOAT | 3,732,080 | 0.3% | 96.9% |  |
| _GUARD_IS_TRUE_POP | 3,732,000 | 0.3% | 97.2% | 0.0% |
| POP_TOP | 3,732,000 | 0.3% | 97.5% |  |
| CALL_BUILTIN_O | 3,732,000 | 0.3% | 97.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 3,732,000 | 0.3% | 98.0% |  |
| TO_BOOL_LIST | 3,732,000 | 0.3% | 98.3% |  |
| _CHECK_ATTR_MODULE | 3,732,000 | 0.3% | 98.6% |  |
| _LOAD_ATTR_MODULE | 3,732,000 | 0.3% | 98.9% |  |
| _STORE_ATTR_SLOT | 3,732,000 | 0.3% | 99.2% |  |
| _LOAD_CONST_INLINE | 3,732,000 | 0.3% | 99.4% |  |
| _CHECK_GLOBALS | 3,732,000 | 0.3% | 99.7% |  |
| _JUMP_TO_TOP | 3,731,920 | 0.3% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 20 | 0.0% | 100.0% | 100.0% |
| _ITER_CHECK_TUPLE | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL_FUNCTION_EX | 536,600 |


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
