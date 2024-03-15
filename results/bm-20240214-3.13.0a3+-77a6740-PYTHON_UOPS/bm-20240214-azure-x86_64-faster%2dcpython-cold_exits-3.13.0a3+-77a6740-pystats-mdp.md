
# Pystats results

- benchmark: mdp
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,102,494,480 | 14.7% | 14.7% |  |
| RESUME_CHECK | 576,289,580 | 7.7% | 22.4% | 0.0% |
| INTERPRETER_EXIT | 435,891,180 | 5.8% | 28.3% |  |
| POP_TOP | 388,578,040 | 5.2% | 33.5% |  |
| ENTER_EXECUTOR | 363,386,220 | 4.9% | 38.3% |  |
| YIELD_VALUE | 324,495,840 | 4.3% | 42.7% |  |
| LOAD_FAST_LOAD_FAST | 307,498,900 | 4.1% | 46.8% |  |
| STORE_FAST | 268,063,220 | 3.6% | 50.4% |  |
| LOAD_DEREF | 239,879,080 | 3.2% | 53.6% |  |
| RETURN_VALUE | 193,172,620 | 2.6% | 56.1% |  |
| LOAD_GLOBAL_MODULE | 166,946,640 | 2.2% | 58.4% |  |
| LOAD_CONST | 166,553,560 | 2.2% | 60.6% |  |
| LOAD_GLOBAL_BUILTIN | 163,145,180 | 2.2% | 62.8% |  |
| CALL_PY_EXACT_ARGS | 160,345,080 | 2.1% | 64.9% | 1.1% |
| POP_JUMP_IF_FALSE | 144,168,640 | 1.9% | 66.9% |  |
| COPY_FREE_VARS | 141,718,960 | 1.9% | 68.8% |  |
| BINARY_SUBSCR | 130,948,820 | 1.8% | 70.5% |  |
| LOAD_ATTR_SLOT | 130,016,240 | 1.7% | 72.2% |  |
| FOR_ITER_LIST | 126,232,500 | 1.7% | 73.9% | 0.1% |
| PUSH_NULL | 100,104,320 | 1.3% | 75.3% |  |
| BINARY_OP_MULTIPLY_INT | 97,943,940 | 1.3% | 76.6% |  |
| BINARY_OP | 85,728,080 | 1.1% | 77.7% |  |
| STORE_ATTR_SLOT | 80,104,680 | 1.1% | 78.8% |  |
| COMPARE_OP_INT | 71,896,020 | 1.0% | 79.8% |  |
| BUILD_TUPLE | 71,399,660 | 1.0% | 80.7% |  |
| STORE_SUBSCR | 67,388,100 | 0.9% | 81.6% |  |
| GET_ITER | 65,504,800 | 0.9% | 82.5% |  |
| STORE_FAST_STORE_FAST | 64,515,460 | 0.9% | 83.4% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 63,311,220 | 0.8% | 84.2% |  |
| RETURN_CONST | 63,239,120 | 0.8% | 85.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 63,234,860 | 0.8% | 85.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 63,128,540 | 0.8% | 86.7% |  |
| MAKE_FUNCTION | 63,032,400 | 0.8% | 87.6% |  |
| RETURN_GENERATOR | 62,832,560 | 0.8% | 88.4% |  |
| BINARY_SUBSCR_DICT | 62,740,460 | 0.8% | 89.3% |  |
| NOP | 62,739,520 | 0.8% | 90.1% |  |
| SET_FUNCTION_ATTRIBUTE | 62,353,760 | 0.8% | 90.9% |  |
| CALL_BUILTIN_FAST | 58,829,240 | 0.8% | 91.7% |  |
| LOAD_ATTR_MODULE | 58,243,860 | 0.8% | 92.5% |  |
| LOAD_ATTR | 48,231,200 | 0.6% | 93.1% |  |
| CALL | 47,619,600 | 0.6% | 93.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 43,596,920 | 0.6% | 94.4% |  |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 0.6% | 94.9% |  |
| LOAD_SUPER_ATTR_METHOD | 40,052,360 | 0.5% | 95.5% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 35,344,000 | 0.5% | 95.9% |  |
| TO_BOOL_BOOL | 33,679,260 | 0.5% | 96.4% |  |
| CALL_ISINSTANCE | 33,089,520 | 0.4% | 96.8% |  |
| POP_JUMP_IF_TRUE | 31,470,380 | 0.4% | 97.2% |  |
| COMPARE_OP_FLOAT | 31,185,840 | 0.4% | 97.7% |  |
| BINARY_OP_ADD_INT | 31,168,220 | 0.4% | 98.1% |  |
| BINARY_SUBSCR_TUPLE_INT | 14,898,020 | 0.2% | 98.3% |  |
| SWAP | 13,634,280 | 0.2% | 98.5% |  |
| JUMP_FORWARD | 12,611,120 | 0.2% | 98.6% |  |
| COPY | 10,378,840 | 0.1% | 98.8% |  |
| IS_OP | 10,113,040 | 0.1% | 98.9% |  |
| CALL_TYPE_1 | 10,112,980 | 0.1% | 99.0% |  |
| EXTENDED_ARG | 9,457,360 | 0.1% | 99.2% |  |
| POP_JUMP_IF_NOT_NONE | 9,448,480 | 0.1% | 99.3% |  |
| CALL_BUILTIN_CLASS | 9,419,180 | 0.1% | 99.4% |  |
| CALL_LEN | 4,647,240 | 0.1% | 99.5% |  |
| CALL_KW | 4,647,120 | 0.1% | 99.5% |  |
| TO_BOOL | 4,356,140 | 0.1% | 99.6% |  |
| LOAD_ATTR_METHOD_NO_DICT | 4,287,020 | 0.1% | 99.6% | 1.2% |
| LOAD_ATTR_PROPERTY | 3,246,800 | 0.0% | 99.7% | 0.8% |
| FOR_ITER_TUPLE | 2,461,300 | 0.0% | 99.7% | 6.9% |
| STORE_FAST_LOAD_FAST | 2,286,340 | 0.0% | 99.8% |  |
| UNARY_NEGATIVE | 1,900,540 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 1,655,280 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,615,560 | 0.0% | 99.8% | 55.4% |
| FOR_ITER | 1,603,780 | 0.0% | 99.8% |  |
| BUILD_LIST | 1,171,520 | 0.0% | 99.9% |  |
| FOR_ITER_RANGE | 1,171,320 | 0.0% | 99.9% |  |
| CALL_LIST_APPEND | 771,640 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 734,960 | 0.0% | 99.9% |  |
| BUILD_MAP | 720,800 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 680,040 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 665,460 | 0.0% | 99.9% |  |
| LIST_APPEND | 586,160 | 0.0% | 99.9% |  |
| MAP_ADD | 535,560 | 0.0% | 99.9% |  |
| CALL_METHOD_DESCRIPTOR_O | 491,860 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 453,960 | 0.0% | 100.0% |  |
| CONTAINS_OP | 448,020 | 0.0% | 100.0% |  |
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
| LOAD_GLOBAL | 4,340 | 0.0% | 100.0% |  |
| RESUME | 1,000 | 0.0% | 100.0% | 96.0% |
| UNPACK_SEQUENCE | 680 | 0.0% | 100.0% |  |
| STORE_ATTR | 480 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 440 | 0.0% | 100.0% |  |
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
| CACHE RESUME_CHECK | 333,005,880 | 4.5% | 4.5% |
| POP_TOP ENTER_EXECUTOR | 325,249,700 | 4.3% | 8.8% |
| YIELD_VALUE INTERPRETER_EXIT | 324,495,840 | 4.3% | 13.1% |
| RESUME_CHECK POP_TOP | 324,495,720 | 4.3% | 17.5% |
| ENTER_EXECUTOR YIELD_VALUE | 260,347,860 | 3.5% | 21.0% |
| LOAD_DEREF LOAD_FAST | 191,857,320 | 2.6% | 23.5% |
| LOAD_FAST LOAD_ATTR_SLOT | 130,015,840 | 1.7% | 25.3% |
| LOAD_FAST BINARY_SUBSCR | 126,108,600 | 1.7% | 26.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 110,329,820 | 1.5% | 28.4% |
| RESUME_CHECK LOAD_FAST | 106,363,340 | 1.4% | 29.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 97,480,760 | 1.3% | 31.1% |
| PUSH_NULL LOAD_FAST_LOAD_FAST | 88,230,880 | 1.2% | 32.3% |
| COPY_FREE_VARS RESUME_CHECK | 79,365,060 | 1.1% | 33.4% |
| LOAD_FAST LOAD_CONST | 75,062,840 | 1.0% | 34.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 74,750,740 | 1.0% | 35.4% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 71,896,020 | 1.0% | 36.4% |
| STORE_FAST LOAD_FAST | 71,417,680 | 1.0% | 37.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 71,320,680 | 1.0% | 38.3% |
| RETURN_VALUE RETURN_VALUE | 67,699,120 | 0.9% | 39.2% |
| LOAD_CONST COMPARE_OP_INT | 67,261,860 | 0.9% | 40.1% |
| STORE_FAST LOAD_DEREF | 66,708,760 | 0.9% | 41.0% |
| LOAD_ATTR_SLOT LOAD_FAST | 65,008,120 | 0.9% | 41.8% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 64,338,560 | 0.9% | 42.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 63,311,160 | 0.8% | 43.5% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 63,310,960 | 0.8% | 44.4% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 63,125,380 | 0.8% | 45.2% |
| ENTER_EXECUTOR FOR_ITER_LIST | 63,096,720 | 0.8% | 46.1% |
| LOAD_CONST MAKE_FUNCTION | 63,032,400 | 0.8% | 46.9% |
| LOAD_FAST BUILD_TUPLE | 63,029,100 | 0.8% | 47.8% |
| RETURN_CONST INTERPRETER_EXIT | 62,867,220 | 0.8% | 48.6% |
| CACHE POP_TOP | 62,832,560 | 0.8% | 49.4% |
| POP_TOP RESUME_CHECK | 62,832,440 | 0.8% | 50.3% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 62,742,600 | 0.8% | 51.1% |
| LOAD_FAST BINARY_SUBSCR_DICT | 62,740,420 | 0.8% | 52.0% |
| RETURN_VALUE GET_ITER | 62,739,600 | 0.8% | 52.8% |
| NOP LOAD_FAST | 62,739,440 | 0.8% | 53.6% |
| RESUME_CHECK NOP | 62,739,420 | 0.8% | 54.5% |
| GET_ITER CALL_PY_EXACT_ARGS | 62,739,400 | 0.8% | 55.3% |
| LOAD_FAST STORE_SUBSCR | 62,565,320 | 0.8% | 56.1% |
| BUILD_TUPLE LOAD_CONST | 62,539,680 | 0.8% | 57.0% |
| FOR_ITER_LIST RETURN_CONST | 62,390,320 | 0.8% | 57.8% |
| LOAD_FAST FOR_ITER_LIST | 62,390,240 | 0.8% | 58.6% |
| MAKE_FUNCTION SET_FUNCTION_ATTRIBUTE | 62,353,760 | 0.8% | 59.5% |
| COPY_FREE_VARS RETURN_GENERATOR | 62,353,760 | 0.8% | 60.3% |
| SET_FUNCTION_ATTRIBUTE LOAD_FAST | 62,353,760 | 0.8% | 61.1% |
| BINARY_SUBSCR_DICT RETURN_VALUE | 62,353,760 | 0.8% | 62.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS LOAD_DEREF | 62,353,680 | 0.8% | 62.8% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 62,353,680 | 0.8% | 63.6% |
| RETURN_GENERATOR CALL_BUILTIN_FAST_WITH_KEYWORDS | 62,353,600 | 0.8% | 64.5% |
| LOAD_ATTR_SLOT STORE_FAST_STORE_FAST | 61,207,680 | 0.8% | 65.3% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 60,189,860 | 0.8% | 66.1% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 58,243,560 | 0.8% | 66.9% |
| LOAD_FAST_LOAD_FAST CALL_BUILTIN_FAST | 56,928,840 | 0.8% | 67.6% |
| LOAD_ATTR_MODULE PUSH_NULL | 54,150,740 | 0.7% | 68.4% |
| CALL_BUILTIN_FAST STORE_FAST | 54,150,560 | 0.7% | 69.1% |
| LOAD_FAST RETURN_VALUE | 50,118,160 | 0.7% | 69.8% |
| RETURN_VALUE INTERPRETER_EXIT | 48,528,120 | 0.6% | 70.4% |
| LOAD_FAST_LOAD_FAST BINARY_OP_MULTIPLY_INT | 48,105,760 | 0.6% | 71.1% |
| BINARY_SUBSCR LOAD_FAST | 47,427,700 | 0.6% | 71.7% |
| CALL STORE_FAST | 45,285,640 | 0.6% | 72.3% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 44,188,880 | 0.6% | 72.9% |
| LOAD_DEREF PUSH_NULL | 43,667,280 | 0.6% | 73.5% |
| STORE_FAST STORE_FAST | 42,251,800 | 0.6% | 74.0% |
| BINARY_OP_MULTIPLY_FLOAT YIELD_VALUE | 41,716,800 | 0.6% | 74.6% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST | 41,716,800 | 0.6% | 75.2% |
| LOAD_FAST BINARY_OP_MULTIPLY_FLOAT | 41,716,760 | 0.6% | 75.7% |
| FOR_ITER_LIST UNPACK_SEQUENCE_TWO_TUPLE | 41,716,760 | 0.6% | 76.3% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 41,229,620 | 0.6% | 76.8% |
| LOAD_FAST BINARY_OP | 41,093,700 | 0.5% | 77.4% |
| LOAD_FAST CALL | 40,933,680 | 0.5% | 77.9% |
| CACHE COPY_FREE_VARS | 40,052,400 | 0.5% | 78.4% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST | 40,052,360 | 0.5% | 79.0% |
| STORE_ATTR_SLOT LOAD_FAST | 40,052,340 | 0.5% | 79.5% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 40,052,320 | 0.5% | 80.1% |
| LOAD_GLOBAL_BUILTIN LOAD_GLOBAL_MODULE | 40,052,320 | 0.5% | 80.6% |
| LOAD_FAST_LOAD_FAST BINARY_OP | 39,723,520 | 0.5% | 81.1% |
| BINARY_OP BINARY_OP_MULTIPLY_INT | 36,261,020 | 0.5% | 81.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 35,282,320 | 0.5% | 82.1% |
| CALL_BOUND_METHOD_EXACT_ARGS COPY_FREE_VARS | 34,958,180 | 0.5% | 82.5% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 33,679,040 | 0.5% | 83.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 33,089,440 | 0.4% | 83.4% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 32,954,800 | 0.4% | 83.9% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 32,913,600 | 0.4% | 84.3% |
| STORE_FAST_STORE_FAST LOAD_FAST | 32,683,720 | 0.4% | 84.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 31,952,840 | 0.4% | 85.2% |
| BINARY_SUBSCR LOAD_DEREF | 31,291,680 | 0.4% | 85.6% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 31,268,440 | 0.4% | 86.0% |
| COMPARE_OP_FLOAT POP_JUMP_IF_TRUE | 31,176,860 | 0.4% | 86.4% |
| BINARY_SUBSCR COMPARE_OP_FLOAT | 31,176,840 | 0.4% | 86.9% |
| STORE_SUBSCR LOAD_GLOBAL_BUILTIN | 31,176,800 | 0.4% | 87.3% |
| STORE_FAST_STORE_FAST LOAD_GLOBAL_MODULE | 31,003,500 | 0.4% | 87.7% |
| BINARY_OP_MULTIPLY_INT LOAD_FAST_LOAD_FAST | 30,896,520 | 0.4% | 88.1% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 30,738,660 | 0.4% | 88.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 30,604,100 | 0.4% | 88.9% |
| POP_JUMP_IF_FALSE LOAD_DEREF | 30,604,000 | 0.4% | 89.3% |
| LOAD_ATTR LOAD_FAST_LOAD_FAST | 30,603,920 | 0.4% | 89.7% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 30,311,160 | 0.4% | 90.1% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 30,162,120 | 0.4% | 90.5% |
| BINARY_OP_MULTIPLY_INT CALL_BOUND_METHOD_EXACT_ARGS | 30,018,280 | 0.4% | 90.9% |
| BINARY_OP_MULTIPLY_INT BINARY_OP_ADD_INT | 28,837,600 | 0.4% | 91.3% |


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
| LOAD_FAST | 126,108,600 | 96.3% |
| COPY | 4,804,260 | 3.7% |
| BINARY_SUBSCR | 35,320 | 0.0% |
| LOAD_CONST | 640 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 47,427,700 | 36.2% |
| LOAD_DEREF | 31,291,680 | 23.9% |
| COMPARE_OP_FLOAT | 31,176,840 | 23.8% |
| YIELD_VALUE | 20,637,440 | 15.8% |
| LOAD_FAST_LOAD_FAST | 264,320 | 0.2% |


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
| RETURN_VALUE | 62,739,600 | 95.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,306,040 | 2.0% |
| CALL_BUILTIN_CLASS | 585,420 | 0.9% |
| LOAD_FAST | 301,920 | 0.5% |
| CALL | 292,940 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 62,739,400 | 95.8% |
| LOAD_FAST_AND_CLEAR | 1,120,400 | 1.7% |
| FOR_ITER | 1,064,180 | 1.6% |
| FOR_ITER_LIST | 301,720 | 0.5% |
| FOR_ITER_TUPLE | 278,840 | 0.4% |


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
| LOAD_CONST | 63,032,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 62,353,760 | 98.9% |
| LOAD_FAST | 385,840 | 0.6% |
| LOAD_CONST | 292,720 | 0.5% |
| CALL | 80 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 62,739,420 | 100.0% |
| POP_TOP | 80 | 0.0% |
| RESUME | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,739,440 | 100.0% |
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
| ENTER_EXECUTOR | 325,249,700 | 83.7% |
| RESUME_CHECK | 62,832,440 | 16.2% |
| LOAD_FAST | 386,040 | 0.1% |
| JUMP_BACKWARD | 108,480 | 0.0% |
| JUMP_FORWARD | 1,100 | 0.0% |


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
| RETURN_VALUE | 67,699,120 | 35.0% |
| BINARY_SUBSCR_DICT | 62,353,760 | 32.3% |
| LOAD_FAST | 50,118,160 | 25.9% |
| CALL_BUILTIN_FAST | 4,678,680 | 2.4% |
| LOAD_ATTR_SLOT | 3,800,440 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 67,699,120 | 35.0% |
| GET_ITER | 62,739,600 | 32.5% |
| INTERPRETER_EXIT | 48,528,120 | 25.1% |
| STORE_FAST | 10,507,600 | 5.4% |
| CALL_BUILTIN_CLASS | 3,214,960 | 1.7% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,565,320 | 92.8% |
| SWAP | 4,804,260 | 7.1% |
| STORE_SUBSCR | 18,360 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 31,176,800 | 46.3% |
| LOAD_DEREF | 20,964,080 | 31.1% |
| JUMP_FORWARD | 10,318,560 | 15.3% |
| ENTER_EXECUTOR | 4,802,900 | 7.1% |
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
| LOAD_FAST | 41,093,700 | 47.9% |
| LOAD_FAST_LOAD_FAST | 39,723,520 | 46.3% |
| LOAD_CONST | 1,761,480 | 2.1% |
| CALL_BUILTIN_CLASS | 1,607,500 | 1.9% |
| BINARY_OP_MULTIPLY_INT | 585,480 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_MULTIPLY_INT | 36,261,020 | 42.3% |
| STORE_FAST | 25,485,260 | 29.7% |
| LOAD_FAST_LOAD_FAST | 14,852,080 | 17.3% |
| SWAP | 4,804,260 | 5.6% |
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
| CALL | 292,760 | 25.0% |
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
| LOAD_FAST | 63,029,100 | 88.3% |
| LOAD_FAST_LOAD_FAST | 4,261,920 | 6.0% |
| BINARY_SUBSCR_TUPLE_INT | 1,849,860 | 2.6% |
| LOAD_CONST | 1,700,980 | 2.4% |
| CALL | 371,840 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 62,539,680 | 87.6% |
| COPY | 4,168,480 | 5.8% |
| YIELD_VALUE | 1,793,620 | 2.5% |
| RETURN_VALUE | 1,607,520 | 2.3% |
| LOAD_FAST | 391,660 | 0.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,933,680 | 86.0% |
| LOAD_FAST_LOAD_FAST | 4,355,000 | 9.1% |
| LOAD_GLOBAL_MODULE | 878,120 | 1.8% |
| LOAD_CONST | 851,080 | 1.8% |
| BUILD_LIST | 292,760 | 0.6% |

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
| ENTER_EXECUTOR | 4,060,120 | 87.4% |
| LOAD_CONST | 586,980 | 12.6% |
| JUMP_BACKWARD | 20 | 0.0% |

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
| LOAD_FAST_LOAD_FAST | 448,020 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 447,700 | 99.9% |
| POP_JUMP_IF_TRUE | 320 | 0.1% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,804,260 | 46.3% |
| BUILD_TUPLE | 4,168,480 | 40.2% |
| SWAP | 664,560 | 6.4% |
| LOAD_FAST_LOAD_FAST | 635,780 | 6.1% |
| BINARY_OP | 105,760 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 4,804,260 | 46.3% |
| COPY | 4,804,260 | 46.3% |
| IS_OP | 664,560 | 6.4% |
| LOAD_DEREF | 105,760 | 1.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 62,353,680 | 44.0% |
| CACHE | 40,052,400 | 28.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 34,958,180 | 24.7% |
| CALL_KW | 4,354,400 | 3.1% |
| CALL | 220 | 0.0% |

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
| POP_TOP | 325,249,700 | 89.5% |
| POP_JUMP_IF_TRUE | 30,738,660 | 8.5% |
| STORE_SUBSCR | 4,802,900 | 1.3% |
| POP_JUMP_IF_FALSE | 596,240 | 0.2% |
| LIST_APPEND | 585,420 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 260,347,860 | 71.6% |
| FOR_ITER_LIST | 63,096,720 | 17.4% |
| POP_JUMP_IF_FALSE | 22,600,960 | 6.2% |
| LOAD_FAST | 8,894,560 | 2.4% |
| CALL_KW | 4,060,120 | 1.1% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,448,480 | 99.9% |
| POP_JUMP_IF_FALSE | 8,800 | 0.1% |
| COMPARE_OP_FLOAT | 60 | 0.0% |
| COMPARE_OP | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 9,448,480 | 99.9% |
| JUMP_BACKWARD | 8,800 | 0.1% |
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
| POP_JUMP_IF_TRUE | 332,460 | 73.2% |
| POP_TOP | 108,480 | 23.9% |
| EXTENDED_ARG | 8,800 | 1.9% |
| STORE_SUBSCR | 1,360 | 0.3% |
| MAP_ADD | 1,020 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 440,420 | 97.0% |
| LOAD_FAST | 9,160 | 2.0% |
| FOR_ITER | 2,800 | 0.6% |
| FOR_ITER_TUPLE | 920 | 0.2% |
| FOR_ITER_RANGE | 380 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 10,318,560 | 81.8% |
| POP_JUMP_IF_FALSE | 664,620 | 5.3% |
| JUMP_FORWARD | 664,560 | 5.3% |
| POP_EXCEPT | 385,680 | 3.1% |
| BINARY_SUBSCR_LIST_INT | 292,700 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 10,318,560 | 81.8% |
| LOAD_FAST | 1,051,700 | 8.3% |
| JUMP_FORWARD | 664,560 | 5.3% |
| STORE_FAST | 294,420 | 2.3% |
| LOAD_GLOBAL_BUILTIN | 185,900 | 1.5% |


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
| LOAD_GLOBAL_MODULE | 30,604,100 | 63.5% |
| LOAD_FAST | 15,126,300 | 31.4% |
| LOAD_ATTR | 1,277,260 | 2.6% |
| BINARY_SUBSCR_TUPLE_INT | 1,222,260 | 2.5% |
| LOAD_ATTR_PROPERTY | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 30,603,920 | 63.5% |
| LOAD_DEREF | 8,708,800 | 18.1% |
| BINARY_OP_MULTIPLY_INT | 3,769,120 | 7.8% |
| LOAD_FAST | 2,053,240 | 4.3% |
| LOAD_ATTR | 1,277,260 | 2.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 75,062,840 | 45.1% |
| BUILD_TUPLE | 62,539,680 | 37.5% |
| BINARY_SUBSCR_TUPLE_INT | 9,348,020 | 5.6% |
| STORE_ATTR_SLOT | 8,783,900 | 5.3% |
| STORE_FAST_LOAD_FAST | 1,700,580 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 67,261,860 | 40.4% |
| MAKE_FUNCTION | 63,032,400 | 37.8% |
| BINARY_SUBSCR_TUPLE_INT | 14,897,720 | 8.9% |
| LOAD_FAST | 10,591,360 | 6.4% |
| BINARY_OP | 1,761,480 | 1.1% |


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
| LOAD_DEREF | 191,857,320 | 17.4% |
| LOAD_GLOBAL_BUILTIN | 110,329,820 | 10.0% |
| RESUME_CHECK | 106,363,340 | 9.6% |
| STORE_FAST | 71,417,680 | 6.5% |
| LOAD_ATTR_SLOT | 65,008,120 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 130,015,840 | 11.8% |
| BINARY_SUBSCR | 126,108,600 | 11.4% |
| LOAD_CONST | 75,062,840 | 6.8% |
| CALL_PY_EXACT_ARGS | 64,338,560 | 5.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 63,310,960 | 5.7% |


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
| STORE_FAST | 60,189,860 | 19.6% |
| POP_JUMP_IF_FALSE | 32,954,800 | 10.7% |
| STORE_ATTR_SLOT | 31,268,440 | 10.2% |
| BINARY_OP_MULTIPLY_INT | 30,896,520 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 71,320,680 | 23.2% |
| CALL_BUILTIN_FAST | 56,928,840 | 18.5% |
| BINARY_OP_MULTIPLY_INT | 48,105,760 | 15.6% |
| LOAD_FAST | 44,188,880 | 14.4% |
| BINARY_OP | 39,723,520 | 12.9% |


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
| COMPARE_OP_INT | 71,896,020 | 49.9% |
| TO_BOOL_BOOL | 33,679,040 | 23.4% |
| ENTER_EXECUTOR | 22,600,960 | 15.7% |
| IS_OP | 10,113,040 | 7.0% |
| TO_BOOL | 4,354,640 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 32,954,800 | 22.9% |
| LOAD_GLOBAL_BUILTIN | 32,913,600 | 22.8% |
| LOAD_GLOBAL_MODULE | 31,952,840 | 22.2% |
| LOAD_DEREF | 30,604,000 | 21.2% |
| LOAD_FAST | 13,742,340 | 9.5% |


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
| COMPARE_OP_FLOAT | 31,176,860 | 99.1% |
| COMPARE_OP | 293,200 | 0.9% |
| CONTAINS_OP | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 30,738,660 | 97.7% |
| JUMP_BACKWARD | 332,460 | 1.1% |
| LOAD_FAST | 293,500 | 0.9% |
| LOAD_DEREF | 105,760 | 0.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 62,390,320 | 98.7% |
| FOR_ITER_TUPLE | 442,240 | 0.7% |
| ENTER_EXECUTOR | 371,520 | 0.6% |
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
| MAKE_FUNCTION | 62,353,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 62,353,760 | 100.0% |


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
| CALL_BUILTIN_FAST | 54,150,560 | 20.2% |
| CALL | 45,285,640 | 16.9% |
| STORE_FAST | 42,251,800 | 15.8% |
| UNPACK_SEQUENCE_TWO_TUPLE | 41,716,800 | 15.6% |
| BINARY_OP | 25,485,260 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,417,680 | 26.6% |
| LOAD_DEREF | 66,708,760 | 24.9% |
| LOAD_FAST_LOAD_FAST | 60,189,860 | 22.5% |
| STORE_FAST | 42,251,800 | 15.8% |
| LOAD_GLOBAL_MODULE | 23,957,960 | 8.9% |


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
| BINARY_OP | 4,804,260 | 35.2% |
| SWAP | 4,804,260 | 35.2% |
| LOAD_FAST_AND_CLEAR | 1,120,400 | 8.2% |
| LOAD_GLOBAL_BUILTIN | 664,540 | 4.9% |
| BUILD_LIST | 585,600 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_SUBSCR | 4,804,260 | 35.2% |
| SWAP | 4,804,260 | 35.2% |
| STORE_FAST | 1,120,320 | 8.2% |
| COPY | 664,560 | 4.9% |
| BUILD_LIST | 585,600 | 4.3% |


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
| ENTER_EXECUTOR | 260,347,860 | 80.2% |
| BINARY_OP_MULTIPLY_FLOAT | 41,716,800 | 12.9% |
| BINARY_SUBSCR | 20,637,440 | 6.4% |
| BUILD_TUPLE | 1,793,620 | 0.6% |
| JUMP_BACKWARD | 80 | 0.0% |

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
| BINARY_OP_MULTIPLY_INT | 28,837,600 | 92.5% |
| LOAD_CONST | 1,179,640 | 3.8% |
| BINARY_OP | 856,760 | 2.7% |
| LOAD_FAST | 294,220 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 22,859,560 | 73.3% |
| LOAD_FAST_LOAD_FAST | 7,428,940 | 23.8% |
| LOAD_FAST | 585,420 | 1.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 294,220 | 0.9% |
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
| LOAD_FAST | 62,740,420 | 100.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 62,353,760 | 99.4% |
| PUSH_EXC_INFO | 385,660 | 0.6% |
| STORE_FAST | 1,040 | 0.0% |


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
| LOAD_CONST | 14,897,720 | 100.0% |
| BINARY_SUBSCR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,348,020 | 62.7% |
| BUILD_TUPLE | 1,849,860 | 12.4% |
| UNARY_NEGATIVE | 1,607,500 | 10.8% |
| LOAD_ATTR | 1,222,260 | 8.2% |
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
| RETURN_GENERATOR | 62,353,600 | 98.6% |
| BINARY_OP_ADD_INT | 294,220 | 0.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 294,220 | 0.5% |
| CALL | 292,820 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 62,353,680 | 98.6% |
| STORE_FAST | 586,940 | 0.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 294,220 | 0.5% |
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
| ENTER_EXECUTOR | 771,020 | 99.9% |
| BUILD_TUPLE | 280 | 0.0% |
| LOAD_FAST | 280 | 0.0% |
| CALL | 40 | 0.0% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 771,640 | 100.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 360 | 81.8% |
| BUILD_LIST | 40 | 9.1% |
| CALL | 40 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 360 | 81.8% |
| POP_TOP | 60 | 13.6% |
| UNPACK_SEQUENCE | 20 | 4.5% |


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
| LOAD_FAST | 64,338,560 | 40.1% |
| GET_ITER | 62,739,400 | 39.1% |
| LOAD_FAST_LOAD_FAST | 30,162,120 | 18.8% |
| LOAD_ATTR_MODULE | 1,900,160 | 1.2% |
| CALL | 586,100 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 97,480,760 | 60.8% |
| COPY_FREE_VARS | 62,353,680 | 38.9% |
| RETURN_GENERATOR | 478,760 | 0.3% |
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
| LOAD_CONST | 67,261,860 | 93.6% |
| LOAD_DEREF | 4,354,360 | 6.1% |
| LOAD_FAST_LOAD_FAST | 279,280 | 0.4% |
| COMPARE_OP | 520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 71,896,020 | 100.0% |


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
| ENTER_EXECUTOR | 291,420 | 43.8% |
| POP_JUMP_IF_FALSE | 1,600 | 0.2% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 63,096,720 | 50.0% |
| LOAD_FAST | 62,390,240 | 49.4% |
| JUMP_BACKWARD | 440,420 | 0.3% |
| GET_ITER | 301,720 | 0.2% |
| FOR_ITER_TUPLE | 3,180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 62,390,320 | 49.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 41,716,760 | 33.0% |
| STORE_FAST | 21,377,960 | 16.9% |
| ENTER_EXECUTOR | 585,100 | 0.5% |
| STORE_FAST_LOAD_FAST | 149,900 | 0.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 585,420 | 50.0% |
| SWAP | 585,420 | 50.0% |
| JUMP_BACKWARD | 380 | 0.0% |
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
| LOAD_FAST | 62,742,600 | 99.4% |
| LOAD_FAST_LOAD_FAST | 385,640 | 0.6% |
| LOAD_ATTR | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,125,380 | 100.0% |
| STORE_FAST | 2,860 | 0.0% |
| STORE_SUBSCR | 120 | 0.0% |
| BUILD_LIST | 60 | 0.0% |
| SWAP | 60 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,514,460 | 82.0% |
| RETURN_VALUE | 478,560 | 11.2% |
| LOAD_FAST_CHECK | 292,680 | 6.8% |
| LOAD_ATTR_METHOD_NO_DICT | 940 | 0.0% |
| LOAD_ATTR | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,301,140 | 53.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,598,600 | 37.3% |
| LOAD_CONST | 385,820 | 9.0% |
| LOAD_ATTR_METHOD_NO_DICT | 940 | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST | 360 | 0.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,310,960 | 100.0% |
| LOAD_ATTR | 220 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 63,311,160 | 100.0% |
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
| RESUME_CHECK | 74,750,740 | 45.8% |
| POP_JUMP_IF_FALSE | 32,913,600 | 20.2% |
| STORE_SUBSCR | 31,176,800 | 19.1% |
| POP_JUMP_IF_NOT_NONE | 9,448,400 | 5.8% |
| CALL_TYPE_1 | 9,448,400 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 110,329,820 | 67.6% |
| LOAD_GLOBAL_MODULE | 40,052,320 | 24.6% |
| IS_OP | 8,783,900 | 5.4% |
| LOAD_CONST | 1,172,360 | 0.7% |
| SWAP | 664,540 | 0.4% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 40,052,320 | 24.0% |
| LOAD_FAST | 35,282,320 | 21.1% |
| POP_JUMP_IF_FALSE | 31,952,840 | 19.1% |
| STORE_FAST_STORE_FAST | 31,003,500 | 18.6% |
| STORE_FAST | 23,957,960 | 14.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 58,243,560 | 34.9% |
| LOAD_FAST | 41,229,620 | 24.7% |
| LOAD_ATTR | 30,604,100 | 18.3% |
| CALL_ISINSTANCE | 30,311,160 | 18.2% |
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
| CACHE | 333,005,880 | 57.8% |
| CALL_PY_EXACT_ARGS | 97,480,760 | 16.9% |
| COPY_FREE_VARS | 79,365,060 | 13.8% |
| POP_TOP | 62,832,440 | 10.9% |
| LOAD_ATTR_PROPERTY | 3,219,240 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 324,495,720 | 56.3% |
| LOAD_FAST | 106,363,340 | 18.5% |
| LOAD_GLOBAL_BUILTIN | 74,750,740 | 13.0% |
| NOP | 62,739,420 | 10.9% |
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
| CALL_ISINSTANCE | 33,089,440 | 98.2% |
| LOAD_FAST | 585,400 | 1.7% |
| LOAD_ATTR | 4,260 | 0.0% |
| TO_BOOL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 33,679,040 | 100.0% |
| ENTER_EXECUTOR | 220 | 0.0% |


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
| LOAD_FAST | 679,980 | 100.0% |
| TO_BOOL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 680,040 | 100.0% |


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
|     deferred | 85,701,100 | 33.4% |
|          hit | 171,236,500 | 66.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 840 | 3.1% |
| Failure | 26,140 | 96.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| floor divide | 22,140 | 84.7% |
| add other | 1,920 | 7.3% |
| true divide other | 580 | 2.2% |
| true divide different types | 500 | 1.9% |
| multiply different types | 480 | 1.8% |
| multiply other | 260 | 1.0% |
| subtract different types | 260 | 1.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 130,913,140 | 62.7% |
|          hit | 77,931,180 | 37.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 360 | 1.0% |
| Failure | 35,320 | 99.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 34,020 | 96.3% |
| buffer int | 1,300 | 3.7% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 50,135,440 | 10.9% |
|          hit | 410,664,440 | 89.1% |
|         miss | 2,581,280 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 50,520 | 77.2% |
| Failure | 14,920 | 22.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| cfunc varargs keywords | 11,560 | 77.5% |
| metaclass | 1,840 | 12.3% |
| class no vectorcall | 1,300 | 8.7% |
| class mutable | 160 | 1.1% |
| cfunc noargs | 60 | 0.4% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 293,840 | 0.3% |
|          hit | 103,747,320 | 99.7% |

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
|          hit | 129,526,260 | 98.5% |
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
|     deferred | 48,284,760 | 13.0% |
|          hit | 322,155,400 | 87.0% |
|         miss | 78,280 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,060 | 12.4% |
| Failure | 21,660 | 87.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not managed dict | 10,500 | 48.5% |
| metaclass attribute | 8,620 | 39.8% |
| method | 1,280 | 5.9% |
| class method obj | 1,260 | 5.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,160 | 0.0% |
|          hit | 330,091,820 | 100.0% |

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
|     deferred | 67,369,720 | 99.4% |
|          hit | 385,660 | 0.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 20 | 0.1% |
| Failure | 18,360 | 99.9% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 18,360 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,354,640 | 11.2% |
|          hit | 34,359,600 | 88.7% |

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
| Basic | 4,619,797,980 | 61.8% |
| Not specialized | 571,263,760 | 7.6% |
| Specialized hits | 2,285,532,080 | 30.6% |
| Specialized misses | 2,999,380 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| BINARY_SUBSCR | 130,913,140 | 33.7% |
| BINARY_OP | 85,701,100 | 22.0% |
| STORE_SUBSCR | 67,369,720 | 17.3% |
| CALL | 50,135,440 | 12.9% |
| LOAD_ATTR | 48,284,760 | 12.4% |
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
| RESUME | 960 | 0.0% |
| RESUME_CHECK | 960 | 0.0% |
| CACHE | 0 | 0.0% |
| CHECK_EXC_MATCH | 0 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 435,891,180 | 68.2% |
| Calls to Python functions inlined | 203,231,960 | 31.8% |
| Calls via PyEval_EvalFrame (total) | 435,891,180 | 68.2% |
| Calls via PyEval_EvalFrame (vector) | 48,562,780 | 7.6% |
| Calls via PyEval_EvalFrame (generator) | 387,328,400 | 60.6% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 48,562,780 | 7.6% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 34,111,680 | 5.3% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 2,223,400 | 0.3% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 385,680 | 0.1% |
| Frames pushed | 201,839,000 | 31.6% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 508,815,400 | 51.5% |
| Frees to freelist | 509,131,720 |  |
| Allocations | 479,309,800 | 48.5% |
| Allocations to 512 bytes | 478,702,320 | 48.4% |
| Allocations to 4 kbytes | 605,560 | 0.1% |
| Allocations over 4 kbytes | 1,920 | 0.0% |
| Frees | 479,735,945 |  |
| New values | 20 |  |
| Interpreter increfs | 5,392,171,080 | 72.6% |
| Interpreter decrefs | 6,330,286,380 | 75.3% |
| Increfs | 2,037,155,938 | 27.4% |
| Decrefs | 2,079,460,960 | 24.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 101,412,585 |  |
| Method cache misses | 942,275 |  |
| Method cache collisions | 1,825,305 |  |
| Method cache dunder hits | 70,341,487 |  |
| Method cache dunder misses | 883,453 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 8,480 | 0 | 45,645,680 |
| 1 | 760 | 60 | 43,341,080 |
| 2 | 60 | 0 | 22,375,360 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 960 |  |
| Traces created | 963,720 | 100,387.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 8,295,940 | 864,160.4% |
| Inner loop found | 100 | 10.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 80 | 8.3% |
| Traces executed | 672,699,540 |  |
| Uops executed | 7,018,839,320 | 10.43 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 120 | 0.0% |
| <= 32 | 220 | 0.0% |
| <= 64 | 706,420 | 73.3% |
| <= 128 | 256,920 | 26.7% |
| <= 256 | 40 | 0.0% |


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
| <= 128 | 20 | 0.0% |
| <= 256 | 100 | 0.0% |
| <= 512 | 280 | 0.0% |
| <= 1,024 | 160 | 0.0% |
| <= 2,048 | 20 | 0.0% |
| <= 4,096 | 20 | 0.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,792,440 | 0.3% |
| <= 4 | 63,917,940 | 9.5% |
| <= 8 | 1,792,060 | 0.3% |
| <= 16 | 36,442,780 | 5.4% |
| <= 32 | 265,227,100 | 39.4% |
| <= 64 | 5,204,100 | 0.8% |
| <= 128 | 449,020 | 0.1% |
| <= 256 | 243,960 | 0.0% |
| <= 512 | 103,240 | 0.0% |
| <= 1,024 | 1,249,380 | 0.2% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 808,380,460 | 11.5% | 11.5% |  |
| LOAD_FAST | 786,645,300 | 11.2% | 22.7% |  |
| _CHECK_VALIDITY | 708,391,020 | 10.1% | 32.8% |  |
| STORE_FAST | 616,151,120 | 8.8% | 41.6% |  |
| _ITER_CHECK_LIST | 389,822,440 | 5.6% | 47.2% | 0.4% |
| _GUARD_NOT_EXHAUSTED_LIST | 388,215,200 | 5.5% | 52.7% | 16.2% |
| _START_EXECUTOR | 376,422,020 | 5.4% | 58.0% |  |
| _ITER_NEXT_LIST | 325,175,020 | 4.6% | 62.7% |  |
| _COLD_EXIT | 296,277,520 | 4.2% | 66.9% |  |
| _EXIT_TRACE | 290,810,320 | 4.1% | 71.0% | 100.0% |
| _BINARY_SUBSCR | 284,195,620 | 4.0% | 75.1% |  |
| LOAD_DEREF | 260,162,200 | 3.7% | 78.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 249,972,100 | 3.6% | 82.4% |  |
| _GUARD_BOTH_FLOAT | 239,525,400 | 3.4% | 85.8% |  |
| _BINARY_OP_MULTIPLY_FLOAT | 239,525,400 | 3.4% | 89.2% |  |
| _LOAD_CONST_INLINE_BORROW | 87,538,740 | 1.2% | 90.4% |  |
| _JUMP_TO_TOP | 51,764,160 | 0.7% | 91.2% |  |
| COPY | 48,066,840 | 0.7% | 91.9% |  |
| SWAP | 48,066,840 | 0.7% | 92.5% |  |
| _BINARY_OP | 47,567,340 | 0.7% | 93.2% |  |
| CONTAINS_OP | 44,559,580 | 0.6% | 93.9% |  |
| _GUARD_IS_FALSE_POP | 34,323,460 | 0.5% | 94.3% | 24.5% |
| BINARY_SUBSCR_TUPLE_INT | 29,337,200 | 0.4% | 94.8% |  |
| COMPARE_OP_INT | 27,883,860 | 0.4% | 95.2% |  |
| _GUARD_BOTH_INT | 26,677,740 | 0.4% | 95.5% |  |
| _STORE_SUBSCR | 24,033,420 | 0.3% | 95.9% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 22,831,840 | 0.3% | 96.2% | 2.6% |
| _ITER_CHECK_RANGE | 22,831,840 | 0.3% | 96.5% |  |
| LIST_APPEND | 22,246,400 | 0.3% | 96.8% |  |
| _BINARY_OP_MULTIPLY_INT | 22,246,400 | 0.3% | 97.2% |  |
| _ITER_NEXT_RANGE | 22,246,400 | 0.3% | 97.5% |  |
| _GUARD_IS_TRUE_POP | 19,976,400 | 0.3% | 97.8% | 50.5% |
| _LOAD_ATTR | 17,600,220 | 0.3% | 98.0% |  |
| _CHECK_VALIDITY_AND_SET_IP | 15,791,180 | 0.2% | 98.2% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 13,241,020 | 0.2% | 98.4% |  |
| _CHECK_GLOBALS | 10,496,120 | 0.1% | 98.6% |  |
| _FOR_ITER_TIER_TWO | 9,680,320 | 0.1% | 98.7% | 16.5% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 8,120,280 | 0.1% | 98.8% |  |
| _GUARD_TYPE_VERSION | 7,809,780 | 0.1% | 98.9% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 7,395,660 | 0.1% | 99.0% |  |
| _CHECK_BUILTINS | 5,667,040 | 0.1% | 99.1% |  |
| _LOAD_CONST_INLINE | 5,570,560 | 0.1% | 99.2% |  |
| RESUME_CHECK | 4,616,940 | 0.1% | 99.3% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 4,616,940 | 0.1% | 99.3% |  |
| _CHECK_STACK_SPACE | 4,616,940 | 0.1% | 99.4% |  |
| _INIT_CALL_PY_EXACT_ARGS | 4,616,940 | 0.1% | 99.5% |  |
| _PUSH_FRAME | 4,616,940 | 0.1% | 99.5% |  |
| _SAVE_RETURN_OFFSET | 4,616,940 | 0.1% | 99.6% |  |
| _BINARY_OP_ADD_INT | 4,431,340 | 0.1% | 99.7% |  |
| UNARY_NEGATIVE | 3,875,460 | 0.1% | 99.7% |  |
| BUILD_TUPLE | 3,171,700 | 0.0% | 99.8% |  |
| MAP_ADD | 2,556,040 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 2,178,960 | 0.0% | 99.8% |  |
| TO_BOOL_LIST | 1,792,060 | 0.0% | 99.9% |  |
| CALL_BUILTIN_CLASS | 1,314,340 | 0.0% | 99.9% |  |
| _COMPARE_OP | 1,314,340 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 1,314,340 | 0.0% | 99.9% |  |
| TO_BOOL_BOOL | 873,780 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 556,800 | 0.0% | 99.9% | 50.0% |
| COMPARE_OP_STR | 556,800 | 0.0% | 99.9% |  |
| _ITER_CHECK_TUPLE | 556,800 | 0.0% | 100.0% |  |
| POP_TOP | 385,520 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 385,520 | 0.0% | 100.0% |  |
| GET_ITER | 292,560 | 0.0% | 100.0% |  |
| CALL_LEN | 292,560 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 291,660 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 278,400 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 278,400 | 0.0% | 100.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 228,520 | 0.0% | 100.0% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 228,520 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 185,600 | 0.0% | 100.0% |  |
| _GUARD_KEYS_VERSION | 185,600 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 185,600 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 184,680 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 8,136,000 |
| CALL_KW | 126,920 |
| CALL | 33,240 |
| CALL_LIST_APPEND | 40 |


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
