
# Pystats results

- benchmark: sqlglot_parse
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 461,225,520 | 25.2% | 25.2% |  |
| LOAD_ATTR_SLOT | 259,665,080 | 14.2% | 39.4% | 0.3% |
| POP_JUMP_IF_FALSE | 90,501,340 | 5.0% | 44.4% |  |
| STORE_ATTR_SLOT | 86,048,740 | 4.7% | 49.1% | 5.5% |
| RESUME_CHECK | 74,671,060 | 4.1% | 53.2% | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 51,329,660 | 2.8% | 56.0% |  |
| RETURN_CONST | 42,885,660 | 2.3% | 58.3% |  |
| POP_JUMP_IF_TRUE | 39,604,160 | 2.2% | 60.5% |  |
| CALL_PY_EXACT_ARGS | 38,807,980 | 2.1% | 62.6% | 2.6% |
| LOAD_CONST | 37,723,280 | 2.1% | 64.7% |  |
| STORE_FAST | 34,486,440 | 1.9% | 66.6% |  |
| RETURN_VALUE | 33,004,580 | 1.8% | 68.4% |  |
| LOAD_GLOBAL_MODULE | 32,546,260 | 1.8% | 70.2% | 0.0% |
| COPY | 31,928,800 | 1.7% | 71.9% |  |
| BINARY_OP_ADD_INT | 30,344,160 | 1.7% | 73.6% |  |
| COMPARE_OP_INT | 30,304,320 | 1.7% | 75.2% |  |
| SWAP | 29,461,240 | 1.6% | 76.8% |  |
| BINARY_SUBSCR_STR_INT | 27,066,100 | 1.5% | 78.3% |  |
| TO_BOOL_ALWAYS_TRUE | 25,505,740 | 1.4% | 79.7% | 6.3% |
| LOAD_ATTR | 23,587,220 | 1.3% | 81.0% |  |
| POP_TOP | 23,296,680 | 1.3% | 82.3% |  |
| ENTER_EXECUTOR | 22,067,600 | 1.2% | 83.5% |  |
| COMPARE_OP | 20,366,460 | 1.1% | 84.6% |  |
| TO_BOOL_NONE | 20,118,840 | 1.1% | 85.7% | 11.0% |
| LOAD_FAST_LOAD_FAST | 18,724,020 | 1.0% | 86.7% |  |
| CALL_PY_WITH_DEFAULTS | 18,708,000 | 1.0% | 87.8% |  |
| TO_BOOL_BOOL | 17,678,380 | 1.0% | 88.7% | 3.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 16,901,440 | 0.9% | 89.6% |  |
| BINARY_OP_SUBTRACT_INT | 16,396,000 | 0.9% | 90.5% |  |
| LOAD_GLOBAL_BUILTIN | 14,234,720 | 0.8% | 91.3% | 0.0% |
| JUMP_FORWARD | 13,571,720 | 0.7% | 92.1% |  |
| INTERPRETER_EXIT | 11,939,020 | 0.7% | 92.7% |  |
| TO_BOOL_STR | 11,840,240 | 0.6% | 93.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 9,209,180 | 0.5% | 93.9% |  |
| CONTAINS_OP | 9,016,640 | 0.5% | 94.4% |  |
| TO_BOOL_INT | 8,949,720 | 0.5% | 94.9% |  |
| LOAD_ATTR_INSTANCE_VALUE | 6,922,260 | 0.4% | 95.2% | 0.0% |
| CALL_BUILTIN_O | 6,860,800 | 0.4% | 95.6% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 5,469,220 | 0.3% | 95.9% |  |
| NOP | 5,212,980 | 0.3% | 96.2% |  |
| GET_ITER | 4,978,060 | 0.3% | 96.5% |  |
| FOR_ITER | 4,953,660 | 0.3% | 96.7% |  |
| LOAD_DEREF | 4,935,920 | 0.3% | 97.0% |  |
| BINARY_SUBSCR_LIST_INT | 4,332,020 | 0.2% | 97.2% | 0.7% |
| STORE_FAST_STORE_FAST | 4,262,300 | 0.2% | 97.5% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,262,220 | 0.2% | 97.7% |  |
| PUSH_NULL | 4,024,960 | 0.2% | 97.9% |  |
| BINARY_SLICE | 3,573,760 | 0.2% | 98.1% |  |
| CALL_LIST_APPEND | 2,979,760 | 0.2% | 98.3% |  |
| CALL_ISINSTANCE | 2,940,580 | 0.2% | 98.4% |  |
| LOAD_ATTR_PROPERTY | 2,919,240 | 0.2% | 98.6% |  |
| LOAD_ATTR_MODULE | 2,119,460 | 0.1% | 98.7% |  |
| BUILD_TUPLE | 1,812,760 | 0.1% | 98.8% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,715,180 | 0.1% | 98.9% | 79.1% |
| COMPARE_OP_STR | 1,609,700 | 0.1% | 99.0% |  |
| CALL_KW | 1,607,680 | 0.1% | 99.1% |  |
| CALL | 1,529,040 | 0.1% | 99.2% |  |
| CALL_LEN | 1,515,580 | 0.1% | 99.3% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,413,100 | 0.1% | 99.3% |  |
| POP_JUMP_IF_NOT_NONE | 1,382,740 | 0.1% | 99.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,337,160 | 0.1% | 99.5% | 71.0% |
| CALL_TYPE_1 | 1,208,280 | 0.1% | 99.6% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,029,900 | 0.1% | 99.6% | 79.0% |
| CALL_FUNCTION_EX | 1,013,920 | 0.1% | 99.7% |  |
| DICT_MERGE | 1,013,760 | 0.1% | 99.7% |  |
| BUILD_MAP | 1,003,520 | 0.1% | 99.8% |  |
| MAKE_CELL | 839,680 | 0.0% | 99.8% |  |
| IS_OP | 604,160 | 0.0% | 99.9% |  |
| EXTENDED_ARG | 594,600 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 320,020 | 0.0% | 99.9% |  |
| POP_JUMP_IF_NONE | 297,920 | 0.0% | 99.9% |  |
| BUILD_LIST | 226,320 | 0.0% | 99.9% |  |
| STORE_DEREF | 174,080 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 161,640 | 0.0% | 100.0% |  |
| FOR_ITER_LIST | 154,380 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 82,000 | 0.0% | 100.0% |  |
| CALL_STR_1 | 71,640 | 0.0% | 100.0% |  |
| UNARY_NOT | 61,440 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 61,440 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 61,440 | 0.0% | 100.0% |  |
| TO_BOOL_LIST | 60,880 | 0.0% | 100.0% | 15.7% |
| BUILD_CONST_KEY_MAP | 51,200 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 40,940 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 30,720 | 0.0% | 100.0% |  |
| POP_EXCEPT | 30,720 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 30,720 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 20,480 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 20,480 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 20,460 | 0.0% | 100.0% |  |
| TO_BOOL | 16,880 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 11,280 | 0.0% | 100.0% |  |
| DICT_UPDATE | 10,240 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 10,220 | 0.0% | 100.0% | 0.6% |
| BINARY_OP_SUBTRACT_FLOAT | 10,220 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 10,220 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 6,640 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,200 | 0.0% | 100.0% |  |
| RESUME | 2,040 | 0.0% | 100.0% | 205.9% |
| STORE_ATTR | 1,720 | 0.0% | 100.0% |  |
| BINARY_OP | 760 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 460 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 160 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 80 | 0.0% | 100.0% |  |
| LIST_EXTEND | 80 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_SLOT | 212,122,060 | 11.6% | 11.6% |
| LOAD_ATTR_SLOT LOAD_FAST | 112,798,780 | 6.2% | 17.8% |
| STORE_ATTR_SLOT LOAD_FAST | 60,498,920 | 3.3% | 21.1% |
| POP_JUMP_IF_FALSE LOAD_FAST | 53,044,140 | 2.9% | 24.0% |
| RESUME_CHECK LOAD_FAST | 52,776,920 | 2.9% | 26.9% |
| LOAD_FAST STORE_ATTR_SLOT | 50,278,400 | 2.8% | 29.6% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 38,297,520 | 2.1% | 31.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 32,111,860 | 1.8% | 33.5% |
| LOAD_FAST COPY | 28,948,960 | 1.6% | 35.1% |
| BINARY_OP_ADD_INT SWAP | 28,907,920 | 1.6% | 36.6% |
| COPY LOAD_ATTR_SLOT | 28,907,840 | 1.6% | 38.2% |
| SWAP STORE_ATTR_SLOT | 28,907,840 | 1.6% | 39.8% |
| LOAD_FAST BINARY_OP_ADD_INT | 28,499,600 | 1.6% | 41.4% |
| POP_JUMP_IF_TRUE LOAD_FAST | 28,276,380 | 1.5% | 42.9% |
| LOAD_ATTR_SLOT COMPARE_OP_INT | 27,076,280 | 1.5% | 44.4% |
| BINARY_SUBSCR_STR_INT LOAD_FAST | 27,064,760 | 1.5% | 45.9% |
| STORE_FAST LOAD_FAST | 24,983,700 | 1.4% | 47.2% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 22,706,160 | 1.2% | 48.5% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 21,423,340 | 1.2% | 49.7% |
| RETURN_CONST POP_TOP | 21,176,560 | 1.2% | 50.8% |
| COMPARE_OP POP_JUMP_IF_FALSE | 20,338,140 | 1.1% | 51.9% |
| LOAD_ATTR_SLOT LOAD_CONST | 18,854,100 | 1.0% | 53.0% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 18,708,000 | 1.0% | 54.0% |
| POP_JUMP_IF_FALSE RETURN_CONST | 18,626,920 | 1.0% | 55.0% |
| STORE_ATTR_SLOT RETURN_CONST | 18,012,280 | 1.0% | 56.0% |
| LOAD_ATTR_SLOT LOAD_ATTR_SLOT | 17,832,400 | 1.0% | 57.0% |
| LOAD_ATTR_SLOT TO_BOOL_ALWAYS_TRUE | 17,543,660 | 1.0% | 57.9% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 16,528,860 | 0.9% | 58.8% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 16,216,420 | 0.9% | 59.7% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 15,109,300 | 0.8% | 60.5% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 14,972,580 | 0.8% | 61.4% |
| LOAD_FAST LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 14,962,420 | 0.8% | 62.2% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 14,823,780 | 0.8% | 63.0% |
| RETURN_CONST TO_BOOL_NONE | 13,989,340 | 0.8% | 63.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 13,620,880 | 0.7% | 64.5% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_GLOBAL_MODULE | 13,595,980 | 0.7% | 65.2% |
| COMPARE_OP_INT LOAD_FAST | 13,537,500 | 0.7% | 66.0% |
| BINARY_OP_SUBTRACT_INT BINARY_SUBSCR_STR_INT | 13,537,480 | 0.7% | 66.7% |
| LOAD_ATTR_SLOT BINARY_SUBSCR_STR_INT | 13,527,240 | 0.7% | 67.5% |
| POP_TOP LOAD_FAST | 12,421,400 | 0.7% | 68.1% |
| CACHE RESUME_CHECK | 11,938,760 | 0.7% | 68.8% |
| LOAD_FAST COMPARE_OP | 11,366,480 | 0.6% | 69.4% |
| LOAD_ATTR CALL_PY_EXACT_ARGS | 10,769,420 | 0.6% | 70.0% |
| TO_BOOL_STR POP_JUMP_IF_TRUE | 10,434,800 | 0.6% | 70.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 9,955,980 | 0.5% | 71.1% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 9,165,920 | 0.5% | 71.6% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 9,164,880 | 0.5% | 72.1% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 9,126,360 | 0.5% | 72.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT LOAD_ATTR_METHOD_NO_DICT | 9,042,360 | 0.5% | 73.1% |
| LOAD_ATTR_SLOT CALL_METHOD_DESCRIPTOR_FAST | 9,021,360 | 0.5% | 73.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 8,993,860 | 0.5% | 74.1% |
| LOAD_ATTR COMPARE_OP | 8,991,900 | 0.5% | 74.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 8,981,520 | 0.5% | 75.1% |
| LOAD_ATTR_SLOT TO_BOOL_INT | 8,949,680 | 0.5% | 75.6% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_FALSE | 8,946,440 | 0.5% | 76.1% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 8,939,500 | 0.5% | 76.6% |
| LOAD_ATTR_SLOT TO_BOOL_STR | 8,939,480 | 0.5% | 77.1% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 8,937,740 | 0.5% | 77.5% |
| RETURN_VALUE INTERPRETER_EXIT | 8,867,020 | 0.5% | 78.0% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 8,326,440 | 0.5% | 78.5% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 8,038,200 | 0.4% | 78.9% |
| JUMP_FORWARD LOAD_FAST | 7,949,960 | 0.4% | 79.4% |
| LOAD_FAST TO_BOOL_ALWAYS_TRUE | 7,804,900 | 0.4% | 79.8% |
| RETURN_VALUE STORE_FAST | 7,669,740 | 0.4% | 80.2% |
| RETURN_VALUE RETURN_VALUE | 7,639,120 | 0.4% | 80.6% |
| POP_JUMP_IF_FALSE JUMP_FORWARD | 7,118,360 | 0.4% | 81.0% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 6,922,240 | 0.4% | 81.4% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 6,869,780 | 0.4% | 81.8% |
| CALL_BUILTIN_O RETURN_VALUE | 6,860,800 | 0.4% | 82.1% |
| LOAD_ATTR_INSTANCE_VALUE CALL_BUILTIN_O | 6,860,800 | 0.4% | 82.5% |
| LOAD_CONST LOAD_FAST | 6,656,280 | 0.4% | 82.9% |
| LOAD_FAST RETURN_VALUE | 5,939,280 | 0.3% | 83.2% |
| LOAD_CONST STORE_FAST | 5,921,060 | 0.3% | 83.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 5,913,160 | 0.3% | 83.9% |
| LOAD_FAST CONTAINS_OP | 5,509,120 | 0.3% | 84.2% |
| LOAD_ATTR_METHOD_NO_DICT CALL_METHOD_DESCRIPTOR_NOARGS | 5,469,020 | 0.3% | 84.5% |
| GET_ITER FOR_ITER | 4,946,360 | 0.3% | 84.7% |
| LOAD_DEREF LOAD_ATTR_METHOD_NO_DICT | 4,739,200 | 0.3% | 85.0% |
| LOAD_FAST TO_BOOL_NONE | 4,473,860 | 0.2% | 85.2% |
| STORE_FAST LOAD_CONST | 4,405,000 | 0.2% | 85.5% |
| RETURN_VALUE LOAD_FAST | 4,383,320 | 0.2% | 85.7% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 4,341,600 | 0.2% | 85.9% |
| LOAD_FAST_LOAD_FAST BINARY_SUBSCR_LIST_INT | 4,321,160 | 0.2% | 86.2% |
| RESUME_CHECK NOP | 4,301,500 | 0.2% | 86.4% |
| NOP LOAD_FAST_LOAD_FAST | 4,300,800 | 0.2% | 86.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 4,300,760 | 0.2% | 86.9% |
| BINARY_SUBSCR_LIST_INT RETURN_VALUE | 4,280,280 | 0.2% | 87.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT CALL_PY_EXACT_ARGS | 4,269,440 | 0.2% | 87.4% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 4,262,220 | 0.2% | 87.6% |
| POP_TOP JUMP_FORWARD | 4,126,720 | 0.2% | 87.8% |
| JUMP_FORWARD ENTER_EXECUTOR | 4,105,900 | 0.2% | 88.0% |
| BINARY_SLICE RETURN_VALUE | 3,573,760 | 0.2% | 88.2% |
| LOAD_ATTR_SLOT BINARY_SLICE | 3,573,740 | 0.2% | 88.4% |
| POP_TOP RETURN_CONST | 3,471,360 | 0.2% | 88.6% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 3,420,500 | 0.2% | 88.8% |
| LOAD_CONST COMPARE_OP_INT | 3,186,700 | 0.2% | 89.0% |
| LOAD_FAST PUSH_NULL | 3,092,480 | 0.2% | 89.2% |
| RETURN_CONST INTERPRETER_EXIT | 3,072,000 | 0.2% | 89.3% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 3,021,340 | 0.2% | 89.5% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_NO_DICT | 2,962,300 | 0.2% | 89.6% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,573,740 | 100.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,573,760 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,938,760 | 100.0% |
| RESUME | 260 | 0.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,220 | 55.5% |
| ENTER_EXECUTOR | 580 | 26.4% |
| LOAD_ATTR_SLOT | 340 | 15.5% |
| BINARY_OP | 40 | 1.8% |
| JUMP_BACKWARD | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,200 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 10,600 | 94.0% |
| BINARY_SUBSCR | 160 | 1.4% |
| LOAD_FAST_LOAD_FAST | 160 | 1.4% |
| LOAD_ATTR | 80 | 0.7% |
| LOAD_FAST | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 10,520 | 93.3% |
| BINARY_SUBSCR | 160 | 1.4% |
| BINARY_SUBSCR_DICT | 120 | 1.1% |
| BINARY_SUBSCR_LIST_INT | 80 | 0.7% |
| RETURN_VALUE | 60 | 0.5% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 30,700 | 99.9% |
| LOAD_GLOBAL | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 30,720 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 2,570,220 | 51.6% |
| LOAD_FAST | 1,414,460 | 28.4% |
| LOAD_ATTR_SLOT | 982,980 | 19.7% |
| CALL_BUILTIN_CLASS | 10,280 | 0.2% |
| CALL | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 4,946,360 | 99.4% |
| FOR_ITER_LIST | 31,640 | 0.6% |
| FOR_ITER_RANGE | 60 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,867,020 | 74.3% |
| RETURN_CONST | 3,072,000 | 25.7% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 20,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 20,480 | 100.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 4,301,500 | 82.5% |
| POP_JUMP_IF_FALSE | 481,280 | 9.2% |
| STORE_FAST | 430,080 | 8.3% |
| POP_TOP | 80 | 0.0% |
| RESUME | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,300,800 | 82.5% |
| LOAD_FAST | 912,100 | 17.5% |
| LOAD_DEREF | 80 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 30,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 30,720 | 100.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 21,176,560 | 90.9% |
| POP_JUMP_IF_TRUE | 1,064,960 | 4.6% |
| SWAP | 553,240 | 2.4% |
| POP_JUMP_IF_FALSE | 481,280 | 2.1% |
| RETURN_VALUE | 20,480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,421,400 | 53.3% |
| JUMP_FORWARD | 4,126,720 | 17.7% |
| RETURN_CONST | 3,471,360 | 14.9% |
| LOAD_CONST | 1,607,680 | 6.9% |
| RETURN_VALUE | 553,240 | 2.4% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 30,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 30,680 | 99.9% |
| LOAD_GLOBAL | 40 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,092,480 | 76.8% |
| LOAD_ATTR_MODULE | 584,020 | 14.5% |
| LOAD_FAST_LOAD_FAST | 204,800 | 5.1% |
| BINARY_SUBSCR_DICT | 71,660 | 1.8% |
| LOAD_ATTR | 51,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 1,227,140 | 30.5% |
| CALL_PY_EXACT_ARGS | 1,024,820 | 25.5% |
| LOAD_CONST | 983,040 | 24.4% |
| LOAD_FAST | 583,840 | 14.5% |
| LOAD_FAST_LOAD_FAST | 71,680 | 1.8% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,639,120 | 23.1% |
| CALL_BUILTIN_O | 6,860,800 | 20.8% |
| LOAD_FAST | 5,939,280 | 18.0% |
| BINARY_SUBSCR_LIST_INT | 4,280,280 | 13.0% |
| BINARY_SLICE | 3,573,760 | 10.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 8,867,020 | 26.9% |
| STORE_FAST | 7,669,740 | 23.2% |
| RETURN_VALUE | 7,639,120 | 23.1% |
| LOAD_FAST | 4,383,320 | 13.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,679,560 | 5.1% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 20 | 50.0% |
| STORE_SUBSCR_DICT | 20 | 50.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,760 | 69.7% |
| RETURN_CONST | 2,880 | 17.1% |
| COPY | 840 | 5.0% |
| LOAD_ATTR | 380 | 2.3% |
| LOAD_ATTR_SLOT | 300 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,360 | 73.2% |
| TO_BOOL_NONE | 2,020 | 12.0% |
| POP_JUMP_IF_TRUE | 1,000 | 5.9% |
| TO_BOOL_BOOL | 820 | 4.9% |
| TO_BOOL_ALWAYS_TRUE | 180 | 1.1% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 61,420 | 100.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 61,440 | 100.0% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 360 | 47.4% |
| LOAD_FAST | 200 | 26.3% |
| LOAD_ATTR | 40 | 5.3% |
| LOAD_FAST_LOAD_FAST | 40 | 5.3% |
| LOAD_ATTR_SLOT | 40 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 160 | 21.1% |
| BINARY_OP_SUBTRACT_INT | 140 | 18.4% |
| STORE_FAST | 120 | 15.8% |
| CALL | 80 | 10.5% |
| SWAP | 80 | 10.5% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 51,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 20,480 | 40.0% |
| LOAD_DEREF | 20,480 | 40.0% |
| LOAD_FAST | 10,240 | 20.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 113,680 | 50.2% |
| STORE_ATTR_SLOT | 71,620 | 31.6% |
| BUILD_LIST | 20,480 | 9.0% |
| RETURN_VALUE | 10,240 | 4.5% |
| ENTER_EXECUTOR | 9,900 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 112,640 | 49.8% |
| LOAD_FAST | 71,680 | 31.7% |
| BUILD_LIST | 20,480 | 9.0% |
| STORE_FAST | 20,480 | 9.0% |
| COMPARE_OP | 960 | 0.4% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 983,040 | 98.0% |
| BUILD_TUPLE | 10,240 | 1.0% |
| STORE_FAST | 10,240 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 993,280 | 99.0% |
| STORE_FAST | 10,240 | 1.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,689,880 | 93.2% |
| LOAD_GLOBAL_MODULE | 81,900 | 4.5% |
| POP_JUMP_IF_FALSE | 20,480 | 1.1% |
| LOAD_ATTR_MODULE | 20,460 | 1.1% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,126,400 | 62.1% |
| SWAP | 553,240 | 30.5% |
| CALL_ISINSTANCE | 81,880 | 4.5% |
| LOAD_CONST | 20,480 | 1.1% |
| LOAD_FAST | 20,480 | 1.1% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,352,460 | 88.5% |
| ENTER_EXECUTOR | 131,820 | 8.6% |
| PUSH_NULL | 21,800 | 1.4% |
| LOAD_GLOBAL_MODULE | 10,260 | 0.7% |
| LOAD_ATTR | 5,460 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 1,413,160 | 92.4% |
| TO_BOOL_BOOL | 61,400 | 4.0% |
| STORE_FAST | 20,700 | 1.4% |
| RESUME_CHECK | 13,640 | 0.9% |
| LOAD_FAST | 10,280 | 0.7% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 1,013,760 | 100.0% |
| CALL_INTRINSIC_1 | 80 | 0.0% |
| LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 983,040 | 97.0% |
| RETURN_VALUE | 20,480 | 2.0% |
| LOAD_ATTR_METHOD_NO_DICT | 10,200 | 1.0% |
| COPY_FREE_VARS | 80 | 0.0% |
| RESUME_CHECK | 60 | 0.0% |


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
| LOAD_CONST | 1,607,680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 962,500 | 59.9% |
| RETURN_VALUE | 645,120 | 40.1% |
| RESUME | 60 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 11,366,480 | 55.8% |
| LOAD_ATTR | 8,991,900 | 44.2% |
| COMPARE_OP | 6,400 | 0.0% |
| BUILD_LIST | 960 | 0.0% |
| LOAD_CONST | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 20,338,140 | 99.9% |
| STORE_FAST | 20,480 | 0.1% |
| COMPARE_OP | 6,400 | 0.0% |
| POP_JUMP_IF_TRUE | 960 | 0.0% |
| COMPARE_OP_INT | 280 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,509,120 | 61.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 2,092,920 | 23.2% |
| LOAD_FAST_LOAD_FAST | 1,403,200 | 15.6% |
| LOAD_CONST | 10,240 | 0.1% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,993,860 | 99.7% |
| STORE_FAST | 21,840 | 0.2% |
| POP_JUMP_IF_TRUE | 940 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,948,960 | 90.7% |
| RETURN_CONST | 1,607,680 | 5.0% |
| IS_OP | 604,160 | 1.9% |
| CALL_ISINSTANCE | 522,200 | 1.6% |
| RETURN_VALUE | 184,320 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 28,907,840 | 90.5% |
| TO_BOOL_BOOL | 1,576,060 | 4.9% |
| TO_BOOL_NONE | 1,266,240 | 4.0% |
| TO_BOOL_ALWAYS_TRUE | 126,540 | 0.4% |
| TO_BOOL_LIST | 40,920 | 0.1% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 50,360 | 61.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 31,520 | 38.4% |
| CALL_FUNCTION_EX | 80 | 0.1% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 81,960 | 100.0% |
| RESUME | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 983,040 | 97.0% |
| BUILD_CONST_KEY_MAP | 20,480 | 2.0% |
| DICT_UPDATE | 10,240 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,013,760 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 10,240 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 8,937,740 | 40.5% |
| JUMP_FORWARD | 4,105,900 | 18.6% |
| POP_JUMP_IF_FALSE | 2,447,900 | 11.1% |
| COMPARE_OP_INT | 1,657,520 | 7.5% |
| CALL_LIST_APPEND | 1,402,540 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 14,823,780 | 67.2% |
| LOAD_FAST | 1,926,820 | 8.7% |
| RETURN_CONST | 1,626,420 | 7.4% |
| CALL_LIST_APPEND | 1,392,300 | 6.3% |
| LOAD_CONST | 1,105,580 | 5.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 440,380 | 74.1% |
| TO_BOOL_BOOL | 112,500 | 18.9% |
| STORE_FAST | 30,720 | 5.2% |
| TO_BOOL_INT | 10,220 | 1.7% |
| POP_TOP | 340 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 552,960 | 93.0% |
| JUMP_FORWARD | 30,720 | 5.2% |
| POP_JUMP_IF_TRUE | 10,240 | 1.7% |
| JUMP_BACKWARD | 680 | 0.1% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 4,946,360 | 99.9% |
| JUMP_BACKWARD | 5,220 | 0.1% |
| FOR_ITER | 2,080 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,582,580 | 52.1% |
| STORE_FAST | 2,365,940 | 47.8% |
| FOR_ITER | 2,080 | 0.0% |
| RETURN_CONST | 1,660 | 0.0% |
| LOAD_FAST | 580 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_TYPE_1 | 604,140 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 604,160 | 100.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 154,240 | 95.4% |
| POP_JUMP_IF_TRUE | 2,920 | 1.8% |
| STORE_ATTR_SLOT | 1,300 | 0.8% |
| STORE_FAST | 1,020 | 0.6% |
| EXTENDED_ARG | 680 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 154,900 | 95.8% |
| FOR_ITER | 5,220 | 3.2% |
| FOR_ITER_LIST | 960 | 0.6% |
| FOR_ITER_RANGE | 300 | 0.2% |
| RETURN_CONST | 40 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,118,360 | 52.4% |
| POP_TOP | 4,126,720 | 30.4% |
| RETURN_VALUE | 1,351,660 | 10.0% |
| STORE_ATTR_SLOT | 409,580 | 3.0% |
| STORE_FAST | 400,920 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,949,960 | 58.6% |
| ENTER_EXECUTOR | 4,105,900 | 30.3% |
| STORE_FAST | 1,464,320 | 10.8% |
| LOAD_DEREF | 30,720 | 0.2% |
| CALL_PY_EXACT_ARGS | 20,460 | 0.2% |


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
| LOAD_GLOBAL_MODULE | 21,423,340 | 90.8% |
| LOAD_FAST | 2,019,000 | 8.6% |
| LOAD_ATTR_MODULE | 92,100 | 0.4% |
| LOAD_ATTR | 26,180 | 0.1% |
| LOAD_DEREF | 22,400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,769,420 | 45.7% |
| COMPARE_OP | 8,991,900 | 38.1% |
| LOAD_FAST | 1,896,700 | 8.0% |
| LOAD_GLOBAL_MODULE | 900,920 | 3.8% |
| CALL_PY_WITH_DEFAULTS | 849,800 | 3.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 18,854,100 | 50.0% |
| STORE_FAST | 4,405,000 | 11.7% |
| LOAD_FAST | 2,338,380 | 6.2% |
| POP_JUMP_IF_FALSE | 2,233,060 | 5.9% |
| STORE_ATTR_SLOT | 1,791,900 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 14,972,580 | 39.7% |
| LOAD_FAST | 6,656,280 | 17.6% |
| STORE_FAST | 5,921,060 | 15.7% |
| COMPARE_OP_INT | 3,186,700 | 8.4% |
| BINARY_OP_ADD_INT | 1,844,400 | 4.9% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,375,680 | 48.1% |
| STORE_FAST | 1,034,240 | 21.0% |
| RESUME_CHECK | 747,480 | 15.1% |
| LOAD_ATTR_METHOD_NO_DICT | 255,940 | 5.2% |
| STORE_DEREF | 174,080 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,739,200 | 96.0% |
| CALL_PY_EXACT_ARGS | 174,000 | 3.5% |
| LOAD_ATTR | 22,400 | 0.5% |
| PUSH_NULL | 160 | 0.0% |
| CALL | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 112,798,780 | 24.5% |
| STORE_ATTR_SLOT | 60,498,920 | 13.1% |
| POP_JUMP_IF_FALSE | 53,044,140 | 11.5% |
| RESUME_CHECK | 52,776,920 | 11.4% |
| POP_JUMP_IF_TRUE | 28,276,380 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 212,122,060 | 46.0% |
| STORE_ATTR_SLOT | 50,278,400 | 10.9% |
| LOAD_ATTR_METHOD_NO_DICT | 32,111,860 | 7.0% |
| COPY | 28,948,960 | 6.3% |
| BINARY_OP_ADD_INT | 28,499,600 | 6.2% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 61,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 61,400 | 99.9% |
| TO_BOOL | 40 | 0.1% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| NOP | 4,300,800 | 23.0% |
| RESUME_CHECK | 3,021,340 | 16.1% |
| STORE_ATTR_SLOT | 2,880,160 | 15.4% |
| LOAD_GLOBAL_MODULE | 2,755,480 | 14.7% |
| STORE_FAST | 2,399,760 | 12.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 5,913,160 | 31.6% |
| BINARY_SUBSCR_LIST_INT | 4,321,160 | 23.1% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 1,938,260 | 10.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,454,240 | 7.8% |
| LOAD_FAST | 1,424,000 | 7.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 2,140 | 32.2% |
| LOAD_ATTR_METHOD_NO_DICT | 1,860 | 28.0% |
| LOAD_FAST | 560 | 8.4% |
| STORE_FAST | 480 | 7.2% |
| POP_JUMP_IF_FALSE | 400 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,700 | 40.7% |
| LOAD_ATTR | 2,480 | 37.3% |
| LOAD_GLOBAL_BUILTIN | 620 | 9.3% |
| LOAD_FAST | 580 | 8.7% |
| CALL | 80 | 1.2% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 441,260 | 52.6% |
| CALL_BOUND_METHOD_EXACT_ARGS | 224,240 | 26.7% |
| MAKE_CELL | 174,080 | 20.7% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 665,520 | 79.3% |
| MAKE_CELL | 174,080 | 20.7% |
| RESUME | 80 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 20,338,140 | 22.5% |
| TO_BOOL_NONE | 16,216,420 | 17.9% |
| COMPARE_OP_INT | 15,109,300 | 16.7% |
| CONTAINS_OP | 8,993,860 | 9.9% |
| TO_BOOL_ALWAYS_TRUE | 8,946,440 | 9.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,044,140 | 58.6% |
| RETURN_CONST | 18,626,920 | 20.6% |
| JUMP_FORWARD | 7,118,360 | 7.9% |
| ENTER_EXECUTOR | 2,447,900 | 2.7% |
| LOAD_DEREF | 2,375,680 | 2.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 267,200 | 89.7% |
| LOAD_ATTR_INSTANCE_VALUE | 20,480 | 6.9% |
| BINARY_SUBSCR_LIST_INT | 10,220 | 3.4% |
| BINARY_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 287,680 | 96.6% |
| LOAD_FAST_LOAD_FAST | 10,240 | 3.4% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,372,500 | 99.3% |
| LOAD_ATTR_SLOT | 10,220 | 0.7% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,382,740 | 100.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_ALWAYS_TRUE | 16,528,860 | 41.7% |
| TO_BOOL_STR | 10,434,800 | 26.3% |
| TO_BOOL_BOOL | 9,165,920 | 23.1% |
| TO_BOOL_NONE | 3,420,500 | 8.6% |
| TO_BOOL_LIST | 40,940 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,276,380 | 71.4% |
| ENTER_EXECUTOR | 8,937,740 | 22.6% |
| RETURN_CONST | 1,105,920 | 2.8% |
| POP_TOP | 1,064,960 | 2.7% |
| RETURN_VALUE | 133,120 | 0.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 18,626,920 | 43.4% |
| STORE_ATTR_SLOT | 18,012,280 | 42.0% |
| POP_TOP | 3,471,360 | 8.1% |
| ENTER_EXECUTOR | 1,626,420 | 3.8% |
| POP_JUMP_IF_TRUE | 1,105,920 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 21,176,560 | 49.4% |
| TO_BOOL_NONE | 13,989,340 | 32.6% |
| INTERPRETER_EXIT | 3,072,000 | 7.2% |
| COPY | 1,607,680 | 3.7% |
| STORE_FAST | 1,085,440 | 2.5% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 20,480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 20,440 | 99.8% |
| CALL | 40 | 0.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,040 | 60.5% |
| LOAD_FAST_LOAD_FAST | 520 | 30.2% |
| SWAP | 160 | 9.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 860 | 50.0% |
| LOAD_FAST | 280 | 16.3% |
| LOAD_FAST_LOAD_FAST | 180 | 10.5% |
| RETURN_CONST | 120 | 7.0% |
| LOAD_CONST | 100 | 5.8% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 174,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 174,080 | 100.0% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 9,126,360 | 26.5% |
| RETURN_VALUE | 7,669,740 | 22.2% |
| LOAD_CONST | 5,921,060 | 17.2% |
| LOAD_FAST | 2,819,500 | 8.2% |
| FOR_ITER | 2,365,940 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,983,700 | 72.4% |
| LOAD_CONST | 4,405,000 | 12.8% |
| LOAD_FAST_LOAD_FAST | 2,399,760 | 7.0% |
| LOAD_DEREF | 1,034,240 | 3.0% |
| LOAD_GLOBAL_BUILTIN | 655,940 | 1.9% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 4,262,220 | 100.0% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,653,040 | 62.2% |
| LOAD_GLOBAL_BUILTIN | 1,609,260 | 37.8% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 28,907,920 | 98.1% |
| BUILD_TUPLE | 553,240 | 1.9% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 28,907,840 | 98.1% |
| POP_TOP | 553,240 | 1.9% |
| STORE_ATTR | 160 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 80 | 50.0% |
| FOR_ITER | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 80 | 50.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 80 | 50.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,440 | 70.6% |
| CACHE | 260 | 12.7% |
| CALL_BOUND_METHOD_EXACT_ARGS | 120 | 5.9% |
| MAKE_CELL | 80 | 3.9% |
| CALL_KW | 60 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,560 | 76.5% |
| LOAD_GLOBAL | 180 | 8.8% |
| LOAD_DEREF | 120 | 5.9% |
| LOAD_CONST | 80 | 3.9% |
| LOAD_FAST_LOAD_FAST | 60 | 2.9% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_FLOAT | 10,200 | 99.8% |
| BINARY_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,220 | 100.0% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 28,499,600 | 93.9% |
| LOAD_CONST | 1,844,400 | 6.1% |
| BINARY_OP | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 28,907,920 | 95.3% |
| CALL_PY_EXACT_ARGS | 1,423,320 | 4.7% |
| STORE_FAST | 12,900 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,200 | 99.8% |
| BINARY_OP | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_FLOAT | 10,200 | 99.8% |
| BINARY_OP | 20 | 0.2% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 14,972,580 | 91.3% |
| CALL_LEN | 1,413,080 | 8.6% |
| LOAD_ATTR_SLOT | 10,200 | 0.1% |
| BINARY_OP | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_STR_INT | 13,537,480 | 82.6% |
| CALL_PY_EXACT_ARGS | 1,443,720 | 8.8% |
| LOAD_CONST | 1,413,100 | 8.6% |
| LOAD_FAST | 1,340 | 0.0% |
| COMPARE_OP_INT | 260 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 277,100 | 86.6% |
| LOAD_FAST | 20,440 | 6.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 20,440 | 6.4% |
| LOAD_FAST_LOAD_FAST | 1,920 | 0.6% |
| BINARY_SUBSCR | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 204,780 | 64.0% |
| PUSH_NULL | 71,660 | 22.4% |
| RETURN_VALUE | 20,460 | 6.4% |
| CALL_PY_WITH_DEFAULTS | 20,440 | 6.4% |
| STORE_FAST | 2,660 | 0.8% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_NOARGS | 20,440 | 99.9% |
| BINARY_SUBSCR | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 20,460 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,321,160 | 99.7% |
| LOAD_CONST | 10,200 | 0.2% |
| BINARY_SUBSCR_LIST_INT | 580 | 0.0% |
| BINARY_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,280,280 | 98.8% |
| PUSH_EXC_INFO | 30,720 | 0.7% |
| LOAD_FAST_LOAD_FAST | 10,220 | 0.2% |
| POP_JUMP_IF_NONE | 10,220 | 0.2% |
| BINARY_SUBSCR_LIST_INT | 580 | 0.0% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 13,537,480 | 50.0% |
| LOAD_ATTR_SLOT | 13,527,240 | 50.0% |
| LOAD_FAST | 1,320 | 0.0% |
| BINARY_SUBSCR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,064,760 | 100.0% |
| STORE_FAST | 1,340 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,227,140 | 91.8% |
| LOAD_ATTR_SLOT | 71,600 | 5.4% |
| LOAD_FAST | 20,400 | 1.5% |
| CALL_PY_EXACT_ARGS | 17,860 | 1.3% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,063,400 | 79.5% |
| MAKE_CELL | 224,240 | 16.8% |
| COPY_FREE_VARS | 31,520 | 2.4% |
| CALL_PY_EXACT_ARGS | 17,880 | 1.3% |
| RESUME | 120 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 40,920 | 66.6% |
| LOAD_FAST | 10,240 | 16.7% |
| LOAD_ATTR | 10,200 | 16.6% |
| CALL | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40,940 | 66.6% |
| GET_ITER | 10,280 | 16.7% |
| STORE_FAST | 10,220 | 16.6% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,920 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40,920 | 100.0% |
| CALL | 20 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,413,080 | 100.0% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,413,100 | 100.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 6,860,800 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 6,860,800 | 100.0% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,681,720 | 57.2% |
| LOAD_ATTR_MODULE | 634,680 | 21.6% |
| LOAD_ATTR_SLOT | 450,520 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 91,580 | 3.1% |
| BUILD_TUPLE | 81,880 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,418,220 | 82.2% |
| COPY | 522,200 | 17.8% |
| TO_BOOL | 160 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,495,000 | 98.6% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 10,200 | 0.7% |
| LOAD_ATTR_SLOT | 10,200 | 0.7% |
| CALL | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_SUBTRACT_INT | 1,413,080 | 93.2% |
| LOAD_CONST | 40,940 | 2.7% |
| STORE_FAST | 20,660 | 1.4% |
| COMPARE_OP_INT | 20,400 | 1.3% |
| LOAD_FAST | 10,220 | 0.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,413,160 | 47.4% |
| ENTER_EXECUTOR | 1,392,300 | 46.7% |
| LOAD_FAST | 164,080 | 5.5% |
| RETURN_VALUE | 10,200 | 0.3% |
| JUMP_BACKWARD | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,413,100 | 47.4% |
| ENTER_EXECUTOR | 1,402,540 | 47.1% |
| LOAD_FAST | 163,800 | 5.5% |
| JUMP_BACKWARD | 320 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 9,021,360 | 98.0% |
| LOAD_FAST | 93,640 | 1.0% |
| LOAD_CONST | 81,880 | 0.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,200 | 0.1% |
| LOAD_ATTR_METHOD_NO_DICT | 1,020 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 9,126,360 | 99.1% |
| RETURN_VALUE | 81,900 | 0.9% |
| CALL_PY_WITH_DEFAULTS | 900 | 0.0% |
| CALL | 20 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 5,469,020 | 100.0% |
| CALL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,570,220 | 47.0% |
| TO_BOOL_BOOL | 1,433,480 | 26.2% |
| CALL_PY_EXACT_ARGS | 1,403,160 | 25.7% |
| BINARY_SUBSCR_DICT | 20,440 | 0.4% |
| BINARY_SUBSCR_GETITEM | 20,440 | 0.4% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 10,769,420 | 27.8% |
| LOAD_FAST | 8,981,520 | 23.1% |
| LOAD_ATTR_METHOD_NO_DICT | 6,869,780 | 17.7% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 4,269,440 | 11.0% |
| LOAD_ATTR_SLOT | 1,494,960 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 38,297,520 | 98.7% |
| MAKE_CELL | 441,260 | 1.1% |
| COPY_FREE_VARS | 50,360 | 0.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 17,860 | 0.0% |
| CALL | 640 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 14,823,780 | 79.2% |
| LOAD_ATTR_METHOD_NO_DICT | 2,028,940 | 10.8% |
| LOAD_FAST | 973,420 | 5.2% |
| LOAD_ATTR | 849,800 | 4.5% |
| BINARY_SUBSCR_DICT | 20,440 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 18,708,000 | 100.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 71,600 | 99.9% |
| CALL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 71,640 | 100.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,208,240 | 100.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IS_OP | 604,140 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 604,120 | 50.0% |
| LOAD_GLOBAL | 20 | 0.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 27,076,280 | 89.3% |
| LOAD_CONST | 3,186,700 | 10.5% |
| LOAD_FAST_LOAD_FAST | 20,400 | 0.1% |
| CALL_LEN | 20,400 | 0.1% |
| COMPARE_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 15,109,300 | 49.9% |
| LOAD_FAST | 13,537,500 | 44.7% |
| ENTER_EXECUTOR | 1,657,520 | 5.5% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,464,560 | 91.0% |
| LOAD_CONST | 82,380 | 5.1% |
| LOAD_FAST | 62,320 | 3.9% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 260 | 0.0% |
| COMPARE_OP | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,609,700 | 100.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 121,700 | 78.8% |
| GET_ITER | 31,640 | 20.5% |
| JUMP_BACKWARD | 960 | 0.6% |
| FOR_ITER | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 102,060 | 66.1% |
| STORE_FAST | 21,280 | 13.8% |
| LOAD_FAST | 10,240 | 6.6% |
| LOAD_FAST_LOAD_FAST | 10,240 | 6.6% |
| RETURN_CONST | 10,220 | 6.6% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 300 | 65.2% |
| ENTER_EXECUTOR | 80 | 17.4% |
| GET_ITER | 60 | 13.0% |
| FOR_ITER | 20 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 380 | 82.6% |
| LOAD_FAST | 80 | 17.4% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,922,240 | 100.0% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 6,860,800 | 99.1% |
| RETURN_VALUE | 20,480 | 0.3% |
| LOAD_FAST | 20,480 | 0.3% |
| POP_JUMP_IF_NONE | 20,480 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 20 | 0.0% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,111,860 | 62.6% |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 9,042,360 | 17.6% |
| LOAD_DEREF | 4,739,200 | 9.2% |
| LOAD_ATTR_SLOT | 2,962,300 | 5.8% |
| LOAD_FAST_LOAD_FAST | 1,454,240 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 22,706,160 | 44.2% |
| LOAD_GLOBAL_MODULE | 13,595,980 | 26.5% |
| CALL_PY_EXACT_ARGS | 6,869,780 | 13.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 5,469,020 | 10.7% |
| CALL_PY_WITH_DEFAULTS | 2,028,940 | 4.0% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,689,560 | 98.5% |
| LOAD_ATTR_METHOD_WITH_VALUES | 25,600 | 1.5% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,607,680 | 93.7% |
| LOAD_CONST | 81,900 | 4.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 25,600 | 1.5% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,118,760 | 100.0% |
| LOAD_ATTR | 700 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 634,680 | 29.9% |
| PUSH_NULL | 584,020 | 27.6% |
| LOAD_FAST | 419,720 | 19.8% |
| LOAD_FAST_LOAD_FAST | 307,000 | 14.5% |
| LOAD_ATTR | 92,100 | 4.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,962,420 | 88.5% |
| LOAD_FAST_LOAD_FAST | 1,938,260 | 11.5% |
| LOAD_ATTR | 760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 9,042,360 | 53.5% |
| CALL_PY_EXACT_ARGS | 4,269,440 | 25.3% |
| CONTAINS_OP | 2,092,920 | 12.4% |
| STORE_FAST | 1,402,860 | 8.3% |
| LOAD_FAST | 92,840 | 0.5% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,013,520 | 98.4% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 15,340 | 1.5% |
| LOAD_FAST_LOAD_FAST | 600 | 0.1% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_ATTR | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 962,520 | 93.5% |
| LOAD_FAST | 20,440 | 2.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 15,340 | 1.5% |
| PUSH_NULL | 10,220 | 1.0% |
| LOAD_CONST | 10,220 | 1.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,836,960 | 97.2% |
| LOAD_FAST_LOAD_FAST | 81,880 | 2.8% |
| ENTER_EXECUTOR | 300 | 0.0% |
| LOAD_ATTR | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,919,240 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 212,122,060 | 81.7% |
| COPY | 28,907,840 | 11.1% |
| LOAD_ATTR_SLOT | 17,832,400 | 6.9% |
| LOAD_FAST_LOAD_FAST | 800,120 | 0.3% |
| LOAD_ATTR | 2,200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 112,798,780 | 43.4% |
| COMPARE_OP_INT | 27,076,280 | 10.4% |
| LOAD_CONST | 18,854,100 | 7.3% |
| LOAD_ATTR_SLOT | 17,832,400 | 6.9% |
| TO_BOOL_ALWAYS_TRUE | 17,543,660 | 6.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,038,200 | 56.5% |
| STORE_FAST_STORE_FAST | 1,609,260 | 11.3% |
| LOAD_FAST | 1,504,660 | 10.6% |
| STORE_ATTR_SLOT | 1,433,480 | 10.1% |
| STORE_FAST | 655,940 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,620,880 | 95.7% |
| LOAD_FAST_LOAD_FAST | 450,540 | 3.2% |
| CALL_ISINSTANCE | 91,580 | 0.6% |
| LOAD_GLOBAL_BUILTIN | 40,980 | 0.3% |
| CHECK_EXC_MATCH | 30,700 | 0.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 13,595,980 | 41.8% |
| LOAD_FAST | 9,955,980 | 30.6% |
| RESUME_CHECK | 4,341,600 | 13.3% |
| POP_JUMP_IF_FALSE | 1,484,920 | 4.6% |
| LOAD_ATTR_SLOT | 1,444,040 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 21,423,340 | 65.8% |
| LOAD_FAST | 4,300,760 | 13.2% |
| LOAD_FAST_LOAD_FAST | 2,755,480 | 8.5% |
| LOAD_ATTR_MODULE | 2,118,760 | 6.5% |
| CALL_ISINSTANCE | 1,681,720 | 5.2% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 38,297,520 | 51.3% |
| CALL_PY_WITH_DEFAULTS | 18,708,000 | 25.1% |
| CACHE | 11,938,760 | 16.0% |
| LOAD_ATTR_PROPERTY | 2,919,240 | 3.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,063,400 | 1.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 52,776,920 | 70.7% |
| LOAD_GLOBAL_BUILTIN | 8,038,200 | 10.8% |
| LOAD_GLOBAL_MODULE | 4,341,600 | 5.8% |
| NOP | 4,301,500 | 5.8% |
| LOAD_FAST_LOAD_FAST | 3,021,340 | 4.0% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 50,278,400 | 58.4% |
| SWAP | 28,907,840 | 33.6% |
| LOAD_FAST_LOAD_FAST | 5,913,160 | 6.9% |
| ENTER_EXECUTOR | 858,940 | 1.0% |
| STORE_ATTR_SLOT | 89,540 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 60,498,920 | 70.3% |
| RETURN_CONST | 18,012,280 | 20.9% |
| LOAD_FAST_LOAD_FAST | 2,880,160 | 3.3% |
| LOAD_CONST | 1,791,900 | 2.1% |
| LOAD_GLOBAL_BUILTIN | 1,433,480 | 1.7% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 10,200 | 99.8% |
| STORE_SUBSCR | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,220 | 100.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 17,543,660 | 68.8% |
| LOAD_FAST | 7,804,900 | 30.6% |
| COPY | 126,540 | 0.5% |
| TO_BOOL_NONE | 29,220 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 1,240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 16,528,860 | 64.8% |
| POP_JUMP_IF_FALSE | 8,946,440 | 35.1% |
| TO_BOOL_NONE | 29,200 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 1,240 | 0.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 9,164,880 | 51.8% |
| CALL_ISINSTANCE | 2,418,220 | 13.7% |
| LOAD_FAST | 2,155,340 | 12.2% |
| COPY | 1,576,060 | 8.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,433,480 | 8.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 9,165,920 | 51.8% |
| POP_JUMP_IF_FALSE | 8,326,440 | 47.1% |
| EXTENDED_ARG | 112,500 | 0.6% |
| UNARY_NOT | 61,420 | 0.3% |
| TO_BOOL_NONE | 12,100 | 0.1% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 8,949,680 | 100.0% |
| TO_BOOL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,939,500 | 99.9% |
| EXTENDED_ARG | 10,220 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 40,920 | 67.2% |
| LOAD_FAST | 19,740 | 32.4% |
| TO_BOOL_NONE | 180 | 0.3% |
| TO_BOOL | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 40,940 | 67.2% |
| POP_JUMP_IF_FALSE | 19,760 | 32.5% |
| TO_BOOL_NONE | 180 | 0.3% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 13,989,340 | 69.5% |
| LOAD_FAST | 4,473,860 | 22.2% |
| COPY | 1,266,240 | 6.3% |
| LOAD_ATTR_SLOT | 283,900 | 1.4% |
| LOAD_FAST_CHECK | 61,400 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,216,420 | 80.6% |
| POP_JUMP_IF_TRUE | 3,420,500 | 17.0% |
| EXTENDED_ARG | 440,380 | 2.2% |
| TO_BOOL_ALWAYS_TRUE | 29,220 | 0.1% |
| TO_BOOL_BOOL | 12,140 | 0.1% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 8,939,480 | 75.5% |
| LOAD_FAST | 2,808,540 | 23.7% |
| RETURN_VALUE | 81,880 | 0.7% |
| COPY | 10,200 | 0.1% |
| TO_BOOL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 10,434,800 | 88.1% |
| POP_JUMP_IF_FALSE | 1,405,440 | 11.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,582,580 | 60.6% |
| RETURN_VALUE | 1,679,560 | 39.4% |
| UNPACK_SEQUENCE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 4,262,220 | 100.0% |


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
|     deferred | 440 | 0.0% |
|          hit | 46,762,740 | 100.0% |
|         miss | 60 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
| Failure | 0 | 0.0% |


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
|     deferred | 41,560 | 0.1% |
|          hit | 31,707,300 | 99.9% |
|         miss | 31,300 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 860 | 84.3% |
| Failure | 160 | 15.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 160 | 100.0% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,433,380 | 3.7% |
|          hit | 89,979,820 | 96.3% |
|         miss | 1,948,460 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 42,080 | 95.4% |
| Failure | 2,040 | 4.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bound method | 640 | 31.4% |
| no dict | 540 | 26.5% |
| cfunc noargs | 340 | 16.7% |
| meth descr varargs | 200 | 9.8% |
| code complex parameters | 160 | 7.8% |
| metaclass | 160 | 7.8% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20,359,600 | 38.9% |
|          hit | 31,914,020 | 61.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 6.7% |
| Failure | 6,400 | 93.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 6,320 | 98.8% |
| different types | 80 | 1.2% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,951,480 | 96.9% |
|          hit | 154,840 | 3.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 100 | 4.6% |
| Failure | 2,080 | 95.4% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict items | 960 | 46.2% |
| ascii string | 540 | 26.0% |
| dict keys | 420 | 20.2% |
| enumerate | 160 | 7.7% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 26,482,420 | 7.2% |
|          hit | 339,616,420 | 92.7% |
|         miss | 2,985,800 | 0.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 65,160 | 71.9% |
| Failure | 25,440 | 28.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| metaclass attribute | 21,840 | 85.8% |
| method | 3,260 | 12.8% |
| mutable class | 340 | 1.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,480 | 0.0% |
|          hit | 46,776,740 | 100.0% |
|         miss | 4,240 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,400 | 100.0% |
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
|     deferred | 4,657,500 | 5.4% |
|          hit | 81,302,560 | 94.5% |
|         miss | 4,746,180 | 5.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 90,400 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 20 | 0.2% |
|          hit | 10,220 | 99.6% |

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
|     deferred | 4,412,320 | 5.2% |
|          hit | 79,670,700 | 94.7% |
|         miss | 4,483,100 | 5.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 87,500 | 99.8% |
| Failure | 160 | 0.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 160 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 80 | 0.0% |
|          hit | 4,262,220 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 80 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 802,199,180 | 43.9% |
| Not specialized | 185,833,780 | 10.2% |
| Specialized hits | 825,519,820 | 45.2% |
| Specialized misses | 14,203,340 | 0.8% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 26,482,420 | 41.2% |
| COMPARE_OP | 20,359,600 | 31.6% |
| FOR_ITER | 4,951,480 | 7.7% |
| STORE_ATTR | 4,657,500 | 7.2% |
| TO_BOOL | 4,412,320 | 6.9% |
| CALL | 3,433,380 | 5.3% |
| BINARY_SUBSCR | 41,560 | 0.1% |
| LOAD_GLOBAL | 7,480 | 0.0% |
| BINARY_OP | 440 | 0.0% |
| UNPACK_SEQUENCE | 80 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 4,746,180 | 33.4% |
| TO_BOOL_NONE | 2,212,000 | 15.6% |
| TO_BOOL_ALWAYS_TRUE | 1,616,420 | 11.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,357,340 | 9.6% |
| CALL_PY_EXACT_ARGS | 999,320 | 7.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 949,140 | 6.7% |
| LOAD_ATTR_SLOT | 814,380 | 5.7% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 813,980 | 5.7% |
| TO_BOOL_BOOL | 645,140 | 4.5% |
| BINARY_SUBSCR_LIST_INT | 31,300 | 0.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 11,939,020 | 16.0% |
| Calls to Python functions inlined | 62,734,080 | 84.0% |
| Calls via PyEval_EvalFrame (total) | 11,939,020 | 16.0% |
| Calls via PyEval_EvalFrame (vector) | 11,939,020 | 16.0% |
| Calls via PyEval_EvalFrame (generator) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 11,939,020 | 16.0% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 1,126,420 | 1.5% |
| Calls via PyEval_EvalFrame (function ex) | 160 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 7,679,160 | 10.3% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 30,720 | 0.0% |
| Frames pushed | 62,524,400 | 83.7% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 15,950,720 | 20.3% |
| Frees to freelist | 15,954,580 |  |
| Allocations | 62,486,920 | 79.7% |
| Allocations to 512 bytes | 62,486,480 | 79.7% |
| Allocations to 4 kbytes | 440 | 0.0% |
| Allocations over 4 kbytes | 0 | 0.0% |
| Frees | 62,210,476 |  |
| New values | 1,617,920 |  |
| Interpreter increfs | 1,089,137,600 | 89.3% |
| Interpreter decrefs | 1,182,212,780 | 91.4% |
| Increfs | 130,932,617 | 10.7% |
| Decrefs | 111,763,519 | 8.6% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 63,296,609 |  |
| Method cache misses | 670,211 |  |
| Method cache collisions | 782,577 |  |
| Method cache dunder hits | 20,131,154 |  |
| Method cache dunder misses | 113,426 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 4,000 | 1,314,540 | 23,025,040 |
| 1 | 360 | 1,052,940 | 8,849,640 |
| 2 | 20 | 39,360 | 4,255,920 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 740 |  |
| Traces created | 1,160 | 156.8% |
| Trace stack overflow | 260 | 35.1% |
| Trace stack underflow | 660 | 89.2% |
| Trace too long | 0 | 0.0% |
| Trace too short | 540,300 | 73,013.5% |
| Inner loop found | 27,020 | 3,651.4% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 2.7% |
| Traces executed | 56,793,440 |  |
| Uops executed | 753,210,620 | 13.26 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 20 | 1.7% |
| <= 16 | 240 | 20.7% |
| <= 32 | 200 | 17.2% |
| <= 64 | 300 | 25.9% |
| <= 128 | 220 | 19.0% |
| <= 256 | 100 | 8.6% |
| <= 512 | 80 | 6.9% |


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
| <= 256 | 160 | 13.8% |
| <= 512 | 300 | 25.9% |
| <= 1,024 | 160 | 13.8% |
| <= 2,048 | 120 | 10.3% |
| <= 4,096 | 20 | 1.7% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 1,105,160 | 1.9% |
| <= 4 | 3,939,920 | 6.9% |
| <= 8 | 5,544,320 | 9.8% |
| <= 16 | 15,795,520 | 27.8% |
| <= 32 | 9,373,600 | 16.5% |
| <= 64 | 3,581,120 | 6.3% |
| <= 128 | 71,320 | 0.1% |
| <= 256 | 81,680 | 0.1% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 122,905,000 | 16.3% | 16.3% |  |
| _SET_IP | 88,333,240 | 11.7% | 28.0% |  |
| _CHECK_VALIDITY | 76,816,460 | 10.2% | 38.2% |  |
| _GUARD_TYPE_VERSION | 76,452,320 | 10.2% | 48.4% | 4.8% |
| _START_EXECUTOR | 39,492,640 | 5.2% | 53.6% |  |
| STORE_FAST | 31,523,800 | 4.2% | 57.8% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 27,912,780 | 3.7% | 61.5% |  |
| _EXIT_TRACE | 26,079,140 | 3.5% | 65.0% | 100.0% |
| _LOAD_ATTR_SLOT | 25,728,060 | 3.4% | 68.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 19,824,400 | 2.6% | 71.0% |  |
| _GUARD_IS_TRUE_POP | 19,771,200 | 2.6% | 73.7% | 17.5% |
| _GUARD_IS_FALSE_POP | 17,680,420 | 2.3% | 76.0% | 7.8% |
| _COLD_EXIT | 17,300,800 | 2.3% | 78.3% |  |
| _FOR_ITER_TIER_TWO | 11,125,420 | 1.5% | 79.8% | 41.8% |
| _LOAD_CONST_INLINE_BORROW | 10,865,600 | 1.4% | 81.2% |  |
| _STORE_ATTR_SLOT | 10,615,140 | 1.4% | 82.6% |  |
| CONTAINS_OP | 10,029,760 | 1.3% | 84.0% |  |
| TO_BOOL_BOOL | 9,996,620 | 1.3% | 85.3% |  |
| _LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 8,452,040 | 1.1% | 86.4% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 8,075,760 | 1.1% | 87.5% |  |
| _LOAD_ATTR | 7,397,920 | 1.0% | 88.5% |  |
| TO_BOOL_STR | 7,134,340 | 0.9% | 89.4% |  |
| _CHECK_GLOBALS | 6,600,060 | 0.9% | 90.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,250,660 | 0.7% | 91.0% |  |
| _LOAD_CONST_INLINE | 4,633,540 | 0.6% | 91.6% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 4,183,420 | 0.6% | 92.2% |  |
| COMPARE_OP_INT | 3,722,920 | 0.5% | 92.7% |  |
| CALL_ISINSTANCE | 3,694,740 | 0.5% | 93.1% |  |
| _GUARD_BOTH_INT | 3,507,220 | 0.5% | 93.6% |  |
| _COMPARE_OP | 3,059,740 | 0.4% | 94.0% |  |
| RESUME_CHECK | 2,680,020 | 0.4% | 94.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,680,020 | 0.4% | 94.7% |  |
| _CHECK_STACK_SPACE | 2,680,020 | 0.4% | 95.1% |  |
| _INIT_CALL_PY_EXACT_ARGS | 2,680,020 | 0.4% | 95.4% |  |
| _PUSH_FRAME | 2,680,020 | 0.4% | 95.8% |  |
| _SAVE_RETURN_OFFSET | 2,680,020 | 0.4% | 96.2% |  |
| _CHECK_BUILTINS | 2,640,880 | 0.4% | 96.5% |  |
| _BINARY_OP_ADD_INT | 2,331,520 | 0.3% | 96.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,923,860 | 0.3% | 97.1% |  |
| BINARY_SUBSCR_DICT | 1,604,980 | 0.2% | 97.3% |  |
| _BINARY_OP | 1,574,720 | 0.2% | 97.5% |  |
| COMPARE_OP_STR | 1,554,280 | 0.2% | 97.7% |  |
| _POP_FRAME | 1,462,880 | 0.2% | 97.9% |  |
| TO_BOOL_NONE | 1,462,800 | 0.2% | 98.1% | 5.6% |
| _BINARY_SUBSCR | 1,392,320 | 0.2% | 98.3% |  |
| BINARY_SUBSCR_STR_INT | 1,226,960 | 0.2% | 98.4% |  |
| GET_ITER | 1,206,980 | 0.2% | 98.6% |  |
| _JUMP_TO_TOP | 1,176,400 | 0.2% | 98.8% |  |
| _BINARY_OP_SUBTRACT_INT | 1,175,700 | 0.2% | 98.9% |  |
| BUILD_LIST | 1,156,160 | 0.2% | 99.1% |  |
| _GUARD_IS_NOT_NONE_POP | 1,156,160 | 0.2% | 99.2% |  |
| SWAP | 972,040 | 0.1% | 99.3% |  |
| _STORE_ATTR | 930,080 | 0.1% | 99.5% |  |
| POP_TOP | 910,840 | 0.1% | 99.6% |  |
| BUILD_TUPLE | 849,640 | 0.1% | 99.7% |  |
| _LOAD_GLOBAL | 738,920 | 0.1% | 99.8% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 335,940 | 0.0% | 99.8% | 36.2% |
| _ITER_CHECK_LIST | 335,940 | 0.0% | 99.9% |  |
| _ITER_NEXT_LIST | 214,180 | 0.0% | 99.9% |  |
| COPY | 122,400 | 0.0% | 99.9% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 81,880 | 0.0% | 99.9% |  |
| _GUARD_KEYS_VERSION | 81,880 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 81,880 | 0.0% | 100.0% |  |
| _TO_BOOL | 81,620 | 0.0% | 100.0% |  |
| CALL_LEN | 61,200 | 0.0% | 100.0% |  |
| _GUARD_IS_NONE_POP | 61,100 | 0.0% | 100.0% | 100.0% |
| _GUARD_NOT_EXHAUSTED_RANGE | 9,920 | 0.0% | 100.0% | 0.8% |
| _ITER_CHECK_RANGE | 9,920 | 0.0% | 100.0% |  |
| PUSH_NULL | 9,840 | 0.0% | 100.0% |  |
| _CHECK_ATTR_MODULE | 9,840 | 0.0% | 100.0% |  |
| _LOAD_ATTR_MODULE | 9,840 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 9,840 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 510,980 |
| BINARY_OP_INPLACE_ADD_UNICODE | 2,000 |
| CALL_PY_WITH_DEFAULTS | 140 |
| CALL_LIST_APPEND | 40 |
| LOAD_ATTR_PROPERTY | 40 |


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
