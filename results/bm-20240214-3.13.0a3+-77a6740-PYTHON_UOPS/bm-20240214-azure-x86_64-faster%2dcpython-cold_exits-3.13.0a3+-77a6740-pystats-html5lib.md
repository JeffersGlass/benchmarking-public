
# Pystats results

- benchmark: html5lib
- fork: faster-cpython
- ref: cold-exits
- commit hash: 77a6740
- commit date: 2024-02-14T15:57:04+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 101,386,900 | 23.2% | 23.2% |  |
| LOAD_ATTR_INSTANCE_VALUE | 40,572,180 | 9.3% | 32.5% | 0.0% |
| LOAD_CONST | 32,166,920 | 7.4% | 39.8% |  |
| POP_JUMP_IF_FALSE | 28,988,980 | 6.6% | 46.5% |  |
| STORE_FAST | 27,311,300 | 6.2% | 52.7% |  |
| RESUME_CHECK | 15,047,300 | 3.4% | 56.2% | 0.0% |
| BINARY_SUBSCR_DICT | 10,013,420 | 2.3% | 58.5% |  |
| COMPARE_OP_INT | 9,339,920 | 2.1% | 60.6% |  |
| CALL_PY_EXACT_ARGS | 9,037,020 | 2.1% | 62.7% | 28.3% |
| LOAD_GLOBAL_MODULE | 8,997,760 | 2.1% | 64.7% | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 8,587,380 | 2.0% | 66.7% | 0.1% |
| LOAD_FAST_LOAD_FAST | 7,834,620 | 1.8% | 68.5% |  |
| RETURN_VALUE | 7,722,760 | 1.8% | 70.3% |  |
| COMPARE_OP_STR | 7,295,960 | 1.7% | 71.9% | 0.1% |
| TO_BOOL_BOOL | 7,239,680 | 1.7% | 73.6% |  |
| RETURN_CONST | 6,905,900 | 1.6% | 75.2% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,404,080 | 1.5% | 76.6% | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 5,895,240 | 1.3% | 78.0% | 0.1% |
| POP_JUMP_IF_TRUE | 5,420,420 | 1.2% | 79.2% |  |
| JUMP_FORWARD | 4,890,220 | 1.1% | 80.3% |  |
| POP_TOP | 4,684,540 | 1.1% | 81.4% |  |
| CONTAINS_OP | 4,330,420 | 1.0% | 82.4% |  |
| LOAD_GLOBAL_BUILTIN | 4,251,160 | 1.0% | 83.4% |  |
| LOAD_ATTR_SLOT | 3,896,640 | 0.9% | 84.3% | 0.2% |
| ENTER_EXECUTOR | 3,848,480 | 0.9% | 85.1% |  |
| BINARY_OP_ADD_INT | 3,555,420 | 0.8% | 86.0% |  |
| BINARY_SUBSCR_STR_INT | 3,477,400 | 0.8% | 86.8% | 0.9% |
| LOAD_ATTR | 3,447,100 | 0.8% | 87.5% |  |
| BINARY_SUBSCR | 3,346,860 | 0.8% | 88.3% |  |
| EXTENDED_ARG | 2,524,020 | 0.6% | 88.9% |  |
| LOAD_ATTR_PROPERTY | 2,455,760 | 0.6% | 89.4% |  |
| SWAP | 2,213,060 | 0.5% | 90.0% |  |
| COPY | 2,156,860 | 0.5% | 90.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,000,980 | 0.5% | 90.9% | 8.6% |
| BUILD_LIST | 1,863,140 | 0.4% | 91.3% |  |
| CALL_LEN | 1,862,500 | 0.4% | 91.8% |  |
| BINARY_OP_ADD_UNICODE | 1,740,560 | 0.4% | 92.2% |  |
| POP_JUMP_IF_NOT_NONE | 1,518,860 | 0.3% | 92.5% |  |
| TO_BOOL_ALWAYS_TRUE | 1,466,220 | 0.3% | 92.8% | 0.0% |
| STORE_SUBSCR_DICT | 1,433,120 | 0.3% | 93.2% |  |
| POP_JUMP_IF_NONE | 1,391,420 | 0.3% | 93.5% |  |
| TO_BOOL | 1,327,540 | 0.3% | 93.8% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,161,580 | 0.3% | 94.1% | 55.8% |
| CALL_LIST_APPEND | 1,139,600 | 0.3% | 94.3% |  |
| GET_ITER | 1,135,740 | 0.3% | 94.6% |  |
| BUILD_TUPLE | 1,119,560 | 0.3% | 94.8% |  |
| NOP | 1,111,820 | 0.3% | 95.1% |  |
| IS_OP | 1,069,240 | 0.2% | 95.3% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 1,068,960 | 0.2% | 95.6% | 0.4% |
| CALL | 1,050,260 | 0.2% | 95.8% |  |
| COMPARE_OP | 1,036,600 | 0.2% | 96.1% |  |
| CALL_PY_WITH_DEFAULTS | 1,019,700 | 0.2% | 96.3% |  |
| CALL_ISINSTANCE | 996,420 | 0.2% | 96.5% |  |
| TO_BOOL_LIST | 916,420 | 0.2% | 96.7% |  |
| BINARY_SLICE | 771,440 | 0.2% | 96.9% |  |
| BUILD_CONST_KEY_MAP | 756,340 | 0.2% | 97.1% |  |
| CALL_BUILTIN_CLASS | 740,800 | 0.2% | 97.2% |  |
| FOR_ITER_LIST | 738,560 | 0.2% | 97.4% |  |
| STORE_ATTR | 725,460 | 0.2% | 97.6% |  |
| JUMP_BACKWARD | 700,820 | 0.2% | 97.7% |  |
| LOAD_FAST_CHECK | 694,020 | 0.2% | 97.9% |  |
| YIELD_VALUE | 691,760 | 0.2% | 98.1% |  |
| FOR_ITER_GEN | 691,740 | 0.2% | 98.2% |  |
| FOR_ITER | 524,000 | 0.1% | 98.3% |  |
| STORE_FAST_STORE_FAST | 469,360 | 0.1% | 98.4% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 467,440 | 0.1% | 98.5% |  |
| BINARY_SUBSCR_LIST_INT | 465,440 | 0.1% | 98.7% | 0.1% |
| PUSH_NULL | 463,920 | 0.1% | 98.8% |  |
| STORE_SUBSCR_LIST_INT | 448,960 | 0.1% | 98.9% |  |
| FORMAT_SIMPLE | 445,840 | 0.1% | 99.0% |  |
| CONVERT_VALUE | 445,760 | 0.1% | 99.1% |  |
| BUILD_SLICE | 380,740 | 0.1% | 99.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 371,140 | 0.1% | 99.2% |  |
| CALL_BUILTIN_FAST | 316,980 | 0.1% | 99.3% | 0.1% |
| BINARY_OP_SUBTRACT_INT | 265,460 | 0.1% | 99.4% |  |
| TO_BOOL_INT | 259,600 | 0.1% | 99.4% |  |
| INTERPRETER_EXIT | 259,040 | 0.1% | 99.5% |  |
| CALL_KW | 250,040 | 0.1% | 99.5% |  |
| TO_BOOL_NONE | 242,420 | 0.1% | 99.6% | 7.8% |
| LOAD_ATTR_MODULE | 228,480 | 0.1% | 99.7% | 0.1% |
| LOAD_DEREF | 225,640 | 0.1% | 99.7% |  |
| COPY_FREE_VARS | 224,900 | 0.1% | 99.8% |  |
| EXIT_INIT_CHECK | 224,520 | 0.1% | 99.8% |  |
| CALL_ALLOC_AND_ENTER_INIT | 224,520 | 0.1% | 99.9% |  |
| BUILD_STRING | 222,920 | 0.1% | 99.9% |  |
| BINARY_OP | 102,300 | 0.0% | 99.9% |  |
| LOAD_ATTR_CLASS | 88,420 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 25,960 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 21,800 | 0.0% | 100.0% | 73.5% |
| CALL_BUILTIN_O | 18,500 | 0.0% | 100.0% |  |
| FOR_ITER_RANGE | 15,180 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 9,940 | 0.0% | 100.0% |  |
| STORE_NAME | 9,740 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 8,000 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 7,880 | 0.0% | 100.0% |  |
| STORE_ATTR_SLOT | 7,580 | 0.0% | 100.0% | 91.8% |
| MAKE_FUNCTION | 7,080 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 6,940 | 0.0% | 100.0% | 1.7% |
| LOAD_NAME | 6,520 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 5,660 | 0.0% | 100.0% |  |
| BUILD_MAP | 5,640 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 4,940 | 0.0% | 100.0% |  |
| RESUME | 4,280 | 0.0% | 100.0% | 15.9% |
| BINARY_OP_INPLACE_ADD_UNICODE | 4,220 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 4,100 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 2,200 | 0.0% | 100.0% |  |
| MAP_ADD | 2,180 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 1,740 | 0.0% | 100.0% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 1,700 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,520 | 0.0% | 100.0% |  |
| CALL_FUNCTION_EX | 920 | 0.0% | 100.0% |  |
| SET_FUNCTION_ATTRIBUTE | 900 | 0.0% | 100.0% |  |
| CALL_TYPE_1 | 880 | 0.0% | 100.0% |  |
| DICT_MERGE | 840 | 0.0% | 100.0% |  |
| CHECK_EXC_MATCH | 820 | 0.0% | 100.0% |  |
| POP_EXCEPT | 820 | 0.0% | 100.0% |  |
| PUSH_EXC_INFO | 820 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 700 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 640 | 0.0% | 100.0% |  |
| UNARY_NOT | 620 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 600 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 560 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 480 | 0.0% | 100.0% |  |
| MAKE_CELL | 460 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 400 | 0.0% | 100.0% |  |
| BEFORE_WITH | 360 | 0.0% | 100.0% |  |
| IMPORT_FROM | 360 | 0.0% | 100.0% |  |
| IMPORT_NAME | 340 | 0.0% | 100.0% |  |
| LOAD_LOCALS | 320 | 0.0% | 100.0% |  |
| LOAD_FROM_DICT_OR_DEREF | 320 | 0.0% | 100.0% |  |
| STORE_DEREF | 240 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 200 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 180 | 0.0% | 100.0% |  |
| RETURN_GENERATOR | 160 | 0.0% | 100.0% |  |
| UNARY_INVERT | 160 | 0.0% | 100.0% |  |
| LIST_EXTEND | 160 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 140 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 140 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 120 | 0.0% | 100.0% |  |
| CALL_STR_1 | 120 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 120 | 0.0% | 100.0% |  |
| STORE_SLICE | 80 | 0.0% | 100.0% |  |
| END_FOR | 80 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 60 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 40 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 40 | 0.0% | 100.0% |  |
| DICT_UPDATE | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 34,508,900 | 7.9% | 7.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 21,042,560 | 4.8% | 12.7% |
| STORE_FAST LOAD_FAST | 19,687,720 | 4.5% | 17.2% |
| LOAD_FAST LOAD_CONST | 15,971,340 | 3.7% | 20.9% |
| RESUME_CHECK LOAD_FAST | 12,726,440 | 2.9% | 23.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_FAST | 9,746,100 | 2.2% | 26.0% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 8,988,100 | 2.1% | 28.1% |
| LOAD_CONST BINARY_SUBSCR_DICT | 8,020,780 | 1.8% | 29.9% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 7,766,240 | 1.8% | 31.7% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 7,273,040 | 1.7% | 33.3% |
| COMPARE_OP_STR POP_JUMP_IF_FALSE | 6,490,960 | 1.5% | 34.8% |
| LOAD_CONST COMPARE_OP_STR | 6,170,900 | 1.4% | 36.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 5,503,560 | 1.3% | 37.5% |
| LOAD_ATTR_INSTANCE_VALUE STORE_FAST | 4,574,660 | 1.0% | 38.6% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 4,552,080 | 1.0% | 39.6% |
| RETURN_VALUE STORE_FAST | 4,503,400 | 1.0% | 40.6% |
| LOAD_FAST RETURN_VALUE | 4,457,680 | 1.0% | 41.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 4,279,540 | 1.0% | 42.6% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST | 4,117,160 | 0.9% | 43.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 4,022,900 | 0.9% | 44.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 3,994,280 | 0.9% | 45.4% |
| LOAD_ATTR_INSTANCE_VALUE COMPARE_OP_INT | 3,992,240 | 0.9% | 46.3% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_CONST | 3,905,600 | 0.9% | 47.2% |
| RETURN_CONST TO_BOOL_BOOL | 3,768,220 | 0.9% | 48.1% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 3,682,320 | 0.8% | 48.9% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,553,520 | 0.8% | 49.7% |
| LOAD_CONST BINARY_OP_ADD_INT | 3,552,940 | 0.8% | 50.5% |
| BINARY_SUBSCR_STR_INT STORE_FAST | 3,458,760 | 0.8% | 51.3% |
| BINARY_OP_ADD_INT LOAD_FAST | 3,458,700 | 0.8% | 52.1% |
| LOAD_FAST BINARY_SUBSCR_STR_INT | 3,443,560 | 0.8% | 52.9% |
| POP_JUMP_IF_FALSE ENTER_EXECUTOR | 3,442,140 | 0.8% | 53.7% |
| LOAD_FAST LOAD_ATTR_SLOT | 3,200,060 | 0.7% | 54.4% |
| LOAD_GLOBAL_MODULE CONTAINS_OP | 3,091,180 | 0.7% | 55.1% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 2,931,680 | 0.7% | 55.8% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_INSTANCE_VALUE | 2,769,420 | 0.6% | 56.4% |
| LOAD_CONST BINARY_SUBSCR | 2,699,000 | 0.6% | 57.1% |
| LOAD_ATTR LOAD_FAST | 2,679,740 | 0.6% | 57.7% |
| BINARY_SUBSCR_DICT STORE_FAST | 2,622,540 | 0.6% | 58.3% |
| STORE_ATTR_INSTANCE_VALUE RETURN_CONST | 2,579,860 | 0.6% | 58.9% |
| LOAD_FAST_LOAD_FAST COMPARE_OP_INT | 2,553,880 | 0.6% | 59.4% |
| LOAD_FAST LOAD_ATTR | 2,521,360 | 0.6% | 60.0% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 2,456,200 | 0.6% | 60.6% |
| LOAD_ATTR_PROPERTY RESUME_CHECK | 2,455,760 | 0.6% | 61.1% |
| POP_TOP LOAD_FAST | 2,393,340 | 0.5% | 61.7% |
| ENTER_EXECUTOR CALL_PY_EXACT_ARGS | 2,276,420 | 0.5% | 62.2% |
| LOAD_FAST LOAD_ATTR_PROPERTY | 2,187,440 | 0.5% | 62.7% |
| LOAD_GLOBAL_MODULE LOAD_CONST | 2,112,960 | 0.5% | 63.2% |
| JUMP_FORWARD STORE_FAST | 2,075,280 | 0.5% | 63.7% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,954,000 | 0.4% | 64.1% |
| POP_JUMP_IF_TRUE LOAD_FAST | 1,952,620 | 0.4% | 64.6% |
| RETURN_CONST POP_TOP | 1,907,300 | 0.4% | 65.0% |
| POP_TOP RETURN_CONST | 1,900,100 | 0.4% | 65.4% |
| STORE_FAST JUMP_FORWARD | 1,877,140 | 0.4% | 65.9% |
| LOAD_CONST LOAD_CONST | 1,862,020 | 0.4% | 66.3% |
| LOAD_CONST STORE_FAST | 1,777,840 | 0.4% | 66.7% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 1,728,900 | 0.4% | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 1,670,960 | 0.4% | 67.5% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 1,659,980 | 0.4% | 67.9% |
| BINARY_SUBSCR_DICT LOAD_FAST | 1,655,680 | 0.4% | 68.2% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 1,635,800 | 0.4% | 68.6% |
| LOAD_ATTR_SLOT LOAD_ATTR_INSTANCE_VALUE | 1,621,640 | 0.4% | 69.0% |
| JUMP_FORWARD LOAD_FAST | 1,550,960 | 0.4% | 69.3% |
| LOAD_FAST STORE_FAST | 1,527,900 | 0.3% | 69.7% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,517,900 | 0.3% | 70.0% |
| COMPARE_OP_INT POP_JUMP_IF_TRUE | 1,489,140 | 0.3% | 70.4% |
| LOAD_FAST TO_BOOL_BOOL | 1,476,000 | 0.3% | 70.7% |
| TO_BOOL_ALWAYS_TRUE POP_JUMP_IF_FALSE | 1,466,220 | 0.3% | 71.1% |
| LOAD_FAST TO_BOOL_ALWAYS_TRUE | 1,466,160 | 0.3% | 71.4% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 1,417,820 | 0.3% | 71.7% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 1,409,460 | 0.3% | 72.0% |
| STORE_FAST LOAD_CONST | 1,389,400 | 0.3% | 72.4% |
| RETURN_VALUE JUMP_FORWARD | 1,383,480 | 0.3% | 72.7% |
| BINARY_SUBSCR_DICT LOAD_GLOBAL_MODULE | 1,307,160 | 0.3% | 73.0% |
| POP_JUMP_IF_NOT_NONE LOAD_FAST | 1,293,200 | 0.3% | 73.3% |
| LOAD_ATTR_SLOT LOAD_ATTR_METHOD_WITH_VALUES | 1,246,080 | 0.3% | 73.5% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,235,840 | 0.3% | 73.8% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 1,219,200 | 0.3% | 74.1% |
| LOAD_CONST LOAD_FAST | 1,210,300 | 0.3% | 74.4% |
| BINARY_OP_ADD_UNICODE SWAP | 1,190,620 | 0.3% | 74.7% |
| CALL_BOUND_METHOD_EXACT_ARGS RESUME_CHECK | 1,148,460 | 0.3% | 74.9% |
| CALL_LEN LOAD_CONST | 1,129,200 | 0.3% | 75.2% |
| POP_JUMP_IF_TRUE LOAD_FAST_LOAD_FAST | 1,120,620 | 0.3% | 75.4% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL | 1,093,860 | 0.3% | 75.7% |
| BINARY_SUBSCR_DICT LOAD_CONST | 1,091,180 | 0.2% | 75.9% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 1,072,720 | 0.2% | 76.2% |
| IS_OP POP_JUMP_IF_FALSE | 1,068,860 | 0.2% | 76.4% |
| LOAD_GLOBAL_MODULE IS_OP | 1,068,400 | 0.2% | 76.7% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 1,019,500 | 0.2% | 76.9% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,013,100 | 0.2% | 77.1% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 995,340 | 0.2% | 77.4% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 990,460 | 0.2% | 77.6% |
| LOAD_CONST COMPARE_OP_INT | 985,620 | 0.2% | 77.8% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 933,360 | 0.2% | 78.0% |
| LOAD_CONST COPY | 932,460 | 0.2% | 78.2% |
| COPY COPY | 931,760 | 0.2% | 78.5% |
| SWAP SWAP | 931,760 | 0.2% | 78.7% |
| TO_BOOL POP_JUMP_IF_FALSE | 920,780 | 0.2% | 78.9% |
| TO_BOOL_LIST POP_JUMP_IF_FALSE | 905,920 | 0.2% | 79.1% |
| LOAD_FAST BINARY_OP_ADD_UNICODE | 894,620 | 0.2% | 79.3% |
| BINARY_SUBSCR_DICT COMPARE_OP_INT | 871,440 | 0.2% | 79.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 530,140 | 68.7% |
| LOAD_CONST | 237,060 | 30.7% |
| BINARY_OP_ADD_INT | 4,160 | 0.5% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 529,680 | 68.7% |
| GET_ITER | 228,400 | 29.6% |
| CALL_METHOD_DESCRIPTOR_O | 4,080 | 0.5% |
| RETURN_VALUE | 3,200 | 0.4% |
| STORE_FAST | 2,120 | 0.3% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 257,380 | 99.2% |
| RESUME | 940 | 0.4% |
| COPY_FREE_VARS | 880 | 0.3% |
| POP_TOP | 100 | 0.0% |
| RETURN_GENERATOR | 80 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 160 | 44.4% |
| RETURN_VALUE | 80 | 22.2% |
| LOAD_ATTR_INSTANCE_VALUE | 80 | 22.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 11.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 320 | 88.9% |
| STORE_FAST | 40 | 11.1% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 2,040 | 48.3% |
| RETURN_VALUE | 1,400 | 33.2% |
| ENTER_EXECUTOR | 340 | 8.1% |
| LOAD_FAST_LOAD_FAST | 340 | 8.1% |
| BINARY_OP | 80 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 2,060 | 48.8% |
| LOAD_GLOBAL_BUILTIN | 1,300 | 30.8% |
| LOAD_FAST | 840 | 19.9% |
| LOAD_GLOBAL | 20 | 0.5% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,699,000 | 80.6% |
| BUILD_SLICE | 380,740 | 11.4% |
| LOAD_FAST | 260,520 | 7.8% |
| BINARY_SUBSCR | 6,140 | 0.2% |
| COPY | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 691,760 | 20.7% |
| STORE_FAST | 600,240 | 17.9% |
| LOAD_CONST | 599,780 | 17.9% |
| GET_ITER | 380,560 | 11.4% |
| LOAD_ATTR_PROPERTY | 265,400 | 7.9% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 780 | 95.1% |
| LOAD_GLOBAL | 40 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 820 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 40 | 100.0% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 80 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 224,520 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 224,520 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONVERT_VALUE | 445,760 | 100.0% |
| LOAD_FAST | 40 | 0.0% |
| LOAD_ATTR_MODULE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_STRING | 222,920 | 50.0% |
| LOAD_CONST | 222,920 | 50.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 380,560 | 33.5% |
| CALL_BUILTIN_CLASS | 378,500 | 33.3% |
| BINARY_SLICE | 228,400 | 20.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 142,120 | 12.5% |
| LOAD_FAST | 3,680 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 548,920 | 48.3% |
| FOR_ITER | 519,780 | 45.8% |
| EXTENDED_ARG | 63,040 | 5.6% |
| FOR_ITER_TUPLE | 1,760 | 0.2% |
| FOR_ITER_RANGE | 1,540 | 0.1% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 236,680 | 91.4% |
| RETURN_VALUE | 22,180 | 8.6% |
| YIELD_VALUE | 100 | 0.0% |
| RETURN_GENERATOR | 80 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 440 | 68.8% |
| STORE_DEREF | 160 | 25.0% |
| STORE_NAME | 20 | 3.1% |
| RESUME | 20 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 640 | 100.0% |


