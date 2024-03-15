
# Pystats results

- benchmark: pycparser
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,860,468,640 | 28.5% | 28.5% |  |
| LOAD_CONST | 545,585,500 | 8.3% | 36.8% |  |
| STORE_FAST | 341,122,840 | 5.2% | 42.0% |  |
| LOAD_ATTR_INSTANCE_VALUE | 292,539,440 | 4.5% | 46.5% | 3.9% |
| STORE_ATTR_INSTANCE_VALUE | 261,221,440 | 4.0% | 50.5% | 0.0% |
| POP_JUMP_IF_FALSE | 223,897,020 | 3.4% | 53.9% |  |
| RESUME_CHECK | 190,729,900 | 2.9% | 56.8% | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 149,659,720 | 2.3% | 59.1% |  |
| LOAD_GLOBAL_BUILTIN | 143,046,140 | 2.2% | 61.3% | 0.0% |
| BINARY_SUBSCR_LIST_INT | 135,248,520 | 2.1% | 63.4% | 0.0% |
| LOAD_FAST_LOAD_FAST | 134,316,000 | 2.1% | 65.4% |  |
| UNARY_NEGATIVE | 124,482,300 | 1.9% | 67.3% |  |
| RETURN_VALUE | 118,974,660 | 1.8% | 69.1% |  |
| COMPARE_OP_INT | 112,041,000 | 1.7% | 70.9% |  |
| CALL | 109,142,740 | 1.7% | 72.5% |  |
| CALL_LIST_APPEND | 94,016,380 | 1.4% | 74.0% |  |
| RETURN_CONST | 92,571,800 | 1.4% | 75.4% |  |
| ENTER_EXECUTOR | 91,674,440 | 1.4% | 76.8% |  |
| BINARY_SUBSCR_DICT | 82,149,480 | 1.3% | 78.0% |  |
| POP_JUMP_IF_TRUE | 77,977,700 | 1.2% | 79.2% |  |
| BUILD_SLICE | 69,799,540 | 1.1% | 80.3% |  |
| DELETE_SUBSCR | 69,798,760 | 1.1% | 81.4% |  |
| TO_BOOL_BOOL | 62,248,380 | 1.0% | 82.3% | 0.0% |
| INTERPRETER_EXIT | 61,296,160 | 0.9% | 83.2% |  |
| POP_TOP | 54,070,020 | 0.8% | 84.1% |  |
| CALL_PY_EXACT_ARGS | 53,524,380 | 0.8% | 84.9% | 37.6% |
| LOAD_GLOBAL_MODULE | 52,653,240 | 0.8% | 85.7% | 0.0% |
| CALL_ISINSTANCE | 51,790,860 | 0.8% | 86.5% |  |
| BINARY_SUBSCR_GETITEM | 47,356,660 | 0.7% | 87.2% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 46,804,720 | 0.7% | 87.9% |  |
| STORE_ATTR_SLOT | 46,355,940 | 0.7% | 88.6% | 0.5% |
| TO_BOOL_INT | 46,103,720 | 0.7% | 89.3% | 0.0% |
| BINARY_OP_SUBTRACT_INT | 40,172,360 | 0.6% | 90.0% |  |
| JUMP_FORWARD | 38,653,220 | 0.6% | 90.6% |  |
| TO_BOOL_NONE | 36,923,440 | 0.6% | 91.1% | 38.5% |
| BINARY_SUBSCR | 35,950,820 | 0.5% | 91.7% |  |
| NOP | 35,733,340 | 0.5% | 92.2% |  |
| STORE_SUBSCR | 35,730,160 | 0.5% | 92.8% |  |
| BINARY_SLICE | 35,467,060 | 0.5% | 93.3% |  |
| STORE_SUBSCR_LIST_INT | 34,913,100 | 0.5% | 93.8% |  |
| LOAD_ATTR | 34,224,800 | 0.5% | 94.4% |  |
| LOAD_ATTR_WITH_HINT | 34,205,420 | 0.5% | 94.9% | 0.3% |
| EXTENDED_ARG | 28,252,640 | 0.4% | 95.3% |  |
| TO_BOOL_ALWAYS_TRUE | 28,056,640 | 0.4% | 95.7% | 33.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 27,199,140 | 0.4% | 96.2% | 70.3% |
| POP_JUMP_IF_NONE | 26,296,360 | 0.4% | 96.6% |  |
| CALL_LEN | 22,070,380 | 0.3% | 96.9% |  |
| PUSH_NULL | 17,210,420 | 0.3% | 97.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 16,814,080 | 0.3% | 97.4% | 0.0% |
| CALL_BUILTIN_FAST | 16,389,540 | 0.3% | 97.7% | 0.0% |
| LOAD_ATTR_MODULE | 14,889,740 | 0.2% | 97.9% | 0.0% |
| SWAP | 14,478,980 | 0.2% | 98.1% |  |
| STORE_FAST_LOAD_FAST | 13,933,680 | 0.2% | 98.3% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,336,500 | 0.2% | 98.5% |  |
| CALL_KW | 11,793,080 | 0.2% | 98.7% |  |
| STORE_ATTR_WITH_HINT | 10,701,900 | 0.2% | 98.9% | 0.0% |
| BUILD_LIST | 9,217,600 | 0.1% | 99.0% |  |
| LOAD_ATTR_SLOT | 7,312,640 | 0.1% | 99.1% | 17.6% |
| GET_ITER | 5,520,740 | 0.1% | 99.2% |  |
| TO_BOOL_STR | 5,399,840 | 0.1% | 99.3% | 0.0% |
| POP_JUMP_IF_NOT_NONE | 5,236,600 | 0.1% | 99.4% |  |
| FOR_ITER_LIST | 5,204,560 | 0.1% | 99.4% | 0.0% |
| COMPARE_OP_STR | 4,307,100 | 0.1% | 99.5% | 0.0% |
| TO_BOOL | 4,073,380 | 0.1% | 99.6% |  |
| FOR_ITER | 3,523,760 | 0.1% | 99.6% |  |
| COPY | 3,506,140 | 0.1% | 99.7% |  |
| CALL_BUILTIN_CLASS | 3,249,180 | 0.0% | 99.7% |  |
| CONTAINS_OP | 2,016,420 | 0.0% | 99.8% |  |
| BINARY_OP | 1,793,000 | 0.0% | 99.8% |  |
| LOAD_FAST_AND_CLEAR | 1,672,100 | 0.0% | 99.8% |  |
| BINARY_OP_ADD_INT | 1,630,560 | 0.0% | 99.8% |  |
| LOAD_DEREF | 1,456,160 | 0.0% | 99.9% |  |
| COPY_FREE_VARS | 1,455,840 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 1,448,140 | 0.0% | 99.9% |  |
| TO_BOOL_LIST | 1,338,900 | 0.0% | 99.9% | 0.1% |
| BINARY_OP_ADD_UNICODE | 1,111,080 | 0.0% | 99.9% |  |
| CALL_PY_WITH_DEFAULTS | 897,380 | 0.0% | 100.0% |  |
| LIST_APPEND | 841,600 | 0.0% | 100.0% |  |
| COMPARE_OP | 548,360 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 226,300 | 0.0% | 100.0% | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 208,720 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 128,280 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 121,960 | 0.0% | 100.0% |  |
| STORE_FAST_STORE_FAST | 86,760 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 82,440 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 82,440 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 74,920 | 0.0% | 100.0% |  |
| IS_OP | 62,120 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 58,380 | 0.0% | 100.0% |  |
| LOAD_ATTR_PROPERTY | 45,180 | 0.0% | 100.0% |  |
| BUILD_STRING | 41,220 | 0.0% | 100.0% |  |
| CALL_STR_1 | 40,660 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 39,140 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 37,380 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 28,880 | 0.0% | 100.0% | 0.4% |
| LOAD_NAME | 18,420 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 14,700 | 0.0% | 100.0% | 1.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 14,140 | 0.0% | 100.0% |  |
| STORE_ATTR | 13,940 | 0.0% | 100.0% |  |
| STORE_NAME | 11,260 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 11,220 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 10,920 | 0.0% | 100.0% |  |
| UNARY_NOT | 8,600 | 0.0% | 100.0% |  |
| LIST_EXTEND | 7,220 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 6,740 | 0.0% | 100.0% |  |
| BUILD_MAP | 6,360 | 0.0% | 100.0% |  |
| RESUME | 5,580 | 0.0% | 100.0% | 60.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,520 | 0.0% | 100.0% |  |
| UNARY_INVERT | 4,160 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 4,100 | 0.0% | 100.0% |  |
| MAP_ADD | 3,400 | 0.0% | 100.0% |  |
| EXIT_INIT_CHECK | 3,360 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 3,360 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 2,280 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 1,940 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 960 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 800 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 660 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 640 | 0.0% | 100.0% |  |
| BEFORE_WITH | 600 | 0.0% | 100.0% |  |
| IMPORT_NAME | 480 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 400 | 0.0% | 100.0% |  |
| POP_EXCEPT | 400 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 400 | 0.0% | 100.0% |  |
| DICT_MERGE | 360 | 0.0% | 100.0% |  |
| YIELD_VALUE | 320 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 320 | 0.0% | 100.0% |  |
| BINARY_OP_INPLACE_ADD_UNICODE | 240 | 0.0% | 100.0% |  |
| DICT_UPDATE | 200 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 160 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 120 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 120 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 0.0% | 100.0% |  |
| MAKE_CELL | 80 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| DELETE_NAME | 40 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_FAST | 312,882,920 | 4.8% | 4.8% |
| LOAD_FAST LOAD_CONST | 270,360,320 | 4.1% | 8.9% |
| STORE_FAST LOAD_FAST | 257,640,600 | 3.9% | 12.9% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 201,516,920 | 3.1% | 15.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 199,577,780 | 3.1% | 19.0% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 177,760,920 | 2.7% | 21.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 149,719,540 | 2.3% | 24.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 125,317,220 | 1.9% | 25.9% |
| LOAD_FAST UNARY_NEGATIVE | 124,482,300 | 1.9% | 27.8% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 116,142,900 | 1.8% | 29.6% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 111,089,860 | 1.7% | 31.3% |
| LOAD_CONST COMPARE_OP_INT | 110,156,640 | 1.7% | 33.0% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 109,960,020 | 1.7% | 34.7% |
| UNARY_NEGATIVE LOAD_CONST | 104,698,080 | 1.6% | 36.3% |
| LOAD_FAST BINARY_SUBSCR_LIST_INT | 99,728,960 | 1.5% | 37.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 93,817,820 | 1.4% | 39.2% |
| CALL STORE_FAST | 90,457,240 | 1.4% | 40.6% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 88,527,780 | 1.4% | 42.0% |
| LOAD_FAST CALL_LIST_APPEND | 82,656,280 | 1.3% | 43.2% |
| LOAD_CONST BUILD_SLICE | 69,799,540 | 1.1% | 44.3% |
| DELETE_SUBSCR LOAD_FAST | 69,798,720 | 1.1% | 45.4% |
| BUILD_SLICE DELETE_SUBSCR | 69,798,720 | 1.1% | 46.4% |
| CACHE RESUME_CHECK | 61,303,780 | 0.9% | 47.4% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 55,023,440 | 0.8% | 48.2% |
| RETURN_VALUE LOAD_FAST | 53,515,300 | 0.8% | 49.0% |
| ENTER_EXECUTOR CALL | 52,590,400 | 0.8% | 49.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 52,442,500 | 0.8% | 50.6% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 51,749,200 | 0.8% | 51.4% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 50,954,380 | 0.8% | 52.2% |
| RETURN_CONST INTERPRETER_EXIT | 50,367,520 | 0.8% | 53.0% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 48,141,620 | 0.7% | 53.7% |
| LOAD_CONST LOAD_FAST | 48,133,940 | 0.7% | 54.4% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 48,122,700 | 0.7% | 55.2% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 47,610,460 | 0.7% | 55.9% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 47,407,520 | 0.7% | 56.6% |
| BINARY_SUBSCR_GETITEM RESUME_CHECK | 47,356,660 | 0.7% | 57.4% |
| BINARY_SUBSCR_LIST_INT LOAD_ATTR_INSTANCE_VALUE | 47,352,760 | 0.7% | 58.1% |
| LOAD_CONST BINARY_SUBSCR_GETITEM | 47,350,940 | 0.7% | 58.8% |
| CALL_LIST_APPEND LOAD_FAST | 46,819,340 | 0.7% | 59.5% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 46,090,460 | 0.7% | 60.2% |
| LOAD_FAST TO_BOOL_INT | 46,078,460 | 0.7% | 60.9% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 45,451,720 | 0.7% | 61.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 43,186,440 | 0.7% | 62.3% |
| LOAD_FAST BINARY_SUBSCR_DICT | 40,726,500 | 0.6% | 62.9% |
| RETURN_CONST POP_TOP | 39,125,100 | 0.6% | 63.5% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 37,952,900 | 0.6% | 64.1% |
| RESUME_CHECK LOAD_FAST | 37,734,560 | 0.6% | 64.7% |
| POP_TOP LOAD_FAST | 37,564,020 | 0.6% | 65.2% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 36,564,480 | 0.6% | 65.8% |
| BINARY_SUBSCR_DICT STORE_FAST | 36,504,720 | 0.6% | 66.4% |
| JUMP_FORWARD LOAD_FAST | 36,408,780 | 0.6% | 66.9% |
| BINARY_SUBSCR_DICT LOAD_FAST | 36,358,400 | 0.6% | 67.5% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 36,306,160 | 0.6% | 68.0% |
| BINARY_SUBSCR_LIST_INT STORE_ATTR_INSTANCE_VALUE | 36,129,520 | 0.6% | 68.6% |
| TO_BOOL_NONE POP_JUMP_IF_TRUE | 36,102,820 | 0.6% | 69.1% |
| LOAD_CONST BINARY_SUBSCR | 35,936,360 | 0.5% | 69.7% |
| STORE_FAST JUMP_FORWARD | 35,891,560 | 0.5% | 70.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_CONST | 35,783,280 | 0.5% | 70.8% |
| NOP LOAD_FAST | 35,725,400 | 0.5% | 71.3% |
| LOAD_CONST STORE_SUBSCR | 35,697,940 | 0.5% | 71.9% |
| BINARY_SUBSCR BINARY_SUBSCR_DICT | 35,692,480 | 0.5% | 72.4% |
| STORE_ATTR_INSTANCE_VALUE NOP | 35,691,440 | 0.5% | 73.0% |
| LOAD_CONST BINARY_SLICE | 35,465,540 | 0.5% | 73.5% |
| STORE_SUBSCR RETURN_CONST | 35,259,660 | 0.5% | 74.0% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 35,046,940 | 0.5% | 74.6% |
| BINARY_OP_SUBTRACT_INT LOAD_CONST | 34,905,460 | 0.5% | 75.1% |
| LOAD_CONST BINARY_OP_SUBTRACT_INT | 34,904,040 | 0.5% | 75.6% |
| BINARY_SLICE STORE_FAST | 34,902,100 | 0.5% | 76.2% |
| STORE_SUBSCR_LIST_INT LOAD_FAST | 34,899,660 | 0.5% | 76.7% |
| LOAD_CONST STORE_SUBSCR_LIST_INT | 34,899,320 | 0.5% | 77.2% |
| LOAD_FAST TO_BOOL_NONE | 34,607,760 | 0.5% | 77.8% |
| LOAD_FAST LOAD_ATTR | 33,974,820 | 0.5% | 78.3% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 33,420,240 | 0.5% | 78.8% |
| POP_JUMP_IF_TRUE LOAD_FAST | 32,405,800 | 0.5% | 79.3% |
| LOAD_GLOBAL_MODULE CALL | 32,033,600 | 0.5% | 79.8% |
| POP_JUMP_IF_TRUE ENTER_EXECUTOR | 30,545,920 | 0.5% | 80.3% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 30,350,540 | 0.5% | 80.7% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 29,042,580 | 0.4% | 81.2% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_TRUE | 27,756,380 | 0.4% | 81.6% |
| LOAD_FAST TO_BOOL_ALWAYS_TRUE | 27,603,220 | 0.4% | 82.0% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 26,470,120 | 0.4% | 82.4% |
| POP_JUMP_IF_NONE LOAD_FAST | 26,266,200 | 0.4% | 82.8% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 26,082,580 | 0.4% | 83.2% |
| EXTENDED_ARG POP_JUMP_IF_NONE | 25,433,000 | 0.4% | 83.6% |
| LOAD_FAST EXTENDED_ARG | 25,433,000 | 0.4% | 84.0% |
| LOAD_CONST LOAD_CONST | 24,274,320 | 0.4% | 84.4% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 23,522,700 | 0.4% | 84.7% |
| LOAD_FAST CALL_BOUND_METHOD_EXACT_ARGS | 23,427,940 | 0.4% | 85.1% |
| STORE_FAST LOAD_GLOBAL_MODULE | 21,242,880 | 0.3% | 85.4% |
| ENTER_EXECUTOR LOAD_ATTR_METHOD_NO_DICT | 20,493,180 | 0.3% | 85.7% |
| BINARY_SUBSCR_LIST_INT STORE_FAST | 19,817,580 | 0.3% | 86.0% |
| UNARY_NEGATIVE BINARY_SUBSCR_LIST_INT | 19,783,360 | 0.3% | 86.3% |
| RETURN_VALUE STORE_FAST | 19,652,440 | 0.3% | 86.6% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 19,595,300 | 0.3% | 86.9% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 18,153,860 | 0.3% | 87.2% |
| BINARY_SUBSCR_LIST_INT LOAD_CONST | 18,003,960 | 0.3% | 87.5% |
| CALL LOAD_FAST | 16,979,920 | 0.3% | 87.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 16,675,360 | 0.3% | 88.0% |
| LOAD_CONST CALL_BUILTIN_FAST | 16,340,400 | 0.2% | 88.2% |
| CALL_BUILTIN_FAST RETURN_VALUE | 16,202,040 | 0.2% | 88.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,465,540 | 100.0% |
| LOAD_FAST | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 34,902,100 | 98.4% |
| GET_ITER | 540,640 | 1.5% |
| LOAD_FAST | 7,040 | 0.0% |
| BINARY_OP_ADD_UNICODE | 6,760 | 0.0% |
| LOAD_CONST | 5,420 | 0.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 61,303,780 | 100.0% |
| RESUME | 1,800 | 0.0% |
| POP_TOP | 160 | 0.0% |
| COPY_FREE_VARS | 120 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 260 | 43.3% |
| CALL | 180 | 30.0% |
| RETURN_VALUE | 80 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 320 | 53.3% |
| STORE_FAST | 280 | 46.7% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 240 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 240 | 100.0% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,936,360 | 100.0% |
| BINARY_SUBSCR | 10,800 | 0.0% |
| LOAD_FAST | 2,420 | 0.0% |
| BUILD_SLICE | 820 | 0.0% |
| LOAD_FAST_LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 35,692,480 | 99.3% |
| LOAD_FAST | 109,720 | 0.3% |
| LOAD_ATTR_METHOD_NO_DICT | 102,100 | 0.3% |
| STORE_FAST | 17,500 | 0.0% |
| BINARY_SUBSCR | 10,800 | 0.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 400 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 69,798,720 | 100.0% |
| LOAD_FAST | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 69,798,720 | 100.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,360 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 82,440 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 81,780 | 99.2% |
| BUILD_STRING | 660 | 0.8% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 2,951,280 | 53.5% |
| LOAD_FAST | 1,136,540 | 20.6% |
| LOAD_ATTR_SLOT | 868,920 | 15.7% |
| BINARY_SLICE | 540,640 | 9.8% |
| LOAD_ATTR_INSTANCE_VALUE | 12,620 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 3,497,620 | 63.4% |
| FOR_ITER_LIST | 888,000 | 16.1% |
| LOAD_FAST_AND_CLEAR | 837,060 | 15.2% |
| EXTENDED_ARG | 280,540 | 5.1% |
| FOR_ITER_TUPLE | 16,960 | 0.3% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 50,367,520 | 82.2% |
| RETURN_VALUE | 10,928,320 | 17.8% |
| YIELD_VALUE | 320 | 0.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,940 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,160 | 59.8% |
| STORE_FAST | 660 | 34.0% |
| SET_FUNCTION_ATTRIBUTE | 120 | 6.2% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 35,691,440 | 99.9% |
| STORE_FAST | 29,380 | 0.1% |
| NOP | 2,980 | 0.0% |
| STORE_FAST_STORE_FAST | 2,980 | 0.0% |
| POP_JUMP_IF_FALSE | 2,740 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 35,725,400 | 100.0% |
| NOP | 2,980 | 0.0% |
| LOAD_GLOBAL_MODULE | 2,600 | 0.0% |
| LOAD_CONST | 1,280 | 0.0% |
| BUILD_LIST | 580 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 160 | 40.0% |
| STORE_ATTR_INSTANCE_VALUE | 160 | 40.0% |
| STORE_FAST | 80 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 160 | 40.0% |
| RETURN_CONST | 160 | 40.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 20.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 39,125,100 | 72.4% |
| SWAP | 10,375,560 | 19.2% |
| STORE_FAST | 1,875,120 | 3.5% |
| POP_JUMP_IF_TRUE | 1,329,600 | 2.5% |
| CALL_METHOD_DESCRIPTOR_FAST | 1,068,160 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,564,020 | 69.5% |
| RETURN_VALUE | 10,375,640 | 19.2% |
| RETURN_CONST | 2,615,280 | 4.8% |
| EXTENDED_ARG | 1,883,740 | 3.5% |
| LOAD_GLOBAL_BUILTIN | 846,760 | 1.6% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 240 | 60.0% |
| BINARY_SUBSCR_STR_INT | 160 | 40.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 400 | 100.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 8,750,860 | 50.8% |
| LOAD_FAST | 6,992,900 | 40.6% |
| LOAD_DEREF | 1,455,760 | 8.5% |
| STORE_FAST_LOAD_FAST | 8,640 | 0.1% |
| LOAD_ATTR | 1,520 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,930,720 | 86.8% |
| LOAD_FAST_LOAD_FAST | 1,461,520 | 8.5% |
| LOAD_CONST | 729,600 | 4.2% |
| LOAD_GLOBAL_BUILTIN | 46,720 | 0.3% |
| LOAD_GLOBAL_MODULE | 28,420 | 0.2% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 80 | 50.0% |
| CALL_PY_WITH_DEFAULTS | 60 | 37.5% |
| CALL | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 50.0% |
| CALL | 40 | 25.0% |
| CALL_BUILTIN_CLASS | 40 | 25.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 47,407,520 | 39.8% |
| CALL_BUILTIN_FAST | 16,202,040 | 13.6% |
| LOAD_FAST | 10,958,980 | 9.2% |
| CALL_LEN | 10,811,840 | 9.1% |
| LOAD_ATTR_WITH_HINT | 10,541,800 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 53,515,300 | 45.0% |
| STORE_FAST | 19,652,440 | 16.5% |
| INTERPRETER_EXIT | 10,928,320 | 9.2% |
| CALL | 8,213,620 | 6.9% |
| LOAD_CONST | 6,205,760 | 5.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 35,697,940 | 99.9% |
| STORE_SUBSCR | 29,380 | 0.1% |
| LOAD_FAST | 2,260 | 0.0% |
| LOAD_FAST_LOAD_FAST | 420 | 0.0% |
| LOAD_NAME | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 35,259,660 | 98.7% |
| LOAD_FAST | 438,180 | 1.2% |
| STORE_SUBSCR | 29,380 | 0.1% |
| EXTENDED_ARG | 1,800 | 0.0% |
| ENTER_EXECUTOR | 420 | 0.0% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,895,220 | 95.6% |
| TO_BOOL_NONE | 88,840 | 2.2% |
| TO_BOOL | 79,620 | 2.0% |
| COPY | 6,300 | 0.2% |
| LOAD_ATTR_INSTANCE_VALUE | 840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 3,897,260 | 95.7% |
| TO_BOOL_NONE | 89,140 | 2.2% |
| TO_BOOL | 79,620 | 2.0% |
| POP_JUMP_IF_FALSE | 5,520 | 0.1% |
| TO_BOOL_BOOL | 1,100 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 4,160 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 124,482,300 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 104,698,080 | 84.1% |
| BINARY_SUBSCR_LIST_INT | 19,783,360 | 15.9% |
| CALL_BUILTIN_CLASS | 820 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 8,440 | 98.1% |
| TO_BOOL_LIST | 160 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 4,320 | 50.2% |
| STORE_FAST | 4,120 | 47.9% |
| CALL_PY_EXACT_ARGS | 160 | 1.9% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,082,900 | 60.4% |
| RETURN_VALUE | 541,760 | 30.2% |
| POP_JUMP_IF_TRUE | 105,360 | 5.9% |
| BUILD_LIST | 23,600 | 1.3% |
| LOAD_GLOBAL_MODULE | 20,460 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 652,300 | 36.4% |
| LOAD_CONST | 540,860 | 30.2% |
| BINARY_OP_ADD_UNICODE | 540,700 | 30.2% |
| JUMP_FORWARD | 23,600 | 1.3% |
| TO_BOOL_INT | 22,840 | 1.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 121,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 121,760 | 99.8% |
| STORE_NAME | 80 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |
| DICT_UPDATE | 40 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 2,543,520 | 27.6% |
| RETURN_VALUE | 2,393,680 | 26.0% |
| LOAD_GLOBAL_BUILTIN | 846,380 | 9.2% |
| SWAP | 837,060 | 9.1% |
| LOAD_FAST | 811,520 | 8.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 2,543,520 | 27.6% |
| LOAD_FAST | 2,389,000 | 25.9% |
| LOAD_CONST | 1,445,800 | 15.7% |
| STORE_FAST | 1,430,060 | 15.5% |
| SWAP | 837,060 | 9.1% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 3,180 | 50.0% |
| POP_JUMP_IF_FALSE | 860 | 13.5% |
| LOAD_CONST | 480 | 7.5% |
| FOR_ITER | 340 | 5.3% |
| LOAD_FAST | 320 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,000 | 78.6% |
| LOAD_NAME | 860 | 13.5% |
| STORE_FAST | 240 | 3.8% |
| LOAD_CONST | 120 | 1.9% |
| EXTENDED_ARG | 80 | 1.3% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 69,799,540 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 69,798,720 | 100.0% |
| BINARY_SUBSCR | 820 | 0.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40,560 | 98.4% |
| FORMAT_SIMPLE | 660 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40,560 | 98.4% |
| LOAD_FAST | 660 | 1.6% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,251,800 | 86.4% |
| LOAD_ATTR | 81,220 | 5.6% |
| BINARY_SUBSCR_TUPLE_INT | 41,020 | 2.8% |
| LOAD_FAST_LOAD_FAST | 25,400 | 1.8% |
| LOAD_FAST | 17,460 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 1,285,700 | 88.8% |
| CALL_LIST_APPEND | 66,180 | 4.6% |
| RETURN_VALUE | 48,620 | 3.4% |
| LOAD_FAST | 11,640 | 0.8% |
| STORE_FAST | 8,780 | 0.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 52,590,400 | 48.2% |
| LOAD_GLOBAL_MODULE | 32,033,600 | 29.4% |
| LOAD_ATTR_METHOD_NO_DICT | 12,249,680 | 11.2% |
| RETURN_VALUE | 8,213,620 | 7.5% |
| LOAD_ATTR_SLOT | 2,151,120 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 90,457,240 | 82.9% |
| LOAD_FAST | 16,979,920 | 15.6% |
| BINARY_OP_ADD_INT | 1,592,840 | 1.5% |
| TO_BOOL_BOOL | 54,320 | 0.0% |
| CALL | 36,020 | 0.0% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 72,060 | 96.2% |
| LOAD_FAST | 2,280 | 3.0% |
| DICT_MERGE | 360 | 0.5% |
| JUMP_BACKWARD | 140 | 0.2% |
| CALL_INTRINSIC_1 | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 74,360 | 99.3% |
| RESUME_CHECK | 320 | 0.4% |
| RETURN_VALUE | 80 | 0.1% |
| COPY_FREE_VARS | 80 | 0.1% |
| CALL | 40 | 0.1% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 80 | 66.7% |
| BUILD_MAP | 40 | 33.3% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,187,760 | 94.9% |
| ENTER_EXECUTOR | 605,280 | 5.1% |
| JUMP_BACKWARD | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 5,290,080 | 44.9% |
| LOAD_FAST | 2,801,440 | 23.8% |
| STORE_FAST | 2,277,240 | 19.3% |
| RESUME_CHECK | 1,140,220 | 9.7% |
| BUILD_LIST | 216,960 | 1.8% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 541,680 | 98.8% |
| LOAD_GLOBAL_MODULE | 3,060 | 0.6% |
| LOAD_CONST | 2,400 | 0.4% |
| LOAD_FAST | 660 | 0.1% |
| COMPARE_OP | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 545,380 | 99.5% |
| POP_JUMP_IF_TRUE | 1,220 | 0.2% |
| COMPARE_OP_INT | 960 | 0.2% |
| COMPARE_OP | 400 | 0.1% |
| COMPARE_OP_STR | 380 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,091,120 | 54.1% |
| BINARY_SUBSCR_DICT | 754,660 | 37.4% |
| LOAD_ATTR_INSTANCE_VALUE | 131,400 | 6.5% |
| LOAD_FAST_LOAD_FAST | 16,440 | 0.8% |
| LOAD_GLOBAL_MODULE | 9,120 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 699,780 | 34.7% |
| POP_JUMP_IF_FALSE | 698,180 | 34.6% |
| STORE_FAST | 599,880 | 29.7% |
| EXTENDED_ARG | 12,620 | 0.6% |
| ENTER_EXECUTOR | 5,460 | 0.3% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,880 | 50.8% |
| LOAD_ATTR_INSTANCE_VALUE | 40,540 | 49.2% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 82,440 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,597,220 | 45.6% |
| LOAD_FAST | 1,027,200 | 29.3% |
| RETURN_VALUE | 746,140 | 21.3% |
| LOAD_CONST | 75,220 | 2.1% |
| CALL_BUILTIN_FAST | 40,540 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,592,840 | 45.4% |
| TO_BOOL_NONE | 1,496,800 | 42.7% |
| TO_BOOL_ALWAYS_TRUE | 153,160 | 4.4% |
| TO_BOOL_LIST | 123,900 | 3.5% |
| LOAD_FAST | 65,360 | 1.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BOUND_METHOD_EXACT_ARGS | 754,180 | 51.8% |
| CALL_PY_EXACT_ARGS | 701,420 | 48.2% |
| CACHE | 120 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |
| CALL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,455,720 | 100.0% |
| RETURN_GENERATOR | 80 | 0.0% |
| RESUME | 40 | 0.0% |


