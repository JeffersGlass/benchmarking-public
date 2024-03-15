
# Pystats results

- benchmark: mdp
- fork: faster-cpython
- ref: watched-dict-stats
- commit hash: 7b9e10f
- commit date: 2024-02-08T14:11:09+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,003,899,600 | 14.2% | 14.2% |  |
| RESUME_CHECK | 555,634,280 | 7.8% | 22.0% | 0.0% |
| INTERPRETER_EXIT | 435,891,180 | 6.1% | 28.1% |  |
| POP_TOP | 388,578,040 | 5.5% | 33.6% |  |
| ENTER_EXECUTOR | 373,459,680 | 5.3% | 38.9% |  |
| YIELD_VALUE | 324,495,840 | 4.6% | 43.5% |  |
| LOAD_FAST_LOAD_FAST | 307,837,140 | 4.3% | 47.8% |  |
| STORE_FAST | 269,186,520 | 3.8% | 51.6% |  |
| LOAD_DEREF | 239,879,080 | 3.4% | 55.0% |  |
| RETURN_VALUE | 172,332,640 | 2.4% | 57.4% |  |
| LOAD_GLOBAL_MODULE | 168,004,500 | 2.4% | 59.8% |  |
| LOAD_CONST | 146,384,420 | 2.1% | 61.8% |  |
| LOAD_GLOBAL_BUILTIN | 142,674,560 | 2.0% | 63.8% |  |
| COPY_FREE_VARS | 141,718,960 | 2.0% | 65.8% |  |
| BINARY_SUBSCR | 131,177,400 | 1.8% | 67.7% |  |
| LOAD_ATTR_SLOT | 130,016,240 | 1.8% | 69.5% |  |
| FOR_ITER_LIST | 125,786,540 | 1.8% | 71.3% | 0.1% |
| POP_JUMP_IF_FALSE | 123,890,960 | 1.7% | 73.0% |  |
| CALL_PY_EXACT_ARGS | 118,849,800 | 1.7% | 74.7% | 1.4% |
| PUSH_NULL | 100,104,320 | 1.4% | 76.1% |  |
| BINARY_OP_MULTIPLY_INT | 97,943,940 | 1.4% | 77.5% |  |
| BINARY_OP | 86,126,860 | 1.2% | 78.7% |  |
| STORE_ATTR_SLOT | 80,104,680 | 1.1% | 79.9% |  |
| COMPARE_OP_INT | 71,522,220 | 1.0% | 80.9% |  |
| STORE_SUBSCR | 67,616,680 | 1.0% | 81.8% |  |
| STORE_FAST_STORE_FAST | 64,515,460 | 0.9% | 82.7% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,604,220 | 0.9% | 83.6% |  |
| RETURN_CONST | 63,239,120 | 0.9% | 84.5% |  |
| RETURN_GENERATOR | 62,832,560 | 0.9% | 85.4% |  |
| CALL_BUILTIN_FAST | 58,829,240 | 0.8% | 86.2% |  |
| LOAD_ATTR_MODULE | 58,243,860 | 0.8% | 87.1% |  |
| LOAD_ATTR | 50,823,320 | 0.7% | 87.8% |  |
| BUILD_TUPLE | 50,559,680 | 0.7% | 88.5% |  |
| CALL | 47,619,660 | 0.7% | 89.2% |  |
| GET_ITER | 44,656,340 | 0.6% | 89.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 43,596,920 | 0.6% | 90.4% |  |
| LOAD_ATTR_INSTANCE_VALUE | 42,517,080 | 0.6% | 91.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 42,471,240 | 0.6% | 91.6% |  |
| MAKE_FUNCTION | 42,192,420 | 0.6% | 92.2% |  |
| BINARY_SUBSCR_DICT | 42,192,140 | 0.6% | 92.8% |  |
| NOP | 41,899,540 | 0.6% | 93.4% |  |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 0.6% | 94.0% |  |
| SET_FUNCTION_ATTRIBUTE | 41,513,780 | 0.6% | 94.5% |  |
| LOAD_SUPER_ATTR_METHOD | 40,052,360 | 0.6% | 95.1% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 35,344,000 | 0.5% | 95.6% |  |
| TO_BOOL_BOOL | 34,553,040 | 0.5% | 96.1% |  |
| CALL_ISINSTANCE | 33,089,520 | 0.5% | 96.6% |  |
| POP_JUMP_IF_TRUE | 31,855,900 | 0.4% | 97.0% |  |
| BINARY_OP_ADD_INT | 31,344,420 | 0.4% | 97.5% |  |
| COMPARE_OP_FLOAT | 31,185,840 | 0.4% | 97.9% |  |
| JUMP_FORWARD | 15,114,160 | 0.2% | 98.1% |  |
| BINARY_SUBSCR_TUPLE_INT | 14,524,220 | 0.2% | 98.3% |  |
| SWAP | 14,091,320 | 0.2% | 98.5% |  |
| COPY | 10,835,880 | 0.2% | 98.7% |  |
| IS_OP | 10,113,040 | 0.1% | 98.8% |  |
| CALL_TYPE_1 | 10,112,980 | 0.1% | 99.0% |  |
| EXTENDED_ARG | 9,448,900 | 0.1% | 99.1% |  |
| POP_JUMP_IF_NOT_NONE | 9,448,480 | 0.1% | 99.2% |  |
| CALL_BUILTIN_CLASS | 9,419,180 | 0.1% | 99.3% |  |
| LOAD_ATTR_METHOD_NO_DICT | 4,857,220 | 0.1% | 99.4% | 1.0% |
| CALL_LEN | 4,647,240 | 0.1% | 99.5% |  |
| CALL_KW | 4,647,120 | 0.1% | 99.5% |  |
| TO_BOOL | 4,356,140 | 0.1% | 99.6% |  |
| LOAD_ATTR_PROPERTY | 3,246,800 | 0.0% | 99.7% | 0.8% |
| TO_BOOL_LIST | 2,472,100 | 0.0% | 99.7% |  |
| FOR_ITER_TUPLE | 2,461,300 | 0.0% | 99.7% | 6.9% |
| STORE_FAST_LOAD_FAST | 2,286,340 | 0.0% | 99.8% |  |
| UNARY_NEGATIVE | 1,900,540 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 1,655,280 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,615,560 | 0.0% | 99.8% | 55.4% |
| FOR_ITER | 1,603,780 | 0.0% | 99.9% |  |
| BUILD_LIST | 1,171,520 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 1,171,320 | 0.0% | 99.9% |  |
| CALL_LIST_APPEND | 771,640 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 734,960 | 0.0% | 99.9% |  |
| BUILD_MAP | 720,800 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 665,460 | 0.0% | 99.9% |  |
| LIST_APPEND | 586,160 | 0.0% | 99.9% |  |
| MAP_ADD | 535,560 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 491,860 | 0.0% | 100.0% |  |
| CONTAINS_OP | 387,580 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 385,680 | 0.0% | 100.0% |  |
| POP_EXCEPT | 385,680 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 385,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 385,660 | 0.0% | 100.0% |  |
| COMPARE_OP | 294,960 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 292,960 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 292,800 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 292,700 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 292,700 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 105,800 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 9,040 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 7,960 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 4,340 | 0.0% | 100.0% |  |
| RESUME | 1,000 | 0.0% | 100.0% | 92.0% |
| UNPACK_SEQUENCE | 680 | 0.0% | 100.0% |  |
| STORE_ATTR | 480 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 380 | 0.0% | 100.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 360 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 300 | 0.0% | 100.0% |  |
| MAKE_CELL | 160 | 0.0% | 100.0% |  |
| STORE_DEREF | 160 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 80 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 60 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 60 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 60 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| CACHE RESUME_CHECK | 333,005,880 | 4.7% | 4.7% |
| POP_TOP ENTER_EXECUTOR | 324,970,380 | 4.6% | 9.3% |
| YIELD_VALUE INTERPRETER_EXIT | 324,495,840 | 4.6% | 13.9% |
| RESUME_CHECK POP_TOP | 324,495,720 | 4.6% | 18.4% |
| ENTER_EXECUTOR YIELD_VALUE | 260,347,940 | 3.7% | 22.1% |
| LOAD_DEREF LOAD_FAST | 191,857,320 | 2.7% | 24.8% |
| LOAD_FAST LOAD_ATTR_SLOT | 130,015,840 | 1.8% | 26.6% |
| LOAD_FAST BINARY_SUBSCR | 126,108,600 | 1.8% | 28.4% |
| RESUME_CHECK LOAD_FAST | 106,363,340 | 1.5% | 29.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 89,674,520 | 1.3% | 31.2% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 88,230,880 | 1.2% | 32.4% |
| COPY_FREE_VARS RESUME_CHECK | 79,365,060 | 1.1% | 33.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 76,825,460 | 1.1% | 34.6% |
| LOAD_FAST LOAD_CONST | 75,049,920 | 1.1% | 35.7% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 74,935,420 | 1.1% | 36.7% |
| STORE_FAST LOAD_FAST | 72,467,660 | 1.0% | 37.8% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 71,522,220 | 1.0% | 38.8% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 71,320,680 | 1.0% | 39.8% |
| RETURN_VALUE RETURN_VALUE | 67,699,120 | 1.0% | 40.7% |
| LOAD_CONST COMPARE_OP_INT | 66,888,060 | 0.9% | 41.7% |
| STORE_FAST LOAD_DEREF | 66,708,760 | 0.9% | 42.6% |
| LOAD_ATTR_SLOT LOAD_FAST | 65,008,120 | 0.9% | 43.5% |
| ENTER_EXECUTOR FOR_ITER_LIST | 63,096,860 | 0.9% | 44.4% |
| RETURN_CONST INTERPRETER_EXIT | 62,867,220 | 0.9% | 45.3% |
| CACHE POP_TOP | 62,832,560 | 0.9% | 46.2% |
| POP_TOP RESUME_CHECK | 62,832,440 | 0.9% | 47.1% |
| LOAD_FAST STORE_SUBSCR | 62,565,320 | 0.9% | 48.0% |
| FOR_ITER_LIST RETURN_CONST | 62,390,320 | 0.9% | 48.8% |
| LOAD_FAST FOR_ITER_LIST | 62,390,240 | 0.9% | 49.7% |
| COPY_FREE_VARS RETURN_GENERATOR | 62,353,760 | 0.9% | 50.6% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS LOAD_DEREF | 62,353,680 | 0.9% | 51.5% |
| RETURN_GENERATOR CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,353,600 | 0.9% | 52.4% |
| LOAD_ATTR_SLOT STORE_FAST_STORE_FAST | 61,207,680 | 0.9% | 53.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 59,743,900 | 0.8% | 54.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 58,243,560 | 0.8% | 54.9% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 56,928,840 | 0.8% | 55.7% |
| LOAD_ATTR_MODULE PUSH_NULL | 54,150,740 | 0.8% | 56.4% |
| CALL_BUILTIN_FAST STORE_FAST | 54,150,560 | 0.8% | 57.2% |
| LOAD_FAST RETURN_VALUE | 50,118,160 | 0.7% | 57.9% |
| RETURN_VALUE INTERPRETER_EXIT | 48,528,120 | 0.7% | 58.6% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_INT | 48,105,760 | 0.7% | 59.3% |
| BINARY_SUBSCR LOAD_FAST | 47,486,060 | 0.7% | 59.9% |
| CALL STORE_FAST | 45,285,640 | 0.6% | 60.6% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 44,188,880 | 0.6% | 61.2% |
| LOAD_DEREF PUSH_NULL | 43,667,280 | 0.6% | 61.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 43,498,580 | 0.6% | 62.4% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 42,471,180 | 0.6% | 63.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 42,470,980 | 0.6% | 63.6% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 42,287,480 | 0.6% | 64.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 42,285,400 | 0.6% | 64.8% |
| STORE_FAST STORE_FAST | 42,251,800 | 0.6% | 65.4% |
| LOAD_CONST MAKE_FUNCTION | 42,192,420 | 0.6% | 66.0% |
| LOAD_FAST BINARY_SUBSCR_DICT | 42,192,100 | 0.6% | 66.6% |
| LOAD_FAST BUILD_TUPLE | 42,189,120 | 0.6% | 67.2% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 42,131,140 | 0.6% | 67.8% |
| RETURN_VALUE GET_ITER | 41,899,620 | 0.6% | 68.4% |
| NOP LOAD_FAST | 41,899,460 | 0.6% | 69.0% |
| RESUME_CHECK NOP | 41,899,440 | 0.6% | 69.6% |
| GET_ITER CALL_PY_EXACT_ARGS | 41,899,420 | 0.6% | 70.2% |
| BINARY_OP_MULTIPLY_FLOAT YIELD_VALUE | 41,716,800 | 0.6% | 70.8% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST | 41,716,800 | 0.6% | 71.3% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 41,716,760 | 0.6% | 71.9% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 41,716,760 | 0.6% | 72.5% |
| BUILD_TUPLE LOAD_CONST | 41,699,700 | 0.6% | 73.1% |
| MAKE_FUNCTION SET_FUNCTION_ATTRIBUTE | 41,513,780 | 0.6% | 73.7% |
| SET_FUNCTION_ATTRIBUTE LOAD_FAST | 41,513,780 | 0.6% | 74.3% |
| BINARY_SUBSCR_DICT RETURN_VALUE | 41,513,780 | 0.6% | 74.9% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 41,513,700 | 0.6% | 75.4% |
| LOAD_FAST CALL | 41,224,440 | 0.6% | 76.0% |
| LOAD_FAST BINARY_OP | 41,152,060 | 0.6% | 76.6% |
| CACHE COPY_FREE_VARS | 40,052,400 | 0.6% | 77.2% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST | 40,052,360 | 0.6% | 77.7% |
| STORE_ATTR_SLOT LOAD_FAST | 40,052,340 | 0.6% | 78.3% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 40,052,320 | 0.6% | 78.9% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 40,052,320 | 0.6% | 79.4% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 39,893,680 | 0.6% | 80.0% |
| BINARY_OP BINARY_OP_MULTIPLY_INT | 36,261,020 | 0.5% | 80.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 35,282,320 | 0.5% | 81.0% |
| CALL_BOUND_METHOD_EXACT_ARGS COPY_FREE_VARS | 34,958,180 | 0.5% | 81.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 34,553,040 | 0.5% | 82.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 33,089,440 | 0.5% | 82.5% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 32,954,800 | 0.5% | 82.9% |
| STORE_FAST_STORE_FAST LOAD_FAST | 32,683,720 | 0.5% | 83.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 32,429,480 | 0.5% | 83.8% |
| BINARY_SUBSCR LOAD_DEREF | 31,291,680 | 0.4% | 84.3% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 31,268,440 | 0.4% | 84.7% |
| COMPARE_OP_FLOAT POP_JUMP_IF_TRUE | 31,176,860 | 0.4% | 85.2% |
| BINARY_SUBSCR COMPARE_OP_FLOAT | 31,176,840 | 0.4% | 85.6% |
| STORE_SUBSCR LOAD_GLOBAL_BUILTIN | 31,176,800 | 0.4% | 86.0% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 31,070,780 | 0.4% | 86.5% |
| STORE_FAST_STORE_FAST LOAD_GLOBAL_MODULE | 31,003,500 | 0.4% | 86.9% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST_LOAD_FAST | 30,896,520 | 0.4% | 87.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 30,604,100 | 0.4% | 87.8% |
| POP_JUMP_IF_FALSE LOAD_DEREF | 30,604,000 | 0.4% | 88.2% |
| LOAD_ATTR LOAD_FAST_LOAD_FAST | 30,603,920 | 0.4% | 88.6% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 30,311,160 | 0.4% | 89.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 30,162,120 | 0.4% | 89.5% |
| BINARY_OP_MULTIPLY_INT CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 0.4% | 89.9% |
| BINARY_OP_MULTIPLY_INT BINARY_OP_ADD_INT | 28,837,600 | 0.4% | 90.3% |
| BINARY_OP STORE_FAST | 25,485,260 | 0.4% | 90.7% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 333,005,880 | 76.4% |
| POP_TOP | 62,832,560 | 14.4% |
| COPY_FREE_VARS | 40,052,400 | 9.2% |
| RESUME | 340 | 0.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 126,108,600 | 96.1% |
| COPY | 5,032,780 | 3.8% |
| BINARY_SUBSCR | 35,380 | 0.0% |
| LOAD_CONST | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,486,060 | 36.2% |
| LOAD_DEREF | 31,291,680 | 23.9% |
| COMPARE_OP_FLOAT | 31,176,840 | 23.8% |
| YIELD_VALUE | 20,637,440 | 15.7% |
| LOAD_FAST_LOAD_FAST | 434,480 | 0.3% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 385,660 | 100.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 385,680 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 60 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 41,899,620 | 93.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,306,040 | 2.9% |
| CALL_BUILTIN_CLASS | 585,420 | 1.3% |
| LOAD_FAST | 293,440 | 0.7% |
| CALL | 292,940 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 41,899,420 | 93.8% |
| LOAD_FAST_AND_CLEAR | 1,120,400 | 2.5% |
| FOR_ITER | 1,064,180 | 2.4% |
| FOR_ITER_LIST | 293,240 | 0.7% |
| FOR_ITER_TUPLE | 278,840 | 0.6% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 324,495,840 | 74.4% |
| RETURN_CONST | 62,867,220 | 14.4% |
| RETURN_VALUE | 48,528,120 | 11.1% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 42,192,420 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 41,513,780 | 98.4% |
| LOAD_FAST | 385,840 | 0.9% |
| LOAD_CONST | 292,720 | 0.7% |
| CALL | 80 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 41,899,440 | 100.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,899,460 | 100.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 385,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 385,680 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 324,495,720 | 83.5% |
| CACHE | 62,832,560 | 16.2% |
| CALL_METHOD_DESCRIPTOR_O | 491,860 | 0.1% |
| POP_JUMP_IF_FALSE | 385,680 | 0.1% |
| RETURN_CONST | 371,840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 324,970,380 | 83.6% |
| RESUME_CHECK | 62,832,440 | 16.2% |
| LOAD_FAST | 386,040 | 0.1% |
| JUMP_FORWARD | 385,840 | 0.1% |
| JUMP_BACKWARD | 3,060 | 0.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 385,660 | 100.0% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 385,640 | 100.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 54,150,740 | 54.1% |
| LOAD_DEREF | 43,667,280 | 43.6% |
| LOAD_FAST | 2,286,080 | 2.3% |
| LOAD_ATTR | 220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 88,230,880 | 88.1% |
| LOAD_FAST | 11,580,480 | 11.6% |
| LOAD_GLOBAL_MODULE | 292,680 | 0.3% |
| CALL | 240 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 62,353,760 | 99.2% |
| CALL_PY_EXACT_ARGS | 478,760 | 0.8% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,353,600 | 99.2% |
| CALL_METHOD_DESCRIPTOR_O | 385,800 | 0.6% |
| CALL_BUILTIN_CLASS | 92,920 | 0.1% |
| CALL | 240 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 67,699,120 | 39.3% |
| LOAD_FAST | 50,118,160 | 29.1% |
| BINARY_SUBSCR_DICT | 41,513,780 | 24.1% |
| CALL_BUILTIN_FAST | 4,678,680 | 2.7% |
| LOAD_ATTR_SLOT | 3,800,440 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 67,699,120 | 39.3% |
| INTERPRETER_EXIT | 48,528,120 | 28.2% |
| GET_ITER | 41,899,620 | 24.3% |
| STORE_FAST | 10,507,600 | 6.1% |
| CALL_BUILTIN_CLASS | 3,214,960 | 1.9% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,565,320 | 92.5% |
| SWAP | 5,032,780 | 7.4% |
| STORE_SUBSCR | 18,420 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 31,176,800 | 46.1% |
| LOAD_DEREF | 20,964,080 | 31.0% |
| JUMP_FORWARD | 10,318,560 | 15.3% |
| ENTER_EXECUTOR | 5,031,420 | 7.4% |
| LOAD_FAST | 105,860 | 0.2% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,354,600 | 100.0% |
| TO_BOOL | 1,260 | 0.0% |
| LOAD_ATTR | 120 | 0.0% |
| CALL | 80 | 0.0% |
| CALL_ISINSTANCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,354,640 | 100.0% |
| TO_BOOL | 1,260 | 0.0% |
| TO_BOOL_BOOL | 160 | 0.0% |
| TO_BOOL_LIST | 60 | 0.0% |
| TO_BOOL_INT | 20 | 0.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 1,607,500 | 84.6% |
| LOAD_FAST_LOAD_FAST | 293,020 | 15.4% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,607,520 | 84.6% |
| CALL_PY_EXACT_ARGS | 292,980 | 15.4% |
| CALL | 40 | 0.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,152,060 | 47.8% |
| LOAD_FAST_LOAD_FAST | 39,893,680 | 46.3% |
| LOAD_CONST | 1,761,480 | 2.0% |
| CALL_BUILTIN_CLASS | 1,607,500 | 1.9% |
| BINARY_OP_MULTIPLY_INT | 585,480 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 36,261,020 | 42.1% |
| STORE_FAST | 25,485,260 | 29.6% |
| LOAD_FAST_LOAD_FAST | 14,852,080 | 17.2% |
| SWAP | 5,032,780 | 5.8% |
| RETURN_VALUE | 1,607,620 | 1.9% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 585,600 | 50.0% |
| LOAD_FAST | 292,880 | 25.0% |
| LOAD_FAST_LOAD_FAST | 292,720 | 25.0% |
| POP_JUMP_IF_FALSE | 160 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 585,600 | 50.0% |
| CALL | 292,800 | 25.0% |
| LOAD_FAST_LOAD_FAST | 292,720 | 25.0% |
| RETURN_VALUE | 160 | 0.0% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 534,800 | 74.2% |
| CALL | 185,920 | 25.8% |
| RESUME_CHECK | 60 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 534,800 | 74.2% |
| RETURN_VALUE | 185,920 | 25.8% |
| LOAD_FAST | 80 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,189,120 | 83.4% |
| LOAD_FAST_LOAD_FAST | 4,261,920 | 8.4% |
| BINARY_SUBSCR_TUPLE_INT | 1,849,860 | 3.7% |
| LOAD_CONST | 1,700,980 | 3.4% |
| CALL | 371,840 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 41,699,700 | 82.5% |
| COPY | 4,168,480 | 8.2% |
| YIELD_VALUE | 1,793,620 | 3.5% |
| RETURN_VALUE | 1,607,520 | 3.2% |
| LOAD_FAST | 391,660 | 0.8% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,224,440 | 86.6% |
| LOAD_FAST_LOAD_FAST | 4,355,000 | 9.1% |
| LOAD_GLOBAL_MODULE | 878,120 | 1.8% |
| LOAD_CONST | 851,080 | 1.8% |
| BUILD_LIST | 292,800 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 45,285,640 | 95.1% |
| CALL_PY_EXACT_ARGS | 586,100 | 1.2% |
| LOAD_FAST | 585,720 | 1.2% |
| BUILD_TUPLE | 371,840 | 0.8% |
| GET_ITER | 292,940 | 0.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 292,800 | 99.9% |
| CALL_INTRINSIC_1 | 80 | 0.0% |
| STORE_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 292,680 | 99.9% |
| RETURN_VALUE | 80 | 0.0% |
| COPY_FREE_VARS | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |
| CALL | 40 | 0.0% |


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
| ENTER_EXECUTOR | 3,875,460 | 83.4% |
| LOAD_CONST | 771,660 | 16.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 4,354,400 | 93.7% |
| STORE_FAST | 292,720 | 6.3% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 294,220 | 99.7% |
| COMPARE_OP | 460 | 0.2% |
| LOAD_FAST | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 293,200 | 99.4% |
| POP_JUMP_IF_FALSE | 580 | 0.2% |
| COMPARE_OP_INT | 520 | 0.2% |
| COMPARE_OP | 460 | 0.2% |
| COMPARE_OP_FLOAT | 80 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 387,580 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 385,840 | 99.6% |
| POP_JUMP_IF_FALSE | 1,740 | 0.4% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 5,032,780 | 46.4% |
| BUILD_TUPLE | 4,168,480 | 38.5% |
| LOAD_FAST_LOAD_FAST | 864,300 | 8.0% |
| SWAP | 664,560 | 6.1% |
| BINARY_OP | 105,760 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 5,032,780 | 46.4% |
| COPY | 5,032,780 | 46.4% |
| IS_OP | 664,560 | 6.1% |
| LOAD_DEREF | 105,760 | 1.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 41,513,700 | 29.3% |
| CACHE | 40,052,400 | 28.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 34,958,180 | 24.7% |
| ENTER_EXECUTOR | 20,839,980 | 14.7% |
| CALL_KW | 4,354,400 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 79,365,060 | 56.0% |
| RETURN_GENERATOR | 62,353,760 | 44.0% |
| RESUME | 140 | 0.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 324,970,380 | 87.0% |
| POP_JUMP_IF_TRUE | 31,070,780 | 8.3% |
| ENTER_EXECUTOR | 8,494,200 | 2.3% |
| STORE_SUBSCR | 5,031,420 | 1.3% |
| POP_JUMP_IF_FALSE | 2,187,400 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 260,347,940 | 69.7% |
| FOR_ITER_LIST | 63,096,860 | 16.9% |
| COPY_FREE_VARS | 20,839,980 | 5.6% |
| LOAD_FAST | 8,985,840 | 2.4% |
| ENTER_EXECUTOR | 8,494,200 | 2.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,448,480 | 100.0% |
| POP_JUMP_IF_FALSE | 340 | 0.0% |
| COMPARE_OP_FLOAT | 60 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 9,448,480 | 100.0% |
| JUMP_BACKWARD | 340 | 0.0% |
| POP_JUMP_IF_FALSE | 80 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,064,180 | 66.4% |
| SWAP | 534,920 | 33.4% |
| JUMP_BACKWARD | 2,800 | 0.2% |
| FOR_ITER | 1,780 | 0.1% |
| LOAD_FAST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 1,600,420 | 99.8% |
| FOR_ITER | 1,780 | 0.1% |
| UNPACK_SEQUENCE | 380 | 0.0% |
| RETURN_CONST | 300 | 0.0% |
| SWAP | 280 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 8,783,900 | 86.9% |
| COPY | 664,560 | 6.6% |
| CALL_TYPE_1 | 664,540 | 6.6% |
| CALL | 20 | 0.0% |
| LOAD_GLOBAL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,113,040 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 3,060 | 38.4% |
| STORE_SUBSCR | 1,360 | 17.1% |
| MAP_ADD | 1,020 | 12.8% |
| LIST_APPEND | 740 | 9.3% |
| POP_JUMP_IF_FALSE | 600 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,800 | 35.2% |
| FOR_ITER_LIST | 2,800 | 35.2% |
| FOR_ITER_TUPLE | 920 | 11.6% |
| LOAD_FAST | 640 | 8.0% |
| ENTER_EXECUTOR | 440 | 5.5% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 10,318,560 | 68.3% |
| ENTER_EXECUTOR | 1,407,620 | 9.3% |
| POP_JUMP_IF_FALSE | 664,620 | 4.4% |
| JUMP_FORWARD | 664,560 | 4.4% |
| STORE_FAST | 510,320 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 10,318,560 | 68.3% |
| LOAD_FAST | 2,843,760 | 18.8% |
| STORE_FAST | 776,880 | 5.1% |
| JUMP_FORWARD | 664,560 | 4.4% |
| LOAD_FAST_LOAD_FAST | 324,400 | 2.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 585,760 | 99.9% |
| LOAD_FAST | 240 | 0.0% |
| BUILD_TUPLE | 80 | 0.0% |
| JUMP_FORWARD | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 585,420 | 99.9% |
| JUMP_BACKWARD | 740 | 0.1% |


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
| LOAD_GLOBAL_MODULE | 30,604,100 | 60.2% |
| LOAD_FAST | 16,950,960 | 33.4% |
| LOAD_ATTR | 2,044,720 | 4.0% |
| BINARY_SUBSCR_TUPLE_INT | 1,222,260 | 2.4% |
| LOAD_ATTR_PROPERTY | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 30,603,920 | 60.2% |
| LOAD_DEREF | 8,708,800 | 17.1% |
| BINARY_OP_MULTIPLY_INT | 3,769,120 | 7.4% |
| LOAD_FAST | 2,528,680 | 5.0% |
| LOAD_ATTR | 2,044,720 | 4.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,049,920 | 51.3% |
| BUILD_TUPLE | 41,699,700 | 28.5% |
| BINARY_SUBSCR_TUPLE_INT | 8,974,220 | 6.1% |
| STORE_ATTR_SLOT | 8,783,900 | 6.0% |
| STORE_FAST_LOAD_FAST | 1,700,580 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 66,888,060 | 45.7% |
| MAKE_FUNCTION | 42,192,420 | 28.8% |
| BINARY_SUBSCR_TUPLE_INT | 14,523,920 | 9.9% |
| LOAD_FAST | 10,776,040 | 7.4% |
| BINARY_OP | 1,761,480 | 1.2% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 66,708,760 | 27.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,353,680 | 26.0% |
| BINARY_SUBSCR | 31,291,680 | 13.0% |
| POP_JUMP_IF_FALSE | 30,604,000 | 12.8% |
| STORE_SUBSCR | 20,964,080 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 191,857,320 | 80.0% |
| PUSH_NULL | 43,667,280 | 18.2% |
| COMPARE_OP_INT | 4,354,360 | 1.8% |
| LIST_EXTEND | 80 | 0.0% |
| COMPARE_OP | 40 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 191,857,320 | 19.1% |
| RESUME_CHECK | 106,363,340 | 10.6% |
| LOAD_GLOBAL_BUILTIN | 89,674,520 | 8.9% |
| STORE_FAST | 72,467,660 | 7.2% |
| LOAD_ATTR_SLOT | 65,008,120 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 130,015,840 | 13.0% |
| BINARY_SUBSCR | 126,108,600 | 12.6% |
| LOAD_CONST | 75,049,920 | 7.5% |
| STORE_SUBSCR | 62,565,320 | 6.2% |
| FOR_ITER_LIST | 62,390,240 | 6.2% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,120,400 | 67.7% |
| LOAD_FAST_AND_CLEAR | 534,880 | 32.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,120,400 | 67.7% |
| LOAD_FAST_AND_CLEAR | 534,880 | 32.3% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 292,760 | 100.0% |
| LOAD_GLOBAL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 292,680 | 100.0% |
| LOAD_FAST | 80 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 88,230,880 | 28.7% |
| STORE_FAST | 59,743,900 | 19.4% |
| POP_JUMP_IF_FALSE | 32,954,800 | 10.7% |
| STORE_ATTR_SLOT | 31,268,440 | 10.2% |
| BINARY_OP_MULTIPLY_INT | 30,896,520 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 71,320,680 | 23.2% |
| CALL_BUILTIN_FAST | 56,928,840 | 18.5% |
| BINARY_OP_MULTIPLY_INT | 48,105,760 | 15.6% |
| LOAD_FAST | 44,188,880 | 14.4% |
| BINARY_OP | 39,893,680 | 13.0% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 900 | 20.7% |
| POP_JUMP_IF_FALSE | 760 | 17.5% |
| LOAD_FAST | 480 | 11.1% |
| LOAD_CONST | 280 | 6.5% |
| RESUME_CHECK | 280 | 6.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,420 | 32.7% |
| LOAD_GLOBAL_BUILTIN | 760 | 17.5% |
| LOAD_FAST | 700 | 16.1% |
| LOAD_ATTR | 420 | 9.7% |
| LOAD_CONST | 300 | 6.9% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 50.0% |
| LOAD_SUPER_ATTR_METHOD | 40 | 50.0% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 80 | 50.0% |
| CALL_PY_EXACT_ARGS | 60 | 37.5% |
| CALL | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 80 | 50.0% |
| RESUME_CHECK | 60 | 37.5% |
| RESUME | 20 | 12.5% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 293,140 | 54.7% |
| LOAD_FAST | 242,380 | 45.3% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 534,540 | 99.8% |
| JUMP_BACKWARD | 1,020 | 0.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 71,522,220 | 57.7% |
| TO_BOOL_BOOL | 34,553,040 | 27.9% |
| IS_OP | 10,113,040 | 8.2% |
| TO_BOOL | 4,354,640 | 3.5% |
| TO_BOOL_LIST | 2,472,100 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 32,954,800 | 26.6% |
| LOAD_GLOBAL_MODULE | 32,429,480 | 26.2% |
| LOAD_DEREF | 30,604,000 | 24.7% |
| LOAD_FAST | 13,505,820 | 10.9% |
| LOAD_GLOBAL_BUILTIN | 9,939,480 | 8.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 9,448,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 9,448,400 | 100.0% |
| LOAD_GLOBAL | 80 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_FLOAT | 31,176,860 | 97.9% |
| CONTAINS_OP | 385,840 | 1.2% |
| COMPARE_OP | 293,200 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 31,070,780 | 97.5% |
| LOAD_FAST | 679,020 | 2.1% |
| LOAD_DEREF | 105,760 | 0.3% |
| JUMP_BACKWARD | 340 | 0.0% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 62,390,320 | 98.7% |
| FOR_ITER_TUPLE | 442,240 | 0.7% |
| ENTER_EXECUTOR | 371,540 | 0.6% |
| RESUME_CHECK | 34,620 | 0.1% |
| FOR_ITER | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 62,867,220 | 99.4% |
| POP_TOP | 371,840 | 0.6% |
| EXIT_INIT_CHECK | 60 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 41,513,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,513,780 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 58.3% |
| LOAD_FAST_LOAD_FAST | 200 | 41.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 120 | 25.0% |
| STORE_ATTR_SLOT | 120 | 25.0% |
| LOAD_CONST | 80 | 16.7% |
| LOAD_FAST | 60 | 12.5% |
| LOAD_GLOBAL | 60 | 12.5% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 50.0% |
| SWAP | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_DEREF | 80 | 50.0% |
| STORE_FAST | 80 | 50.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 54,150,560 | 20.1% |
| CALL | 45,285,640 | 16.8% |
| STORE_FAST | 42,251,800 | 15.7% |
| UNPACK_SEQUENCE_TWO_TUPLE | 41,716,800 | 15.5% |
| BINARY_OP | 25,485,260 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 72,467,660 | 26.9% |
| LOAD_DEREF | 66,708,760 | 24.8% |
| LOAD_FAST_LOAD_FAST | 59,743,900 | 22.2% |
| STORE_FAST | 42,251,800 | 15.7% |
| LOAD_GLOBAL_MODULE | 24,248,720 | 9.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 1,550,640 | 67.8% |
| FOR_ITER_RANGE | 585,740 | 25.6% |
| FOR_ITER_LIST | 149,900 | 6.6% |
| FOR_ITER | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,700,580 | 74.4% |
| LOAD_FAST | 585,760 | 25.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 61,207,680 | 94.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,880,120 | 2.9% |
| UNPACK_SEQUENCE_TUPLE | 734,960 | 1.1% |
| BINARY_OP_MULTIPLY_INT | 585,420 | 0.9% |
| STORE_FAST_STORE_FAST | 106,800 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,683,720 | 50.7% |
| LOAD_GLOBAL_MODULE | 31,003,500 | 48.1% |
| STORE_FAST | 628,240 | 1.0% |
| STORE_FAST_STORE_FAST | 106,800 | 0.2% |
| LOAD_CONST | 92,960 | 0.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 5,032,780 | 35.7% |
| SWAP | 5,032,780 | 35.7% |
| LOAD_FAST_AND_CLEAR | 1,120,400 | 8.0% |
| LOAD_GLOBAL_BUILTIN | 664,540 | 4.7% |
| BUILD_LIST | 585,600 | 4.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 5,032,780 | 35.7% |
| SWAP | 5,032,780 | 35.7% |
| STORE_FAST | 1,120,320 | 8.0% |
| COPY | 664,560 | 4.7% |
| BUILD_LIST | 585,600 | 4.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 380 | 55.9% |
| LOAD_FAST | 200 | 29.4% |
| FOR_ITER_LIST | 40 | 5.9% |
| CALL | 20 | 2.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 300 | 44.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 260 | 38.2% |
| UNPACK_SEQUENCE_TUPLE | 80 | 11.8% |
| STORE_FAST | 40 | 5.9% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 260,347,940 | 80.2% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 12.9% |
| BINARY_SUBSCR | 20,637,440 | 6.4% |
| BUILD_TUPLE | 1,793,620 | 0.6% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 324,495,840 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 340 | 34.0% |
| CALL | 340 | 34.0% |
| COPY_FREE_VARS | 140 | 14.0% |
| POP_TOP | 120 | 12.0% |
| CALL_FUNCTION_EX | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 42.0% |
| LOAD_GLOBAL | 260 | 26.0% |
| POP_TOP | 120 | 12.0% |
| LOAD_CONST | 60 | 6.0% |
| LOAD_DEREF | 40 | 4.0% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 105,760 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 105,800 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 28,837,600 | 92.0% |
| LOAD_CONST | 1,171,160 | 3.7% |
| BINARY_OP | 856,760 | 2.7% |
| LOAD_FAST | 478,900 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 22,851,080 | 72.9% |
| LOAD_FAST_LOAD_FAST | 7,428,940 | 23.7% |
| LOAD_FAST | 585,420 | 1.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 478,900 | 1.5% |
| RETURN_VALUE | 60 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,716,760 | 100.0% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 41,716,800 | 100.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 48,105,760 | 49.1% |
| BINARY_OP | 36,261,020 | 37.0% |
| LOAD_FAST | 8,898,680 | 9.1% |
| LOAD_ATTR | 3,769,120 | 3.8% |
| LOAD_CONST | 878,080 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 30,896,520 | 31.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 30.6% |
| BINARY_OP_ADD_INT | 28,837,600 | 29.4% |
| LOAD_FAST | 3,071,060 | 3.1% |
| CALL_BUILTIN_FAST | 1,900,200 | 1.9% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 8,880 | 98.2% |
| BINARY_OP | 80 | 0.9% |
| LOAD_FAST | 80 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,920 | 98.7% |
| STORE_FAST | 60 | 0.7% |
| CALL_BUILTIN_O | 40 | 0.4% |
| CALL | 20 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 292,680 | 100.0% |
| BINARY_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 292,700 | 100.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,192,100 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 41,513,780 | 98.4% |
| PUSH_EXC_INFO | 385,660 | 0.9% |
| STORE_FAST | 292,700 | 0.7% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 292,680 | 100.0% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 292,700 | 100.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,523,920 | 100.0% |
| BINARY_SUBSCR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,974,220 | 61.8% |
| BUILD_TUPLE | 1,849,860 | 12.7% |
| UNARY_NEGATIVE | 1,607,500 | 11.1% |
| LOAD_ATTR | 1,222,260 | 8.4% |
| LOAD_FAST | 484,720 | 3.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 60 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 30,018,280 | 84.9% |
| CALL_BUILTIN_CLASS | 4,354,360 | 12.3% |
| LOAD_FAST_LOAD_FAST | 585,400 | 1.7% |
| LOAD_FAST | 385,800 | 1.1% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 34,958,180 | 98.9% |
| RESUME_CHECK | 385,820 | 1.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,647,500 | 49.3% |
| RETURN_VALUE | 3,214,960 | 34.1% |
| LOAD_CONST | 585,400 | 6.2% |
| BINARY_OP_MULTIPLY_INT | 585,400 | 6.2% |
| CALL_FUNCTION_EX | 292,680 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 4,354,360 | 46.2% |
| BINARY_OP | 1,607,500 | 17.1% |
| LOAD_GLOBAL_BUILTIN | 1,607,480 | 17.1% |
| STORE_FAST | 678,480 | 7.2% |
| GET_ITER | 585,420 | 6.2% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 56,928,840 | 96.8% |
| BINARY_OP_MULTIPLY_INT | 1,900,200 | 3.2% |
| CALL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 54,150,560 | 92.0% |
| RETURN_VALUE | 4,678,680 | 8.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 62,353,600 | 98.0% |
| BINARY_OP_ADD_INT | 478,900 | 0.8% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 478,900 | 0.8% |
| CALL | 292,820 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,353,680 | 98.0% |
| STORE_FAST | 771,620 | 1.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 478,900 | 0.8% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 40 | 66.7% |
| CALL | 20 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60 | 100.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 30,311,160 | 91.6% |
| LOAD_ATTR_MODULE | 2,192,880 | 6.6% |
| LOAD_GLOBAL_BUILTIN | 585,400 | 1.8% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 33,089,440 | 100.0% |
| TO_BOOL | 80 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,647,200 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 4,354,380 | 93.7% |
| BINARY_OP | 292,860 | 6.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 385,800 | 50.0% |
| ENTER_EXECUTOR | 385,520 | 50.0% |
| BUILD_TUPLE | 280 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 771,640 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 360 | 94.7% |
| CALL | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 360 | 94.7% |
| UNPACK_SEQUENCE | 20 | 5.3% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,598,600 | 99.0% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 16,820 | 1.0% |
| CALL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,306,040 | 80.8% |
| LOAD_CONST | 292,700 | 18.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 16,820 | 1.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 385,800 | 78.4% |
| LOAD_FAST | 106,000 | 21.6% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 491,860 | 100.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,498,580 | 36.6% |
| GET_ITER | 41,899,420 | 35.3% |
| LOAD_FAST_LOAD_FAST | 30,162,120 | 25.4% |
| LOAD_ATTR_MODULE | 1,900,160 | 1.6% |
| CALL | 586,100 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 76,825,460 | 64.6% |
| COPY_FREE_VARS | 41,513,700 | 34.9% |
| RETURN_GENERATOR | 478,760 | 0.4% |
| CALL_PY_EXACT_ARGS | 31,800 | 0.0% |
| MAKE_CELL | 60 | 0.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,112,920 | 100.0% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 9,448,400 | 93.4% |
| IS_OP | 664,540 | 6.6% |
| LOAD_GLOBAL | 40 | 0.0% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 31,176,840 | 100.0% |
| LOAD_FAST | 8,920 | 0.0% |
| COMPARE_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 31,176,860 | 100.0% |
| POP_JUMP_IF_FALSE | 8,920 | 0.0% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 66,888,060 | 93.5% |
| LOAD_DEREF | 4,354,360 | 6.1% |
| LOAD_FAST_LOAD_FAST | 279,280 | 0.4% |
| COMPARE_OP | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 71,522,220 | 100.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 665,400 | 100.0% |
| COMPARE_OP | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 372,440 | 56.0% |
| POP_JUMP_IF_FALSE | 293,020 | 44.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 63,096,860 | 50.2% |
| LOAD_FAST | 62,390,240 | 49.6% |
| GET_ITER | 293,240 | 0.2% |
| FOR_ITER_TUPLE | 3,180 | 0.0% |
| JUMP_BACKWARD | 2,800 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 62,390,320 | 49.6% |
| UNPACK_SEQUENCE_TWO_TUPLE | 41,716,760 | 33.2% |
| STORE_FAST | 20,932,000 | 16.6% |
| ENTER_EXECUTOR | 585,100 | 0.5% |
| STORE_FAST_LOAD_FAST | 149,900 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 585,440 | 50.0% |
| SWAP | 585,420 | 50.0% |
| JUMP_BACKWARD | 360 | 0.0% |
| GET_ITER | 60 | 0.0% |
| FOR_ITER | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 585,740 | 50.0% |
| SWAP | 585,440 | 50.0% |
| STORE_FAST | 60 | 0.0% |
| LOAD_GLOBAL | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,829,040 | 74.3% |
| LOAD_FAST | 349,260 | 14.2% |
| GET_ITER | 278,840 | 11.3% |
| FOR_ITER_LIST | 3,200 | 0.1% |
| JUMP_BACKWARD | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 1,550,640 | 63.0% |
| RETURN_CONST | 442,240 | 18.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 186,200 | 7.6% |
| LOAD_FAST | 185,920 | 7.6% |
| STORE_FAST | 93,100 | 3.8% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,131,140 | 99.1% |
| LOAD_FAST_LOAD_FAST | 385,640 | 0.9% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,285,400 | 99.5% |
| STORE_FAST | 231,380 | 0.5% |
| STORE_SUBSCR | 120 | 0.0% |
| BUILD_LIST | 60 | 0.0% |
| SWAP | 60 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,084,660 | 84.1% |
| RETURN_VALUE | 478,560 | 9.9% |
| LOAD_FAST_CHECK | 292,680 | 6.0% |
| LOAD_ATTR_METHOD_NO_DICT | 940 | 0.0% |
| LOAD_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,871,340 | 59.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,598,600 | 32.9% |
| LOAD_CONST | 385,820 | 7.9% |
| LOAD_ATTR_METHOD_NO_DICT | 940 | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 360 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,470,980 | 100.0% |
| LOAD_ATTR | 220 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,471,180 | 100.0% |
| LOAD_CONST | 60 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 58,243,560 | 100.0% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 54,150,740 | 93.0% |
| CALL_ISINSTANCE | 2,192,880 | 3.8% |
| CALL_PY_EXACT_ARGS | 1,900,160 | 3.3% |
| CALL | 80 | 0.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,246,240 | 100.0% |
| LOAD_ATTR | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,219,240 | 99.2% |
| BINARY_OP_MULTIPLY_INT | 27,040 | 0.8% |
| LOAD_ATTR | 520 | 0.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 130,015,840 | 100.0% |
| LOAD_ATTR | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 65,008,120 | 50.0% |
| STORE_FAST_STORE_FAST | 61,207,680 | 47.1% |
| RETURN_VALUE | 3,800,440 | 2.9% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 74,935,420 | 52.5% |
| STORE_SUBSCR | 31,176,800 | 21.9% |
| POP_JUMP_IF_FALSE | 9,939,480 | 7.0% |
| POP_JUMP_IF_NOT_NONE | 9,448,400 | 6.6% |
| CALL_TYPE_1 | 9,448,400 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,674,520 | 62.9% |
| LOAD_GLOBAL_MODULE | 40,052,320 | 28.1% |
| IS_OP | 8,783,900 | 6.2% |
| LOAD_CONST | 1,357,040 | 1.0% |
| SWAP | 664,540 | 0.5% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 40,052,320 | 23.8% |
| LOAD_FAST | 35,282,320 | 21.0% |
| POP_JUMP_IF_FALSE | 32,429,480 | 19.3% |
| STORE_FAST_STORE_FAST | 31,003,500 | 18.5% |
| STORE_FAST | 24,248,720 | 14.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 58,243,560 | 34.7% |
| LOAD_FAST | 42,287,480 | 25.2% |
| LOAD_ATTR | 30,604,100 | 18.2% |
| CALL_ISINSTANCE | 30,311,160 | 18.0% |
| LOAD_FAST_LOAD_FAST | 3,950,840 | 2.4% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,052,320 | 100.0% |
| LOAD_SUPER_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,052,360 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 333,005,880 | 59.9% |
| COPY_FREE_VARS | 79,365,060 | 14.3% |
| CALL_PY_EXACT_ARGS | 76,825,460 | 13.8% |
| POP_TOP | 62,832,440 | 11.3% |
| LOAD_ATTR_PROPERTY | 3,219,240 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 324,495,720 | 58.4% |
| LOAD_FAST | 106,363,340 | 19.1% |
| LOAD_GLOBAL_BUILTIN | 74,935,420 | 13.5% |
| NOP | 41,899,440 | 7.5% |
| LOAD_DEREF | 4,354,440 | 0.8% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 240 | 66.7% |
| STORE_ATTR | 120 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 180 | 50.0% |
| LOAD_GLOBAL_MODULE | 80 | 22.2% |
| LOAD_GLOBAL | 60 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 40 | 11.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 71,320,680 | 89.0% |
| LOAD_FAST | 8,783,880 | 11.0% |
| STORE_ATTR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,052,340 | 50.0% |
| LOAD_FAST_LOAD_FAST | 31,268,440 | 39.0% |
| LOAD_CONST | 8,783,900 | 11.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 385,640 | 100.0% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 385,660 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 33,089,440 | 95.8% |
| LOAD_ATTR | 878,040 | 2.5% |
| LOAD_FAST | 585,400 | 1.7% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 34,553,040 | 100.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 93.3% |
| TO_BOOL | 20 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 300 | 100.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,472,040 | 100.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,472,100 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 734,880 | 100.0% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 734,960 | 100.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 41,716,760 | 95.7% |
| FOR_ITER | 1,600,420 | 3.7% |
| FOR_ITER_TUPLE | 186,200 | 0.4% |
| LOAD_FAST | 92,920 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 41,716,800 | 95.7% |
| STORE_FAST_STORE_FAST | 1,880,120 | 4.3% |


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
|     deferred | 86,099,780 | 33.4% |
|          hit | 171,412,700 | 66.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 840 | 3.1% |
| Failure | 26,240 | 96.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 22,140 | 84.4% |
| add other | 1,980 | 7.5% |
| true divide other | 580 | 2.2% |
| true divide different types | 500 | 1.9% |
| multiply different types | 480 | 1.8% |
| multiply other | 300 | 1.1% |
| subtract different types | 260 | 1.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 131,141,660 | 69.7% |
|          hit | 57,009,060 | 30.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 1.0% |
| Failure | 35,380 | 99.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 34,080 | 96.3% |
| buffer int | 1,300 | 3.7% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 50,135,500 | 11.9% |
|          hit | 369,538,460 | 88.0% |
|         miss | 2,581,280 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 50,500 | 77.2% |
| Failure | 14,940 | 22.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc varargs keywords | 11,560 | 77.4% |
| metaclass | 1,840 | 12.3% |
| class no vectorcall | 1,300 | 8.7% |
| class mutable | 160 | 1.1% |
| cfunc noargs | 60 | 0.4% |
| meth descr varargs | 20 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 293,840 | 0.3% |
|          hit | 103,373,520 | 99.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 660 | 58.9% |
| Failure | 460 | 41.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 460 | 100.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,934,240 | 1.5% |
|          hit | 129,080,300 | 98.5% |
|         miss | 338,860 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,620 | 78.8% |
| Failure | 1,780 | 21.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 1,460 | 82.0% |
| zip | 320 | 18.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 50,875,620 | 15.3% |
|          hit | 281,274,160 | 84.7% |
|         miss | 78,280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,060 | 11.8% |
| Failure | 22,920 | 88.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 11,760 | 51.3% |
| metaclass attribute | 8,620 | 37.6% |
| method | 1,280 | 5.6% |
| class method obj | 1,260 | 5.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,160 | 0.0% |
|          hit | 310,679,060 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,180 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 40 | 0.0% |
|          hit | 40,052,360 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 40 | 100.0% |
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
|     deferred | 240 | 0.0% |
|          hit | 80,105,040 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 67,598,240 | 99.4% |
|          hit | 385,660 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 0.1% |
| Failure | 18,420 | 99.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 18,420 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,354,640 | 10.5% |
|          hit | 37,025,440 | 89.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 240 | 16.0% |
| Failure | 1,260 | 84.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 1,260 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 340 | 0.0% |
|          hit | 44,331,880 | 100.0% |

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
| Basic | 4,390,422,820 | 61.9% |
| Not specialized | 554,819,720 | 7.8% |
| Specialized hits | 2,144,557,000 | 30.2% |
| Specialized misses | 2,999,340 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 131,141,660 | 33.4% |
| BINARY_OP | 86,099,780 | 21.9% |
| STORE_SUBSCR | 67,598,240 | 17.2% |
| LOAD_ATTR | 50,875,620 | 13.0% |
| CALL | 50,135,500 | 12.8% |
| TO_BOOL | 4,354,640 | 1.1% |
| FOR_ITER | 1,934,240 | 0.5% |
| COMPARE_OP | 293,840 | 0.1% |
| LOAD_GLOBAL | 2,160 | 0.0% |
| UNPACK_SEQUENCE | 340 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 1,686,380 | 56.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 894,900 | 29.8% |
| FOR_ITER_LIST | 169,600 | 5.7% |
| FOR_ITER_TUPLE | 169,260 | 5.6% |
| LOAD_ATTR_METHOD_NO_DICT | 50,720 | 1.7% |
| LOAD_ATTR_PROPERTY | 27,560 | 0.9% |
| RESUME | 920 | 0.0% |
| RESUME_CHECK | 920 | 0.0% |
| CACHE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 435,891,180 | 72.9% |
| Calls to Python functions inlined | 161,736,680 | 27.1% |
| Calls via PyEval_EvalFrame (total) | 435,891,180 | 72.9% |
| Calls via PyEval_EvalFrame (vector) | 48,562,780 | 8.1% |
| Calls via PyEval_EvalFrame (generator) | 387,328,400 | 64.8% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 48,562,780 | 8.1% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 34,111,680 | 5.7% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 2,223,400 | 0.4% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 385,680 | 0.1% |
| Frames pushed | 201,839,000 | 33.8% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 508,804,940 | 51.5% |
| Frees to freelist | 509,131,700 |  |
| Allocations | 479,320,140 | 48.5% |
| Allocations to 512 bytes | 478,712,820 | 48.4% |
| Allocations to 4 kbytes | 605,400 | 0.1% |
| Allocations over 4 kbytes | 1,920 | 0.0% |
| Frees | 479,746,451 |  |
| New values | 20 |  |
| Interpreter increfs | 5,358,605,080 | 72.5% |
| Interpreter decrefs | 6,296,720,120 | 75.2% |
| Increfs | 2,034,179,048 | 27.5% |
| Decrefs | 2,076,484,544 | 24.8% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 102,148,636 |  |
| Method cache misses | 207,484 |  |
| Method cache collisions | 414,121 |  |
| Method cache dunder hits | 71,017,956 |  |
| Method cache dunder misses | 207,044 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,500 | 0 | 45,879,200 |
| 1 | 760 | 0 | 42,806,920 |
| 2 | 60 | 0 | 21,815,480 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 440 |  |
| Traces created | 440 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 20 | 4.5% |
| Recursive call | 0 | 0.0% |
| Low confidence | 40 | 9.1% |
| Traces executed | 373,459,680 |  |
| Uops executed | 7,390,678,420 | 19.79 |

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
| <= 32 | 120 | 27.3% |
| <= 64 | 120 | 27.3% |
| <= 128 | 140 | 31.8% |
| <= 256 | 60 | 13.6% |


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
| <= 16 | 100 | 22.7% |
| <= 32 | 140 | 31.8% |
| <= 64 | 100 | 22.7% |
| <= 128 | 80 | 18.2% |
| <= 256 | 20 | 4.5% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,607,240 | 0.4% |
| <= 2 | 63,918,020 | 17.1% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 36,029,160 | 9.6% |
| <= 32 | 244,158,640 | 65.4% |
| <= 64 | 4,861,040 | 1.3% |
| <= 128 | 21,290,840 | 5.7% |
| <= 256 | 242,120 | 0.1% |
| <= 512 | 105,400 | 0.0% |
| <= 1,024 | 1,247,220 | 0.3% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 1,006,950,820 | 13.6% | 13.6% |  |
| _CHECK_VALIDITY | 886,696,280 | 12.0% | 25.6% |  |
| LOAD_FAST | 884,563,700 | 12.0% | 37.6% |  |
| STORE_FAST | 615,027,820 | 8.3% | 45.9% |  |
| _ITER_CHECK_LIST | 390,268,480 | 5.3% | 51.2% | 0.4% |
| _GUARD_NOT_EXHAUSTED_LIST | 388,661,240 | 5.3% | 56.5% | 16.2% |
| _ITER_NEXT_LIST | 325,620,980 | 4.4% | 60.9% |  |
| _EXIT_TRACE | 285,927,060 | 3.9% | 64.7% | 100.0% |
| _BINARY_SUBSCR | 283,967,100 | 3.8% | 68.6% |  |
| LOAD_DEREF | 260,162,200 | 3.5% | 72.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 249,972,100 | 3.4% | 75.5% |  |
| _GUARD_BOTH_FLOAT | 239,525,400 | 3.2% | 78.7% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 239,525,400 | 3.2% | 82.0% |  |
| _LOAD_CONST_INLINE_BORROW | 87,343,340 | 1.2% | 83.1% |  |
| _GUARD_IS_FALSE_POP | 56,967,660 | 0.8% | 83.9% | 18.3% |
| _JUMP_TO_TOP | 51,764,160 | 0.7% | 84.6% |  |
| _GUARD_TYPE_VERSION | 48,691,020 | 0.7% | 85.3% |  |
| COPY | 47,609,800 | 0.6% | 85.9% |  |
| SWAP | 47,609,800 | 0.6% | 86.6% |  |
| _BINARY_OP | 47,168,660 | 0.6% | 87.2% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 46,112,220 | 0.6% | 87.8% |  |
| _CHECK_STACK_SPACE | 46,112,220 | 0.6% | 88.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 46,112,220 | 0.6% | 89.1% |  |
| _PUSH_FRAME | 46,112,220 | 0.6% | 89.7% |  |
| _SAVE_RETURN_OFFSET | 46,112,220 | 0.6% | 90.3% |  |
| CONTAINS_OP | 44,620,020 | 0.6% | 90.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 33,130,120 | 0.4% | 91.4% |  |
| _CHECK_GLOBALS | 30,569,000 | 0.4% | 91.8% |  |
| BINARY_SUBSCR_TUPLE_INT | 29,711,000 | 0.4% | 92.2% |  |
| COMPARE_OP_INT | 28,257,660 | 0.4% | 92.6% |  |
| _GUARD_BOTH_INT | 26,501,540 | 0.4% | 92.9% |  |
| _CHECK_BUILTINS | 26,322,340 | 0.4% | 93.3% |  |
| _LOAD_CONST_INLINE | 25,643,440 | 0.3% | 93.6% |  |
| RESUME_CHECK | 25,272,240 | 0.3% | 94.0% |  |
| BUILD_TUPLE | 24,011,680 | 0.3% | 94.3% |  |
| _STORE_SUBSCR | 23,804,900 | 0.3% | 94.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 22,831,840 | 0.3% | 94.9% | 2.6% |
| _ITER_CHECK_RANGE | 22,831,840 | 0.3% | 95.2% |  |
| LIST_APPEND | 22,246,400 | 0.3% | 95.5% |  |
| _BINARY_OP_MULTIPLY_INT | 22,246,400 | 0.3% | 95.8% |  |
| _ITER_NEXT_RANGE | 22,246,400 | 0.3% | 96.1% |  |
| GET_ITER | 21,141,020 | 0.3% | 96.4% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 21,025,580 | 0.3% | 96.7% |  |
| _GUARD_KEYS_VERSION | 21,025,580 | 0.3% | 97.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 21,025,580 | 0.3% | 97.3% |  |
| MAKE_FUNCTION | 20,839,980 | 0.3% | 97.6% |  |
| SET_FUNCTION_ATTRIBUTE | 20,839,980 | 0.3% | 97.8% |  |
| BINARY_SUBSCR_DICT | 20,839,980 | 0.3% | 98.1% |  |
| _POP_FRAME | 20,839,980 | 0.3% | 98.4% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 20,839,980 | 0.3% | 98.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 20,839,980 | 0.3% | 99.0% |  |
| _GUARD_IS_TRUE_POP | 17,224,360 | 0.2% | 99.2% | 58.1% |
| _LOAD_ATTR | 15,009,360 | 0.2% | 99.4% |  |
| _FOR_ITER_TIER_TWO | 9,680,320 | 0.1% | 99.5% | 16.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 7,750,920 | 0.1% | 99.6% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 6,825,460 | 0.1% | 99.7% |  |
| _BINARY_OP_ADD_INT | 4,255,140 | 0.1% | 99.8% |  |
| UNARY_NEGATIVE | 3,875,460 | 0.1% | 99.8% |  |
| MAP_ADD | 2,556,040 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,178,960 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 1,314,340 | 0.0% | 99.9% |  |
| _COMPARE_OP | 1,314,340 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,314,340 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 556,800 | 0.0% | 100.0% | 50.0% |
| COMPARE_OP_STR | 556,800 | 0.0% | 100.0% |  |
| _ITER_CHECK_TUPLE | 556,800 | 0.0% | 100.0% |  |
| POP_TOP | 385,520 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 385,520 | 0.0% | 100.0% |  |
| CALL_LEN | 292,560 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 278,400 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 278,400 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 120 |
| CALL_KW | 20 |
| CALL_LIST_APPEND | 20 |


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