</details>

### LOAD_LOCALS

<details>
<summary> Successors and predecessors for LOAD_LOCALS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 62.5% |
| STORE_NAME | 120 | 37.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FROM_DICT_OR_DEREF | 320 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,080 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 5,900 | 83.3% |
| SET_FUNCTION_ATTRIBUTE | 880 | 12.4% |
| LOAD_CONST | 260 | 3.7% |
| STORE_FAST | 40 | 0.6% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 554,920 | 49.9% |
| RESUME_CHECK | 550,220 | 49.5% |
| JUMP_FORWARD | 2,240 | 0.2% |
| POP_JUMP_IF_TRUE | 1,300 | 0.1% |
| POP_JUMP_IF_FALSE | 780 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 557,740 | 50.2% |
| LOAD_GLOBAL_MODULE | 552,660 | 49.7% |
| NOP | 540 | 0.0% |
| LOAD_CONST | 220 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 200 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 260 | 31.7% |
| STORE_ATTR_INSTANCE_VALUE | 260 | 31.7% |
| STORE_FAST | 160 | 19.5% |
| STORE_SUBSCR_DICT | 100 | 12.2% |
| STORE_SUBSCR | 20 | 2.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 260 | 31.7% |
| RETURN_CONST | 260 | 31.7% |
| EXTENDED_ARG | 200 | 24.4% |
| JUMP_BACKWARD_NO_INTERRUPT | 80 | 9.8% |
| RETURN_VALUE | 20 | 2.4% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,907,300 | 40.7% |
| CALL_METHOD_DESCRIPTOR_O | 860,820 | 18.4% |
| RESUME_CHECK | 691,740 | 14.8% |
| POP_JUMP_IF_FALSE | 293,660 | 6.3% |
| CALL | 225,800 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,393,340 | 51.1% |
| RETURN_CONST | 1,900,100 | 40.6% |
| LOAD_FAST_LOAD_FAST | 223,540 | 4.8% |
| RETURN_VALUE | 84,680 | 1.8% |
| JUMP_FORWARD | 72,700 | 1.6% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 440 | 53.7% |
| BINARY_SUBSCR_STR_INT | 260 | 31.7% |
| ENTER_EXECUTOR | 80 | 9.8% |
| BINARY_SUBSCR | 40 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 760 | 92.7% |
| LOAD_GLOBAL | 60 | 7.3% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 457,640 | 98.6% |
| LOAD_ATTR_MODULE | 2,020 | 0.4% |
| LOAD_ATTR | 1,420 | 0.3% |
| STORE_FAST_LOAD_FAST | 760 | 0.2% |
| LOAD_BUILD_CLASS | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 447,780 | 96.5% |
| LOAD_GLOBAL_MODULE | 7,740 | 1.7% |
| LOAD_CONST | 4,420 | 1.0% |
| LOAD_FAST_LOAD_FAST | 1,920 | 0.4% |
| CALL | 880 | 0.2% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 80 | 50.0% |
| COPY_FREE_VARS | 80 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 80 | 50.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 80 | 50.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,457,680 | 57.7% |
| LOAD_ATTR_INSTANCE_VALUE | 2,456,200 | 31.8% |
| RETURN_CONST | 435,920 | 5.6% |
| EXIT_INIT_CHECK | 224,520 | 2.9% |
| POP_TOP | 84,680 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 4,503,400 | 58.3% |
| JUMP_FORWARD | 1,383,480 | 17.9% |
| LOAD_FAST | 422,160 | 5.5% |
| BINARY_OP_ADD_UNICODE | 379,280 | 4.9% |
| TO_BOOL_BOOL | 280,960 | 3.6% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 34.5% |
| LOAD_FAST | 500 | 28.7% |
| SWAP | 360 | 20.7% |
| BINARY_OP | 220 | 12.6% |
| BUILD_TUPLE | 40 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 24.1% |
| RETURN_CONST | 360 | 20.7% |
| STORE_SUBSCR_DICT | 360 | 20.7% |
| EXTENDED_ARG | 240 | 13.8% |
| LOAD_CONST | 120 | 6.9% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,093,860 | 82.4% |
| LOAD_FAST | 226,920 | 17.1% |
| COPY | 2,680 | 0.2% |
| TO_BOOL | 1,460 | 0.1% |
| LOAD_ATTR | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 920,780 | 69.4% |
| POP_JUMP_IF_TRUE | 403,500 | 30.4% |
| TO_BOOL | 1,460 | 0.1% |
| TO_BOOL_BOOL | 1,360 | 0.1% |
| TO_BOOL_NONE | 240 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 160 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 180 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 360 | 58.1% |
| TO_BOOL_LIST | 260 | 41.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 360 | 58.1% |
| CALL_PY_EXACT_ARGS | 260 | 41.9% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 86,160 | 84.2% |
| LOAD_CONST | 5,100 | 5.0% |
| LOAD_GLOBAL_MODULE | 3,840 | 3.8% |
| LOAD_FAST | 2,620 | 2.6% |
| BINARY_OP | 1,360 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 86,120 | 84.2% |
| COMPARE_OP | 4,120 | 4.0% |
| STORE_FAST | 3,140 | 3.1% |
| TO_BOOL_INT | 3,100 | 3.0% |
| BINARY_OP | 1,360 | 1.3% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 756,340 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 436,160 | 57.7% |
| CALL_METHOD_DESCRIPTOR_O | 255,200 | 33.7% |
| STORE_FAST | 64,360 | 8.5% |
| CALL | 320 | 0.0% |
| RETURN_VALUE | 280 | 0.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 634,860 | 34.1% |
| STORE_ATTR_INSTANCE_VALUE | 447,300 | 24.0% |
| LOAD_FAST | 435,380 | 23.4% |
| LOAD_CONST | 337,900 | 18.1% |
| RETURN_VALUE | 2,480 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 640,060 | 34.4% |
| LOAD_CONST | 628,760 | 33.7% |
| LOAD_FAST | 448,460 | 24.1% |
| CALL_LIST_APPEND | 143,880 | 7.7% |
| CALL | 920 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 3,640 | 64.5% |
| STORE_ATTR_INSTANCE_VALUE | 520 | 9.2% |
| LOAD_FAST | 380 | 6.7% |
| BUILD_TUPLE | 320 | 5.7% |
| POP_JUMP_IF_NOT_NONE | 240 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,040 | 89.4% |
| STORE_FAST | 400 | 7.1% |
| SWAP | 80 | 1.4% |
| LOAD_DEREF | 60 | 1.1% |
| CALL | 20 | 0.4% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 380,740 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR | 380,740 | 100.0% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 222,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 222,920 | 100.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 553,700 | 49.5% |
| LOAD_FAST | 320,720 | 28.6% |
| LOAD_ATTR_INSTANCE_VALUE | 223,080 | 19.9% |
| BUILD_TUPLE | 6,140 | 0.5% |
| CALL_BUILTIN_O | 5,620 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 549,900 | 49.1% |
| STORE_FAST | 318,780 | 28.5% |
| LOAD_FAST | 224,120 | 20.0% |
| BUILD_TUPLE | 6,140 | 0.5% |
| CALL_BUILTIN_O | 5,600 | 0.5% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 780,140 | 74.3% |
| RETURN_VALUE | 224,700 | 21.4% |
| LOAD_FAST | 13,600 | 1.3% |
| LOAD_FAST_LOAD_FAST | 9,060 | 0.9% |
| ENTER_EXECUTOR | 5,560 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 557,980 | 53.1% |
| POP_TOP | 225,800 | 21.5% |
| LOAD_FAST | 224,040 | 21.3% |
| RETURN_VALUE | 17,380 | 1.7% |
| TO_BOOL_BOOL | 5,160 | 0.5% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 840 | 91.3% |
| LOAD_FAST | 80 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 280 | 30.4% |
| POP_TOP | 240 | 26.1% |
| COPY_FREE_VARS | 160 | 17.4% |
| RESUME_CHECK | 100 | 10.9% |
| LOAD_FAST | 80 | 8.7% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 140 | 100.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 250,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 249,860 | 99.9% |
| STORE_FAST | 120 | 0.0% |
| RESUME | 60 | 0.0% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 460,020 | 44.4% |
| LOAD_FAST | 374,540 | 36.1% |
| LOAD_FAST_LOAD_FAST | 85,700 | 8.3% |
| BINARY_SUBSCR | 84,700 | 8.2% |
| LOAD_ATTR_INSTANCE_VALUE | 18,860 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 746,500 | 72.0% |
| POP_JUMP_IF_TRUE | 284,280 | 27.4% |
| COMPARE_OP | 2,900 | 0.3% |
| COMPARE_OP_STR | 1,880 | 0.2% |
| COMPARE_OP_INT | 920 | 0.1% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,091,180 | 71.4% |
| LOAD_ATTR_SLOT | 435,960 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 432,920 | 10.0% |
| LOAD_FAST | 151,440 | 3.5% |
| CALL_BUILTIN_CLASS | 137,260 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,022,900 | 92.9% |
| POP_JUMP_IF_TRUE | 218,480 | 5.0% |
| BINARY_OP | 86,160 | 2.0% |
| RETURN_VALUE | 2,240 | 0.1% |
| EXTENDED_ARG | 600 | 0.0% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 445,760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 445,760 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 932,460 | 43.2% |
| COPY | 931,760 | 43.2% |
| BINARY_SUBSCR | 165,800 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 92,720 | 4.3% |
| COMPARE_OP_STR | 18,780 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 931,760 | 43.2% |
| BINARY_SUBSCR_DICT | 627,320 | 29.1% |
| BINARY_SUBSCR_LIST_INT | 304,080 | 14.1% |
| LOAD_ATTR | 255,880 | 11.9% |
| TO_BOOL_BOOL | 19,120 | 0.9% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ALLOC_AND_ENTER_INIT | 223,340 | 99.3% |
| CACHE | 880 | 0.4% |
| CALL_PY_WITH_DEFAULTS | 200 | 0.1% |
| CALL | 180 | 0.1% |
| CALL_FUNCTION_EX | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 224,180 | 99.7% |
| RESUME | 600 | 0.3% |
| RETURN_GENERATOR | 80 | 0.0% |
| MAKE_CELL | 40 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 840 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 840 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_CONST_KEY_MAP | 20 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 20 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 3,442,140 | 89.4% |
| POP_JUMP_IF_TRUE | 210,300 | 5.5% |
| STORE_SUBSCR_DICT | 141,560 | 3.7% |
| JUMP_FORWARD | 17,980 | 0.5% |
| TO_BOOL_LIST | 9,760 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,276,420 | 59.2% |
| YIELD_VALUE | 691,360 | 18.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 464,920 | 12.1% |
| RETURN_CONST | 149,000 | 3.9% |
| FOR_ITER_LIST | 123,860 | 3.2% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 691,700 | 27.4% |
| LOAD_FAST | 691,680 | 27.4% |
| POP_JUMP_IF_TRUE | 691,680 | 27.4% |
| STORE_FAST | 152,200 | 6.0% |
| STORE_ATTR_INSTANCE_VALUE | 143,900 | 5.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 692,040 | 27.4% |
| FOR_ITER_GEN | 691,720 | 27.4% |
| POP_JUMP_IF_NONE | 691,680 | 27.4% |
| JUMP_FORWARD | 296,880 | 11.8% |
| POP_JUMP_IF_FALSE | 87,340 | 3.5% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 519,780 | 99.2% |
| JUMP_BACKWARD | 1,960 | 0.4% |
| EXTENDED_ARG | 1,000 | 0.2% |
| FOR_ITER | 980 | 0.2% |
| SWAP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 378,480 | 72.2% |
| UNPACK_SEQUENCE_TWO_TUPLE | 142,860 | 27.3% |
| FOR_ITER | 980 | 0.2% |
| RETURN_CONST | 540 | 0.1% |
| LOAD_FAST | 300 | 0.1% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 280 | 77.8% |
| STORE_NAME | 80 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 280 | 77.8% |
| STORE_FAST | 80 | 22.2% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 340 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 280 | 82.4% |
| STORE_NAME | 60 | 17.6% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,068,400 | 99.9% |
| LOAD_FAST | 300 | 0.0% |
| LOAD_GLOBAL | 260 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 260 | 0.0% |
| LOAD_DEREF | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,068,860 | 100.0% |
| POP_JUMP_IF_TRUE | 380 | 0.0% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 692,040 | 98.7% |
| POP_JUMP_IF_TRUE | 3,940 | 0.6% |
| POP_JUMP_IF_FALSE | 1,860 | 0.3% |
| CALL_LIST_APPEND | 960 | 0.1% |
| STORE_SUBSCR_DICT | 380 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 691,700 | 98.7% |
| FOR_ITER_LIST | 2,380 | 0.3% |
| FOR_ITER | 1,960 | 0.3% |
| FOR_ITER_TUPLE | 1,620 | 0.2% |
| LOAD_FAST | 1,540 | 0.2% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 120 | 60.0% |
| POP_EXCEPT | 80 | 40.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 120 | 60.0% |
| LOAD_FAST | 80 | 40.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,877,140 | 38.4% |
| RETURN_VALUE | 1,383,480 | 28.3% |
| BINARY_SUBSCR | 691,760 | 14.1% |
| STORE_ATTR_INSTANCE_VALUE | 529,580 | 10.8% |
| EXTENDED_ARG | 296,880 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,075,280 | 42.4% |
| LOAD_FAST | 1,550,960 | 31.7% |
| LOAD_FAST_LOAD_FAST | 692,320 | 14.2% |
| LOAD_CONST | 550,000 | 11.2% |
| ENTER_EXECUTOR | 17,980 | 0.4% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 660 | 43.4% |
| BINARY_OP | 440 | 28.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 240 | 15.8% |
| CALL_BUILTIN_CLASS | 180 | 11.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 620 | 40.8% |
| ENTER_EXECUTOR | 520 | 34.2% |
| JUMP_BACKWARD | 340 | 22.4% |
| CALL | 20 | 1.3% |
| LOAD_NAME | 20 | 1.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140 | 87.5% |
| LOAD_CONST | 20 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 140 | 87.5% |
| CALL | 20 | 12.5% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,521,360 | 73.1% |
| LOAD_ATTR_INSTANCE_VALUE | 484,200 | 14.0% |
| COPY | 255,880 | 7.4% |
| BINARY_SUBSCR | 166,360 | 4.8% |
| LOAD_ATTR | 11,640 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,679,740 | 77.7% |
| LOAD_FAST_LOAD_FAST | 244,180 | 7.1% |
| TO_BOOL_NONE | 236,200 | 6.9% |
| STORE_FAST | 226,640 | 6.6% |
| TO_BOOL_STR | 19,240 | 0.6% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,971,340 | 49.7% |
| LOAD_ATTR_INSTANCE_VALUE | 3,905,600 | 12.1% |
| LOAD_GLOBAL_MODULE | 2,112,960 | 6.6% |
| LOAD_CONST | 1,862,020 | 5.8% |
| STORE_FAST | 1,389,400 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 8,020,780 | 24.9% |
| COMPARE_OP_STR | 6,170,900 | 19.2% |
| BINARY_OP_ADD_INT | 3,552,940 | 11.0% |
| BINARY_SUBSCR | 2,699,000 | 8.4% |
| LOAD_CONST | 1,862,020 | 5.8% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 223,100 | 98.9% |
| LOAD_CONST | 640 | 0.3% |
| RESUME_CHECK | 600 | 0.3% |
| POP_JUMP_IF_FALSE | 200 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 200 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 223,360 | 99.0% |
| LOAD_FAST | 620 | 0.3% |
| CALL | 580 | 0.3% |
| LOAD_ATTR | 360 | 0.2% |
| PUSH_NULL | 220 | 0.1% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 21,042,560 | 20.8% |
| STORE_FAST | 19,687,720 | 19.4% |
| RESUME_CHECK | 12,726,440 | 12.6% |
| LOAD_ATTR_INSTANCE_VALUE | 9,746,100 | 9.6% |
| STORE_ATTR_INSTANCE_VALUE | 4,117,160 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 34,508,900 | 34.0% |
| LOAD_CONST | 15,971,340 | 15.8% |
| STORE_ATTR_INSTANCE_VALUE | 7,273,040 | 7.2% |
| LOAD_GLOBAL_MODULE | 4,552,080 | 4.5% |
| RETURN_VALUE | 4,457,680 | 4.4% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 620 | 88.6% |
| LOAD_FAST_AND_CLEAR | 80 | 11.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 620 | 88.6% |
| LOAD_FAST_AND_CLEAR | 80 | 11.4% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 691,680 | 99.7% |
| LOAD_FAST | 2,120 | 0.3% |
| POP_TOP | 160 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 0.0% |
| POP_JUMP_IF_NOT_NONE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 691,720 | 99.7% |
| LOAD_CONST | 2,080 | 0.3% |
| POP_JUMP_IF_NOT_NONE | 160 | 0.0% |
| CALL_LIST_APPEND | 40 | 0.0% |
| TO_BOOL_BOOL | 20 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,954,000 | 24.9% |
| POP_JUMP_IF_FALSE | 1,635,800 | 20.9% |
| POP_JUMP_IF_TRUE | 1,120,620 | 14.3% |
| JUMP_FORWARD | 692,320 | 8.8% |
| LOAD_GLOBAL_MODULE | 561,000 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 2,553,880 | 32.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,659,980 | 21.2% |
| STORE_ATTR_INSTANCE_VALUE | 1,235,840 | 15.8% |
| LOAD_ATTR_SLOT | 689,860 | 8.8% |
| BUILD_TUPLE | 553,700 | 7.1% |