</details>

### DELETE_NAME

<details>
<summary> Successors and predecessors for DELETE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 20 | 50.0% |
| BUILD_MAP | 20 | 50.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 360 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 160 | 80.0% |
| BUILD_CONST_KEY_MAP | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 120 | 60.0% |
| STORE_NAME | 40 | 20.0% |
| BUILD_LIST | 20 | 10.0% |
| EXTENDED_ARG | 20 | 10.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 36,564,480 | 39.9% |
| POP_JUMP_IF_TRUE | 30,545,920 | 33.3% |
| POP_JUMP_IF_FALSE | 18,153,860 | 19.8% |
| POP_JUMP_IF_NOT_NONE | 2,945,960 | 3.2% |
| LOAD_FAST | 1,557,140 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 52,590,400 | 57.4% |
| LOAD_ATTR_METHOD_NO_DICT | 20,493,180 | 22.4% |
| CALL_LIST_APPEND | 10,509,860 | 11.5% |
| FOR_ITER_LIST | 2,573,340 | 2.8% |
| RETURN_VALUE | 1,818,040 | 2.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 25,433,000 | 90.0% |
| POP_TOP | 1,883,740 | 6.7% |
| ENTER_EXECUTOR | 617,400 | 2.2% |
| GET_ITER | 280,540 | 1.0% |
| CONTAINS_OP | 12,620 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 25,433,000 | 90.0% |
| JUMP_FORWARD | 1,889,120 | 6.7% |
| FOR_ITER_LIST | 887,960 | 3.1% |
| POP_JUMP_IF_FALSE | 17,240 | 0.1% |
| FOR_ITER | 13,940 | 0.0% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 3,497,620 | 99.3% |
| EXTENDED_ARG | 13,940 | 0.4% |
| JUMP_BACKWARD | 9,180 | 0.3% |
| FOR_ITER | 2,600 | 0.1% |
| SWAP | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,489,720 | 99.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 25,380 | 0.7% |
| RETURN_CONST | 2,760 | 0.1% |
| FOR_ITER | 2,600 | 0.1% |
| STORE_FAST_LOAD_FAST | 960 | 0.0% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 480 | 100.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 61,440 | 98.9% |
| LOAD_CONST | 320 | 0.5% |
| LOAD_FAST | 200 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 160 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 51,500 | 82.9% |
| ENTER_EXECUTOR | 8,880 | 14.3% |
| POP_JUMP_IF_TRUE | 1,420 | 2.3% |
| COPY | 320 | 0.5% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 5,760 | 14.7% |
| EXTENDED_ARG | 5,620 | 14.4% |
| STORE_FAST | 5,240 | 13.4% |
| LIST_APPEND | 5,220 | 13.3% |
| POP_JUMP_IF_TRUE | 4,500 | 11.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 19,440 | 49.7% |
| FOR_ITER | 9,180 | 23.5% |
| EXTENDED_ARG | 4,840 | 12.4% |
| FOR_ITER_TUPLE | 1,600 | 4.1% |
| LOAD_FAST | 1,120 | 2.9% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,891,560 | 92.9% |
| EXTENDED_ARG | 1,889,120 | 4.9% |
| RETURN_VALUE | 768,680 | 2.0% |
| POP_TOP | 67,240 | 0.2% |
| BINARY_OP | 23,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 36,408,780 | 94.2% |
| LOAD_FAST_LOAD_FAST | 2,004,080 | 5.2% |
| STORE_FAST | 109,840 | 0.3% |
| LOAD_GLOBAL_BUILTIN | 58,440 | 0.2% |
| LOAD_CONST | 41,420 | 0.1% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 835,040 | 99.2% |
| BUILD_TUPLE | 4,400 | 0.5% |
| CALL_BUILTIN_CLASS | 820 | 0.1% |
| LOAD_FAST | 560 | 0.1% |
| CALL_METHOD_DESCRIPTOR_O | 520 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 836,380 | 99.4% |
| JUMP_BACKWARD | 5,220 | 0.6% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,100 | 98.3% |
| LOAD_DEREF | 80 | 1.1% |
| LOAD_FAST | 40 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 3,480 | 48.2% |
| BUILD_LIST | 3,360 | 46.5% |
| STORE_FAST | 240 | 3.3% |
| CALL_INTRINSIC_1 | 120 | 1.7% |
| STORE_NAME | 20 | 0.3% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,974,820 | 99.3% |
| LOAD_GLOBAL_MODULE | 124,580 | 0.4% |
| LOAD_ATTR | 71,360 | 0.2% |
| LOAD_FAST_LOAD_FAST | 41,480 | 0.1% |
| BINARY_SUBSCR_TUPLE_INT | 6,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,449,460 | 45.1% |
| STORE_FAST | 12,294,760 | 35.9% |
| LOAD_ATTR_METHOD_NO_DICT | 3,976,900 | 11.6% |
| LOAD_FAST_LOAD_FAST | 867,320 | 2.5% |
| LOAD_CONST | 700,340 | 2.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 270,360,320 | 49.6% |
| UNARY_NEGATIVE | 104,698,080 | 19.2% |
| STORE_ATTR_INSTANCE_VALUE | 35,783,280 | 6.6% |
| BINARY_OP_SUBTRACT_INT | 34,905,460 | 6.4% |
| LOAD_CONST | 24,274,320 | 4.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 110,156,640 | 20.2% |
| BUILD_SLICE | 69,799,540 | 12.8% |
| LOAD_FAST | 48,133,940 | 8.8% |
| BINARY_SUBSCR_GETITEM | 47,350,940 | 8.7% |
| BINARY_SUBSCR | 35,936,360 | 6.6% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,455,600 | 100.0% |
| POP_JUMP_IF_FALSE | 120 | 0.0% |
| BINARY_SLICE | 80 | 0.0% |
| NOP | 80 | 0.0% |
| BUILD_LIST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,455,760 | 100.0% |
| LOAD_FAST | 160 | 0.0% |
| LIST_EXTEND | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 80 | 0.0% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,882,920 | 16.8% |
| STORE_FAST | 257,640,600 | 13.8% |
| POP_JUMP_IF_FALSE | 199,577,780 | 10.7% |
| LOAD_ATTR_INSTANCE_VALUE | 149,719,540 | 8.0% |
| STORE_ATTR_INSTANCE_VALUE | 125,317,220 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 312,882,920 | 16.8% |
| LOAD_CONST | 270,360,320 | 14.5% |
| LOAD_ATTR_INSTANCE_VALUE | 201,516,920 | 10.8% |
| STORE_ATTR_INSTANCE_VALUE | 177,760,920 | 9.6% |
| UNARY_NEGATIVE | 124,482,300 | 6.7% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 837,060 | 50.1% |
| LOAD_FAST_AND_CLEAR | 835,040 | 49.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 837,060 | 50.1% |
| LOAD_FAST_AND_CLEAR | 835,040 | 49.9% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 3,860 | 94.1% |
| POP_TOP | 160 | 3.9% |
| LOAD_FAST | 40 | 1.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,860 | 94.1% |
| POP_JUMP_IF_NOT_NONE | 160 | 3.9% |
| LOAD_FAST | 40 | 1.0% |
| CALL_LIST_APPEND | 40 | 1.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 50,954,380 | 37.9% |
| STORE_ATTR_SLOT | 30,350,540 | 22.6% |
| STORE_ATTR_INSTANCE_VALUE | 26,470,120 | 19.7% |
| STORE_FAST | 19,595,300 | 14.6% |
| JUMP_FORWARD | 2,004,080 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 45,451,720 | 33.8% |
| LOAD_ATTR_INSTANCE_VALUE | 36,306,160 | 27.0% |
| STORE_ATTR_INSTANCE_VALUE | 33,420,240 | 24.9% |
| BINARY_SUBSCR_LIST_INT | 12,249,400 | 9.1% |
| LOAD_CONST | 2,105,640 | 1.6% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,600 | 14.7% |
| RESUME | 1,500 | 13.7% |
| RESUME_CHECK | 1,500 | 13.7% |
| POP_JUMP_IF_FALSE | 1,480 | 13.6% |
| LOAD_FAST | 1,060 | 9.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,080 | 28.2% |
| LOAD_GLOBAL_BUILTIN | 2,440 | 22.3% |
| LOAD_ATTR | 2,380 | 21.8% |
| LOAD_FAST | 2,180 | 20.0% |
| CALL | 360 | 3.3% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 8,160 | 44.3% |
| STORE_NAME | 5,280 | 28.7% |
| BINARY_SUBSCR_DICT | 1,340 | 7.3% |
| BUILD_MAP | 860 | 4.7% |
| PUSH_NULL | 680 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 8,160 | 44.3% |
| CONTAINS_OP | 4,540 | 24.6% |
| STORE_SUBSCR_DICT | 2,080 | 11.3% |
| LOAD_CONST | 1,360 | 7.4% |
| BINARY_SUBSCR_DICT | 1,300 | 7.1% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 80 | 100.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 3,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,800 | 52.9% |
| EXTENDED_ARG | 1,400 | 41.2% |
| DICT_UPDATE | 160 | 4.7% |
| BUILD_MAP | 40 | 1.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 111,089,860 | 49.6% |
| TO_BOOL_BOOL | 55,023,440 | 24.6% |
| TO_BOOL_INT | 46,090,460 | 20.6% |
| TO_BOOL_STR | 5,398,800 | 2.4% |
| COMPARE_OP_STR | 4,300,080 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 199,577,780 | 89.1% |
| ENTER_EXECUTOR | 18,153,860 | 8.1% |
| LOAD_FAST_LOAD_FAST | 1,905,500 | 0.9% |
| LOAD_GLOBAL_MODULE | 1,762,800 | 0.8% |
| LOAD_CONST | 1,703,520 | 0.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 25,433,000 | 96.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 599,820 | 2.3% |
| RETURN_VALUE | 120,980 | 0.5% |
| LOAD_ATTR_WITH_HINT | 65,340 | 0.2% |
| LOAD_ATTR_SLOT | 49,300 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 26,266,200 | 99.9% |
| LOAD_FAST_LOAD_FAST | 16,920 | 0.1% |
| LOAD_CONST | 9,860 | 0.0% |
| EXTENDED_ARG | 1,920 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 1,140 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,973,160 | 56.8% |
| RETURN_VALUE | 856,120 | 16.3% |
| BINARY_SUBSCR_DICT | 854,180 | 16.3% |
| LOAD_ATTR_SLOT | 254,040 | 4.9% |
| LOAD_ATTR_WITH_HINT | 216,820 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,945,960 | 56.3% |
| LOAD_FAST | 1,583,200 | 30.2% |
| LOAD_GLOBAL_BUILTIN | 663,360 | 12.7% |
| RETURN_CONST | 21,080 | 0.4% |
| LOAD_GLOBAL_MODULE | 9,920 | 0.2% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 36,102,820 | 46.3% |
| TO_BOOL_ALWAYS_TRUE | 27,756,380 | 35.6% |
| TO_BOOL_BOOL | 7,219,820 | 9.3% |
| TO_BOOL | 3,897,260 | 5.0% |
| TO_BOOL_LIST | 1,337,440 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 32,405,800 | 41.6% |
| ENTER_EXECUTOR | 30,545,920 | 39.2% |
| LOAD_GLOBAL_MODULE | 13,091,920 | 16.8% |
| POP_TOP | 1,329,600 | 1.7% |
| LOAD_GLOBAL_BUILTIN | 247,880 | 0.3% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 37,952,900 | 41.0% |
| STORE_SUBSCR | 35,259,660 | 38.1% |
| STORE_ATTR_SLOT | 14,583,500 | 15.8% |
| POP_TOP | 2,615,280 | 2.8% |
| ENTER_EXECUTOR | 1,573,040 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 50,367,520 | 54.4% |
| POP_TOP | 39,125,100 | 42.3% |
| STORE_FAST | 3,053,400 | 3.3% |
| TO_BOOL_BOOL | 22,140 | 0.0% |
| EXIT_INIT_CHECK | 3,360 | 0.0% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 80 | 66.7% |
| STORE_FAST | 40 | 33.3% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 6,880 | 49.4% |
| LOAD_FAST | 6,420 | 46.1% |
| STORE_ATTR | 320 | 2.3% |
| BINARY_SUBSCR | 60 | 0.4% |
| LOAD_ATTR | 60 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,880 | 20.7% |
| STORE_ATTR_INSTANCE_VALUE | 2,840 | 20.4% |
| LOAD_FAST_LOAD_FAST | 2,100 | 15.1% |
| RETURN_CONST | 1,920 | 13.8% |
| LOAD_FAST | 1,280 | 9.2% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 90,457,240 | 26.5% |
| LOAD_ATTR_INSTANCE_VALUE | 48,141,620 | 14.1% |
| BINARY_SUBSCR_DICT | 36,504,720 | 10.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 35,046,940 | 10.3% |
| BINARY_SLICE | 34,902,100 | 10.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 257,640,600 | 75.5% |
| JUMP_FORWARD | 35,891,560 | 10.5% |
| LOAD_GLOBAL_MODULE | 21,242,880 | 6.2% |
| LOAD_FAST_LOAD_FAST | 19,595,300 | 5.7% |
| LOAD_GLOBAL_BUILTIN | 2,619,160 | 0.8% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,420 | 87.9% |
| FOR_ITER_LIST | 1,674,400 | 12.0% |
| CALL_LEN | 8,640 | 0.1% |
| FOR_ITER | 960 | 0.0% |
| FOR_ITER_TUPLE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 12,249,400 | 87.9% |
| LIST_APPEND | 835,040 | 6.0% |
| LOAD_ATTR_SLOT | 835,000 | 6.0% |
| PUSH_NULL | 8,640 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 4,320 | 0.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 76,440 | 88.1% |
| COPY | 9,860 | 11.4% |
| UNPACK_SEQUENCE_TUPLE | 240 | 0.3% |
| UNPACK_SEQUENCE | 220 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 39,280 | 45.3% |
| LOAD_FAST | 28,860 | 33.3% |
| LOAD_GLOBAL_BUILTIN | 14,360 | 16.6% |
| NOP | 2,980 | 3.4% |
| BUILD_LIST | 720 | 0.8% |


