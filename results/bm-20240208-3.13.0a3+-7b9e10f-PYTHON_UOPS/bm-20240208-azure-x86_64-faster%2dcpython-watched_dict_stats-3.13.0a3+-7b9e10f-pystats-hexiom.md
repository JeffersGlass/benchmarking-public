
# Pystats results

- benchmark: hexiom
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 97,263,980 | 13.3% | 13.3% |  |
| RESUME_CHECK | 60,348,900 | 8.2% | 21.5% |  |
| ENTER_EXECUTOR | 56,007,820 | 7.6% | 29.2% |  |
| LOAD_CONST | 49,125,520 | 6.7% | 35.9% |  |
| POP_TOP | 39,334,380 | 5.4% | 41.2% |  |
| INTERPRETER_EXIT | 38,299,740 | 5.2% | 46.5% |  |
| YIELD_VALUE | 36,383,120 | 5.0% | 51.4% |  |
| BINARY_SUBSCR_LIST_INT | 34,912,120 | 4.8% | 56.2% |  |
| STORE_FAST | 32,323,440 | 4.4% | 60.6% |  |
| LOAD_ATTR_INSTANCE_VALUE | 32,270,200 | 4.4% | 65.0% |  |
| POP_JUMP_IF_FALSE | 24,710,140 | 3.4% | 68.4% |  |
| COMPARE_OP_INT | 24,329,120 | 3.3% | 71.7% |  |
| RETURN_VALUE | 19,543,400 | 2.7% | 74.4% |  |
| LOAD_FAST_LOAD_FAST | 16,828,160 | 2.3% | 76.7% |  |
| CALL_PY_EXACT_ARGS | 13,515,960 | 1.8% | 78.5% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 11,816,760 | 1.6% | 80.1% |  |
| LOAD_GLOBAL_BUILTIN | 11,712,100 | 1.6% | 81.7% |  |
| FOR_ITER_LIST | 10,499,140 | 1.4% | 83.2% | 0.1% |
| TO_BOOL_BOOL | 9,943,500 | 1.4% | 84.5% |  |
| CALL_LEN | 9,372,300 | 1.3% | 85.8% |  |
| BINARY_SUBSCR_GETITEM | 9,245,180 | 1.3% | 87.0% |  |
| BINARY_OP_ADD_INT | 8,971,100 | 1.2% | 88.3% |  |
| LOAD_GLOBAL_MODULE | 8,873,900 | 1.2% | 89.5% |  |
| POP_JUMP_IF_TRUE | 8,465,120 | 1.2% | 90.6% |  |
| JUMP_FORWARD | 8,317,720 | 1.1% | 91.8% |  |
| GET_ITER | 6,634,020 | 0.9% | 92.7% |  |
| LOAD_DEREF | 5,924,940 | 0.8% | 93.5% |  |
| CONTAINS_OP | 5,608,860 | 0.8% | 94.3% |  |
| FOR_ITER_RANGE | 5,164,580 | 0.7% | 95.0% | 0.2% |
| RETURN_CONST | 4,976,220 | 0.7% | 95.6% |  |
| SWAP | 4,047,760 | 0.6% | 96.2% |  |
| COPY | 3,260,560 | 0.4% | 96.6% |  |
| CALL_BUILTIN_CLASS | 2,779,460 | 0.4% | 97.0% |  |
| RETURN_GENERATOR | 1,914,960 | 0.3% | 97.3% |  |
| COPY_FREE_VARS | 1,914,960 | 0.3% | 97.5% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,860 | 0.3% | 97.8% |  |
| STORE_SUBSCR_LIST_INT | 1,869,480 | 0.3% | 98.1% |  |
| BINARY_OP_SUBTRACT_INT | 1,637,780 | 0.2% | 98.3% |  |
| BUILD_TUPLE | 1,347,420 | 0.2% | 98.5% |  |
| MAKE_FUNCTION | 1,233,180 | 0.2% | 98.6% |  |
| SET_FUNCTION_ATTRIBUTE | 1,233,100 | 0.2% | 98.8% |  |
| BUILD_LIST | 974,060 | 0.1% | 98.9% |  |
| STORE_ATTR_INSTANCE_VALUE | 944,360 | 0.1% | 99.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 920,820 | 0.1% | 99.2% |  |
| POP_JUMP_IF_NOT_NONE | 678,720 | 0.1% | 99.3% |  |
| CALL_LIST_APPEND | 597,700 | 0.1% | 99.4% |  |
| EXTENDED_ARG | 553,620 | 0.1% | 99.4% |  |
| BINARY_SLICE | 549,720 | 0.1% | 99.5% |  |
| CALL_METHOD_DESCRIPTOR_O | 466,280 | 0.1% | 99.6% |  |
| EXIT_INIT_CHECK | 313,480 | 0.0% | 99.6% |  |
| CALL_ALLOC_AND_ENTER_INIT | 313,480 | 0.0% | 99.7% |  |
| STORE_DEREF | 277,660 | 0.0% | 99.7% |  |
| MAKE_CELL | 257,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 255,000 | 0.0% | 99.8% |  |
| LOAD_ATTR_CLASS | 250,860 | 0.0% | 99.8% |  |
| LIST_APPEND | 209,740 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 208,640 | 0.0% | 99.9% |  |
| STORE_FAST_LOAD_FAST | 208,500 | 0.0% | 99.9% |  |
| CALL_PY_WITH_DEFAULTS | 206,000 | 0.0% | 99.9% |  |
| STORE_FAST_STORE_FAST | 143,760 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 143,700 | 0.0% | 100.0% |  |
| NOP | 114,320 | 0.0% | 100.0% |  |
| CALL_KW | 38,400 | 0.0% | 100.0% |  |
| BINARY_OP | 32,440 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 24,280 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 23,760 | 0.0% | 100.0% |  |
| CALL_STR_1 | 15,320 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 14,280 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 14,220 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 8,760 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 7,900 | 0.0% | 100.0% |  |
| CALL | 7,440 | 0.0% | 100.0% |  |
| LOAD_ATTR | 4,760 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,240 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 2,120 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,980 | 0.0% | 100.0% |  |
| COMPARE_OP | 1,560 | 0.0% | 100.0% |  |
| FOR_ITER | 1,560 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,320 | 0.0% | 100.0% |  |
| BUILD_MAP | 1,280 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,260 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 1,260 | 0.0% | 100.0% |  |
| TO_BOOL | 960 | 0.0% | 100.0% |  |
| PUSH_NULL | 860 | 0.0% | 100.0% |  |
| RESUME | 700 | 0.0% | 100.0% |  |
| LOAD_ATTR_MODULE | 600 | 0.0% | 100.0% |  |
| STORE_ATTR | 560 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 400 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 160 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 120 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| POP_TOP ENTER_EXECUTOR | 36,421,680 | 5.0% | 5.0% |
| CACHE RESUME_CHECK | 36,384,640 | 5.0% | 9.9% |
| YIELD_VALUE INTERPRETER_EXIT | 36,383,120 | 5.0% | 14.9% |
| RESUME_CHECK POP_TOP | 36,383,080 | 5.0% | 19.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 27,740,540 | 3.8% | 23.7% |
| ENTER_EXECUTOR YIELD_VALUE | 26,362,620 | 3.6% | 27.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 22,411,120 | 3.1% | 30.3% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 22,017,500 | 3.0% | 33.3% |
| STORE_FAST LOAD_FAST | 17,410,020 | 2.4% | 35.7% |
| RESUME_CHECK LOAD_FAST | 13,854,340 | 1.9% | 37.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 13,121,600 | 1.8% | 39.4% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 12,027,820 | 1.6% | 41.0% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 11,245,400 | 1.5% | 42.6% |
| LOAD_CONST COMPARE_OP_INT | 11,055,240 | 1.5% | 44.1% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 10,559,720 | 1.4% | 45.5% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 10,532,560 | 1.4% | 46.9% |
| BINARY_SUBSCR_GETITEM RESUME_CHECK | 9,245,180 | 1.3% | 48.2% |
| CALL_LEN LOAD_CONST | 9,198,240 | 1.3% | 49.5% |
| POP_JUMP_IF_FALSE LOAD_FAST | 9,118,600 | 1.2% | 50.7% |
| LOAD_FAST LOAD_CONST | 8,884,200 | 1.2% | 51.9% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 8,854,400 | 1.2% | 53.1% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 8,797,300 | 1.2% | 54.3% |
| LOAD_CONST BINARY_OP_ADD_INT | 8,779,480 | 1.2% | 55.5% |
| BINARY_OP_ADD_INT STORE_FAST | 8,770,340 | 1.2% | 56.7% |
| JUMP_FORWARD YIELD_VALUE | 8,189,440 | 1.1% | 57.8% |
| LOAD_CONST JUMP_FORWARD | 8,189,440 | 1.1% | 59.0% |
| ENTER_EXECUTOR LOAD_CONST | 8,109,820 | 1.1% | 60.1% |
| LOAD_CONST BINARY_SUBSCR_LIST_INT | 7,551,760 | 1.0% | 61.1% |
| LOAD_GLOBAL_MODULE COMPARE_OP_INT | 7,317,560 | 1.0% | 62.1% |
| RETURN_VALUE TO_BOOL_BOOL | 7,294,520 | 1.0% | 63.1% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 7,285,980 | 1.0% | 64.1% |
| RETURN_VALUE LOAD_CONST | 7,204,940 | 1.0% | 65.1% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 6,788,580 | 0.9% | 66.0% |
| COMPARE_OP_INT RETURN_VALUE | 6,719,600 | 0.9% | 66.9% |
| BINARY_SUBSCR_LIST_INT CALL_LEN | 6,719,580 | 0.9% | 67.8% |
| STORE_FAST ENTER_EXECUTOR | 6,569,820 | 0.9% | 68.7% |
| LOAD_CONST STORE_FAST | 6,292,540 | 0.9% | 69.6% |
| FOR_ITER_LIST STORE_FAST | 5,695,740 | 0.8% | 70.4% |
| BINARY_SUBSCR_LIST_INT LOAD_GLOBAL_MODULE | 5,642,040 | 0.8% | 71.1% |
| ENTER_EXECUTOR FOR_ITER_LIST | 5,544,920 | 0.8% | 71.9% |
| ENTER_EXECUTOR BINARY_SUBSCR_GETITEM | 4,922,460 | 0.7% | 72.6% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 4,816,740 | 0.7% | 73.2% |
| POP_JUMP_IF_FALSE LOAD_CONST | 4,640,900 | 0.6% | 73.8% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 4,487,920 | 0.6% | 74.5% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 4,415,120 | 0.6% | 75.1% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_GETITEM | 4,299,060 | 0.6% | 75.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 4,298,240 | 0.6% | 76.2% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 3,568,380 | 0.5% | 76.7% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 3,417,720 | 0.5% | 77.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 3,264,380 | 0.4% | 77.6% |
| LOAD_DEREF LOAD_FAST | 3,173,760 | 0.4% | 78.1% |
| LOAD_FAST CONTAINS_OP | 3,173,760 | 0.4% | 78.5% |
| ENTER_EXECUTOR LOAD_FAST | 3,013,420 | 0.4% | 78.9% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 2,669,660 | 0.4% | 79.3% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,657,520 | 0.4% | 79.6% |
| CALL_BUILTIN_CLASS GET_ITER | 2,638,380 | 0.4% | 80.0% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 2,637,220 | 0.4% | 80.4% |
| STORE_FAST LOAD_CONST | 2,628,940 | 0.4% | 80.7% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 2,617,460 | 0.4% | 81.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 2,616,580 | 0.4% | 81.4% |
| ENTER_EXECUTOR FOR_ITER_RANGE | 2,506,140 | 0.3% | 81.8% |
| GET_ITER FOR_ITER_RANGE | 2,494,940 | 0.3% | 82.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST_LOAD_FAST | 2,473,040 | 0.3% | 82.5% |
| LOAD_DEREF BINARY_SUBSCR_LIST_INT | 2,432,100 | 0.3% | 82.8% |
| GET_ITER FOR_ITER_LIST | 2,420,100 | 0.3% | 83.1% |
| LOAD_FAST GET_ITER | 2,418,640 | 0.3% | 83.4% |
| RETURN_CONST TO_BOOL_BOOL | 2,377,300 | 0.3% | 83.8% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 2,376,300 | 0.3% | 84.1% |
| BINARY_SUBSCR_LIST_INT CONTAINS_OP | 2,320,300 | 0.3% | 84.4% |
| FOR_ITER_RANGE STORE_FAST | 2,235,320 | 0.3% | 84.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_DEREF | 2,192,500 | 0.3% | 85.0% |
| LOAD_FAST COMPARE_OP_INT | 2,111,920 | 0.3% | 85.3% |
| RETURN_VALUE LOAD_ATTR_INSTANCE_VALUE | 2,006,640 | 0.3% | 85.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 2,000,540 | 0.3% | 85.8% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,917,900 | 0.3% | 86.1% |
| RETURN_CONST INTERPRETER_EXIT | 1,916,360 | 0.3% | 86.4% |
| BINARY_SUBSCR_LIST_INT LOAD_FAST | 1,916,280 | 0.3% | 86.6% |
| FOR_ITER_LIST RETURN_CONST | 1,916,240 | 0.3% | 86.9% |
| STORE_FAST LOAD_DEREF | 1,915,200 | 0.3% | 87.2% |
| CACHE POP_TOP | 1,914,960 | 0.3% | 87.4% |
| POP_TOP RESUME_CHECK | 1,914,920 | 0.3% | 87.7% |
| LOAD_FAST FOR_ITER_LIST | 1,914,920 | 0.3% | 87.9% |
| COPY_FREE_VARS RETURN_GENERATOR | 1,914,880 | 0.3% | 88.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS STORE_FAST | 1,914,860 | 0.3% | 88.5% |
| RETURN_GENERATOR CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,840 | 0.3% | 88.7% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,904,260 | 0.3% | 89.0% |
| RETURN_VALUE CALL_LEN | 1,864,920 | 0.3% | 89.2% |
| LOAD_CONST YIELD_VALUE | 1,830,720 | 0.2% | 89.5% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BUILTIN_CLASS | 1,776,320 | 0.2% | 89.7% |
| FOR_ITER_RANGE ENTER_EXECUTOR | 1,693,360 | 0.2% | 90.0% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 1,634,600 | 0.2% | 90.2% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 1,631,900 | 0.2% | 90.4% |
| COPY COPY | 1,630,280 | 0.2% | 90.6% |
| SWAP SWAP | 1,630,280 | 0.2% | 90.9% |
| COPY BINARY_SUBSCR_LIST_INT | 1,630,120 | 0.2% | 91.1% |
| SWAP STORE_SUBSCR_LIST_INT | 1,630,120 | 0.2% | 91.3% |
| BINARY_OP_SUBTRACT_INT SWAP | 1,619,360 | 0.2% | 91.5% |
| LOAD_ATTR_INSTANCE_VALUE GET_ITER | 1,510,800 | 0.2% | 91.7% |
| ENTER_EXECUTOR LOAD_FAST_LOAD_FAST | 1,428,440 | 0.2% | 91.9% |
| CONTAINS_OP POP_JUMP_IF_TRUE | 1,308,480 | 0.2% | 92.1% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 546,300 | 99.4% |
| BINARY_OP_ADD_INT | 3,380 | 0.6% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 406,040 | 73.9% |
| LIST_APPEND | 143,680 | 26.1% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 36,384,640 | 95.0% |
| POP_TOP | 1,914,960 | 5.0% |
| RESUME | 140 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 680 | 32.1% |
| LOAD_FAST_LOAD_FAST | 680 | 32.1% |
| LOAD_FAST | 440 | 20.8% |
| COPY | 160 | 7.5% |
| LOAD_DEREF | 120 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 620 | 29.2% |
| LOAD_CONST | 460 | 21.7% |
| BINARY_SUBSCR_GETITEM | 260 | 12.3% |
| CALL | 140 | 6.6% |
| LOAD_GLOBAL | 100 | 4.7% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 313,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 313,480 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,638,380 | 39.8% |
| LOAD_FAST | 2,418,640 | 36.5% |
| LOAD_ATTR_INSTANCE_VALUE | 1,510,800 | 22.8% |
| RETURN_VALUE | 62,700 | 0.9% |
| LOAD_GLOBAL_MODULE | 1,580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 2,494,940 | 37.6% |
| FOR_ITER_LIST | 2,420,100 | 36.5% |
| CALL_PY_EXACT_ARGS | 1,233,100 | 18.6% |
| EXTENDED_ARG | 276,480 | 4.2% |
| LOAD_FAST_AND_CLEAR | 208,640 | 3.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 36,383,120 | 95.0% |
| RETURN_CONST | 1,916,360 | 5.0% |
| RETURN_VALUE | 260 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,233,180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 1,233,100 | 100.0% |
| LOAD_FAST_CHECK | 80 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 113,920 | 99.7% |
| JUMP_BACKWARD | 320 | 0.3% |
| POP_TOP | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 114,160 | 99.9% |
| LOAD_DEREF | 80 | 0.1% |
| LOAD_GLOBAL | 80 | 0.1% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 36,383,080 | 92.5% |
| CACHE | 1,914,960 | 4.9% |
| CALL_METHOD_DESCRIPTOR_O | 466,220 | 1.2% |
| RETURN_CONST | 368,960 | 0.9% |
| SWAP | 162,560 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 36,421,680 | 92.6% |
| RESUME_CHECK | 1,914,920 | 4.9% |
| RETURN_CONST | 609,600 | 1.5% |
| RETURN_VALUE | 162,560 | 0.4% |
| LOAD_GLOBAL_MODULE | 145,760 | 0.4% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 600 | 69.8% |
| LOAD_DEREF | 160 | 18.6% |
| LOAD_ATTR | 100 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 700 | 81.4% |
| LOAD_FAST | 160 | 18.6% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 1,914,880 | 100.0% |
| CALL_PY_EXACT_ARGS | 60 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,914,840 | 100.0% |
| CALL | 80 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 40 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 11,245,400 | 57.5% |
| COMPARE_OP_INT | 6,719,600 | 34.4% |
| LOAD_FAST | 779,600 | 4.0% |
| EXIT_INIT_CHECK | 313,480 | 1.6% |
| RETURN_VALUE | 208,680 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 7,294,520 | 37.3% |
| LOAD_CONST | 7,204,940 | 36.9% |
| LOAD_ATTR_INSTANCE_VALUE | 2,006,640 | 10.3% |
| CALL_LEN | 1,864,920 | 9.5% |
| STORE_FAST | 642,480 | 3.3% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 160 | 40.0% |
| LOAD_FAST | 120 | 30.0% |
| LOAD_ATTR | 40 | 10.0% |
| LOAD_FAST_LOAD_FAST | 40 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR_LIST_INT | 160 | 40.0% |
| LOAD_FAST | 80 | 20.0% |
| LOAD_FAST_LOAD_FAST | 60 | 15.0% |
| JUMP_BACKWARD | 40 | 10.0% |
| STORE_SUBSCR_DICT | 40 | 10.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 680 | 70.8% |
| LOAD_FAST | 160 | 16.7% |
| RETURN_CONST | 120 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 480 | 50.0% |
| POP_JUMP_IF_FALSE | 360 | 37.5% |
| POP_JUMP_IF_TRUE | 120 | 12.5% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,880 | 79.8% |
| BUILD_LIST | 2,560 | 7.9% |
| BINARY_OP_SUBTRACT_INT | 1,500 | 4.6% |
| LOAD_CONST | 1,320 | 4.1% |
| BINARY_OP | 740 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 27,440 | 84.6% |
| STORE_FAST | 1,700 | 5.2% |
| LOAD_FAST | 1,340 | 4.1% |
| BINARY_OP | 740 | 2.3% |
| BINARY_OP_ADD_INT | 580 | 1.8% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 483,920 | 49.7% |
| STORE_FAST | 273,920 | 28.1% |
| SWAP | 208,640 | 21.4% |
| LOAD_FAST_LOAD_FAST | 3,420 | 0.4% |
| LOAD_CONST | 2,560 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 547,840 | 56.2% |
| LOAD_FAST | 209,920 | 21.6% |
| SWAP | 208,640 | 21.4% |
| CALL_ALLOC_AND_ENTER_INIT | 3,340 | 0.3% |
| BINARY_OP | 2,560 | 0.3% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 1,260 | 98.4% |
| STORE_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,280 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,233,100 | 91.5% |
| LOAD_FAST_LOAD_FAST | 77,200 | 5.7% |
| LOAD_GLOBAL_MODULE | 37,100 | 2.8% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,233,100 | 91.5% |
| LIST_APPEND | 62,900 | 4.7% |
| CALL_LIST_APPEND | 37,080 | 2.8% |
| STORE_FAST | 10,300 | 0.8% |
| CALL_PY_EXACT_ARGS | 2,100 | 0.2% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,680 | 22.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,440 | 19.4% |
| ENTER_EXECUTOR | 900 | 12.1% |
| PUSH_NULL | 700 | 9.4% |
| LOAD_FAST_LOAD_FAST | 440 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,000 | 40.3% |
| CALL_PY_EXACT_ARGS | 900 | 12.1% |
| CALL_BUILTIN_CLASS | 620 | 8.3% |
| GET_ITER | 500 | 6.7% |
| RESUME | 440 | 5.9% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 80 | 50.0% |
| LOAD_FAST | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 50.0% |
| RESUME_CHECK | 60 | 37.5% |
| RESUME | 20 | 12.5% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 34,940 | 91.0% |
| ENTER_EXECUTOR | 3,460 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 37,120 | 96.7% |
| RESUME_CHECK | 1,260 | 3.3% |
| RESUME | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 38.5% |
| LOAD_FAST_LOAD_FAST | 240 | 15.4% |
| LOAD_GLOBAL | 200 | 12.8% |
| LOAD_GLOBAL_MODULE | 200 | 12.8% |
| LOAD_ATTR | 100 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 680 | 43.6% |
| POP_JUMP_IF_FALSE | 520 | 33.3% |
| POP_JUMP_IF_TRUE | 240 | 15.4% |
| COMPARE_OP_STR | 100 | 6.4% |
| RETURN_VALUE | 20 | 1.3% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,173,760 | 56.6% |
| BINARY_SUBSCR_LIST_INT | 2,320,300 | 41.4% |
| RETURN_VALUE | 112,600 | 2.0% |
| LOAD_ATTR_INSTANCE_VALUE | 2,120 | 0.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,298,240 | 76.6% |
| POP_JUMP_IF_TRUE | 1,308,480 | 23.3% |
| RETURN_VALUE | 2,140 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,630,280 | 50.0% |
| LOAD_FAST_LOAD_FAST | 1,284,480 | 39.4% |
| BINARY_SUBSCR_LIST_INT | 345,780 | 10.6% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,630,280 | 50.0% |
| BINARY_SUBSCR_LIST_INT | 1,630,120 | 50.0% |
| BINARY_SUBSCR | 160 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,233,080 | 64.4% |
| ENTER_EXECUTOR | 681,780 | 35.6% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,914,880 | 100.0% |
| RESUME_CHECK | 60 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 36,421,680 | 65.0% |
| STORE_FAST | 6,569,820 | 11.7% |
| POP_JUMP_IF_FALSE | 4,816,740 | 8.6% |
| POP_JUMP_IF_TRUE | 4,415,120 | 7.9% |
| FOR_ITER_RANGE | 1,693,360 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 26,362,620 | 47.1% |
| LOAD_CONST | 8,109,820 | 14.5% |
| FOR_ITER_LIST | 5,544,920 | 9.9% |
| BINARY_SUBSCR_GETITEM | 4,922,460 | 8.8% |
| LOAD_FAST | 3,013,420 | 5.4% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 276,480 | 49.9% |
| ENTER_EXECUTOR | 275,200 | 49.7% |
| JUMP_BACKWARD | 1,600 | 0.3% |
| FOR_ITER_LIST | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 547,340 | 98.9% |
| FOR_ITER_RANGE | 5,900 | 1.1% |
| JUMP_BACKWARD | 340 | 0.1% |
| FOR_ITER | 40 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 720 | 46.2% |
| GET_ITER | 680 | 43.6% |
| SWAP | 80 | 5.1% |
| EXTENDED_ARG | 40 | 2.6% |
| LOAD_FAST | 40 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 680 | 43.6% |
| FOR_ITER_RANGE | 520 | 33.3% |
| FOR_ITER_LIST | 260 | 16.7% |
| STORE_FAST_LOAD_FAST | 80 | 5.1% |
| STORE_DEREF | 20 | 1.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,780 | 28.5% |
| POP_JUMP_IF_TRUE | 5,360 | 22.6% |
| POP_JUMP_IF_FALSE | 3,380 | 14.2% |
| POP_TOP | 2,760 | 11.6% |
| LIST_APPEND | 1,360 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 12,320 | 51.9% |
| FOR_ITER_LIST | 7,440 | 31.3% |
| EXTENDED_ARG | 1,600 | 6.7% |
| ENTER_EXECUTOR | 1,360 | 5.7% |
| FOR_ITER | 720 | 3.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,189,440 | 98.5% |
| STORE_FAST | 106,520 | 1.3% |
| CALL_STR_1 | 15,320 | 0.2% |
| CALL_BUILTIN_CLASS | 5,080 | 0.1% |
| POP_JUMP_IF_FALSE | 1,280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 8,189,440 | 98.5% |
| LOAD_FAST | 80,640 | 1.0% |
| LOAD_GLOBAL_BUILTIN | 24,240 | 0.3% |
| STORE_FAST | 20,480 | 0.2% |
| LOAD_FAST_LOAD_FAST | 1,560 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 143,680 | 68.5% |
| BUILD_TUPLE | 62,900 | 30.0% |
| BUILD_LIST | 1,600 | 0.8% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,540 | 0.7% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 208,380 | 99.4% |
| JUMP_BACKWARD | 1,360 | 0.6% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 80 | 100.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,240 | 68.1% |
| LOAD_FAST_LOAD_FAST | 360 | 7.6% |
| RETURN_VALUE | 240 | 5.0% |
| LOAD_GLOBAL | 200 | 4.2% |
| LOAD_GLOBAL_MODULE | 200 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,260 | 26.5% |
| LOAD_FAST | 820 | 17.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 680 | 14.3% |
| CALL | 420 | 8.8% |
| STORE_FAST | 320 | 6.7% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 9,198,240 | 18.7% |
| LOAD_FAST | 8,884,200 | 18.1% |
| ENTER_EXECUTOR | 8,109,820 | 16.5% |
| RETURN_VALUE | 7,204,940 | 14.7% |
| POP_JUMP_IF_FALSE | 4,640,900 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 11,055,240 | 22.5% |
| BINARY_OP_ADD_INT | 8,779,480 | 17.9% |
| JUMP_FORWARD | 8,189,440 | 16.7% |
| BINARY_SUBSCR_LIST_INT | 7,551,760 | 15.4% |
| STORE_FAST | 6,292,540 | 12.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 2,192,500 | 37.0% |
| STORE_FAST | 1,915,200 | 32.3% |
| ENTER_EXECUTOR | 1,247,560 | 21.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 296,940 | 5.0% |
| LOAD_FAST | 261,440 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,173,760 | 53.6% |
| BINARY_SUBSCR_LIST_INT | 2,432,100 | 41.0% |
| CALL_PY_EXACT_ARGS | 318,640 | 5.4% |
| PUSH_NULL | 160 | 0.0% |
| BINARY_SUBSCR | 120 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 22,411,120 | 23.0% |
| STORE_FAST | 17,410,020 | 17.9% |
| RESUME_CHECK | 13,854,340 | 14.2% |
| LOAD_GLOBAL_BUILTIN | 10,532,560 | 10.8% |
| POP_JUMP_IF_FALSE | 9,118,600 | 9.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 27,740,540 | 28.5% |
| BINARY_SUBSCR_LIST_INT | 22,017,500 | 22.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 10,559,720 | 10.9% |
| LOAD_CONST | 8,884,200 | 9.1% |
| CALL_PY_EXACT_ARGS | 8,797,300 | 9.0% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 208,640 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 208,640 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 40 | 50.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 50.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,264,380 | 19.4% |
| RESUME_CHECK | 2,637,220 | 15.7% |
| LOAD_ATTR_METHOD_WITH_VALUES | 2,473,040 | 14.7% |
| STORE_FAST | 1,904,260 | 11.3% |
| POP_JUMP_IF_TRUE | 1,631,900 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_GETITEM | 4,299,060 | 25.5% |
| COMPARE_OP_INT | 3,417,720 | 20.3% |
| CALL_PY_EXACT_ARGS | 2,616,580 | 15.5% |
| LOAD_ATTR_INSTANCE_VALUE | 2,376,300 | 14.1% |
| COPY | 1,284,480 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,340 | 31.6% |
| POP_JUMP_IF_FALSE | 560 | 13.2% |
| LOAD_FAST | 480 | 11.3% |
| POP_TOP | 240 | 5.7% |
| FOR_ITER_RANGE | 240 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,200 | 28.3% |
| LOAD_GLOBAL_BUILTIN | 920 | 21.7% |
| LOAD_FAST | 640 | 15.1% |
| LOAD_FAST_LOAD_FAST | 480 | 11.3% |
| LOAD_CONST | 260 | 6.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 255,000 | 99.0% |
| CALL_PY_WITH_DEFAULTS | 2,520 | 1.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 257,580 | 100.0% |
| RESUME | 20 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 13,121,600 | 53.1% |
| TO_BOOL_BOOL | 7,285,980 | 29.5% |
| CONTAINS_OP | 4,298,240 | 17.4% |
| COMPARE_OP_STR | 3,440 | 0.0% |
| COMPARE_OP | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,118,600 | 36.9% |
| ENTER_EXECUTOR | 4,816,740 | 19.5% |
| LOAD_CONST | 4,640,900 | 18.8% |
| LOAD_FAST_LOAD_FAST | 3,264,380 | 13.2% |
| RETURN_CONST | 1,917,900 | 7.8% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 678,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 673,600 | 99.2% |
| LOAD_GLOBAL_BUILTIN | 5,040 | 0.7% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 4,487,920 | 53.0% |
| TO_BOOL_BOOL | 2,657,520 | 31.4% |
| CONTAINS_OP | 1,308,480 | 15.5% |
| COMPARE_OP_STR | 10,840 | 0.1% |
| COMPARE_OP | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,415,120 | 52.2% |
| LOAD_FAST_LOAD_FAST | 1,631,900 | 19.3% |
| LOAD_GLOBAL_BUILTIN | 1,121,240 | 13.2% |
| LOAD_FAST | 756,420 | 8.9% |
| LOAD_CONST | 460,800 | 5.4% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,917,900 | 38.5% |
| FOR_ITER_LIST | 1,916,240 | 38.5% |
| POP_TOP | 609,600 | 12.3% |
| STORE_ATTR_INSTANCE_VALUE | 313,520 | 6.3% |
| STORE_SUBSCR_LIST_INT | 209,900 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,377,300 | 47.8% |
| INTERPRETER_EXIT | 1,916,360 | 38.5% |
| POP_TOP | 368,960 | 7.4% |
| EXIT_INIT_CHECK | 313,480 | 6.3% |
| TO_BOOL | 120 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,233,100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,233,100 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 50.0% |
| LOAD_FAST_LOAD_FAST | 280 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 280 | 50.0% |
| LOAD_FAST | 80 | 14.3% |
| RETURN_CONST | 80 | 14.3% |
| LOAD_FAST_LOAD_FAST | 60 | 10.7% |
| LOAD_CONST | 40 | 7.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 277,640 | 100.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 277,660 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 8,770,340 | 27.1% |
| LOAD_CONST | 6,292,540 | 19.5% |
| FOR_ITER_LIST | 5,695,740 | 17.6% |
| BINARY_SUBSCR_LIST_INT | 2,669,660 | 8.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,617,460 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,410,020 | 53.9% |
| ENTER_EXECUTOR | 6,569,820 | 20.3% |
| LOAD_CONST | 2,628,940 | 8.1% |
| LOAD_DEREF | 1,915,200 | 5.9% |
| LOAD_FAST_LOAD_FAST | 1,904,260 | 5.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_RANGE | 143,660 | 68.9% |
| FOR_ITER_LIST | 64,760 | 31.1% |
| FOR_ITER | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 143,640 | 68.9% |
| LOAD_GLOBAL_MODULE | 62,880 | 30.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,820 | 0.9% |
| LOAD_ATTR | 120 | 0.1% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 143,700 | 100.0% |
| UNPACK_SEQUENCE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,080 | 98.8% |
| LOAD_GLOBAL_MODULE | 1,600 | 1.1% |
| LOAD_GLOBAL | 80 | 0.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,630,280 | 40.3% |
| BINARY_OP_SUBTRACT_INT | 1,619,360 | 40.0% |
| BUILD_LIST | 208,640 | 5.2% |
| LOAD_FAST_AND_CLEAR | 208,640 | 5.2% |
| FOR_ITER_RANGE | 144,640 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,630,280 | 40.3% |
| STORE_SUBSCR_LIST_INT | 1,630,120 | 40.3% |
| BUILD_LIST | 208,640 | 5.2% |
| STORE_FAST | 207,360 | 5.1% |
| POP_TOP | 162,560 | 4.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 33.3% |
| BINARY_SUBSCR | 20 | 16.7% |
| LOAD_ATTR | 20 | 16.7% |
| BINARY_SUBSCR_DICT | 20 | 16.7% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 60 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 60 | 50.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,362,620 | 72.5% |
| JUMP_FORWARD | 8,189,440 | 22.5% |
| LOAD_CONST | 1,830,720 | 5.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 320 | 0.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 36,383,120 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 440 | 62.9% |
| CACHE | 140 | 20.0% |
| POP_TOP | 40 | 5.7% |
| CALL_FUNCTION_EX | 20 | 2.9% |
| CALL_KW | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 42.9% |
| LOAD_GLOBAL | 180 | 25.7% |
| LOAD_FAST_LOAD_FAST | 120 | 17.1% |
| POP_TOP | 40 | 5.7% |
| LOAD_CONST | 40 | 5.7% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,779,480 | 97.9% |
| CALL_LEN | 174,040 | 1.9% |
| LOAD_FAST_LOAD_FAST | 11,120 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,200 | 0.0% |
| LOAD_FAST | 1,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,770,340 | 97.8% |
| COMPARE_OP_INT | 174,040 | 1.9% |
| SWAP | 10,840 | 0.1% |
| CALL_BUILTIN_CLASS | 6,720 | 0.1% |
| LOAD_CONST | 4,440 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 5,320 | 67.3% |
| LOAD_FAST | 1,240 | 15.7% |
| BINARY_OP_SUBTRACT_INT | 1,240 | 15.7% |
| BINARY_OP | 100 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,640 | 84.1% |
| LOAD_FAST | 1,260 | 15.9% |


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
| LOAD_CONST | 1,634,600 | 99.8% |
| LOAD_FAST_LOAD_FAST | 2,920 | 0.2% |
| BINARY_OP | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,619,360 | 98.9% |
| CALL_BUILTIN_CLASS | 5,320 | 0.3% |
| LOAD_CONST | 4,440 | 0.3% |
| STORE_FAST | 4,440 | 0.3% |
| BINARY_OP | 1,500 | 0.1% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,880 | 78.5% |
| BUILD_TUPLE | 1,820 | 20.8% |
| BINARY_SUBSCR | 60 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,860 | 78.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 20.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 40 | 0.5% |
| LOAD_ATTR | 20 | 0.2% |
| UNPACK_SEQUENCE | 20 | 0.2% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,922,460 | 53.2% |
| LOAD_FAST_LOAD_FAST | 4,299,060 | 46.5% |
| LOAD_FAST | 23,400 | 0.3% |
| BINARY_SUBSCR | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,245,180 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,017,500 | 63.1% |
| LOAD_CONST | 7,551,760 | 21.6% |
| LOAD_DEREF | 2,432,100 | 7.0% |
| COPY | 1,630,120 | 4.7% |
| LOAD_FAST_LOAD_FAST | 1,280,020 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 11,245,400 | 32.2% |
| CALL_LEN | 6,719,580 | 19.2% |
| LOAD_GLOBAL_MODULE | 5,642,040 | 16.2% |
| LOAD_CONST | 3,568,380 | 10.2% |
| STORE_FAST | 2,669,660 | 7.6% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,140 | 99.4% |
| BINARY_SUBSCR | 80 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,220 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 254,960 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 254,960 | 100.0% |
| CALL | 40 | 0.0% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 143,320 | 45.7% |
| ENTER_EXECUTOR | 100,020 | 31.9% |
| LOAD_CONST | 64,200 | 20.5% |
| BUILD_LIST | 3,340 | 1.1% |
| LOAD_FAST | 2,480 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 313,480 | 100.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,776,320 | 63.9% |
| LOAD_CONST | 845,920 | 30.4% |
| STORE_FAST | 62,680 | 2.3% |
| CALL_BUILTIN_CLASS | 62,680 | 2.3% |
| LOAD_FAST | 17,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,638,380 | 94.9% |
| STORE_FAST | 73,300 | 2.6% |
| CALL_BUILTIN_CLASS | 62,680 | 2.3% |
| JUMP_FORWARD | 5,080 | 0.2% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 1,914,840 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,914,860 | 100.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 6,719,580 | 71.7% |
| RETURN_VALUE | 1,864,920 | 19.9% |
| LOAD_FAST | 787,680 | 8.4% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,198,240 | 98.1% |
| BINARY_OP_ADD_INT | 174,040 | 1.9% |
| BINARY_OP | 20 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 412,280 | 69.0% |
| ENTER_EXECUTOR | 146,460 | 24.5% |
| BUILD_TUPLE | 37,080 | 6.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 0.3% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 559,960 | 93.7% |
| LOAD_FAST | 37,100 | 6.2% |
| JUMP_BACKWARD | 640 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,520 | 76.8% |
| LOAD_ATTR_METHOD_NO_DICT | 380 | 19.2% |
| CALL | 80 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LIST_APPEND | 1,540 | 77.8% |
| YIELD_VALUE | 320 | 16.2% |
| STORE_FAST | 120 | 6.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,280 | 97.0% |
| CALL | 40 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,320 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_LAZY_DICT | 1,240 | 98.4% |
| CALL | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,260 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 466,200 | 100.0% |
| RETURN_GENERATOR | 40 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 466,220 | 100.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,797,300 | 65.1% |
| LOAD_FAST_LOAD_FAST | 2,616,580 | 19.4% |
| GET_ITER | 1,233,100 | 9.1% |
| LOAD_DEREF | 318,640 | 2.4% |
| BINARY_SUBSCR_TUPLE_INT | 254,960 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,027,820 | 89.0% |
| COPY_FREE_VARS | 1,233,080 | 9.1% |
| MAKE_CELL | 255,000 | 1.9% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 203,440 | 98.8% |
| LOAD_FAST | 2,480 | 1.2% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 203,480 | 98.8% |
| MAKE_CELL | 2,520 | 1.2% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 15,280 | 99.7% |
| CALL | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 15,320 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,055,240 | 45.4% |
| LOAD_GLOBAL_MODULE | 7,317,560 | 30.1% |
| LOAD_FAST_LOAD_FAST | 3,417,720 | 14.0% |
| LOAD_FAST | 2,111,920 | 8.7% |
| LOAD_ATTR_CLASS | 250,720 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 13,121,600 | 53.9% |
| RETURN_VALUE | 6,719,600 | 27.6% |
| POP_JUMP_IF_TRUE | 4,487,920 | 18.4% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,140 | 99.0% |
| COMPARE_OP | 100 | 0.7% |
| LOAD_FAST_LOAD_FAST | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 10,840 | 75.9% |
| POP_JUMP_IF_FALSE | 3,440 | 24.1% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,544,920 | 52.8% |
| GET_ITER | 2,420,100 | 23.1% |
| LOAD_FAST | 1,914,920 | 18.2% |
| EXTENDED_ARG | 547,340 | 5.2% |
| SWAP | 63,960 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,695,740 | 54.2% |
| RETURN_CONST | 1,916,240 | 18.3% |
| LOAD_GLOBAL_BUILTIN | 1,117,320 | 10.6% |
| LOAD_FAST_LOAD_FAST | 949,760 | 9.0% |
| LOAD_FAST | 548,960 | 5.2% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,506,140 | 48.5% |
| GET_ITER | 2,494,940 | 48.3% |
| SWAP | 144,600 | 2.8% |
| JUMP_BACKWARD | 12,320 | 0.2% |
| EXTENDED_ARG | 5,900 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,235,320 | 43.3% |
| ENTER_EXECUTOR | 1,693,360 | 32.8% |
| LOAD_FAST | 647,840 | 12.5% |
| STORE_DEREF | 277,640 | 5.4% |
| SWAP | 144,640 | 2.8% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 250,760 | 100.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 250,720 | 99.9% |
| COMPARE_OP | 80 | 0.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,740,540 | 86.0% |
| LOAD_FAST_LOAD_FAST | 2,376,300 | 7.4% |
| RETURN_VALUE | 2,006,640 | 6.2% |
| STORE_FAST_LOAD_FAST | 143,640 | 0.4% |
| BINARY_SUBSCR_DICT | 1,820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,411,120 | 69.4% |
| STORE_FAST | 2,617,460 | 8.1% |
| LOAD_DEREF | 2,192,500 | 6.8% |
| CALL_BUILTIN_CLASS | 1,776,320 | 5.5% |
| GET_ITER | 1,510,800 | 4.7% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,240 | 98.4% |
| LOAD_ATTR | 20 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,240 | 98.4% |
| CALL | 20 | 1.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 466,200 | 50.6% |
| LOAD_FAST | 450,680 | 48.9% |
| STORE_FAST_LOAD_FAST | 1,820 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,820 | 0.2% |
| LOAD_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 917,460 | 99.6% |
| LOAD_CONST | 1,600 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,280 | 0.1% |
| CALL_METHOD_DESCRIPTOR_FAST | 380 | 0.0% |
| CALL | 100 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,559,720 | 89.4% |
| LOAD_ATTR_INSTANCE_VALUE | 1,256,360 | 10.6% |
| LOAD_ATTR | 680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,854,400 | 74.9% |
| LOAD_FAST_LOAD_FAST | 2,473,040 | 20.9% |
| LOAD_DEREF | 296,940 | 2.5% |
| CALL_PY_EXACT_ARGS | 192,280 | 1.6% |
| CALL | 100 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 500 | 83.3% |
| LOAD_ATTR | 100 | 16.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 600 | 100.0% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 6,788,580 | 58.0% |
| POP_JUMP_IF_TRUE | 1,121,240 | 9.6% |
| FOR_ITER_LIST | 1,117,320 | 9.5% |
| STORE_FAST | 1,080,180 | 9.2% |
| ENTER_EXECUTOR | 791,900 | 6.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,532,560 | 89.9% |
| LOAD_CONST | 883,320 | 7.5% |
| LOAD_FAST_LOAD_FAST | 233,520 | 2.0% |
| LOAD_GLOBAL_BUILTIN | 62,680 | 0.5% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 5,642,040 | 63.6% |
| LOAD_FAST | 2,000,540 | 22.5% |
| STORE_FAST | 362,460 | 4.1% |
| POP_JUMP_IF_FALSE | 291,880 | 3.3% |
| POP_TOP | 145,760 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,317,560 | 82.5% |
| LOAD_FAST_LOAD_FAST | 735,620 | 8.3% |
| LOAD_ATTR_CLASS | 250,760 | 2.8% |
| LOAD_FAST | 159,480 | 1.8% |
| RETURN_VALUE | 104,900 | 1.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 36,384,640 | 60.3% |
| CALL_PY_EXACT_ARGS | 12,027,820 | 19.9% |
| BINARY_SUBSCR_GETITEM | 9,245,180 | 15.3% |
| POP_TOP | 1,914,920 | 3.2% |
| CALL_ALLOC_AND_ENTER_INIT | 313,480 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 36,383,080 | 60.3% |
| LOAD_FAST | 13,854,340 | 23.0% |
| LOAD_GLOBAL_BUILTIN | 6,788,580 | 11.2% |
| LOAD_FAST_LOAD_FAST | 2,637,220 | 4.4% |
| LOAD_CONST | 554,520 | 0.9% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 507,880 | 53.8% |
| LOAD_FAST | 436,200 | 46.2% |
| STORE_ATTR | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 433,840 | 45.9% |
| RETURN_CONST | 313,520 | 33.2% |
| LOAD_FAST_LOAD_FAST | 193,220 | 20.5% |
| LOAD_CONST | 2,520 | 0.3% |
| BUILD_MAP | 1,260 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,240 | 99.8% |
| STORE_SUBSCR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 24,280 | 100.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,630,120 | 87.2% |
| LOAD_FAST | 209,880 | 11.2% |
| LOAD_ATTR_INSTANCE_VALUE | 24,240 | 1.3% |
| LOAD_FAST_LOAD_FAST | 5,080 | 0.3% |
| STORE_SUBSCR | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,273,580 | 68.1% |
| ENTER_EXECUTOR | 350,240 | 18.7% |
| RETURN_CONST | 209,900 | 11.2% |
| LOAD_FAST | 35,120 | 1.9% |
| JUMP_BACKWARD | 640 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,294,520 | 73.4% |
| RETURN_CONST | 2,377,300 | 23.9% |
| LOAD_FAST | 271,200 | 2.7% |
| TO_BOOL | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,285,980 | 73.3% |
| POP_JUMP_IF_TRUE | 2,657,520 | 26.7% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 142,040 | 98.8% |
| LOAD_ATTR_INSTANCE_VALUE | 1,560 | 1.1% |
| UNPACK_SEQUENCE | 60 | 0.0% |
| BINARY_SUBSCR_DICT | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 143,700 | 100.0% |


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
|     deferred | 30,780 | 0.3% |
|          hit | 10,616,840 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 960 | 57.8% |
| Failure | 700 | 42.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 400 | 57.1% |
| remainder | 300 | 42.9% |


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
|     deferred | 1,060 | 0.0% |
|          hit | 44,435,280 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,060 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,020 | 0.0% |
|          hit | 29,185,920 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,140 | 88.4% |
| Failure | 280 | 11.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class no vectorcall | 120 | 42.9% |
| wrong number arguments | 100 | 35.7% |
| cfunc noargs | 60 | 21.4% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 780 | 0.0% |
|          hit | 24,343,400 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 780 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,620 | 0.1% |
|          hit | 15,643,520 | 99.9% |
|         miss | 20,200 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,140 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,380 | 0.0% |
|          hit | 45,260,500 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,380 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,120 | 0.0% |
|          hit | 20,586,000 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,120 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> specialization stats for POP_JUMP_IF_FALSE family </summary>


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
|     deferred | 280 | 0.0% |
|          hit | 944,360 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 280 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 1,893,760 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 480 | 0.0% |
|          hit | 9,943,500 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 480 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 0.0% |
|          hit | 143,700 | 99.9% |

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
| Basic | 434,850,040 | 59.4% |
| Not specialized | 34,459,860 | 4.7% |
| Specialized hits | 263,345,680 | 35.9% |
| Specialized misses | 20,200 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_OP | 30,780 | 48.3% |
| FOR_ITER | 20,620 | 32.3% |
| CALL | 5,020 | 7.9% |
| LOAD_ATTR | 2,380 | 3.7% |
| LOAD_GLOBAL | 2,120 | 3.3% |
| BINARY_SUBSCR | 1,060 | 1.7% |
| COMPARE_OP | 780 | 1.2% |
| TO_BOOL | 480 | 0.8% |
| STORE_ATTR | 280 | 0.4% |
| STORE_SUBSCR | 200 | 0.3% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| FOR_ITER_RANGE | 10,600 | 52.5% |
| FOR_ITER_LIST | 9,600 | 47.5% |
| CACHE | 0 | 0.0% |
| EXIT_INIT_CHECK | 0 | 0.0% |
| GET_ITER | 0 | 0.0% |
| INTERPRETER_EXIT | 0 | 0.0% |
| MAKE_FUNCTION | 0 | 0.0% |
| NOP | 0 | 0.0% |
| POP_TOP | 0 | 0.0% |
| PUSH_NULL | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 38,299,740 | 62.2% |
| Calls to Python functions inlined | 23,283,040 | 37.8% |
| Calls via PyEval_EvalFrame (total) | 38,299,740 | 62.2% |
| Calls via PyEval_EvalFrame (vector) | 1,660 | 0.0% |
| Calls via PyEval_EvalFrame (generator) | 38,298,080 | 62.2% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 1,660 | 0.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 260 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 0 | 0.0% |
| Frames pushed | 58,430,600 | 94.9% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 5,808,620 | 22.8% |
| Frees to freelist | 5,809,880 |  |
| Allocations | 19,721,020 | 77.2% |
| Allocations to 512 bytes | 19,718,840 | 77.2% |
| Allocations to 4 kbytes | 2,180 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 20,153,096 |  |
| New values | 1,400 |  |
| Interpreter increfs | 658,282,220 | 97.4% |
| Interpreter decrefs | 680,110,280 | 97.1% |
| Increfs | 17,616,562 | 2.6% |
| Decrefs | 20,457,168 | 2.9% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 71,196 |  |
| Method cache misses | 2,064 |  |
| Method cache collisions | 3,066 |  |
| Method cache dunder hits | 142,912 |  |
| Method cache dunder misses | 1,388 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 1,980 | 147,320 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,360 |  |
| Traces created | 1,360 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 80 | 5.9% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 56,007,820 |  |
| Uops executed | 2,511,349,320 | 44.84 |

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
| <= 32 | 220 | 16.2% |
| <= 64 | 280 | 20.6% |
| <= 128 | 700 | 51.5% |
| <= 256 | 160 | 11.8% |


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
| <= 16 | 220 | 16.2% |
| <= 32 | 260 | 19.1% |
| <= 64 | 680 | 50.0% |
| <= 128 | 180 | 13.2% |
| <= 256 | 20 | 1.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 5,467,440 | 9.8% |
| <= 4 | 931,740 | 1.7% |
| <= 8 | 0 | 0.0% |
| <= 16 | 36,575,920 | 65.3% |
| <= 32 | 1,899,900 | 3.4% |
| <= 64 | 6,209,600 | 11.1% |
| <= 128 | 1,647,160 | 2.9% |
| <= 256 | 773,800 | 1.4% |
| <= 512 | 1,177,540 | 2.1% |
| <= 1,024 | 1,313,240 | 2.3% |
| <= 2,048 | 11,480 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 333,023,520 | 13.3% | 13.3% |  |
| _CHECK_VALIDITY | 321,420,400 | 12.8% | 26.1% |  |
| LOAD_FAST | 266,845,040 | 10.6% | 36.7% |  |
| STORE_FAST | 102,529,020 | 4.1% | 40.8% |  |
| _GUARD_TYPE_VERSION | 94,956,220 | 3.8% | 44.5% |  |
| _LOAD_CONST_INLINE_BORROW | 80,592,240 | 3.2% | 47.8% |  |
| BINARY_SUBSCR_LIST_INT | 65,013,020 | 2.6% | 50.3% |  |
| _GUARD_IS_FALSE_POP | 64,773,660 | 2.6% | 52.9% | 18.1% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 60,575,900 | 2.4% | 55.3% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 60,575,900 | 2.4% | 57.8% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 50,730,960 | 2.0% | 59.8% | 8.8% |
| _ITER_CHECK_LIST | 50,730,960 | 2.0% | 61.8% |  |
| COMPARE_OP_INT | 46,998,200 | 1.9% | 63.7% |  |
| _ITER_NEXT_LIST | 46,269,560 | 1.8% | 65.5% |  |
| LOAD_DEREF | 44,534,180 | 1.8% | 67.3% |  |
| CONTAINS_OP | 43,034,980 | 1.7% | 69.0% |  |
| _CHECK_GLOBALS | 40,497,340 | 1.6% | 70.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 40,175,160 | 1.6% | 72.2% |  |
| _CHECK_BUILTINS | 39,988,980 | 1.6% | 73.8% |  |
| _ITER_CHECK_RANGE | 39,888,840 | 1.6% | 75.4% | 3.4% |
| _GUARD_NOT_EXHAUSTED_RANGE | 38,531,080 | 1.5% | 76.9% | 6.5% |
| CALL_LEN | 37,570,300 | 1.5% | 78.4% |  |
| _ITER_NEXT_RANGE | 36,023,980 | 1.4% | 79.8% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 34,836,500 | 1.4% | 81.2% |  |
| _CHECK_STACK_SPACE | 34,836,500 | 1.4% | 82.6% |  |
| _INIT_CALL_PY_EXACT_ARGS | 34,836,500 | 1.4% | 84.0% |  |
| _PUSH_FRAME | 34,836,500 | 1.4% | 85.4% |  |
| _SAVE_RETURN_OFFSET | 34,836,500 | 1.4% | 86.8% |  |
| _JUMP_TO_TOP | 34,536,580 | 1.4% | 88.2% |  |
| RESUME_CHECK | 34,154,720 | 1.4% | 89.5% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 34,135,840 | 1.4% | 90.9% |  |
| _GUARD_KEYS_VERSION | 34,135,840 | 1.4% | 92.2% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 34,135,840 | 1.4% | 93.6% |  |
| _POP_FRAME | 33,915,060 | 1.4% | 94.9% |  |
| TO_BOOL_BOOL | 33,741,140 | 1.3% | 96.3% |  |
| _EXIT_TRACE | 32,283,360 | 1.3% | 97.6% | 100.0% |
| _GUARD_IS_TRUE_POP | 26,296,920 | 1.0% | 98.6% | 13.9% |
| COPY | 5,530,480 | 0.2% | 98.8% |  |
| SWAP | 5,530,480 | 0.2% | 99.1% |  |
| _GUARD_BOTH_INT | 4,372,360 | 0.2% | 99.2% |  |
| _BINARY_OP_SUBTRACT_INT | 2,777,960 | 0.1% | 99.3% |  |
| STORE_SUBSCR_LIST_INT | 2,765,240 | 0.1% | 99.5% |  |
| LIST_APPEND | 2,667,700 | 0.1% | 99.6% |  |
| BINARY_SLICE | 2,623,400 | 0.1% | 99.7% |  |
| STORE_DEREF | 1,934,180 | 0.1% | 99.7% |  |
| _BINARY_OP_ADD_INT | 1,592,160 | 0.1% | 99.8% |  |
| BUILD_TUPLE | 1,028,260 | 0.0% | 99.9% |  |
| GET_ITER | 776,060 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE | 714,980 | 0.0% | 99.9% |  |
| MAKE_FUNCTION | 681,780 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 681,780 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 244,480 | 0.0% | 100.0% |  |
| POP_TOP | 183,680 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 123,100 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 91,840 | 0.0% | 100.0% |  |
| BUILD_LIST | 43,620 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 34,340 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 34,340 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 22,720 | 0.0% | 100.0% |  |
| MAKE_CELL | 18,880 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 18,880 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 18,880 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 12,960 | 0.0% | 100.0% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 12,960 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 6,180 | 0.0% | 100.0% |  |
| _BINARY_OP | 3,460 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 2,240 | 0.0% | 100.0% |  |
| PUSH_NULL | 900 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 900 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 900 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| BINARY_SUBSCR_GETITEM | 340 |
| CALL_ALLOC_AND_ENTER_INIT | 100 |
| CALL_LIST_APPEND | 80 |
| CALL_KW | 40 |
| YIELD_VALUE | 40 |
| CALL | 20 |


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