</details>

### LOAD_FROM_DICT_OR_DEREF

<details>
<summary> Successors and predecessors for LOAD_FROM_DICT_OR_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_LOCALS | 320 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 200 | 62.5% |
| STORE_NAME | 120 | 37.5% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,600 | 26.2% |
| STORE_FAST | 880 | 8.9% |
| POP_JUMP_IF_FALSE | 840 | 8.5% |
| LOAD_ATTR | 640 | 6.4% |
| RESUME | 580 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,080 | 31.0% |
| LOAD_GLOBAL_BUILTIN | 1,800 | 18.1% |
| LOAD_FAST | 1,640 | 16.5% |
| CONTAINS_OP | 760 | 7.6% |
| LOAD_CONST | 740 | 7.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,440 | 37.4% |
| STORE_NAME | 1,860 | 28.5% |
| LOAD_NAME | 960 | 14.7% |
| RESUME | 640 | 9.8% |
| STORE_ATTR | 340 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,440 | 37.4% |
| LOAD_NAME | 960 | 14.7% |
| LOAD_ATTR | 860 | 13.2% |
| STORE_ATTR | 720 | 11.0% |
| STORE_NAME | 640 | 9.8% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 40 | 33.3% |
| LOAD_SUPER_ATTR_ATTR | 40 | 33.3% |
| CALL | 20 | 16.7% |
| LOAD_SUPER_ATTR_METHOD | 20 | 16.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 260 | 56.5% |
| CALL_PY_EXACT_ARGS | 80 | 17.4% |
| CALL | 40 | 8.7% |
| CALL_FUNCTION_EX | 40 | 8.7% |
| COPY_FREE_VARS | 40 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 260 | 56.5% |
| RESUME | 120 | 26.1% |
| RESUME_CHECK | 80 | 17.4% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,840 | 84.4% |
| LOAD_FAST | 300 | 13.8% |
| LOAD_DEREF | 40 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,500 | 68.8% |
| JUMP_BACKWARD | 340 | 15.6% |
| LOAD_CONST | 320 | 14.7% |
| LOAD_FAST | 20 | 0.9% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 7,766,240 | 26.8% |
| COMPARE_OP_STR | 6,490,960 | 22.4% |
| TO_BOOL_BOOL | 5,503,560 | 19.0% |
| CONTAINS_OP | 4,022,900 | 13.9% |
| TO_BOOL_ALWAYS_TRUE | 1,466,220 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 21,042,560 | 72.6% |
| ENTER_EXECUTOR | 3,442,140 | 11.9% |
| LOAD_FAST_LOAD_FAST | 1,635,800 | 5.6% |
| RETURN_CONST | 1,013,100 | 3.5% |
| LOAD_GLOBAL_MODULE | 761,860 | 2.6% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 698,100 | 50.2% |
| EXTENDED_ARG | 691,680 | 49.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,180 | 0.1% |
| BINARY_SUBSCR_TUPLE_INT | 240 | 0.0% |
| BINARY_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 696,420 | 50.1% |
| LOAD_FAST_CHECK | 691,680 | 49.7% |
| LOAD_FAST_LOAD_FAST | 880 | 0.1% |
| LOAD_CONST | 600 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 480 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,517,900 | 99.9% |
| LOAD_ATTR_INSTANCE_VALUE | 400 | 0.0% |
| CALL_BUILTIN_FAST | 240 | 0.0% |
| LOAD_FAST_CHECK | 160 | 0.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,293,200 | 85.1% |
| LOAD_CONST | 223,040 | 14.7% |
| LOAD_GLOBAL_MODULE | 1,060 | 0.1% |
| BUILD_LIST | 360 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 280 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 1,728,900 | 31.9% |
| COMPARE_OP_INT | 1,489,140 | 27.5% |
| COMPARE_OP_STR | 781,320 | 14.4% |
| TO_BOOL | 403,500 | 7.4% |
| COMPARE_OP | 284,280 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,952,620 | 36.0% |
| LOAD_FAST_LOAD_FAST | 1,120,620 | 20.7% |
| EXTENDED_ARG | 691,680 | 12.8% |
| LOAD_GLOBAL_BUILTIN | 658,140 | 12.1% |
| LOAD_GLOBAL_MODULE | 313,140 | 5.8% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 2,579,860 | 37.4% |
| POP_TOP | 1,900,100 | 27.5% |
| POP_JUMP_IF_FALSE | 1,013,100 | 14.7% |
| STORE_SUBSCR_DICT | 627,120 | 9.1% |
| STORE_ATTR | 258,180 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 3,768,220 | 54.6% |
| POP_TOP | 1,907,300 | 27.6% |
| RETURN_VALUE | 435,920 | 6.3% |
| STORE_FAST | 332,340 | 4.8% |
| INTERPRETER_EXIT | 236,680 | 3.4% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 880 | 97.8% |
| SET_FUNCTION_ATTRIBUTE | 20 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 380 | 42.2% |
| STORE_NAME | 300 | 33.3% |
| STORE_FAST | 80 | 8.9% |
| LOAD_GLOBAL_MODULE | 80 | 8.9% |
| CALL | 20 | 2.2% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 256,080 | 35.3% |
| LOAD_FAST | 228,960 | 31.6% |
| BINARY_SUBSCR | 147,680 | 20.4% |
| LOAD_ATTR_INSTANCE_VALUE | 88,100 | 12.1% |
| LOAD_FAST_LOAD_FAST | 1,640 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 460,360 | 63.5% |
| RETURN_CONST | 258,180 | 35.6% |
| STORE_ATTR_INSTANCE_VALUE | 3,460 | 0.5% |
| STORE_ATTR | 1,500 | 0.2% |
| LOAD_CONST | 500 | 0.1% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 160 | 66.7% |
| BUILD_MAP | 20 | 8.3% |
| LOAD_ATTR | 20 | 8.3% |
| LOAD_DEREF | 20 | 8.3% |
| SET_FUNCTION_ATTRIBUTE | 20 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_BUILD_CLASS | 160 | 66.7% |
| LOAD_FAST | 60 | 25.0% |
| LOAD_DEREF | 20 | 8.3% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 4,574,660 | 16.8% |
| RETURN_VALUE | 4,503,400 | 16.5% |
| BINARY_SUBSCR_STR_INT | 3,458,760 | 12.7% |
| BINARY_SUBSCR_DICT | 2,622,540 | 9.6% |
| JUMP_FORWARD | 2,075,280 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,687,720 | 72.1% |
| LOAD_FAST_LOAD_FAST | 1,954,000 | 7.2% |
| JUMP_FORWARD | 1,877,140 | 6.9% |
| LOAD_CONST | 1,389,400 | 5.1% |
| LOAD_GLOBAL_BUILTIN | 827,320 | 3.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 6,880 | 87.3% |
| CALL_LEN | 760 | 9.6% |
| FOR_ITER_TUPLE | 240 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 3,760 | 47.7% |
| STORE_ATTR_INSTANCE_VALUE | 3,000 | 38.1% |
| PUSH_NULL | 760 | 9.6% |
| TO_BOOL_STR | 240 | 3.0% |
| LOAD_ATTR | 80 | 1.0% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 465,860 | 99.3% |
| UNPACK_SEQUENCE_LIST | 2,200 | 0.5% |
| COPY | 600 | 0.1% |
| UNPACK_SEQUENCE_TUPLE | 460 | 0.1% |
| UNPACK_SEQUENCE | 180 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 455,440 | 97.0% |
| LOAD_FAST | 5,480 | 1.2% |
| LOAD_GLOBAL_MODULE | 4,980 | 1.1% |
| LOAD_FAST_LOAD_FAST | 2,480 | 0.5% |
| STORE_FAST | 400 | 0.1% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 5,900 | 60.6% |
| CALL | 1,420 | 14.6% |
| LOAD_CONST | 820 | 8.4% |
| LOAD_NAME | 640 | 6.6% |
| SET_FUNCTION_ATTRIBUTE | 300 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,900 | 70.8% |
| LOAD_NAME | 1,860 | 19.1% |
| RETURN_CONST | 280 | 2.9% |
| LOAD_FAST | 220 | 2.3% |
| POP_TOP | 200 | 2.1% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 1,190,620 | 53.8% |
| SWAP | 931,760 | 42.1% |
| LOAD_FAST | 85,700 | 3.9% |
| BINARY_OP_SUBTRACT_INT | 2,380 | 0.1% |
| LOAD_FAST_AND_CLEAR | 620 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 931,760 | 42.1% |
| STORE_SUBSCR_DICT | 627,320 | 28.3% |
| STORE_SUBSCR_LIST_INT | 304,080 | 13.7% |
| STORE_ATTR | 256,080 | 11.6% |
| POP_TOP | 84,600 | 3.8% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 160 | 40.0% |
| FOR_ITER_LIST | 60 | 15.0% |
| RETURN_VALUE | 40 | 10.0% |
| BINARY_SUBSCR | 20 | 5.0% |
| CALL | 20 | 5.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 180 | 45.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 180 | 45.0% |
| LOAD_FAST | 20 | 5.0% |
| UNPACK_SEQUENCE_LIST | 20 | 5.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 691,360 | 99.9% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 300 | 0.0% |
| CALL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 691,660 | 100.0% |
| INTERPRETER_EXIT | 100 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 1,360 | 31.8% |
| CACHE | 940 | 22.0% |
| CALL_BOUND_METHOD_EXACT_ARGS | 760 | 17.8% |
| COPY_FREE_VARS | 600 | 14.0% |
| CALL_PY_EXACT_ARGS | 380 | 8.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,360 | 55.1% |
| LOAD_NAME | 640 | 15.0% |
| LOAD_GLOBAL | 580 | 13.6% |
| LOAD_CONST | 220 | 5.1% |
| LOAD_FAST_LOAD_FAST | 220 | 5.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 3,552,940 | 99.9% |
| LOAD_FAST | 1,200 | 0.0% |
| CALL_LEN | 480 | 0.0% |
| BINARY_OP_MULTIPLY_INT | 320 | 0.0% |
| BINARY_OP | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,458,700 | 97.3% |
| STORE_FAST | 87,640 | 2.5% |
| BINARY_SLICE | 4,160 | 0.1% |
| COPY | 3,020 | 0.1% |
| BINARY_OP_SUBTRACT_INT | 1,080 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 894,620 | 51.4% |
| RETURN_VALUE | 379,280 | 21.8% |
| BINARY_OP_ADD_UNICODE | 295,760 | 17.0% |
| LOAD_FAST_LOAD_FAST | 170,280 | 9.8% |
| BINARY_OP | 540 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 1,190,620 | 68.4% |
| BINARY_OP_ADD_UNICODE | 295,760 | 17.0% |
| LOAD_CONST | 253,820 | 14.6% |
| LOAD_FAST | 160 | 0.0% |
| BINARY_OP | 80 | 0.0% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_TUPLE_INT | 320 | 53.3% |
| LOAD_CONST | 200 | 33.3% |
| LOAD_ATTR | 80 | 13.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_INT | 320 | 53.3% |
| LOAD_CONST | 100 | 16.7% |
| CALL_BUILTIN_O | 100 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 80 | 13.3% |


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
| LOAD_CONST | 262,740 | 99.0% |
| LOAD_FAST | 1,080 | 0.4% |
| BINARY_OP_ADD_INT | 1,080 | 0.4% |
| CALL_LEN | 480 | 0.2% |
| BINARY_OP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 260,600 | 98.2% |
| SWAP | 2,380 | 0.9% |
| LOAD_FAST_LOAD_FAST | 760 | 0.3% |
| LOAD_FAST | 740 | 0.3% |
| RETURN_VALUE | 480 | 0.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,020,780 | 80.1% |
| LOAD_FAST | 748,680 | 7.5% |
| COPY | 627,320 | 6.3% |
| BUILD_TUPLE | 549,900 | 5.5% |
| BINARY_SUBSCR_DICT | 64,280 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,622,540 | 26.2% |
| LOAD_FAST | 1,655,680 | 16.5% |
| LOAD_GLOBAL_MODULE | 1,307,160 | 13.1% |
| LOAD_CONST | 1,091,180 | 10.9% |
| COMPARE_OP_INT | 871,440 | 8.7% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,560 | 94.5% |
| ENTER_EXECUTOR | 380 | 4.8% |
| BINARY_SUBSCR | 60 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,000 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 304,080 | 65.3% |
| LOAD_CONST | 153,760 | 33.0% |
| LOAD_FAST | 7,200 | 1.5% |
| BINARY_SUBSCR | 260 | 0.1% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 306,360 | 65.9% |
| LOAD_ATTR_METHOD_NO_DICT | 148,800 | 32.0% |
| LOAD_GLOBAL_MODULE | 4,080 | 0.9% |
| RETURN_VALUE | 2,300 | 0.5% |
| LOAD_CONST | 2,100 | 0.5% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,443,560 | 99.0% |
| ENTER_EXECUTOR | 20,940 | 0.6% |
| LOAD_CONST | 9,940 | 0.3% |
| LOAD_ATTR_INSTANCE_VALUE | 2,360 | 0.1% |
| BINARY_SUBSCR_STR_INT | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 3,458,760 | 99.5% |
| LOAD_CONST | 15,400 | 0.4% |
| LOAD_FAST | 2,380 | 0.1% |
| BINARY_SUBSCR_STR_INT | 560 | 0.0% |
| PUSH_EXC_INFO | 260 | 0.0% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 25,700 | 99.0% |
| BINARY_SUBSCR | 260 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 11,760 | 45.3% |
| STORE_FAST | 11,380 | 43.8% |
| CALL_BUILTIN_O | 960 | 3.7% |
| LOAD_CONST | 380 | 1.5% |
| BINARY_OP_MULTIPLY_INT | 320 | 1.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 222,880 | 99.3% |
| LOAD_FAST | 460 | 0.2% |
| BINARY_SUBSCR_DICT | 280 | 0.1% |
| LOAD_GLOBAL_MODULE | 260 | 0.1% |
| BINARY_SUBSCR | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY_FREE_VARS | 223,340 | 99.5% |
| RESUME_CHECK | 1,180 | 0.5% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 561,940 | 48.4% |
| ENTER_EXECUTOR | 464,920 | 40.0% |
| LOAD_ATTR_INSTANCE_VALUE | 118,260 | 10.2% |
| CALL_PY_EXACT_ARGS | 12,180 | 1.0% |
| LOAD_CONST | 2,600 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,148,460 | 98.9% |
| CALL_PY_EXACT_ARGS | 12,200 | 1.1% |
| RESUME | 760 | 0.1% |
| POP_TOP | 160 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 376,720 | 50.9% |
| LOAD_FAST | 223,180 | 30.1% |
| LOAD_CONST | 138,840 | 18.7% |
| CALL_LEN | 1,160 | 0.2% |
| CALL_BUILTIN_FAST | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 378,500 | 51.1% |
| STORE_FAST | 223,040 | 30.1% |
| CONTAINS_OP | 137,260 | 18.5% |
| BUILD_TUPLE | 1,320 | 0.2% |
| RETURN_VALUE | 280 | 0.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 312,920 | 98.7% |
| LOAD_FAST | 1,820 | 0.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,040 | 0.3% |
| ENTER_EXECUTOR | 280 | 0.1% |
| LOAD_FAST_LOAD_FAST | 260 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 314,020 | 99.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 1,020 | 0.3% |
| POP_TOP | 440 | 0.1% |
| TO_BOOL_BOOL | 400 | 0.1% |
| CALL_BUILTIN_CLASS | 280 | 0.1% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,220 | 75.2% |
| LOAD_GLOBAL_MODULE | 1,200 | 17.3% |
| CALL_TUPLE_1 | 260 | 3.7% |
| LOAD_CONST | 120 | 1.7% |
| RETURN_GENERATOR | 80 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 5,180 | 74.6% |
| BUILD_TUPLE | 600 | 8.6% |
| LOAD_GLOBAL_BUILTIN | 600 | 8.6% |
| RETURN_VALUE | 500 | 7.2% |
| BEFORE_WITH | 40 | 0.6% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,960 | 43.0% |
| BUILD_TUPLE | 5,600 | 30.3% |
| LOAD_GLOBAL_MODULE | 1,300 | 7.0% |
| BINARY_SUBSCR | 1,080 | 5.8% |
| BINARY_SUBSCR_TUPLE_INT | 960 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 10,900 | 58.9% |
| BUILD_TUPLE | 5,620 | 30.4% |
| STORE_FAST | 1,100 | 5.9% |
| BINARY_OP | 420 | 2.3% |
| LOAD_CONST | 420 | 2.3% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 535,800 | 53.8% |
| LOAD_GLOBAL_BUILTIN | 458,020 | 46.0% |
| BUILD_TUPLE | 1,700 | 0.2% |
| CALL | 260 | 0.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 995,340 | 99.9% |
| RETURN_VALUE | 520 | 0.1% |
| LOAD_FAST | 260 | 0.0% |
| TO_BOOL | 240 | 0.0% |
| STORE_FAST | 60 | 0.0% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,219,200 | 65.5% |
| LOAD_FAST | 632,580 | 34.0% |
| LOAD_ATTR | 3,960 | 0.2% |
| LOAD_ATTR_SLOT | 3,960 | 0.2% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,080 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,129,200 | 60.6% |
| TO_BOOL_INT | 255,520 | 13.7% |
| COMPARE_OP_INT | 234,860 | 12.6% |
| LOAD_GLOBAL_BUILTIN | 227,540 | 12.2% |
| RETURN_VALUE | 5,860 | 0.3% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SLICE | 529,680 | 46.5% |
| LOAD_FAST | 447,300 | 39.3% |
| BUILD_LIST | 143,880 | 12.6% |
| RETURN_VALUE | 7,600 | 0.7% |
| ENTER_EXECUTOR | 7,500 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 598,820 | 52.5% |
| LOAD_FAST_LOAD_FAST | 529,280 | 46.4% |
| ENTER_EXECUTOR | 8,720 | 0.8% |
| JUMP_BACKWARD | 960 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 840 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 754,000 | 70.5% |
| LOAD_ATTR_INSTANCE_VALUE | 226,680 | 21.2% |
| LOAD_FAST | 86,020 | 8.0% |
| LOAD_CONST | 700 | 0.1% |
| CALL | 640 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 990,460 | 92.7% |
| LOAD_FAST | 61,460 | 5.7% |
| POP_TOP | 10,520 | 1.0% |
| RETURN_VALUE | 3,820 | 0.4% |
| CALL_PY_EXACT_ARGS | 2,280 | 0.2% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,760 | 67.3% |
| LOAD_FAST | 1,080 | 26.3% |
| LOAD_GLOBAL_MODULE | 180 | 4.4% |
| CALL | 80 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,340 | 57.1% |
| CALL_LEN | 1,080 | 26.3% |
| RETURN_VALUE | 240 | 5.9% |
| LOAD_ATTR_METHOD_NO_DICT | 240 | 5.9% |
| LOAD_CONST | 180 | 4.4% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 370,700 | 99.9% |
| CALL | 320 | 0.1% |
| LOAD_ATTR_METHOD_LAZY_DICT | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 222,860 | 60.0% |
| GET_ITER | 142,120 | 38.3% |
| LOAD_FAST | 2,580 | 0.7% |
| COMPARE_OP_STR | 2,520 | 0.7% |
| YIELD_VALUE | 300 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,072,720 | 53.6% |
| LOAD_GLOBAL_MODULE | 579,640 | 29.0% |
| BUILD_CONST_KEY_MAP | 255,200 | 12.8% |
| LOAD_FAST_LOAD_FAST | 84,440 | 4.2% |
| BINARY_SLICE | 4,080 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 860,820 | 43.0% |
| LOAD_FAST | 579,700 | 29.0% |
| STORE_FAST | 549,840 | 27.5% |
| CALL_PY_EXACT_ARGS | 4,400 | 0.2% |
| CALL_METHOD_DESCRIPTOR_O | 3,240 | 0.2% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_WITH_VALUES | 4,279,540 | 47.4% |
| ENTER_EXECUTOR | 2,276,420 | 25.2% |
| LOAD_FAST | 1,417,820 | 15.7% |
| LOAD_ATTR_INSTANCE_VALUE | 575,460 | 6.4% |
| LOAD_CONST | 304,280 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 8,988,100 | 99.5% |
| CALL_PY_EXACT_ARGS | 36,140 | 0.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 12,180 | 0.1% |
| RESUME | 380 | 0.0% |
| COPY_FREE_VARS | 140 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 313,960 | 30.8% |
| BINARY_SUBSCR_DICT | 265,040 | 26.0% |
| LOAD_FAST | 258,400 | 25.3% |
| RETURN_VALUE | 168,880 | 16.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 12,480 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,019,500 | 100.0% |
| COPY_FREE_VARS | 200 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 66.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 33.3% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 62.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 80 | 16.7% |
| CALL | 60 | 12.5% |
| LOAD_GLOBAL_MODULE | 40 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 260 | 54.2% |
| BUILD_TUPLE | 60 | 12.5% |
| STORE_FAST | 60 | 12.5% |
| CALL | 40 | 8.3% |
| LOAD_GLOBAL_BUILTIN | 40 | 8.3% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 780 | 88.6% |
| LOAD_CONST | 40 | 4.5% |
| LOAD_GLOBAL_MODULE | 40 | 4.5% |
| CALL | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 520 | 59.1% |
| LOAD_FAST | 260 | 29.5% |
| PUSH_NULL | 40 | 4.5% |
| CALL_ISINSTANCE | 40 | 4.5% |
| CALL | 20 | 2.3% |


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
| LOAD_ATTR_INSTANCE_VALUE | 3,992,240 | 42.7% |
| LOAD_FAST_LOAD_FAST | 2,553,880 | 27.3% |
| LOAD_CONST | 985,620 | 10.6% |
| BINARY_SUBSCR_DICT | 871,440 | 9.3% |
| LOAD_FAST | 699,100 | 7.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 7,766,240 | 83.2% |
| POP_JUMP_IF_TRUE | 1,489,140 | 15.9% |
| EXTENDED_ARG | 84,460 | 0.9% |
| RETURN_VALUE | 40 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,170,900 | 84.6% |
| LOAD_ATTR_INSTANCE_VALUE | 694,260 | 9.5% |
| BINARY_SUBSCR_DICT | 252,440 | 3.5% |
| LOAD_FAST | 89,120 | 1.2% |
| LOAD_FAST_LOAD_FAST | 65,300 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,490,960 | 89.0% |
| POP_JUMP_IF_TRUE | 781,320 | 10.7% |
| COPY | 18,780 | 0.3% |
| STORE_FAST | 2,580 | 0.0% |
| EXTENDED_ARG | 2,160 | 0.0% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 691,720 | 100.0% |
| FOR_ITER | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 691,660 | 100.0% |
| POP_TOP | 60 | 0.0% |
| RESUME | 20 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 548,920 | 74.3% |
| ENTER_EXECUTOR | 123,860 | 16.8% |
| EXTENDED_ARG | 63,240 | 8.6% |
| JUMP_BACKWARD | 2,380 | 0.3% |
| FOR_ITER | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 268,260 | 36.3% |
| LOAD_FAST | 228,700 | 31.0% |
| LOAD_GLOBAL_BUILTIN | 170,160 | 23.0% |
| RETURN_CONST | 65,660 | 8.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,000 | 0.4% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 13,360 | 88.0% |
| GET_ITER | 1,540 | 10.1% |
| SWAP | 180 | 1.2% |
| JUMP_BACKWARD | 80 | 0.5% |
| FOR_ITER | 20 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_FORWARD | 11,400 | 75.1% |
| LOAD_FAST | 1,780 | 11.7% |
| RETURN_CONST | 1,100 | 7.2% |
| STORE_FAST | 640 | 4.2% |
| SWAP | 180 | 1.2% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 1,760 | 35.6% |
| JUMP_BACKWARD | 1,620 | 32.8% |
| ENTER_EXECUTOR | 1,220 | 24.7% |
| SWAP | 240 | 4.9% |
| FOR_ITER | 100 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 2,740 | 55.5% |
| ENTER_EXECUTOR | 600 | 12.1% |
| UNPACK_SEQUENCE_TWO_TUPLE | 520 | 10.5% |
| JUMP_BACKWARD | 340 | 6.9% |
| LOAD_FAST | 240 | 4.9% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 88,240 | 99.8% |
| LOAD_GLOBAL_MODULE | 120 | 0.1% |
| LOAD_ATTR | 60 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 88,280 | 99.8% |
| LOAD_FAST | 140 | 0.2% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 34,508,900 | 85.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,769,420 | 6.8% |
| LOAD_FAST_LOAD_FAST | 1,659,980 | 4.1% |
| LOAD_ATTR_SLOT | 1,621,640 | 4.0% |
| LOAD_ATTR | 6,340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,746,100 | 24.0% |
| STORE_FAST | 4,574,660 | 11.3% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,994,280 | 9.8% |
| COMPARE_OP_INT | 3,992,240 | 9.8% |
| LOAD_CONST | 3,905,600 | 9.6% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,800 | 67.1% |
| LOAD_ATTR_INSTANCE_VALUE | 1,340 | 23.7% |
| LOAD_FAST | 320 | 5.7% |
| LOAD_ATTR | 200 | 3.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,220 | 92.2% |
| LOAD_CONST | 300 | 5.3% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 120 | 2.1% |
| CALL | 20 | 0.4% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,931,680 | 49.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,670,960 | 28.3% |
| BINARY_SUBSCR_DICT | 582,240 | 9.9% |
| LOAD_CONST | 556,480 | 9.4% |
| BINARY_SUBSCR_LIST_INT | 148,800 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,682,320 | 62.5% |
| LOAD_GLOBAL_MODULE | 836,060 | 14.2% |
| CALL_METHOD_DESCRIPTOR_FAST | 754,000 | 12.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 370,700 | 6.3% |
| LOAD_CONST | 230,140 | 3.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 3,994,280 | 62.4% |
| LOAD_ATTR_SLOT | 1,246,080 | 19.5% |
| LOAD_FAST | 933,360 | 14.6% |
| BINARY_SUBSCR | 222,860 | 3.5% |
| LOAD_GLOBAL_MODULE | 4,440 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 4,279,540 | 66.8% |
| LOAD_FAST | 1,409,460 | 22.0% |
| LOAD_CONST | 464,000 | 7.2% |
| LOAD_GLOBAL_MODULE | 235,960 | 3.7% |
| CALL_PY_WITH_DEFAULTS | 12,480 | 0.2% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_DEREF | 223,360 | 97.8% |
| LOAD_GLOBAL_MODULE | 4,460 | 2.0% |
| LOAD_ATTR | 380 | 0.2% |
| LOAD_FAST | 240 | 0.1% |
| RETURN_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 223,780 | 97.9% |
| PUSH_NULL | 2,020 | 0.9% |
| CALL | 660 | 0.3% |
| LOAD_CONST | 540 | 0.2% |
| LOAD_ATTR_SLOT | 360 | 0.2% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,420 | 83.5% |
| LOAD_FAST_LOAD_FAST | 260 | 15.3% |
| LOAD_ATTR | 20 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,180 | 69.4% |
| CALL_ISINSTANCE | 260 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 260 | 15.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,187,440 | 89.1% |
| BINARY_SUBSCR | 265,400 | 10.8% |
| LOAD_FAST_LOAD_FAST | 940 | 0.0% |
| LOAD_ATTR | 720 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,455,760 | 100.0% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,200,060 | 82.1% |
| LOAD_FAST_LOAD_FAST | 689,860 | 17.7% |
| STORE_FAST_LOAD_FAST | 3,760 | 0.1% |
| LOAD_ATTR | 2,460 | 0.1% |
| LOAD_ATTR_MODULE | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,621,640 | 41.6% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,246,080 | 32.0% |
| LOAD_FAST | 519,900 | 13.3% |
| CONTAINS_OP | 435,960 | 11.2% |
| STORE_ATTR_INSTANCE_VALUE | 65,520 | 1.7% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 827,320 | 19.5% |
| POP_JUMP_IF_FALSE | 696,560 | 16.4% |
| POP_JUMP_IF_TRUE | 658,140 | 15.5% |
| LOAD_FAST | 605,900 | 14.3% |
| RESUME_CHECK | 584,200 | 13.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,553,520 | 83.6% |
| CALL_ISINSTANCE | 458,020 | 10.8% |
| LOAD_CONST | 137,960 | 3.2% |
| LOAD_ATTR_CLASS | 88,240 | 2.1% |
| LOAD_GLOBAL_BUILTIN | 5,400 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,552,080 | 50.6% |
| BINARY_SUBSCR_DICT | 1,307,160 | 14.5% |
| LOAD_ATTR_METHOD_NO_DICT | 836,060 | 9.3% |
| POP_JUMP_IF_FALSE | 761,860 | 8.5% |
| NOP | 552,660 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 3,091,180 | 34.4% |
| LOAD_CONST | 2,112,960 | 23.5% |
| IS_OP | 1,068,400 | 11.9% |
| CALL_METHOD_DESCRIPTOR_O | 579,640 | 6.4% |
| LOAD_FAST_LOAD_FAST | 561,000 | 6.2% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 66.7% |
| LOAD_SUPER_ATTR | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 120 | 100.0% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120 | 85.7% |
| LOAD_SUPER_ATTR | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 57.1% |
| CALL | 60 | 42.9% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 8,988,100 | 59.7% |
| LOAD_ATTR_PROPERTY | 2,455,760 | 16.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 1,148,460 | 7.6% |
| CALL_PY_WITH_DEFAULTS | 1,019,500 | 6.8% |
| FOR_ITER_GEN | 691,660 | 4.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,726,440 | 84.6% |
| POP_TOP | 691,740 | 4.6% |
| LOAD_GLOBAL_BUILTIN | 584,200 | 3.9% |
| NOP | 550,220 | 3.7% |
| LOAD_FAST_LOAD_FAST | 243,580 | 1.6% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,273,040 | 84.7% |
| LOAD_FAST_LOAD_FAST | 1,235,840 | 14.4% |
| LOAD_ATTR_SLOT | 65,520 | 0.8% |
| SWAP | 5,780 | 0.1% |
| STORE_ATTR | 3,460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,117,160 | 47.9% |
| RETURN_CONST | 2,579,860 | 30.0% |
| JUMP_FORWARD | 529,580 | 6.2% |
| BUILD_LIST | 447,300 | 5.2% |
| LOAD_CONST | 294,740 | 3.4% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,720 | 49.1% |
| LOAD_FAST_LOAD_FAST | 3,640 | 48.0% |
| STORE_ATTR | 140 | 1.8% |
| STORE_ATTR_SLOT | 80 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 3,640 | 48.0% |
| RETURN_CONST | 1,940 | 25.6% |
| LOAD_FAST_LOAD_FAST | 1,820 | 24.0% |
| STORE_ATTR_SLOT | 80 | 1.1% |
| BUILD_LIST | 60 | 0.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 658,800 | 46.0% |
| SWAP | 627,320 | 43.8% |
| LOAD_FAST | 146,480 | 10.2% |
| STORE_SUBSCR | 360 | 0.0% |
| BUILD_TUPLE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 659,660 | 46.0% |
| RETURN_CONST | 627,120 | 43.8% |
| ENTER_EXECUTOR | 141,560 | 9.9% |
| LOAD_GLOBAL_BUILTIN | 4,020 | 0.3% |
| JUMP_BACKWARD | 380 | 0.0% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 304,080 | 67.7% |
| LOAD_CONST | 143,880 | 32.0% |
| LOAD_FAST_LOAD_FAST | 800 | 0.2% |
| STORE_SUBSCR | 100 | 0.0% |
| LOAD_FAST | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160,200 | 35.7% |
| RETURN_CONST | 144,320 | 32.1% |
| LOAD_FAST | 143,900 | 32.1% |
| ENTER_EXECUTOR | 540 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,466,160 | 100.0% |
| TO_BOOL_NONE | 40 | 0.0% |
| TO_BOOL | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,466,220 | 100.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,768,220 | 52.0% |
| LOAD_FAST | 1,476,000 | 20.4% |
| CALL_ISINSTANCE | 995,340 | 13.7% |
| BINARY_SUBSCR_DICT | 435,680 | 6.0% |
| RETURN_VALUE | 280,960 | 3.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 5,503,560 | 76.0% |
| POP_JUMP_IF_TRUE | 1,728,900 | 23.9% |
| ENTER_EXECUTOR | 7,160 | 0.1% |
| EXTENDED_ARG | 60 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 255,520 | 98.4% |
| BINARY_OP | 3,100 | 1.2% |
| LOAD_FAST | 720 | 0.3% |
| COPY | 200 | 0.1% |
| CALL_BUILTIN_O | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 256,400 | 98.8% |
| POP_JUMP_IF_FALSE | 2,840 | 1.1% |
| UNARY_NOT | 360 | 0.1% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 692,460 | 75.6% |
| BINARY_SUBSCR_DICT | 212,920 | 23.2% |
| LOAD_FAST | 10,960 | 1.2% |
| TO_BOOL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 905,920 | 98.9% |
| ENTER_EXECUTOR | 9,760 | 1.1% |
| POP_JUMP_IF_TRUE | 480 | 0.1% |
| UNARY_NOT | 260 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 236,200 | 97.4% |
| LOAD_FAST | 3,280 | 1.4% |
| LOAD_ATTR_INSTANCE_VALUE | 2,320 | 1.0% |
| TO_BOOL_STR | 300 | 0.1% |
| TO_BOOL | 240 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 236,360 | 97.5% |
| POP_JUMP_IF_FALSE | 5,680 | 2.3% |
| TO_BOOL_STR | 300 | 0.1% |
| ENTER_EXECUTOR | 40 | 0.0% |
| TO_BOOL_ALWAYS_TRUE | 40 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 19,240 | 88.3% |
| LOAD_FAST | 1,440 | 6.6% |
| COPY | 400 | 1.8% |
| TO_BOOL_NONE | 300 | 1.4% |
| STORE_FAST_LOAD_FAST | 240 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 21,180 | 97.2% |
| POP_JUMP_IF_FALSE | 320 | 1.5% |
| TO_BOOL_NONE | 300 | 1.4% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,180 | 99.1% |
| UNPACK_SEQUENCE | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 2,200 | 100.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 320 | 57.1% |
| LOAD_FAST | 160 | 28.6% |
| CALL_METHOD_DESCRIPTOR_O | 80 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 460 | 82.1% |
| STORE_FAST | 100 | 17.9% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_SUBSCR_DICT | 312,440 | 66.8% |
| FOR_ITER | 142,860 | 30.6% |
| LOAD_ATTR_INSTANCE_VALUE | 4,920 | 1.1% |
| FOR_ITER_LIST | 3,000 | 0.6% |
| RETURN_VALUE | 2,320 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 465,860 | 99.7% |
| LOAD_FAST | 1,180 | 0.3% |
| STORE_FAST | 400 | 0.1% |


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
|     deferred | 100,120 | 1.8% |
|          hit | 5,566,320 | 98.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,000 | 45.9% |
| Failure | 1,180 | 54.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| multiply different types | 300 | 25.4% |
| xor | 220 | 18.6% |
| and int | 180 | 15.3% |
| remainder | 160 | 13.6% |
| add other | 140 | 11.9% |
| or | 100 | 8.5% |
| add different types | 40 | 3.4% |
| and different types | 20 | 1.7% |
| floor divide | 20 | 1.7% |


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
|     deferred | 3,369,020 | 19.4% |
|          hit | 13,958,520 | 80.5% |
|         miss | 31,700 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,420 | 35.8% |
| Failure | 6,120 | 64.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 4,280 | 69.9% |
| buffer int | 960 | 15.7% |
| buffer slice | 660 | 10.8% |
| list slice | 220 | 3.6% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 4,363,120 | 20.1% |
|          hit | 17,281,540 | 79.6% |
|         miss | 3,386,160 | 15.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 70,700 | 96.5% |
| Failure | 2,600 | 3.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 700 | 26.9% |
| meth descr method fastcall keywords | 580 | 22.3% |
| class no vectorcall | 440 | 16.9% |
| operator wrapper | 220 | 8.5% |
| code complex parameters | 180 | 6.9% |
| metaclass | 160 | 6.2% |
| no dict | 100 | 3.8% |
| out of versions | 60 | 2.3% |
| cfunc noargs | 60 | 2.3% |
| class mutable | 60 | 2.3% |
| str | 40 | 1.5% |
| other | 20 | 0.8% |
| cfunc varargs | 20 | 0.8% |
| cfunc varargs keywords | 20 | 0.8% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,040,740 | 5.9% |
|          hit | 16,625,920 | 94.1% |
|         miss | 10,000 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,800 | 47.8% |
| Failure | 3,060 | 52.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| different types | 1,300 | 42.5% |
| baseobject | 660 | 21.6% |
| tuple | 420 | 13.7% |
| long float | 260 | 8.5% |
| bytes | 240 | 7.8% |
| other | 120 | 3.9% |
| big int | 60 | 2.0% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 522,720 | 26.5% |
|          hit | 1,450,420 | 73.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 300 | 23.4% |
| Failure | 980 | 76.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| reversed list | 460 | 46.9% |
| dict items | 320 | 32.7% |
| set | 120 | 12.2% |
| other | 60 | 6.1% |
| dict keys | 20 | 2.0% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 3,443,860 | 5.5% |
|        deopt | 40 | 0.0% |
|          hit | 59,529,100 | 94.5% |
|         miss | 19,060 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 14,980 | 67.2% |
| Failure | 7,320 | 32.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| method | 4,240 | 57.9% |
| not managed dict | 1,260 | 17.2% |
| has managed dict | 600 | 8.2% |
| class attr simple | 500 | 6.8% |
| mutable class | 460 | 6.3% |
| metaclass attribute | 200 | 2.7% |
| overridden | 20 | 0.3% |
| out of versions | 20 | 0.3% |
| module attr not found | 20 | 0.3% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 5,780 | 0.0% |
|          hit | 13,248,200 | 99.9% |
|         miss | 720 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,880 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 60 | 15.8% |
|          hit | 260 | 68.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
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
|     deferred | 735,020 | 7.9% |
|          hit | 8,580,100 | 92.1% |
|         miss | 14,860 | 0.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 3,800 | 71.7% |
| Failure | 1,500 | 28.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| overriding descriptor | 980 | 65.3% |
| property | 400 | 26.7% |
| no dict | 100 | 6.7% |
| overridden | 20 | 1.3% |