</details>

### STORE_GLOBAL

<details>
<summary> Successors and predecessors for STORE_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 720 | 75.0% |
| LOAD_FAST | 240 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 960 | 100.0% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 5,220 | 46.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,140 | 45.6% |
| IMPORT_NAME | 480 | 4.3% |
| LOAD_CONST | 120 | 1.1% |
| BUILD_CONST_KEY_MAP | 80 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_NAME | 5,280 | 46.9% |
| STORE_NAME | 5,220 | 46.4% |
| RETURN_CONST | 500 | 4.4% |
| LOAD_CONST | 160 | 1.4% |
| BUILD_MAP | 80 | 0.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,375,520 | 71.7% |
| BINARY_OP_ADD_INT | 1,592,860 | 11.0% |
| BUILD_LIST | 837,060 | 5.8% |
| LOAD_FAST_AND_CLEAR | 837,060 | 5.8% |
| FOR_ITER_LIST | 835,040 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,375,560 | 71.7% |
| STORE_ATTR_INSTANCE_VALUE | 1,592,840 | 11.0% |
| BUILD_LIST | 837,060 | 5.8% |
| STORE_FAST | 836,340 | 5.8% |
| FOR_ITER_LIST | 835,460 | 5.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 420 | 65.6% |
| RETURN_VALUE | 80 | 12.5% |
| FOR_ITER_LIST | 60 | 9.4% |
| LOAD_FAST | 40 | 6.2% |
| BINARY_SUBSCR | 20 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 320 | 50.0% |
| STORE_FAST_STORE_FAST | 220 | 34.4% |
| STORE_NAME | 80 | 12.5% |
| STORE_FAST_LOAD_FAST | 20 | 3.1% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 240 | 75.0% |
| CALL | 80 | 25.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 320 | 100.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 1,800 | 32.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,520 | 27.2% |
| CALL | 1,140 | 20.4% |
| CALL_PY_EXACT_ARGS | 920 | 16.5% |
| CALL_KW | 100 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,100 | 37.6% |
| LOAD_GLOBAL | 1,500 | 26.9% |
| LOAD_FAST_LOAD_FAST | 1,120 | 20.1% |
| LOAD_CONST | 720 | 12.9% |
| BUILD_LIST | 60 | 1.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,592,840 | 97.7% |
| LOAD_CONST | 25,140 | 1.5% |
| LOAD_FAST_LOAD_FAST | 10,000 | 0.6% |
| BINARY_OP_MULTIPLY_INT | 2,480 | 0.2% |
| BINARY_OP | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,592,860 | 97.7% |
| LOAD_FAST | 14,740 | 0.9% |
| STORE_FAST | 14,140 | 0.9% |
| CALL_BUILTIN_O | 4,160 | 0.3% |
| CALL_PY_EXACT_ARGS | 4,160 | 0.3% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 541,220 | 48.7% |
| BINARY_OP | 540,700 | 48.7% |
| RETURN_VALUE | 21,880 | 2.0% |
| BINARY_SLICE | 6,760 | 0.6% |
| LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 569,460 | 51.3% |
| STORE_FAST | 541,340 | 48.7% |
| BINARY_OP_INPLACE_ADD_UNICODE | 240 | 0.0% |
| CALL | 40 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,260 | 63.2% |
| BINARY_SUBSCR_TUPLE_INT | 2,480 | 36.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,160 | 61.7% |
| BINARY_OP_ADD_INT | 2,480 | 36.8% |
| CALL_BUILTIN_O | 100 | 1.5% |


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
| BINARY_OP | 60 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 34,904,040 | 86.9% |
| LOAD_FAST | 5,268,280 | 13.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 34,905,460 | 86.9% |
| STORE_FAST | 5,256,140 | 13.1% |
| LOAD_FAST_LOAD_FAST | 8,640 | 0.0% |
| LOAD_FAST | 1,820 | 0.0% |
| BUILD_TUPLE | 300 | 0.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,726,500 | 49.6% |
| BINARY_SUBSCR | 35,692,480 | 43.4% |
| LOAD_CONST | 4,700,660 | 5.7% |
| LOAD_FAST_LOAD_FAST | 1,025,480 | 1.2% |
| BUILD_TUPLE | 1,920 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 36,504,720 | 44.4% |
| LOAD_FAST | 36,358,400 | 44.3% |
| LOAD_ATTR_METHOD_NO_DICT | 5,789,900 | 7.0% |
| POP_JUMP_IF_NOT_NONE | 854,180 | 1.0% |
| CONTAINS_OP | 754,660 | 0.9% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 47,350,940 | 100.0% |
| BINARY_SUBSCR | 4,780 | 0.0% |
| ENTER_EXECUTOR | 940 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 47,356,660 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 99,728,960 | 73.7% |
| UNARY_NEGATIVE | 19,783,360 | 14.6% |
| LOAD_FAST_LOAD_FAST | 12,249,400 | 9.1% |
| LOAD_CONST | 3,486,140 | 2.6% |
| BINARY_SUBSCR | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 47,352,760 | 35.0% |
| STORE_ATTR_INSTANCE_VALUE | 36,129,520 | 26.7% |
| STORE_FAST | 19,817,580 | 14.7% |
| LOAD_CONST | 18,003,960 | 13.3% |
| UNPACK_SEQUENCE_TWO_TUPLE | 12,249,560 | 9.1% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,920 | 74.3% |
| LOAD_CONST | 2,340 | 15.9% |
| LOAD_FAST_LOAD_FAST | 1,240 | 8.4% |
| ENTER_EXECUTOR | 160 | 1.1% |
| BINARY_SUBSCR | 40 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 10,920 | 74.3% |
| LOAD_CONST | 1,720 | 11.7% |
| LOAD_FAST | 1,260 | 8.6% |
| CALL_BUILTIN_O | 620 | 4.2% |
| PUSH_EXC_INFO | 160 | 1.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 208,420 | 99.9% |
| BINARY_SUBSCR | 300 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 42,740 | 20.5% |
| BUILD_TUPLE | 41,020 | 19.7% |
| CALL_STR_1 | 40,520 | 19.4% |
| LOAD_GLOBAL_BUILTIN | 40,520 | 19.4% |
| CALL_LEN | 10,760 | 5.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 1,780 | 53.0% |
| LOAD_GLOBAL_MODULE | 560 | 16.7% |
| LOAD_ATTR_MODULE | 400 | 11.9% |
| LOAD_FAST | 240 | 7.1% |
| LOAD_ATTR_INSTANCE_VALUE | 200 | 6.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,360 | 100.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,427,940 | 86.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,945,720 | 10.8% |
| LOAD_ATTR_WITH_HINT | 433,520 | 1.6% |
| CALL_PY_EXACT_ARGS | 360,700 | 1.3% |
| LOAD_CONST | 14,260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 26,082,580 | 95.9% |
| COPY_FREE_VARS | 754,180 | 2.8% |
| CALL_PY_EXACT_ARGS | 360,700 | 1.3% |
| RESUME | 1,520 | 0.0% |
| POP_TOP | 160 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 3,011,760 | 92.7% |
| LOAD_GLOBAL_BUILTIN | 217,560 | 6.7% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 10,160 | 0.3% |
| LOAD_CONST | 4,500 | 0.1% |
| CALL_BUILTIN_FAST | 2,720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,951,280 | 90.8% |
| CALL_LIST_APPEND | 216,760 | 6.7% |
| LOAD_FAST | 65,780 | 2.0% |
| STORE_FAST | 11,140 | 0.3% |
| RETURN_VALUE | 2,720 | 0.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,340,400 | 99.7% |
| LOAD_ATTR | 40,520 | 0.2% |
| LOAD_FAST_LOAD_FAST | 4,360 | 0.0% |
| ENTER_EXECUTOR | 2,700 | 0.0% |
| LOAD_FAST | 1,220 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 16,202,040 | 98.9% |
| STORE_FAST | 81,300 | 0.5% |
| TO_BOOL_BOOL | 56,720 | 0.3% |
| COPY | 40,540 | 0.2% |
| BUILD_TUPLE | 4,360 | 0.0% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 19,720 | 68.3% |
| LOAD_FAST_LOAD_FAST | 7,520 | 26.0% |
| LOAD_FAST | 760 | 2.6% |
| BINARY_OP | 400 | 1.4% |
| CALL_TUPLE_1 | 160 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 9,860 | 34.1% |
| LOAD_GLOBAL_BUILTIN | 9,860 | 34.1% |
| STORE_FAST | 8,000 | 27.7% |
| POP_TOP | 440 | 1.5% |
| RETURN_VALUE | 400 | 1.4% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 16,380 | 28.1% |
| LOAD_CONST | 12,420 | 21.3% |
| RETURN_VALUE | 7,240 | 12.4% |
| LOAD_FAST | 6,700 | 11.5% |
| BINARY_SUBSCR_TUPLE_INT | 6,260 | 10.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 56,580 | 96.9% |
| BUILD_TUPLE | 1,760 | 3.0% |
| TO_BOOL_INT | 40 | 0.1% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 48,122,700 | 92.9% |
| LOAD_ATTR_MODULE | 2,319,920 | 4.5% |
| BUILD_TUPLE | 1,285,700 | 2.5% |
| LOAD_ATTR | 40,920 | 0.1% |
| LOAD_GLOBAL_MODULE | 13,160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 51,749,200 | 99.9% |
| RETURN_VALUE | 40,860 | 0.1% |
| TO_BOOL | 640 | 0.0% |
| LOAD_FAST | 160 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,837,340 | 49.1% |
| LOAD_ATTR_INSTANCE_VALUE | 10,801,160 | 48.9% |
| LOAD_ATTR_WITH_HINT | 216,760 | 1.0% |
| BINARY_SUBSCR_DICT | 202,560 | 0.9% |
| BINARY_SUBSCR_TUPLE_INT | 10,760 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 11,231,840 | 50.9% |
| RETURN_VALUE | 10,811,840 | 49.0% |
| LOAD_FAST | 9,700 | 0.0% |
| STORE_FAST_LOAD_FAST | 8,640 | 0.0% |
| CALL_BUILTIN_O | 3,760 | 0.0% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 82,656,280 | 87.9% |
| ENTER_EXECUTOR | 10,509,860 | 11.2% |
| RETURN_VALUE | 484,240 | 0.5% |
| CALL_BUILTIN_CLASS | 216,760 | 0.2% |
| CALL_FUNCTION_EX | 74,360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,819,340 | 49.8% |
| ENTER_EXECUTOR | 36,564,480 | 38.9% |
| LOAD_CONST | 10,374,520 | 11.0% |
| RETURN_CONST | 228,940 | 0.2% |
| LOAD_GLOBAL_MODULE | 20,640 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,042,580 | 62.1% |
| LOAD_ATTR_METHOD_NO_DICT | 12,470,560 | 26.6% |
| LOAD_CONST | 5,249,580 | 11.2% |
| LOAD_ATTR | 40,760 | 0.1% |
| CALL | 580 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 35,046,940 | 74.9% |
| LOAD_FAST | 9,876,900 | 21.1% |
| POP_TOP | 1,068,160 | 2.3% |
| POP_JUMP_IF_NONE | 599,820 | 1.3% |
| TO_BOOL_BOOL | 102,100 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,680 | 81.4% |
| LOAD_GLOBAL_MODULE | 820 | 18.1% |
| CALL | 20 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,700 | 81.9% |
| LOAD_CONST | 820 | 18.1% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 13,960 | 98.7% |
| CALL | 180 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 10,160 | 71.9% |
| GET_ITER | 1,700 | 12.0% |
| TO_BOOL_BOOL | 1,400 | 9.9% |
| CONTAINS_OP | 860 | 6.1% |
| CALL | 20 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 219,560 | 97.0% |
| BINARY_SLICE | 4,120 | 1.8% |
| LOAD_FAST | 1,500 | 0.7% |
| STORE_FAST | 440 | 0.2% |
| LOAD_CONST | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 220,420 | 97.4% |
| STORE_FAST | 4,220 | 1.9% |
| LIST_APPEND | 520 | 0.2% |
| RETURN_VALUE | 460 | 0.2% |
| CALL_LIST_APPEND | 400 | 0.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,186,440 | 80.7% |
| LOAD_CONST | 5,826,080 | 10.9% |
| LOAD_FAST_LOAD_FAST | 1,665,500 | 3.1% |
| RETURN_VALUE | 688,600 | 1.3% |
| BINARY_SUBSCR_DICT | 661,920 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 52,442,500 | 98.0% |
| COPY_FREE_VARS | 701,420 | 1.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 360,700 | 0.7% |
| CALL_PY_EXACT_ARGS | 18,760 | 0.0% |
| RESUME | 920 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 851,440 | 94.9% |
| LOAD_FAST | 41,440 | 4.6% |
| ENTER_EXECUTOR | 4,060 | 0.5% |
| CALL | 200 | 0.0% |
| LOAD_FAST_LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 897,320 | 100.0% |
| RETURN_GENERATOR | 60 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 40,520 | 99.7% |
| LOAD_FAST | 120 | 0.3% |
| CALL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40,540 | 99.7% |
| STORE_FAST | 80 | 0.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 0.1% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 580 | 72.5% |
| LOAD_FAST | 160 | 20.0% |
| LOAD_GLOBAL_MODULE | 40 | 5.0% |
| CALL | 20 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 600 | 75.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 160 | 20.0% |
| CALL | 40 | 5.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,240 | 98.2% |
| LOAD_GLOBAL_MODULE | 40 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,080 | 91.2% |
| LOAD_FAST | 160 | 7.0% |
| PUSH_NULL | 40 | 1.8% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 40 | 100.0% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 110,156,640 | 98.3% |
| LOAD_FAST_LOAD_FAST | 1,876,000 | 1.7% |
| LOAD_GLOBAL_MODULE | 4,480 | 0.0% |
| CALL_LEN | 2,120 | 0.0% |
| COMPARE_OP | 960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 111,089,860 | 99.2% |
| POP_JUMP_IF_TRUE | 950,120 | 0.8% |
| EXTENDED_ARG | 940 | 0.0% |
| RETURN_VALUE | 40 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,285,920 | 99.5% |
| LOAD_ATTR_INSTANCE_VALUE | 18,260 | 0.4% |
| LOAD_FAST_LOAD_FAST | 1,840 | 0.0% |
| LOAD_GLOBAL_MODULE | 400 | 0.0% |
| COMPARE_OP | 380 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,300,080 | 99.8% |
| POP_JUMP_IF_TRUE | 5,620 | 0.1% |
| EXTENDED_ARG | 1,400 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 2,573,340 | 49.4% |
| GET_ITER | 888,000 | 17.1% |
| EXTENDED_ARG | 887,960 | 17.1% |
| SWAP | 835,460 | 16.1% |
| JUMP_BACKWARD | 19,440 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 1,674,400 | 32.2% |
| LOAD_FAST | 1,474,340 | 28.3% |
| ENTER_EXECUTOR | 861,180 | 16.5% |
| SWAP | 835,040 | 16.0% |
| STORE_FAST | 317,800 | 6.1% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 9,840 | 87.7% |
| SWAP | 820 | 7.3% |
| GET_ITER | 480 | 4.3% |
| JUMP_BACKWARD | 60 | 0.5% |
| FOR_ITER | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,320 | 65.2% |
| JUMP_FORWARD | 1,780 | 15.9% |
| STORE_FAST | 1,300 | 11.6% |
| SWAP | 820 | 7.3% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 17,560 | 47.0% |
| GET_ITER | 16,960 | 45.4% |
| JUMP_BACKWARD | 1,600 | 4.3% |
| EXTENDED_ARG | 680 | 1.8% |
| SWAP | 460 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 17,940 | 48.0% |
| ENTER_EXECUTOR | 14,220 | 38.0% |
| EXTENDED_ARG | 3,180 | 8.5% |
| LOAD_CONST | 720 | 1.9% |
| SWAP | 480 | 1.3% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 201,516,920 | 68.9% |
| BINARY_SUBSCR_LIST_INT | 47,352,760 | 16.2% |
| LOAD_FAST_LOAD_FAST | 36,306,160 | 12.4% |
| LOAD_ATTR_WITH_HINT | 5,256,120 | 1.8% |
| COPY | 1,592,840 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 149,719,540 | 51.2% |
| STORE_FAST | 48,141,620 | 16.5% |
| RETURN_VALUE | 47,407,520 | 16.2% |
| CALL_LEN | 10,801,160 | 3.7% |
| LOAD_CONST | 8,183,200 | 2.8% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 109,960,020 | 73.5% |
| ENTER_EXECUTOR | 20,493,180 | 13.7% |
| LOAD_ATTR_INSTANCE_VALUE | 7,321,680 | 4.9% |
| BINARY_SUBSCR_DICT | 5,789,900 | 3.9% |
| LOAD_ATTR | 3,976,900 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 116,142,900 | 77.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 12,470,560 | 8.3% |
| CALL | 12,249,680 | 8.2% |
| LOAD_CONST | 8,493,520 | 5.7% |
| LOAD_GLOBAL_BUILTIN | 216,800 | 0.1% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,675,360 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 130,800 | 0.8% |
| BINARY_SUBSCR | 4,160 | 0.0% |
| BINARY_SUBSCR_TUPLE_INT | 1,780 | 0.0% |
| LOAD_ATTR_WITH_HINT | 1,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,776,320 | 93.8% |
| LOAD_CONST | 1,003,580 | 6.0% |
| CALL_PY_EXACT_ARGS | 32,540 | 0.2% |
| LOAD_GLOBAL_MODULE | 840 | 0.0% |
| LOAD_FAST_LOAD_FAST | 520 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 14,882,180 | 99.9% |
| LOAD_FAST | 2,920 | 0.0% |
| LOAD_ATTR | 2,640 | 0.0% |
| LOAD_FAST_LOAD_FAST | 1,400 | 0.0% |
| BINARY_SUBSCR_DICT | 400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 8,750,860 | 58.8% |
| LOAD_GLOBAL_MODULE | 2,480,860 | 16.7% |
| CALL_ISINSTANCE | 2,319,920 | 15.6% |
| BUILD_TUPLE | 1,251,800 | 8.4% |
| LOAD_ATTR_METHOD_NO_DICT | 41,240 | 0.3% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 50.0% |
| LOAD_FAST_LOAD_FAST | 160 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 160 | 50.0% |
| LOAD_GLOBAL_BUILTIN | 160 | 50.0% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,840 | 99.2% |
| LOAD_ATTR_INSTANCE_VALUE | 320 | 0.7% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 45,180 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,911,440 | 39.8% |
| LOAD_FAST | 2,622,460 | 35.9% |
| BINARY_SUBSCR_LIST_INT | 842,480 | 11.5% |
| STORE_FAST_LOAD_FAST | 835,000 | 11.4% |
| LOAD_ATTR_SLOT | 61,880 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,151,120 | 29.4% |
| LOAD_CONST | 1,118,560 | 15.3% |
| GET_ITER | 868,920 | 11.9% |
| LOAD_GLOBAL_MODULE | 672,720 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 584,000 | 8.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,522,700 | 68.8% |
| LOAD_ATTR_WITH_HINT | 5,425,160 | 15.9% |
| LOAD_ATTR_INSTANCE_VALUE | 5,256,120 | 15.4% |
| LOAD_ATTR | 640 | 0.0% |
| ENTER_EXECUTOR | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 10,541,800 | 30.8% |
| LOAD_FAST | 8,267,440 | 24.2% |
| LOAD_ATTR_WITH_HINT | 5,425,160 | 15.9% |
| LOAD_ATTR_INSTANCE_VALUE | 5,256,120 | 15.4% |
| CALL_BUILTIN_CLASS | 3,011,760 | 8.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 88,527,780 | 61.9% |
| LOAD_FAST | 47,610,460 | 33.3% |
| STORE_FAST | 2,619,160 | 1.8% |
| RETURN_VALUE | 1,339,760 | 0.9% |
| POP_TOP | 846,760 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 93,817,820 | 65.6% |
| CALL_ISINSTANCE | 48,122,700 | 33.6% |
| BUILD_LIST | 846,380 | 0.6% |
| CALL_BUILTIN_CLASS | 217,560 | 0.2% |
| STORE_FAST | 24,340 | 0.0% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 21,242,880 | 40.3% |
| POP_JUMP_IF_TRUE | 13,091,920 | 24.9% |
| RESUME_CHECK | 10,075,340 | 19.1% |
| LOAD_ATTR_MODULE | 2,480,860 | 4.7% |
| LOAD_FAST | 2,258,600 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 32,033,600 | 60.8% |
| LOAD_ATTR_MODULE | 14,882,180 | 28.3% |
| LOAD_FAST | 5,372,460 | 10.2% |
| LOAD_ATTR | 124,580 | 0.2% |
| IS_OP | 61,440 | 0.1% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 100.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 61,303,780 | 32.1% |
| CALL_PY_EXACT_ARGS | 52,442,500 | 27.5% |
| BINARY_SUBSCR_GETITEM | 47,356,660 | 24.8% |
| CALL_BOUND_METHOD_EXACT_ARGS | 26,082,580 | 13.7% |
| COPY_FREE_VARS | 1,455,720 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 88,527,780 | 46.4% |
| LOAD_FAST_LOAD_FAST | 50,954,380 | 26.7% |
| LOAD_FAST | 37,734,560 | 19.8% |
| LOAD_GLOBAL_MODULE | 10,075,340 | 5.3% |
| LOAD_CONST | 1,973,520 | 1.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 177,760,920 | 68.0% |
| BINARY_SUBSCR_LIST_INT | 36,129,520 | 13.8% |
| LOAD_FAST_LOAD_FAST | 33,420,240 | 12.8% |
| STORE_FAST_LOAD_FAST | 12,249,400 | 4.7% |
| SWAP | 1,592,840 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,317,220 | 48.0% |
| RETURN_CONST | 37,952,900 | 14.5% |
| LOAD_CONST | 35,783,280 | 13.7% |
| NOP | 35,691,440 | 13.7% |
| LOAD_FAST_LOAD_FAST | 26,470,120 | 10.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 45,451,720 | 98.0% |
| LOAD_FAST | 889,740 | 1.9% |
| RETURN_VALUE | 6,760 | 0.0% |
| STORE_ATTR_SLOT | 4,540 | 0.0% |
| STORE_ATTR | 2,880 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 30,350,540 | 65.5% |
| RETURN_CONST | 14,583,500 | 31.5% |
| LOAD_FAST | 1,416,720 | 3.1% |
| STORE_ATTR_SLOT | 4,540 | 0.0% |
| LOAD_CONST | 640 | 0.0% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,701,520 | 100.0% |
| LOAD_ATTR_WITH_HINT | 200 | 0.0% |
| STORE_ATTR | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,505,660 | 98.2% |
| RETURN_CONST | 196,020 | 1.8% |
| LOAD_CONST | 220 | 0.0% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 125,140 | 97.6% |
| LOAD_NAME | 2,080 | 1.6% |
| LOAD_CONST | 600 | 0.5% |
| STORE_SUBSCR | 380 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 102,440 | 79.9% |
| LOAD_GLOBAL_BUILTIN | 16,280 | 12.7% |
| JUMP_BACKWARD | 2,940 | 2.3% |
| ENTER_EXECUTOR | 1,940 | 1.5% |
| LOAD_FAST | 1,600 | 1.2% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 34,899,320 | 100.0% |
| LOAD_FAST_LOAD_FAST | 8,640 | 0.0% |
| LOAD_FAST | 5,120 | 0.0% |
| STORE_SUBSCR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,899,660 | 100.0% |
| ENTER_EXECUTOR | 5,360 | 0.0% |
| RETURN_CONST | 4,320 | 0.0% |
| JUMP_BACKWARD | 3,760 | 0.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 27,603,220 | 98.4% |
| TO_BOOL_NONE | 179,120 | 0.6% |
| COPY | 153,160 | 0.5% |
| CALL_KW | 65,320 | 0.2% |
| STORE_FAST | 40,520 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 27,756,380 | 98.9% |
| TO_BOOL_NONE | 179,100 | 0.6% |
| POP_JUMP_IF_FALSE | 121,160 | 0.4% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 51,749,200 | 83.1% |
| LOAD_ATTR_INSTANCE_VALUE | 4,979,440 | 8.0% |
| RETURN_VALUE | 3,028,980 | 4.9% |
| LOAD_FAST | 2,242,020 | 3.6% |
| CALL_METHOD_DESCRIPTOR_FAST | 102,100 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 55,023,440 | 88.4% |
| POP_JUMP_IF_TRUE | 7,219,820 | 11.6% |
| ENTER_EXECUTOR | 3,260 | 0.0% |
| EXTENDED_ARG | 1,820 | 0.0% |
| TO_BOOL_INT | 40 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,078,460 | 99.9% |
| BINARY_OP | 22,840 | 0.0% |
| COPY | 2,240 | 0.0% |
| TO_BOOL | 60 | 0.0% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 46,090,460 | 100.0% |
| UNARY_NOT | 8,440 | 0.0% |
| POP_JUMP_IF_TRUE | 4,780 | 0.0% |
| TO_BOOL_BOOL | 40 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 837,200 | 62.5% |
| BINARY_SUBSCR_DICT | 377,440 | 28.2% |
| COPY | 123,900 | 9.3% |
| LOAD_ATTR_INSTANCE_VALUE | 200 | 0.0% |
| TO_BOOL | 140 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 1,337,440 | 99.9% |
| POP_JUMP_IF_FALSE | 1,280 | 0.1% |
| UNARY_NOT | 160 | 0.0% |
| TO_BOOL_NONE | 20 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,607,760 | 93.7% |
| COPY | 1,496,800 | 4.1% |
| LOAD_ATTR_SLOT | 548,820 | 1.5% |
| TO_BOOL_ALWAYS_TRUE | 179,100 | 0.5% |
| TO_BOOL | 89,140 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 36,102,820 | 97.8% |
| POP_JUMP_IF_FALSE | 552,640 | 1.5% |
| TO_BOOL_ALWAYS_TRUE | 179,120 | 0.5% |
| TO_BOOL | 88,840 | 0.2% |
| TO_BOOL_LIST | 20 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 5,397,520 | 100.0% |
| BINARY_SUBSCR_TUPLE_INT | 1,000 | 0.0% |
| LOAD_FAST | 600 | 0.0% |
| ENTER_EXECUTOR | 300 | 0.0% |
| STORE_FAST_LOAD_FAST | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,398,800 | 100.0% |
| POP_JUMP_IF_TRUE | 1,040 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 320 | 48.5% |
| RETURN_VALUE | 160 | 24.2% |
| LOAD_FAST | 100 | 15.2% |
| CALL_METHOD_DESCRIPTOR_O | 80 | 12.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 420 | 63.6% |
| STORE_FAST_STORE_FAST | 240 | 36.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_LIST_INT | 12,249,560 | 99.3% |
| RETURN_VALUE | 30,600 | 0.2% |
| FOR_ITER | 25,380 | 0.2% |
| FOR_ITER_LIST | 21,900 | 0.2% |
| ENTER_EXECUTOR | 7,360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 12,249,420 | 99.3% |
| STORE_FAST_STORE_FAST | 76,440 | 0.6% |
| STORE_FAST | 5,500 | 0.0% |
| STORE_NAME | 5,140 | 0.0% |


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
|     deferred | 1,790,520 | 4.0% |
|          hit | 42,921,040 | 96.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 260 | 10.5% |
| Failure | 2,220 | 89.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 880 | 39.6% |
| multiply different types | 640 | 28.8% |
| and int | 360 | 16.2% |
| remainder | 200 | 9.0% |
| or | 120 | 5.4% |
| add different types | 20 | 0.9% |


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
|     deferred | 35,943,320 | 11.9% |
|          hit | 264,968,020 | 88.1% |
|         miss | 10,060 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 6,900 | 39.3% |
| Failure | 10,660 | 60.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 10,600 | 99.4% |
| buffer slice | 40 | 0.4% |
| list slice | 20 | 0.2% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 147,594,480 | 32.6% |
|          hit | 304,286,360 | 67.2% |
|         miss | 39,233,900 | 8.7% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 746,400 | 95.4% |
| Failure | 35,760 | 4.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| init not python | 12,200 | 34.1% |
| meth descr method fastcall keywords | 9,140 | 25.6% |
| no dict | 8,120 | 22.7% |
| meth descr varargs | 5,580 | 15.6% |
| class no vectorcall | 220 | 0.6% |
| cfunc varargs | 180 | 0.5% |
| wrong number arguments | 160 | 0.4% |
| cfunc noargs | 100 | 0.3% |
| code complex parameters | 60 | 0.2% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 546,780 | 0.5% |
|          hit | 116,347,980 | 99.5% |
|         miss | 160 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,340 | 77.0% |
| Failure | 400 | 23.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| list | 320 | 80.0% |
| other | 60 | 15.0% |
| tuple | 20 | 5.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,521,520 | 40.1% |
|          hit | 5,252,280 | 59.8% |
|         miss | 880 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 16.0% |
| Failure | 2,620 | 84.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| reversed list | 900 | 34.4% |
| dict items | 560 | 21.4% |
| ascii string | 320 | 12.2% |
| zip | 200 | 7.6% |
| seq iter | 180 | 6.9% |
| dict keys | 160 | 6.1% |
| dict values | 160 | 6.1% |
| enumerate | 120 | 4.6% |
| map | 20 | 0.8% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 46,628,300 | 8.5% |
|          hit | 502,791,440 | 91.5% |
|         miss | 12,675,100 | 2.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 248,120 | 91.4% |
| Failure | 23,480 | 8.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 17,620 | 75.0% |
| not managed dict | 3,320 | 14.1% |
| method | 720 | 3.1% |
| overridden | 680 | 2.9% |
| module attr not found | 660 | 2.8% |
| non object slot | 320 | 1.4% |
| metaclass attribute | 80 | 0.3% |
| shadowed | 60 | 0.3% |
| class attr simple | 20 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 31,160 | 0.0% |
|        deopt | 80 | 0.0% |
|          hit | 195,673,240 | 100.0% |
|         miss | 26,140 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,900 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|          hit | 80 | 100.0% |


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
|     deferred | 247,200 | 0.1% |
|          hit | 318,035,260 | 99.9% |
|         miss | 244,020 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 10,440 | 97.0% |
| Failure | 320 | 3.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| not in keys | 120 | 37.5% |
| not in dict | 120 | 37.5% |
| overriding descriptor | 80 | 25.0% |


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 35,700,380 | 50.4% |
|          hit | 35,041,380 | 49.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 400 | 1.3% |
| Failure | 29,380 | 98.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 29,340 | 99.9% |
| out of range | 20 | 0.1% |
| bytearray int | 20 | 0.1% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 27,162,040 | 14.8% |
|          hit | 156,364,720 | 84.9% |
|         miss | 23,706,200 | 12.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 449,080 | 72.7% |
| Failure | 168,460 | 27.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 164,260 | 97.5% |
| dict | 3,680 | 2.2% |
| tuple | 440 | 0.3% |
| mapping | 80 | 0.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 320 | 0.0% |
|          hit | 12,337,160 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 320 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 3,752,020,880 | 57.4% |
| Not specialized | 593,887,260 | 9.1% |
| Specialized hits | 2,117,546,500 | 32.4% |
| Specialized misses | 75,899,840 | 1.2% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 147,594,480 | 49.3% |
| LOAD_ATTR | 46,628,300 | 15.6% |
| BINARY_SUBSCR | 35,943,320 | 12.0% |
| STORE_SUBSCR | 35,700,380 | 11.9% |
| TO_BOOL | 27,162,040 | 9.1% |
| FOR_ITER | 3,521,520 | 1.2% |
| BINARY_OP | 1,790,520 | 0.6% |
| COMPARE_OP | 546,780 | 0.2% |
| STORE_ATTR | 247,200 | 0.1% |
| LOAD_GLOBAL | 31,160 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 20,112,200 | 26.5% |
| CALL_BOUND_METHOD_EXACT_ARGS | 19,118,760 | 25.2% |
| TO_BOOL_NONE | 14,206,740 | 18.7% |
| LOAD_ATTR_INSTANCE_VALUE | 11,288,360 | 14.9% |
| TO_BOOL_ALWAYS_TRUE | 9,493,940 | 12.5% |
| LOAD_ATTR_SLOT | 1,289,180 | 1.7% |
| STORE_ATTR_SLOT | 242,780 | 0.3% |
| LOAD_ATTR_WITH_HINT | 96,500 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 15,220 | 0.0% |
| LOAD_GLOBAL_MODULE | 10,920 | 0.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 61,305,860 | 32.1% |
| Calls to Python functions inlined | 129,429,780 | 67.9% |
| Calls via PyEval_EvalFrame (total) | 61,305,860 | 32.1% |
| Calls via PyEval_EvalFrame (vector) | 61,305,380 | 32.1% |
| Calls via PyEval_EvalFrame (generator) | 480 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 520 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 61,304,860 | 32.1% |
| Calls via PyEval_EvalFrame (build class) | 0 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 46,532,980 | 24.4% |
| Calls via PyEval_EvalFrame (function ex) | 440 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 102,700 | 0.1% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 19,800 | 0.0% |
| Frames pushed | 110,774,580 | 58.1% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 85,267,600 | 22.8% |
| Frees to freelist | 85,417,320 |  |
| Allocations | 288,643,480 | 77.2% |
| Allocations to 512 bytes | 251,966,680 | 67.4% |
| Allocations to 4 kbytes | 36,673,000 | 9.8% |
| Allocations over 4 kbytes | 3,800 | 0.0% |
| Frees | 324,891,164 |  |
| New values | 48,025,580 |  |
| Interpreter increfs | 3,954,001,200 | 84.2% |
| Interpreter decrefs | 4,299,175,260 | 85.6% |
| Increfs | 743,130,999 | 15.8% |
| Decrefs | 725,508,837 | 14.4% |
| Materialize dict (on request) | 480 | 0.0% |
| Materialize dict (new key) | 120 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 120 | 0.0% |
| Method cache hits | 67,300,342 |  |
| Method cache misses | 213,718 |  |
| Method cache collisions | 247,221 |  |
| Method cache dunder hits | 118,728,952 |  |
| Method cache dunder misses | 48,388 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 23,340 | 600 | 116,591,480 |
| 1 | 2,140 | 60 | 122,257,480 |
| 2 | 180 | 11,338,080 | 193,066,560 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 2,560 |  |
| Traces created | 3,900 | 152.3% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 69,220 | 2,703.9% |
| Trace too long | 0 | 0.0% |
| Trace too short | 2,062,240 | 80,556.2% |
| Inner loop found | 660 | 25.8% |
| Recursive call | 220 | 8.6% |
| Low confidence | 100 | 3.9% |
| Traces executed | 237,606,560 |  |
| Uops executed | 3,701,468,160 | 15.58 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 140 | 3.6% |
| <= 16 | 280 | 7.2% |
| <= 32 | 1,240 | 31.8% |
| <= 64 | 980 | 25.1% |
| <= 128 | 980 | 25.1% |
| <= 256 | 280 | 7.2% |


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
| <= 128 | 100 | 2.6% |
| <= 256 | 420 | 10.8% |
| <= 512 | 1,080 | 27.7% |
| <= 1,024 | 860 | 22.1% |
| <= 2,048 | 760 | 19.5% |
| <= 4,096 | 160 | 4.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 16,580 | 0.0% |
| <= 4 | 4,543,820 | 1.9% |
| <= 8 | 22,341,180 | 9.4% |
| <= 16 | 95,266,280 | 40.1% |
| <= 32 | 15,380,160 | 6.5% |
| <= 64 | 23,056,140 | 9.7% |
| <= 128 | 10,950,040 | 4.6% |
| <= 256 | 9,840 | 0.0% |
| <= 512 | 1,180 | 0.0% |
| <= 1,024 | 340 | 0.0% |
| <= 2,048 | 500 | 0.0% |
| <= 4,096 | 460 | 0.0% |
| <= 8,192 | 20 | 0.0% |
| <= 16,384 | 300 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 773,530,060 | 20.9% | 20.9% |  |
| _SET_IP | 347,135,500 | 9.4% | 30.3% |  |
| _CHECK_VALIDITY | 312,092,320 | 8.4% | 38.7% | 0.1% |
| STORE_FAST | 247,234,300 | 6.7% | 45.4% |  |
| _GUARD_TYPE_VERSION | 226,543,720 | 6.1% | 51.5% | 1.1% |
| _START_EXECUTOR | 171,566,840 | 4.6% | 56.1% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 126,976,500 | 3.4% | 59.6% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 126,976,500 | 3.4% | 63.0% |  |
| _GUARD_IS_TRUE_POP | 111,673,780 | 3.0% | 66.0% | 9.7% |
| _EXIT_TRACE | 78,945,860 | 2.1% | 68.2% | 100.0% |
| _GUARD_IS_FALSE_POP | 77,156,160 | 2.1% | 70.2% | 46.6% |
| _LOAD_ATTR_METHOD_NO_DICT | 72,960,420 | 2.0% | 72.2% |  |
| CONTAINS_OP | 70,414,020 | 1.9% | 74.1% |  |
| _COLD_EXIT | 66,039,720 | 1.8% | 75.9% |  |
| _CHECK_VALIDITY_AND_SET_IP | 65,222,580 | 1.8% | 77.7% | 31.4% |
| COMPARE_OP_INT | 58,267,840 | 1.6% | 79.2% |  |
| _LOAD_CONST_INLINE_BORROW | 55,247,680 | 1.5% | 80.7% |  |
| BINARY_SUBSCR_DICT | 44,920,160 | 1.2% | 81.9% |  |
| _ITER_CHECK_LIST | 41,538,860 | 1.1% | 83.1% | 0.0% |
| _GUARD_NOT_EXHAUSTED_LIST | 41,534,140 | 1.1% | 84.2% | 7.7% |
| _ITER_NEXT_LIST | 38,347,820 | 1.0% | 85.2% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 37,095,920 | 1.0% | 86.2% |  |
| TO_BOOL_ALWAYS_TRUE | 34,299,480 | 0.9% | 87.1% | 22.7% |
| CALL_METHOD_DESCRIPTOR_FAST | 25,555,080 | 0.7% | 87.8% |  |
| BINARY_SUBSCR_STR_INT | 23,487,580 | 0.6% | 88.5% | 0.0% |
| _GUARD_IS_NOT_NONE_POP | 21,412,900 | 0.6% | 89.1% | 0.0% |
| RESUME_CHECK | 20,976,080 | 0.6% | 89.6% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 20,976,080 | 0.6% | 90.2% |  |
| _CHECK_STACK_SPACE | 20,976,080 | 0.6% | 90.8% |  |
| _INIT_CALL_PY_EXACT_ARGS | 20,976,080 | 0.6% | 91.3% |  |
| _PUSH_FRAME | 20,976,080 | 0.6% | 91.9% |  |
| _SAVE_RETURN_OFFSET | 20,976,080 | 0.6% | 92.5% |  |
| _TO_BOOL | 16,669,440 | 0.5% | 92.9% |  |
| BINARY_SUBSCR_LIST_INT | 15,928,400 | 0.4% | 93.3% |  |
| UNARY_NEGATIVE | 15,908,040 | 0.4% | 93.8% |  |
| _CHECK_GLOBALS | 15,301,940 | 0.4% | 94.2% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 15,207,160 | 0.4% | 94.6% |  |
| GET_ITER | 13,502,360 | 0.4% | 95.0% |  |
| TO_BOOL_NONE | 11,489,180 | 0.3% | 95.3% | 77.1% |
| _GUARD_BOTH_INT | 11,274,060 | 0.3% | 95.6% |  |
| _BINARY_OP_ADD_INT | 11,235,860 | 0.3% | 95.9% |  |
| PUSH_NULL | 11,048,660 | 0.3% | 96.2% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 10,505,160 | 0.3% | 96.5% |  |
| _GUARD_KEYS_VERSION | 10,505,160 | 0.3% | 96.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 10,505,160 | 0.3% | 97.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 10,409,600 | 0.3% | 97.3% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 10,409,600 | 0.3% | 97.6% |  |
| _CHECK_ATTR_WITH_HINT | 10,390,160 | 0.3% | 97.9% |  |
| _LOAD_ATTR_WITH_HINT | 10,390,160 | 0.3% | 98.1% |  |
| TO_BOOL_LIST | 10,384,860 | 0.3% | 98.4% |  |
| _FOR_ITER_TIER_TWO | 6,106,020 | 0.2% | 98.6% | 28.3% |
| _LOAD_CONST_INLINE | 4,499,700 | 0.1% | 98.7% |  |
| _GUARD_GLOBALS_VERSION | 3,877,300 | 0.1% | 98.8% |  |
| _LOAD_GLOBAL_MODULE | 3,704,500 | 0.1% | 98.9% |  |
| _GUARD_IS_NONE_POP | 3,594,760 | 0.1% | 99.0% | 31.5% |
| TO_BOOL_BOOL | 3,540,180 | 0.1% | 99.1% |  |
| _CHECK_ATTR_MODULE | 3,403,740 | 0.1% | 99.2% |  |
| _LOAD_ATTR_MODULE | 3,403,740 | 0.1% | 99.3% |  |
| _LOAD_ATTR | 3,181,380 | 0.1% | 99.4% |  |
| _JUMP_TO_TOP | 3,057,000 | 0.1% | 99.5% |  |
| _CHECK_BUILTINS | 3,025,200 | 0.1% | 99.5% |  |
| CALL_ISINSTANCE | 2,779,540 | 0.1% | 99.6% |  |
| _LOAD_ATTR_SLOT | 2,224,640 | 0.1% | 99.7% |  |
| POP_TOP | 1,970,940 | 0.1% | 99.7% |  |
| SWAP | 1,796,800 | 0.0% | 99.8% |  |
| LOAD_NAME | 1,592,800 | 0.0% | 99.8% |  |
| _STORE_ATTR_SLOT | 941,820 | 0.0% | 99.8% |  |
| _STORE_ATTR | 812,000 | 0.0% | 99.9% |  |
| _BINARY_SUBSCR | 772,120 | 0.0% | 99.9% |  |
| STORE_SUBSCR_DICT | 655,240 | 0.0% | 99.9% |  |
| STORE_NAME | 521,320 | 0.0% | 99.9% |  |
| _LOAD_GLOBAL | 282,480 | 0.0% | 99.9% |  |
| COMPARE_OP_STR | 196,420 | 0.0% | 99.9% |  |
| _LOAD_GLOBAL_BUILTINS | 172,800 | 0.0% | 99.9% |  |
| CALL_LEN | 170,880 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 164,680 | 0.0% | 99.9% |  |
| _GUARD_DORV_VALUES | 164,120 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 164,120 | 0.0% | 100.0% |  |
| _POP_FRAME | 158,440 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 145,860 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 138,720 | 0.0% | 100.0% | 7.8% |
| LIST_APPEND | 137,840 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 130,040 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 116,760 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 93,740 | 0.0% | 100.0% | 2.9% |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 76,000 | 0.0% | 100.0% |  |
| BINARY_SLICE | 74,280 | 0.0% | 100.0% |  |
| IS_OP | 55,180 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 50,600 | 0.0% | 100.0% | 19.4% |
| _ITER_CHECK_RANGE | 50,600 | 0.0% | 100.0% |  |
| _ITER_NEXT_RANGE | 40,760 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 40,340 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 34,140 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 30,700 | 0.0% | 100.0% |  |
| _BINARY_OP | 23,400 | 0.0% | 100.0% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 21,280 | 0.0% | 100.0% | 83.0% |
| _ITER_CHECK_TUPLE | 21,280 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 16,720 | 0.0% | 100.0% | 31.9% |
| CALL_METHOD_DESCRIPTOR_O | 16,200 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 14,760 | 0.0% | 100.0% |  |
| LOAD_FAST_CHECK | 14,620 | 0.0% | 100.0% |  |
| BUILD_MAP | 12,960 | 0.0% | 100.0% |  |
| COPY | 11,580 | 0.0% | 100.0% |  |
| BUILD_LIST | 9,380 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 7,900 | 0.0% | 100.0% |  |
| BUILD_SLICE | 7,240 | 0.0% | 100.0% |  |
| FORMAT_SIMPLE | 5,400 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 5,400 | 0.0% | 100.0% |  |
| UNARY_NOT | 4,220 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 4,200 | 0.0% | 100.0% |  |
| _BINARY_OP_MULTIPLY_INT | 4,060 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 3,620 | 0.0% | 100.0% |  |
| MAKE_FUNCTION | 3,220 | 0.0% | 100.0% |  |
| _COMPARE_OP | 2,940 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 2,820 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 2,820 | 0.0% | 100.0% |  |
| BUILD_STRING | 2,700 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 2,020 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,972,760 |
| CALL_KW | 19,060 |
| CALL_FUNCTION_EX | 2,460 |
| CALL_LIST_APPEND | 520 |
| BINARY_SUBSCR_GETITEM | 80 |
| CALL_PY_WITH_DEFAULTS | 20 |


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
| watched dict modification | 240 |
| watched globals modification | 240 |


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