</details>

### STORE_SLICE

<details>
<summary> specialization stats for STORE_SLICE family </summary>


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,260 | 0.1% |
|          hit | 1,882,080 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 95.8% |
| Failure | 20 | 4.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytearray int | 20 | 100.0% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 1,358,740 | 11.8% |
|          hit | 10,111,060 | 88.1% |
|         miss | 35,080 | 0.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,420 | 62.4% |
| Failure | 1,460 | 37.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict | 480 | 32.9% |
| sequence | 420 | 28.8% |
| mapping | 280 | 19.2% |
| bytes | 180 | 12.3% |
| other | 80 | 5.5% |
| number | 20 | 1.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 200 | 0.0% |
|          hit | 470,200 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 200 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 220,786,580 | 50.5% |
| Not specialized | 49,663,520 | 11.4% |
| Specialized hits | 163,053,860 | 37.3% |
| Specialized misses | 3,498,260 | 0.8% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL | 4,363,120 | 29.2% |
| LOAD_ATTR | 3,443,860 | 23.1% |
| BINARY_SUBSCR | 3,369,020 | 22.5% |
| TO_BOOL | 1,358,740 | 9.1% |
| COMPARE_OP | 1,040,740 | 7.0% |
| STORE_ATTR | 735,020 | 4.9% |
| FOR_ITER | 522,720 | 3.5% |
| BINARY_OP | 100,120 | 0.7% |
| LOAD_GLOBAL | 5,780 | 0.0% |
| STORE_SUBSCR | 1,260 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,561,840 | 73.2% |
| CALL_BOUND_METHOD_EXACT_ARGS | 647,840 | 18.5% |
| CALL_METHOD_DESCRIPTOR_O | 172,200 | 4.9% |
| BINARY_SUBSCR_STR_INT | 31,340 | 0.9% |
| TO_BOOL_NONE | 18,820 | 0.5% |
| TO_BOOL_STR | 16,020 | 0.5% |
| COMPARE_OP_STR | 10,000 | 0.3% |
| LOAD_ATTR_SLOT | 8,560 | 0.2% |
| STORE_ATTR_INSTANCE_VALUE | 7,900 | 0.2% |
| STORE_ATTR_SLOT | 6,960 | 0.2% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 259,380 | 1.7% |
| Calls to Python functions inlined | 14,792,340 | 98.3% |
| Calls via PyEval_EvalFrame (total) | 259,380 | 1.7% |
| Calls via PyEval_EvalFrame (vector) | 259,200 | 1.7% |
| Calls via PyEval_EvalFrame (generator) | 180 | 0.0% |
| Calls via PyEval_EvalFrame (legacy) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 258,520 | 1.7% |
| Calls via PyEval_EvalFrame (build class) | 640 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 12,980 | 0.1% |
| Calls via PyEval_EvalFrame (function ex) | 320 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 224,800 | 1.5% |
| Calls via PyEval_EvalFrame (method) | 0 | 0.0% |
| Frame objects created | 1,500 | 0.0% |
| Frames pushed | 10,989,040 | 73.0% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 6,946,160 | 26.6% |
| Frees to freelist | 6,961,720 |  |
| Allocations | 19,165,540 | 73.4% |
| Allocations to 512 bytes | 19,018,140 | 72.8% |
| Allocations to 4 kbytes | 141,300 | 0.5% |
| Allocations over 4 kbytes | 6,100 | 0.0% |
| Frees | 19,855,225 |  |
| New values | 8,880 |  |
| Interpreter increfs | 225,394,560 | 82.8% |
| Interpreter decrefs | 251,240,620 | 85.0% |
| Increfs | 46,874,945 | 17.2% |
| Decrefs | 44,490,119 | 15.0% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 0 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 4,734,091 |  |
| Method cache misses | 11,649 |  |
| Method cache collisions | 12,640 |  |
| Method cache dunder hits | 1,163,500 |  |
| Method cache dunder misses | 2,620 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 1,740 | 1,920 | 7,167,400 |
| 1 | 160 | 340 | 7,124,760 |
| 2 | 20 | 675,720 | 10,486,200 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 1,040 |  |
| Traces created | 660 | 63.5% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 2,980 | 286.5% |
| Trace too long | 0 | 0.0% |
| Trace too short | 25,580 | 2,459.6% |
| Inner loop found | 40 | 3.8% |
| Recursive call | 0 | 0.0% |
| Low confidence | 20 | 1.9% |
| Traces executed | 5,427,980 |  |
| Uops executed | 146,374,940 | 26.97 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 20 | 3.0% |
| <= 32 | 220 | 33.3% |
| <= 64 | 320 | 48.5% |
| <= 128 | 80 | 12.1% |
| <= 256 | 20 | 3.0% |


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
| <= 256 | 20 | 3.0% |
| <= 512 | 340 | 51.5% |
| <= 1,024 | 240 | 36.4% |
| <= 2,048 | 60 | 9.1% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 6,480 | 0.1% |
| <= 4 | 267,700 | 4.9% |
| <= 8 | 1,780 | 0.0% |
| <= 16 | 734,200 | 13.5% |
| <= 32 | 3,474,260 | 64.0% |
| <= 64 | 51,520 | 0.9% |
| <= 128 | 20,540 | 0.4% |
| <= 256 | 54,360 | 1.0% |
| <= 512 | 10,160 | 0.2% |
| <= 1,024 | 840 | 0.0% |
| <= 2,048 | 400 | 0.0% |
| <= 4,096 | 320 | 0.0% |
| <= 8,192 | 160 | 0.0% |
| <= 16,384 | 0 | 0.0% |
| <= 32,768 | 0 | 0.0% |
| <= 65,536 | 240 | 0.0% |
| <= 131,072 | 80 | 0.0% |
| <= 262,144 | 80 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 19,521,300 | 13.3% | 13.3% |  |
| _GUARD_TYPE_VERSION | 15,598,520 | 10.7% | 24.0% |  |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 14,826,320 | 10.1% | 34.1% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 14,826,320 | 10.1% | 44.3% |  |
| _SET_IP | 13,958,980 | 9.5% | 53.8% |  |
| _CHECK_VALIDITY | 10,431,240 | 7.1% | 60.9% |  |
| _GUARD_IS_FALSE_POP | 8,970,400 | 6.1% | 67.0% | 8.9% |
| _START_EXECUTOR | 4,623,120 | 3.2% | 70.2% |  |
| TO_BOOL_LIST | 3,434,000 | 2.3% | 72.5% |  |
| _TO_BOOL | 3,433,780 | 2.3% | 74.9% |  |
| STORE_FAST | 3,190,220 | 2.2% | 77.1% |  |
| _JUMP_TO_TOP | 2,894,920 | 2.0% | 79.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 2,808,620 | 1.9% | 81.0% | 97.6% |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 2,770,860 | 1.9% | 82.9% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 2,770,860 | 1.9% | 84.8% |  |
| _LOAD_CONST_INLINE_BORROW | 2,666,140 | 1.8% | 86.6% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 2,505,620 | 1.7% | 88.3% | 0.5% |
| _ITER_CHECK_RANGE | 2,505,620 | 1.7% | 90.0% |  |
| _ITER_NEXT_RANGE | 2,492,260 | 1.7% | 91.7% |  |
| _STORE_SUBSCR | 2,483,020 | 1.7% | 93.4% |  |
| TO_BOOL_BOOL | 1,499,060 | 1.0% | 94.4% |  |
| _CHECK_VALIDITY_AND_SET_IP | 1,253,800 | 0.9% | 95.3% |  |
| _COLD_EXIT | 804,860 | 0.5% | 95.8% |  |
| _EXIT_TRACE | 762,340 | 0.5% | 96.3% | 100.0% |
| _LOAD_ATTR_METHOD_NO_DICT | 712,780 | 0.5% | 96.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 691,360 | 0.5% | 97.3% |  |
| _FOR_ITER_TIER_TWO | 647,660 | 0.4% | 97.8% | 22.0% |
| CONTAINS_OP | 536,380 | 0.4% | 98.1% |  |
| _BINARY_OP | 517,600 | 0.4% | 98.5% |  |
| _COMPARE_OP | 501,960 | 0.3% | 98.8% |  |
| _ITER_CHECK_LIST | 150,200 | 0.1% | 98.9% | 0.1% |
| _GUARD_NOT_EXHAUSTED_LIST | 150,000 | 0.1% | 99.0% | 83.3% |
| _LOAD_CONST_INLINE | 82,940 | 0.1% | 99.1% |  |
| _CHECK_GLOBALS | 75,500 | 0.1% | 99.1% |  |
| _GUARD_IS_TRUE_POP | 72,440 | 0.0% | 99.2% | 22.5% |
| RESUME_CHECK | 67,620 | 0.0% | 99.2% | 0.0% |
| _CHECK_STACK_SPACE | 67,620 | 0.0% | 99.3% |  |
| _INIT_CALL_PY_EXACT_ARGS | 67,620 | 0.0% | 99.3% |  |
| _PUSH_FRAME | 67,620 | 0.0% | 99.4% |  |
| _SAVE_RETURN_OFFSET | 67,620 | 0.0% | 99.4% |  |
| PUSH_NULL | 65,720 | 0.0% | 99.5% |  |
| _BINARY_OP_ADD_INT | 47,180 | 0.0% | 99.5% |  |
| _GUARD_BOTH_INT | 44,740 | 0.0% | 99.5% |  |
| IS_OP | 43,700 | 0.0% | 99.5% |  |
| BINARY_SLICE | 39,800 | 0.0% | 99.6% |  |
| COMPARE_OP_STR | 37,200 | 0.0% | 99.6% | 0.1% |
| BINARY_SUBSCR_STR_INT | 37,000 | 0.0% | 99.6% | 56.6% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 35,800 | 0.0% | 99.6% |  |
| _GUARD_KEYS_VERSION | 35,800 | 0.0% | 99.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 35,800 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_TUPLE_INT | 30,480 | 0.0% | 99.7% |  |
| CALL_BUILTIN_CLASS | 29,820 | 0.0% | 99.7% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 29,280 | 0.0% | 99.8% |  |
| TO_BOOL_NONE | 25,460 | 0.0% | 99.8% | 0.3% |
| _ITER_NEXT_LIST | 25,040 | 0.0% | 99.8% |  |
| _GUARD_DORV_VALUES | 23,560 | 0.0% | 99.8% |  |
| _STORE_ATTR_INSTANCE_VALUE | 23,560 | 0.0% | 99.8% |  |
| _POP_FRAME | 22,940 | 0.0% | 99.8% |  |
| _CHECK_BUILTINS | 21,560 | 0.0% | 99.9% |  |
| CALL_BUILTIN_O | 19,800 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_DICT | 18,860 | 0.0% | 99.9% |  |
| BUILD_TUPLE | 18,500 | 0.0% | 99.9% |  |
| LIST_APPEND | 18,160 | 0.0% | 99.9% |  |
| _BINARY_OP_SUBTRACT_INT | 17,980 | 0.0% | 99.9% |  |
| POP_TOP | 16,220 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_BORROW_WITH_NULL | 13,420 | 0.0% | 99.9% |  |
| GET_ITER | 13,200 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 9,660 | 0.0% | 100.0% |  |
| _GUARD_IS_NOT_NONE_POP | 9,440 | 0.0% | 100.0% | 2.8% |
| _GUARD_NOT_EXHAUSTED_TUPLE | 6,940 | 0.0% | 100.0% | 17.9% |
| _ITER_CHECK_TUPLE | 6,940 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 6,720 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 5,700 | 0.0% | 100.0% |  |
| COMPARE_OP_INT | 3,800 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 3,760 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 3,500 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 3,400 | 0.0% | 100.0% |  |
| COPY | 2,520 | 0.0% | 100.0% |  |
| CALL_LEN | 2,060 | 0.0% | 100.0% |  |
| _BINARY_SUBSCR | 2,000 | 0.0% | 100.0% |  |
| _LOAD_GLOBAL | 1,700 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 1,460 | 0.0% | 100.0% | 19.2% |
| _LOAD_ATTR | 1,380 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 960 | 0.0% | 100.0% | 12.5% |
| BUILD_LIST | 800 | 0.0% | 100.0% |  |
| TO_BOOL_INT | 600 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 480 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_LIST | 420 | 0.0% | 100.0% |  |
| BUILD_SLICE | 360 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 180 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 180 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 100 | 0.0% | 100.0% |  |
| SWAP | 60 | 0.0% | 100.0% |  |
| _CHECK_ATTR_METHOD_LAZY_DICT | 60 | 0.0% | 100.0% |  |
| _LOAD_ATTR_METHOD_LAZY_DICT | 60 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 20 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| YIELD_VALUE | 21,620 |
| FOR_ITER_GEN | 600 |
| CALL | 540 |
| CALL_LIST_APPEND | 140 |
| BINARY_OP_INPLACE_ADD_UNICODE | 60 |
| LOAD_ATTR_PROPERTY | 60 |


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
