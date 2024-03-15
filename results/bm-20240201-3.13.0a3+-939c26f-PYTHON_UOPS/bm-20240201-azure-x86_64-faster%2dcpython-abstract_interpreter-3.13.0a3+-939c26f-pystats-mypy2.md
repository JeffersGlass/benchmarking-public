
# Pystats results

- benchmark: mypy2
- fork: faster-cpython
- ref: abstract-interpreter-generator
- commit hash: 939c26f
- commit date: 2024-02-01T15:28:16+00:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 1,449,204,216 | 20.7% | 20.7% |  |
| LOAD_CONST | 345,145,656 | 4.9% | 25.6% |  |
| RESUME_CHECK | 344,554,501 | 4.9% | 30.5% | 0.0% |
| STORE_ATTR_SLOT | 305,233,998 | 4.4% | 34.9% | 21.6% |
| LOAD_GLOBAL_MODULE | 300,620,324 | 4.3% | 39.1% | 0.0% |
| LOAD_FAST_LOAD_FAST | 280,581,638 | 4.0% | 43.1% |  |
| LOAD_GLOBAL_BUILTIN | 270,990,958 | 3.9% | 47.0% | 0.0% |
| POP_JUMP_IF_FALSE | 268,244,336 | 3.8% | 50.8% |  |
| LOAD_ATTR_SLOT | 246,548,676 | 3.5% | 54.4% | 1.7% |
| STORE_FAST | 244,560,124 | 3.5% | 57.8% |  |
| CALL_PY_EXACT_ARGS | 216,101,231 | 3.1% | 60.9% | 10.3% |
| TO_BOOL_BOOL | 204,387,951 | 2.9% | 63.8% | 0.0% |
| RETURN_VALUE | 197,961,349 | 2.8% | 66.7% |  |
| RETURN_CONST | 149,843,756 | 2.1% | 68.8% |  |
| CALL_ISINSTANCE | 136,124,021 | 1.9% | 70.7% |  |
| LOAD_ATTR_METHOD_NO_DICT | 130,325,286 | 1.9% | 72.6% | 21.9% |
| POP_TOP | 109,883,144 | 1.6% | 74.2% |  |
| POP_JUMP_IF_TRUE | 108,733,781 | 1.6% | 75.7% |  |
| LOAD_ATTR_INSTANCE_VALUE | 76,982,253 | 1.1% | 76.8% | 3.7% |
| LOAD_DEREF | 64,661,163 | 0.9% | 77.7% |  |
| FOR_ITER_LIST | 61,501,390 | 0.9% | 78.6% | 1.6% |
| INTERPRETER_EXIT | 60,483,687 | 0.9% | 79.5% |  |
| GET_ITER | 60,184,055 | 0.9% | 80.3% |  |
| BINARY_SUBSCR_DICT | 58,592,272 | 0.8% | 81.2% |  |
| ENTER_EXECUTOR | 58,237,672 | 0.8% | 82.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 56,388,831 | 0.8% | 82.8% | 12.8% |
| LOAD_ATTR | 55,709,903 | 0.8% | 83.6% |  |
| POP_JUMP_IF_NOT_NONE | 47,169,460 | 0.7% | 84.3% |  |
| COPY_FREE_VARS | 46,994,120 | 0.7% | 84.9% |  |
| CONTAINS_OP | 46,707,452 | 0.7% | 85.6% |  |
| SWAP | 43,739,780 | 0.6% | 86.2% |  |
| LOAD_SUPER_ATTR_METHOD | 43,009,540 | 0.6% | 86.8% |  |
| BUILD_LIST | 41,573,035 | 0.6% | 87.4% |  |
| POP_JUMP_IF_NONE | 39,627,880 | 0.6% | 88.0% |  |
| STORE_ATTR_INSTANCE_VALUE | 38,998,600 | 0.6% | 88.6% | 2.2% |
| CALL_KW | 38,254,460 | 0.5% | 89.1% |  |
| CALL | 34,420,020 | 0.5% | 89.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 31,400,161 | 0.4% | 90.0% | 8.8% |
| IS_OP | 28,376,120 | 0.4% | 90.4% |  |
| NOP | 26,877,320 | 0.4% | 90.8% |  |
| COPY | 25,226,667 | 0.4% | 91.2% |  |
| JUMP_FORWARD | 24,371,308 | 0.3% | 91.5% |  |
| TO_BOOL_LIST | 22,845,760 | 0.3% | 91.9% | 0.7% |
| COMPARE_OP_STR | 21,677,130 | 0.3% | 92.2% | 0.3% |
| COMPARE_OP | 21,051,961 | 0.3% | 92.5% |  |
| BINARY_SUBSCR | 20,172,413 | 0.3% | 92.8% |  |
| CALL_BUILTIN_CLASS | 20,032,746 | 0.3% | 93.0% |  |
| COMPARE_OP_INT | 18,683,810 | 0.3% | 93.3% | 2.1% |
| PUSH_NULL | 17,798,019 | 0.3% | 93.6% |  |
| CALL_LEN | 17,716,980 | 0.3% | 93.8% |  |
| MAKE_CELL | 16,597,880 | 0.2% | 94.1% |  |
| CALL_LIST_APPEND | 16,072,640 | 0.2% | 94.3% |  |
| TO_BOOL_NONE | 16,063,442 | 0.2% | 94.5% | 8.3% |
| BUILD_TUPLE | 15,665,116 | 0.2% | 94.7% |  |
| LOAD_ATTR_WITH_HINT | 15,282,620 | 0.2% | 95.0% | 2.1% |
| FOR_ITER_TUPLE | 15,106,959 | 0.2% | 95.2% | 6.4% |
| MAP_ADD | 14,781,868 | 0.2% | 95.4% |  |
| TO_BOOL_ALWAYS_TRUE | 14,511,518 | 0.2% | 95.6% | 13.2% |
| LOAD_FAST_AND_CLEAR | 13,893,760 | 0.2% | 95.8% |  |
| LOAD_ATTR_PROPERTY | 13,761,645 | 0.2% | 96.0% | 6.5% |
| LOAD_ATTR_MODULE | 13,203,331 | 0.2% | 96.2% | 0.0% |
| UNARY_NOT | 13,081,200 | 0.2% | 96.4% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 12,933,880 | 0.2% | 96.5% | 31.0% |
| LIST_APPEND | 12,680,036 | 0.2% | 96.7% |  |
| STORE_FAST_STORE_FAST | 12,362,990 | 0.2% | 96.9% |  |
| EXTENDED_ARG | 12,017,640 | 0.2% | 97.1% |  |
| CALL_PY_WITH_DEFAULTS | 10,357,660 | 0.1% | 97.2% | 2.1% |
| TO_BOOL | 10,218,040 | 0.1% | 97.4% |  |
| CALL_TUPLE_1 | 10,168,216 | 0.1% | 97.5% |  |
| FOR_ITER | 9,338,276 | 0.1% | 97.6% |  |
| BINARY_SUBSCR_LIST_INT | 9,024,900 | 0.1% | 97.8% | 0.0% |
| CALL_BUILTIN_O | 7,910,173 | 0.1% | 97.9% | 8.4% |
| LOAD_ATTR_CLASS | 7,444,760 | 0.1% | 98.0% | 2.3% |
| UNPACK_SEQUENCE_LIST | 7,224,280 | 0.1% | 98.1% |  |
| CALL_BUILTIN_FAST | 6,394,619 | 0.1% | 98.2% | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 5,901,499 | 0.1% | 98.3% | 0.0% |
| STORE_ATTR | 5,843,160 | 0.1% | 98.4% |  |
| DELETE_ATTR | 5,627,200 | 0.1% | 98.4% |  |
| YIELD_VALUE | 5,624,780 | 0.1% | 98.5% |  |
| CALL_TYPE_1 | 5,557,100 | 0.1% | 98.6% |  |
| BUILD_MAP | 5,500,159 | 0.1% | 98.7% |  |
| FOR_ITER_RANGE | 4,710,919 | 0.1% | 98.7% |  |
| TO_BOOL_STR | 4,587,680 | 0.1% | 98.8% | 4.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,329,035 | 0.1% | 98.9% |  |
| MAKE_FUNCTION | 4,103,180 | 0.1% | 98.9% |  |
| CALL_FUNCTION_EX | 3,983,600 | 0.1% | 99.0% |  |
| RETURN_GENERATOR | 3,893,160 | 0.1% | 99.0% |  |
| STORE_FAST_LOAD_FAST | 3,793,048 | 0.1% | 99.1% |  |
| BINARY_OP_ADD_INT | 3,680,288 | 0.1% | 99.1% | 0.5% |
| CALL_ALLOC_AND_ENTER_INIT | 3,333,780 | 0.0% | 99.2% | 0.1% |
| EXIT_INIT_CHECK | 3,329,280 | 0.0% | 99.2% |  |
| BINARY_SLICE | 2,930,280 | 0.0% | 99.3% |  |
| BINARY_OP_ADD_UNICODE | 2,745,780 | 0.0% | 99.3% |  |
| SET_FUNCTION_ATTRIBUTE | 2,571,580 | 0.0% | 99.4% |  |
| STORE_SUBSCR_DICT | 2,380,978 | 0.0% | 99.4% |  |
| STORE_DEREF | 2,362,140 | 0.0% | 99.4% |  |
| BINARY_OP | 2,348,688 | 0.0% | 99.5% |  |
| CHECK_EXC_MATCH | 2,076,400 | 0.0% | 99.5% |  |
| POP_EXCEPT | 2,076,400 | 0.0% | 99.5% |  |
| PUSH_EXC_INFO | 2,076,400 | 0.0% | 99.5% |  |
| DICT_MERGE | 1,932,720 | 0.0% | 99.6% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 1,923,260 | 0.0% | 99.6% | 0.0% |
| STORE_SUBSCR | 1,888,260 | 0.0% | 99.6% |  |
| BINARY_OP_SUBTRACT_INT | 1,881,609 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,516,960 | 0.0% | 99.7% | 10.9% |
| LOAD_FAST_CHECK | 1,411,600 | 0.0% | 99.7% |  |
| BINARY_SUBSCR_GETITEM | 1,397,980 | 0.0% | 99.7% | 0.0% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 1,388,880 | 0.0% | 99.7% |  |
| BEFORE_WITH | 1,338,400 | 0.0% | 99.8% |  |
| IMPORT_FROM | 1,214,560 | 0.0% | 99.8% |  |
| FORMAT_SIMPLE | 1,185,920 | 0.0% | 99.8% |  |
| IMPORT_NAME | 991,840 | 0.0% | 99.8% |  |
| UNARY_NEGATIVE | 974,900 | 0.0% | 99.8% |  |
| UNPACK_SEQUENCE_TUPLE | 957,580 | 0.0% | 99.8% |  |
| TO_BOOL_INT | 949,161 | 0.0% | 99.8% | 4.5% |
| BUILD_SET | 939,760 | 0.0% | 99.9% |  |
| JUMP_BACKWARD | 896,740 | 0.0% | 99.9% |  |
| BINARY_SUBSCR_TUPLE_INT | 839,240 | 0.0% | 99.9% |  |
| STORE_ATTR_WITH_HINT | 821,860 | 0.0% | 99.9% | 3.0% |
| BUILD_STRING | 730,240 | 0.0% | 99.9% |  |
| SET_ADD | 700,730 | 0.0% | 99.9% |  |
| FOR_ITER_GEN | 663,900 | 0.0% | 99.9% |  |
| CALL_STR_1 | 609,940 | 0.0% | 99.9% |  |
| LOAD_SUPER_ATTR_ATTR | 541,560 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_NO_DICT | 534,840 | 0.0% | 99.9% |  |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 533,300 | 0.0% | 100.0% | 2.0% |
| BINARY_SUBSCR_STR_INT | 464,319 | 0.0% | 100.0% | 0.0% |
| BINARY_OP_INPLACE_ADD_UNICODE | 286,720 | 0.0% | 100.0% |  |
| RERAISE | 271,840 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 242,840 | 0.0% | 100.0% |  |
| SEND_GEN | 229,500 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 217,160 | 0.0% | 100.0% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 189,200 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 169,840 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 146,420 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_FLOAT | 143,080 | 0.0% | 100.0% | 13.6% |
| DELETE_FAST | 100,960 | 0.0% | 100.0% |  |
| CALL_INTRINSIC_1 | 96,620 | 0.0% | 100.0% |  |
| LIST_EXTEND | 75,340 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 74,879 | 0.0% | 100.0% |  |
| END_SEND | 48,000 | 0.0% | 100.0% |  |
| GET_YIELD_FROM_ITER | 48,000 | 0.0% | 100.0% |  |
| RESUME | 40,880 | 0.0% | 100.0% | 0.0% |
| DELETE_SUBSCR | 38,140 | 0.0% | 100.0% |  |
| CONVERT_VALUE | 34,040 | 0.0% | 100.0% |  |
| END_FOR | 27,040 | 0.0% | 100.0% |  |
| LOAD_ATTR_METHOD_LAZY_DICT | 16,440 | 0.0% | 100.0% |  |
| BUILD_SLICE | 9,400 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 4,820 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_INT | 3,240 | 0.0% | 100.0% |  |
| STORE_NAME | 2,240 | 0.0% | 100.0% |  |
| LOAD_NAME | 2,100 | 0.0% | 100.0% |  |
| UNARY_INVERT | 920 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 760 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 620 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 520 | 0.0% | 100.0% |  |
| STORE_SLICE | 480 | 0.0% | 100.0% |  |
| UNPACK_EX | 380 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 360 | 0.0% | 100.0% |  |
| SET_UPDATE | 160 | 0.0% | 100.0% |  |
| SEND | 120 | 0.0% | 100.0% |  |
| SETUP_ANNOTATIONS | 80 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 40 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_SLOT | 217,327,781 | 3.1% | 3.1% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 187,798,718 | 2.7% | 5.8% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 187,249,916 | 2.7% | 8.4% |
| LOAD_FAST STORE_ATTR_SLOT | 179,530,299 | 2.6% | 11.0% |
| RESUME_CHECK LOAD_FAST | 150,584,697 | 2.1% | 13.2% |
| LOAD_CONST LOAD_FAST | 140,029,840 | 2.0% | 15.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 138,134,325 | 2.0% | 17.1% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 133,064,751 | 1.9% | 19.0% |
| CALL_ISINSTANCE TO_BOOL_BOOL | 133,033,603 | 1.9% | 20.9% |
| POP_JUMP_IF_FALSE LOAD_FAST | 124,176,427 | 1.8% | 22.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 124,049,340 | 1.8% | 24.5% |
| STORE_FAST LOAD_FAST | 120,089,730 | 1.7% | 26.2% |
| LOAD_GLOBAL_MODULE CALL_ISINSTANCE | 114,689,090 | 1.6% | 27.8% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 94,137,682 | 1.3% | 29.1% |
| STORE_ATTR_SLOT LOAD_CONST | 84,645,340 | 1.2% | 30.4% |
| RESUME_CHECK LOAD_GLOBAL_BUILTIN | 84,035,264 | 1.2% | 31.6% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 80,412,339 | 1.1% | 32.7% |
| LOAD_FAST LOAD_CONST | 76,467,519 | 1.1% | 33.8% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 70,357,660 | 1.0% | 34.8% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_BUILTIN | 65,430,109 | 0.9% | 35.7% |
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 61,938,168 | 0.9% | 36.6% |
| STORE_ATTR_SLOT RETURN_CONST | 60,343,400 | 0.9% | 37.5% |
| LOAD_FAST RETURN_VALUE | 59,209,023 | 0.8% | 38.3% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 57,853,862 | 0.8% | 39.1% |
| LOAD_GLOBAL_MODULE LOAD_FAST | 57,269,389 | 0.8% | 40.0% |
| STORE_ATTR_SLOT LOAD_FAST | 56,436,999 | 0.8% | 40.8% |
| RETURN_CONST POP_TOP | 52,750,020 | 0.8% | 41.5% |
| LOAD_FAST_LOAD_FAST CALL_PY_EXACT_ARGS | 51,162,000 | 0.7% | 42.2% |
| LOAD_CONST BINARY_SUBSCR_DICT | 50,556,380 | 0.7% | 43.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 50,313,766 | 0.7% | 43.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 48,737,708 | 0.7% | 44.4% |
| POP_TOP LOAD_FAST | 46,776,128 | 0.7% | 45.0% |
| COPY_FREE_VARS RESUME_CHECK | 46,507,260 | 0.7% | 45.7% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 46,059,646 | 0.7% | 46.4% |
| LOAD_GLOBAL_BUILTIN LOAD_DEREF | 46,031,900 | 0.7% | 47.0% |
| RETURN_VALUE STORE_FAST | 44,701,023 | 0.6% | 47.7% |
| LOAD_DEREF LOAD_FAST | 44,051,819 | 0.6% | 48.3% |
| LOAD_FAST LOAD_SUPER_ATTR_METHOD | 43,007,140 | 0.6% | 48.9% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 41,245,400 | 0.6% | 49.5% |
| RETURN_VALUE RETURN_VALUE | 40,322,475 | 0.6% | 50.1% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 39,478,231 | 0.6% | 50.6% |
| CONTAINS_OP POP_JUMP_IF_FALSE | 39,389,511 | 0.6% | 51.2% |
| LOAD_FAST LOAD_FAST | 38,463,557 | 0.5% | 51.7% |
| LOAD_CONST CALL_KW | 37,421,240 | 0.5% | 52.3% |
| LOAD_FAST LOAD_ATTR | 37,203,103 | 0.5% | 52.8% |
| LOAD_ATTR_METHOD_NO_DICT CALL_PY_EXACT_ARGS | 37,184,112 | 0.5% | 53.3% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 35,845,511 | 0.5% | 53.8% |
| LOAD_SUPER_ATTR_METHOD LOAD_FAST_LOAD_FAST | 35,810,960 | 0.5% | 54.4% |
| CACHE RESUME_CHECK | 34,891,867 | 0.5% | 54.9% |
| RESUME_CHECK RETURN_CONST | 33,811,860 | 0.5% | 55.3% |
| RETURN_CONST INTERPRETER_EXIT | 30,999,340 | 0.4% | 55.8% |
| RETURN_CONST LOAD_FAST | 30,810,880 | 0.4% | 56.2% |
| RESUME_CHECK LOAD_FAST_LOAD_FAST | 30,206,540 | 0.4% | 56.6% |
| LOAD_ATTR_SLOT LOAD_FAST | 29,775,212 | 0.4% | 57.1% |
| STORE_FAST LOAD_GLOBAL_MODULE | 29,108,358 | 0.4% | 57.5% |
| LOAD_CONST LOAD_CONST | 26,735,640 | 0.4% | 57.9% |
| FOR_ITER_LIST STORE_FAST | 26,557,685 | 0.4% | 58.2% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 26,429,680 | 0.4% | 58.6% |
| CALL_METHOD_DESCRIPTOR_FAST STORE_FAST | 25,888,372 | 0.4% | 59.0% |
| RETURN_VALUE LOAD_FAST | 25,055,820 | 0.4% | 59.4% |
| LOAD_ATTR LOAD_FAST | 24,813,912 | 0.4% | 59.7% |
| RETURN_VALUE INTERPRETER_EXIT | 24,631,267 | 0.4% | 60.1% |
| LOAD_ATTR_SLOT GET_ITER | 23,940,916 | 0.3% | 60.4% |
| ENTER_EXECUTOR FOR_ITER_LIST | 23,900,257 | 0.3% | 60.7% |
| CALL_PY_EXACT_ARGS COPY_FREE_VARS | 23,723,100 | 0.3% | 61.1% |
| LOAD_FAST CONTAINS_OP | 23,587,220 | 0.3% | 61.4% |
| POP_JUMP_IF_FALSE LOAD_GLOBAL_MODULE | 23,041,420 | 0.3% | 61.7% |
| LOAD_GLOBAL_MODULE LOAD_FAST_LOAD_FAST | 22,881,620 | 0.3% | 62.1% |
| GET_ITER FOR_ITER_LIST | 22,327,527 | 0.3% | 62.4% |
| LOAD_ATTR_SLOT STORE_FAST | 22,174,660 | 0.3% | 62.7% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 22,102,080 | 0.3% | 63.0% |
| CACHE COPY_FREE_VARS | 21,747,640 | 0.3% | 63.3% |
| CALL_KW RESUME_CHECK | 21,713,260 | 0.3% | 63.6% |
| RETURN_CONST RETURN_VALUE | 21,376,660 | 0.3% | 63.9% |
| LOAD_GLOBAL_MODULE IS_OP | 20,791,560 | 0.3% | 64.2% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 20,697,751 | 0.3% | 64.5% |
| LOAD_FAST LOAD_GLOBAL_BUILTIN | 19,766,760 | 0.3% | 64.8% |
| LOAD_FAST POP_JUMP_IF_NONE | 19,363,320 | 0.3% | 65.1% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 19,246,809 | 0.3% | 65.4% |
| COPY TO_BOOL_BOOL | 19,175,948 | 0.3% | 65.6% |
| IS_OP POP_JUMP_IF_FALSE | 19,064,900 | 0.3% | 65.9% |
| POP_JUMP_IF_NONE LOAD_FAST | 18,875,340 | 0.3% | 66.2% |
| STORE_ATTR_INSTANCE_VALUE LOAD_FAST_LOAD_FAST | 18,308,380 | 0.3% | 66.4% |
| LOAD_ATTR_SLOT RETURN_VALUE | 18,246,975 | 0.3% | 66.7% |
| POP_JUMP_IF_NOT_NONE LOAD_GLOBAL_BUILTIN | 18,197,520 | 0.3% | 67.0% |
| POP_TOP LOAD_FAST_LOAD_FAST | 17,641,240 | 0.3% | 67.2% |
| LOAD_GLOBAL_BUILTIN CALL_ISINSTANCE | 17,546,400 | 0.3% | 67.5% |
| TO_BOOL_LIST POP_JUMP_IF_TRUE | 17,346,660 | 0.2% | 67.7% |
| LOAD_ATTR_SLOT LOAD_ATTR_SLOT | 17,337,421 | 0.2% | 68.0% |
| LOAD_FAST TO_BOOL_LIST | 17,337,420 | 0.2% | 68.2% |
| RETURN_VALUE POP_TOP | 17,222,880 | 0.2% | 68.5% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_FAST | 17,155,499 | 0.2% | 68.7% |
| LOAD_FAST TO_BOOL_BOOL | 17,080,080 | 0.2% | 68.9% |
| LOAD_GLOBAL_MODULE LOAD_GLOBAL_MODULE | 16,341,960 | 0.2% | 69.2% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 16,248,820 | 0.2% | 69.4% |
| BUILD_LIST STORE_FAST | 16,125,260 | 0.2% | 69.6% |
| STORE_ATTR_SLOT LOAD_GLOBAL_BUILTIN | 15,842,020 | 0.2% | 69.9% |
| LOAD_CONST COMPARE_OP_STR | 15,472,516 | 0.2% | 70.1% |
| NOP LOAD_FAST | 15,244,680 | 0.2% | 70.3% |
| LOAD_ATTR_SLOT POP_JUMP_IF_NONE | 15,204,780 | 0.2% | 70.5% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,228,300 | 76.0% |
| BINARY_OP_SUBTRACT_INT | 445,100 | 15.2% |
| LOAD_FAST | 189,180 | 6.5% |
| BINARY_OP_ADD_INT | 50,980 | 1.7% |
| LOAD_ATTR_SLOT | 11,980 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,170,120 | 39.9% |
| CALL_PY_EXACT_ARGS | 445,540 | 15.2% |
| STORE_FAST | 350,860 | 12.0% |
| GET_ITER | 323,200 | 11.0% |
| BUILD_TUPLE | 151,320 | 5.2% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 480 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 34,891,867 | 57.7% |
| COPY_FREE_VARS | 21,747,640 | 35.9% |
| POP_TOP | 3,796,780 | 6.3% |
| RETURN_GENERATOR | 46,720 | 0.1% |
| PUSH_EXC_INFO | 21,440 | 0.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 1,297,400 | 96.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 24,040 | 1.8% |
| CALL | 16,820 | 1.3% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 0.0% |
| LOAD_FAST | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,190,900 | 89.0% |
| STORE_FAST | 147,500 | 11.0% |


</details>

### BINARY_OP_INPLACE_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_INPLACE_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 164,520 | 57.4% |
| RETURN_VALUE | 98,480 | 34.3% |
| BUILD_STRING | 22,120 | 7.7% |
| LOAD_FAST_LOAD_FAST | 920 | 0.3% |
| BINARY_SUBSCR_STR_INT | 400 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 261,640 | 91.3% |
| LOAD_FAST | 23,360 | 8.1% |
| JUMP_BACKWARD | 640 | 0.2% |
| JUMP_FORWARD | 620 | 0.2% |
| LOAD_FAST_LOAD_FAST | 460 | 0.2% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,949,995 | 49.3% |
| LOAD_FAST_LOAD_FAST | 7,512,060 | 37.2% |
| LOAD_FAST | 1,746,100 | 8.7% |
| LOAD_GLOBAL_MODULE | 599,360 | 3.0% |
| COPY | 143,720 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,580,180 | 42.5% |
| CONTAINS_OP | 2,232,420 | 11.1% |
| LOAD_CONST | 2,169,040 | 10.8% |
| LOAD_FAST | 1,600,620 | 7.9% |
| RETURN_VALUE | 1,415,320 | 7.0% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,067,320 | 99.6% |
| BUILD_TUPLE | 8,320 | 0.4% |
| LOAD_GLOBAL_MODULE | 420 | 0.0% |
| LOAD_GLOBAL | 340 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,076,400 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 21,760 | 57.1% |
| BUILD_SLICE | 8,640 | 22.7% |
| LOAD_FAST | 6,300 | 16.5% |
| LOAD_FAST_LOAD_FAST | 1,440 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 26,820 | 70.3% |
| LOAD_DEREF | 8,640 | 22.7% |
| JUMP_BACKWARD | 1,180 | 3.1% |
| RETURN_CONST | 960 | 2.5% |
| LOAD_FAST | 320 | 0.8% |


</details>

### END_FOR

<details>
<summary> Successors and predecessors for END_FOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 27,040 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 27,040 | 100.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 48,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 48,000 | 100.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 3,329,280 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,329,280 | 100.0% |


</details>

### FORMAT_SIMPLE

<details>
<summary> Successors and predecessors for FORMAT_SIMPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 772,280 | 65.1% |
| RETURN_VALUE | 206,640 | 17.4% |
| BINARY_SUBSCR_TUPLE_INT | 140,800 | 11.9% |
| CONVERT_VALUE | 34,040 | 2.9% |
| LOAD_ATTR_SLOT | 19,300 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 694,240 | 58.5% |
| BUILD_STRING | 491,660 | 41.5% |
| LOAD_FAST | 20 | 0.0% |


</details>

### FORMAT_WITH_SPEC

<details>
<summary> Successors and predecessors for FORMAT_WITH_SPEC </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 760 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 600 | 78.9% |
| LOAD_CONST | 160 | 21.1% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 23,940,916 | 39.8% |
| LOAD_FAST | 14,306,620 | 23.8% |
| CALL_BUILTIN_CLASS | 9,501,680 | 15.8% |
| BINARY_SUBSCR_DICT | 6,242,220 | 10.4% |
| CALL | 1,326,920 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 22,327,527 | 37.1% |
| LOAD_FAST_AND_CLEAR | 13,269,820 | 22.0% |
| FOR_ITER_TUPLE | 9,469,933 | 15.7% |
| FOR_ITER | 7,262,235 | 12.1% |
| FOR_ITER_RANGE | 2,976,620 | 4.9% |


</details>

### GET_YIELD_FROM_ITER

<details>
<summary> Successors and predecessors for GET_YIELD_FROM_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 48,000 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 48,000 | 100.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 30,999,340 | 51.3% |
| RETURN_VALUE | 24,631,267 | 40.7% |
| YIELD_VALUE | 4,806,360 | 7.9% |
| RETURN_GENERATOR | 46,720 | 0.1% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 20 | 50.0% |
| STORE_NAME | 20 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 40 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,103,180 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,079,780 | 50.7% |
| SET_FUNCTION_ATTRIBUTE | 1,985,800 | 48.4% |
| LOAD_CONST | 24,060 | 0.6% |
| LOAD_GLOBAL_MODULE | 7,080 | 0.2% |
| LOAD_GLOBAL_BUILTIN | 3,560 | 0.1% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,569,120 | 28.2% |
| POP_JUMP_IF_TRUE | 7,043,520 | 26.2% |
| POP_JUMP_IF_FALSE | 4,695,640 | 17.5% |
| RESUME_CHECK | 3,222,960 | 12.0% |
| POP_JUMP_IF_NOT_NONE | 1,307,220 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 15,244,680 | 56.7% |
| LOAD_CONST | 7,389,160 | 27.5% |
| LOAD_GLOBAL_BUILTIN | 2,386,780 | 8.9% |
| LOAD_GLOBAL_MODULE | 1,516,340 | 5.6% |
| LOAD_FAST_LOAD_FAST | 278,060 | 1.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,306,500 | 62.9% |
| SWAP | 633,920 | 30.5% |
| COPY | 128,320 | 6.2% |
| STORE_FAST | 7,000 | 0.3% |
| POP_JUMP_IF_FALSE | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,305,940 | 62.9% |
| RETURN_VALUE | 633,920 | 30.5% |
| RERAISE | 128,320 | 6.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 7,320 | 0.4% |
| EXTENDED_ARG | 320 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 52,750,020 | 48.0% |
| RETURN_VALUE | 17,222,880 | 15.7% |
| POP_JUMP_IF_FALSE | 10,313,024 | 9.4% |
| POP_JUMP_IF_TRUE | 8,672,052 | 7.9% |
| RESUME_CHECK | 4,015,960 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,776,128 | 42.6% |
| LOAD_FAST_LOAD_FAST | 17,641,240 | 16.1% |
| ENTER_EXECUTOR | 15,023,379 | 13.7% |
| RETURN_CONST | 11,525,120 | 10.5% |
| LOAD_CONST | 4,407,340 | 4.0% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST | 1,143,320 | 55.1% |
| LOAD_ATTR_SLOT | 631,960 | 30.4% |
| RERAISE | 106,720 | 5.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 88,420 | 4.3% |
| RAISE_VARARGS | 62,880 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 2,075,300 | 99.9% |
| LOAD_GLOBAL | 740 | 0.0% |
| LOAD_GLOBAL_MODULE | 360 | 0.0% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,768,819 | 49.3% |
| LOAD_ATTR | 4,204,780 | 23.6% |
| LOAD_ATTR_MODULE | 2,926,880 | 16.4% |
| BINARY_SUBSCR_DICT | 740,960 | 4.2% |
| LOAD_SUPER_ATTR_ATTR | 538,680 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,392,699 | 80.9% |
| LOAD_FAST_LOAD_FAST | 2,808,560 | 15.8% |
| CALL | 285,380 | 1.6% |
| LOAD_CONST | 143,260 | 0.8% |
| LOAD_GLOBAL_BUILTIN | 93,960 | 0.5% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 2,111,440 | 54.2% |
| CALL_FUNCTION_EX | 1,140,960 | 29.3% |
| COPY_FREE_VARS | 483,780 | 12.4% |
| ENTER_EXECUTOR | 107,280 | 2.8% |
| CACHE | 46,720 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 2,372,800 | 60.9% |
| LOAD_FAST | 1,163,680 | 29.9% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 206,240 | 5.3% |
| GET_YIELD_FROM_ITER | 48,000 | 1.2% |
| INTERPRETER_EXIT | 46,720 | 1.2% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 59,209,023 | 29.9% |
| RETURN_VALUE | 40,322,475 | 20.4% |
| RETURN_CONST | 21,376,660 | 10.8% |
| LOAD_ATTR_SLOT | 18,246,975 | 9.2% |
| CALL | 6,285,840 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 44,701,023 | 22.6% |
| RETURN_VALUE | 40,322,475 | 20.4% |
| LOAD_FAST | 25,055,820 | 12.7% |
| INTERPRETER_EXIT | 24,631,267 | 12.4% |
| POP_TOP | 17,222,880 | 8.7% |


</details>

### SETUP_ANNOTATIONS

<details>
<summary> Successors and predecessors for SETUP_ANNOTATIONS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 40 | 50.0% |
| RESUME | 40 | 50.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 50.0% |
| LOAD_NAME | 40 | 50.0% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,516,620 | 80.3% |
| LOAD_FAST | 174,480 | 9.2% |
| SWAP | 143,720 | 7.6% |
| LOAD_CONST | 40,460 | 2.1% |
| LOAD_ATTR_SLOT | 8,700 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 1,515,560 | 80.3% |
| LOAD_CONST | 171,800 | 9.1% |
| LOAD_FAST | 120,600 | 6.4% |
| RETURN_CONST | 74,940 | 4.0% |
| STORE_SUBSCR | 1,780 | 0.1% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 4,707,640 | 46.1% |
| LOAD_FAST | 3,449,020 | 33.8% |
| LOAD_ATTR_SLOT | 1,334,560 | 13.1% |
| COPY | 549,060 | 5.4% |
| LOAD_ATTR_WITH_HINT | 37,420 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 8,521,840 | 83.4% |
| POP_JUMP_IF_TRUE | 1,437,080 | 14.1% |
| UNARY_NOT | 149,280 | 1.5% |
| TO_BOOL_BOOL | 48,620 | 0.5% |
| TO_BOOL | 27,860 | 0.3% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 700 | 76.1% |
| LOAD_FAST | 220 | 23.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 920 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 504,500 | 51.7% |
| CALL_LEN | 445,240 | 45.7% |
| LOAD_GLOBAL_MODULE | 11,820 | 1.2% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 8,620 | 0.9% |
| LOAD_ATTR_INSTANCE_VALUE | 4,620 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 445,120 | 45.7% |
| COMPARE_OP_INT | 445,080 | 45.7% |
| CALL_PY_EXACT_ARGS | 43,160 | 4.4% |
| RETURN_VALUE | 13,280 | 1.4% |
| BUILD_TUPLE | 11,840 | 1.2% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 11,412,180 | 87.2% |
| TO_BOOL_LIST | 1,262,660 | 9.7% |
| TO_BOOL_STR | 184,780 | 1.4% |
| TO_BOOL | 149,280 | 1.1% |
| TO_BOOL_INT | 69,840 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 6,844,460 | 52.3% |
| RETURN_VALUE | 4,598,720 | 35.2% |
| COPY | 1,285,360 | 9.8% |
| LOAD_FAST | 228,480 | 1.7% |
| STORE_FAST | 76,160 | 0.6% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LEN | 1,322,060 | 56.3% |
| LOAD_FAST | 233,848 | 10.0% |
| BUILD_LIST | 187,120 | 8.0% |
| STORE_FAST | 173,320 | 7.4% |
| LOAD_ATTR | 95,200 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 950,860 | 40.5% |
| STORE_FAST | 611,660 | 26.0% |
| CALL_PY_EXACT_ARGS | 253,840 | 10.8% |
| GET_ITER | 105,320 | 4.5% |
| LOAD_CONST | 67,480 | 2.9% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160 | 44.4% |
| STORE_FAST | 140 | 38.9% |
| RETURN_VALUE | 60 | 16.7% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 12,068,800 | 29.0% |
| STORE_FAST | 9,246,520 | 22.2% |
| LOAD_GLOBAL_MODULE | 5,538,160 | 13.3% |
| RESUME_CHECK | 4,333,700 | 10.4% |
| STORE_ATTR_SLOT | 2,105,820 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 16,125,260 | 38.8% |
| SWAP | 12,068,800 | 29.0% |
| CALL | 5,724,240 | 13.8% |
| LOAD_FAST | 4,046,120 | 9.7% |
| LOAD_GLOBAL_BUILTIN | 1,268,840 | 3.1% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,053,300 | 37.3% |
| LOAD_CONST | 833,160 | 15.1% |
| STORE_ATTR_INSTANCE_VALUE | 479,740 | 8.7% |
| RESUME_CHECK | 441,480 | 8.0% |
| POP_JUMP_IF_FALSE | 398,240 | 7.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,177,880 | 57.8% |
| LOAD_CONST | 805,800 | 14.7% |
| STORE_FAST | 721,299 | 13.1% |
| SWAP | 327,180 | 5.9% |
| RETURN_VALUE | 135,680 | 2.5% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| SWAP | 873,840 | 93.0% |
| LOAD_CONST | 54,880 | 5.8% |
| LOAD_FAST | 10,880 | 1.2% |
| POP_JUMP_IF_FALSE | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 873,840 | 93.0% |
| STORE_FAST | 32,160 | 3.4% |
| CALL_PY_EXACT_ARGS | 22,680 | 2.4% |
| BINARY_OP | 5,600 | 0.6% |
| LOAD_CONST | 5,440 | 0.6% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 9,400 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 8,640 | 91.9% |
| BINARY_SUBSCR | 760 | 8.1% |


</details>

### BUILD_STRING

<details>
<summary> Successors and predecessors for BUILD_STRING </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 491,660 | 67.3% |
| LOAD_CONST | 238,580 | 32.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 239,460 | 32.8% |
| RETURN_VALUE | 188,320 | 25.8% |
| LOAD_FAST | 83,840 | 11.5% |
| CALL | 47,980 | 6.6% |
| CALL_PY_EXACT_ARGS | 42,680 | 5.8% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,510,141 | 35.2% |
| LOAD_GLOBAL_MODULE | 2,606,340 | 16.6% |
| LOAD_ATTR_SLOT | 2,554,539 | 16.3% |
| LOAD_FAST_LOAD_FAST | 2,134,460 | 13.6% |
| LOAD_ATTR_INSTANCE_VALUE | 1,183,460 | 7.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 4,113,060 | 26.3% |
| CALL_BUILTIN_O | 2,834,875 | 18.1% |
| CALL_ISINSTANCE | 2,260,840 | 14.4% |
| LOAD_CONST | 1,986,600 | 12.7% |
| LOAD_FAST | 1,779,400 | 11.4% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,323,668 | 18.4% |
| BUILD_LIST | 5,724,240 | 16.6% |
| LOAD_FAST_LOAD_FAST | 3,482,160 | 10.1% |
| ENTER_EXECUTOR | 3,328,752 | 9.7% |
| RETURN_VALUE | 3,111,475 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 13,585,020 | 39.5% |
| RETURN_VALUE | 6,285,840 | 18.3% |
| LIST_APPEND | 3,514,360 | 10.2% |
| RESUME_CHECK | 2,270,440 | 6.6% |
| TO_BOOL_BOOL | 1,843,700 | 5.4% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_MERGE | 1,932,720 | 48.5% |
| LOAD_FAST | 1,021,680 | 25.6% |
| MAP_ADD | 805,600 | 20.2% |
| LOAD_ATTR | 137,600 | 3.5% |
| CALL_INTRINSIC_1 | 72,400 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 2,017,460 | 50.6% |
| RETURN_GENERATOR | 1,140,960 | 28.6% |
| POP_TOP | 541,440 | 13.6% |
| STORE_FAST | 184,640 | 4.6% |
| RESUME_CHECK | 70,920 | 1.8% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 75,180 | 77.8% |
| RERAISE | 21,440 | 22.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 72,400 | 74.9% |
| RERAISE | 21,440 | 22.2% |
| BUILD_MAP | 2,780 | 2.9% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 37,421,240 | 97.8% |
| ENTER_EXECUTOR | 833,220 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 21,713,260 | 56.8% |
| UNPACK_SEQUENCE_LIST | 7,090,880 | 18.5% |
| RETURN_VALUE | 2,708,100 | 7.1% |
| MAKE_CELL | 2,435,400 | 6.4% |
| CALL_PY_EXACT_ARGS | 1,876,160 | 4.9% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 9,127,082 | 43.4% |
| LOAD_GLOBAL_MODULE | 4,283,460 | 20.3% |
| LOAD_CONST | 3,877,000 | 18.4% |
| LOAD_ATTR_MODULE | 1,253,300 | 6.0% |
| LOAD_FAST | 1,081,120 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 8,443,936 | 40.1% |
| POP_JUMP_IF_FALSE | 6,577,980 | 31.2% |
| RETURN_VALUE | 4,202,960 | 20.0% |
| POP_JUMP_IF_TRUE | 1,281,720 | 6.1% |
| EXTENDED_ARG | 396,960 | 1.9% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,587,220 | 50.5% |
| LOAD_FAST_LOAD_FAST | 8,654,405 | 18.5% |
| LOAD_ATTR_INSTANCE_VALUE | 3,905,799 | 8.4% |
| LOAD_ATTR_SLOT | 2,428,328 | 5.2% |
| BINARY_SUBSCR | 2,232,420 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 39,389,511 | 84.3% |
| POP_JUMP_IF_TRUE | 5,484,401 | 11.7% |
| RETURN_VALUE | 1,426,540 | 3.1% |
| EXTENDED_ARG | 218,460 | 0.5% |
| COPY | 111,680 | 0.2% |


</details>

### CONVERT_VALUE

<details>
<summary> Successors and predecessors for CONVERT_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 33,660 | 98.9% |
| RETURN_CONST | 320 | 0.9% |
| LOAD_GLOBAL_MODULE | 60 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FORMAT_SIMPLE | 34,040 | 100.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP | 8,443,936 | 33.5% |
| LOAD_FAST | 3,062,600 | 12.1% |
| CALL_ISINSTANCE | 2,057,800 | 8.2% |
| SWAP | 1,791,960 | 7.1% |
| COMPARE_OP_STR | 1,547,764 | 6.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 19,175,948 | 76.0% |
| COMPARE_OP_INT | 1,790,160 | 7.1% |
| TO_BOOL_NONE | 898,620 | 3.6% |
| TO_BOOL_STR | 752,600 | 3.0% |
| TO_BOOL | 549,060 | 2.2% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 23,723,100 | 50.5% |
| CACHE | 21,747,640 | 46.3% |
| CALL | 962,800 | 2.0% |
| CALL_ALLOC_AND_ENTER_INIT | 225,240 | 0.5% |
| CALL_KW | 212,160 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 46,507,260 | 99.0% |
| RETURN_GENERATOR | 483,780 | 1.0% |
| RESUME | 3,080 | 0.0% |


</details>

### DELETE_ATTR

<details>
<summary> Successors and predecessors for DELETE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,627,200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,402,080 | 78.2% |
| NOP | 1,140,960 | 20.3% |
| RETURN_CONST | 84,160 | 1.5% |


</details>

### DELETE_FAST

<details>
<summary> Successors and predecessors for DELETE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 100,960 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RERAISE | 100,640 | 99.7% |
| JUMP_BACKWARD | 320 | 0.3% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,932,720 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 1,932,720 | 100.0% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 15,111,942 | 25.9% |
| POP_TOP | 15,023,379 | 25.8% |
| LIST_APPEND | 12,636,056 | 21.7% |
| CALL_LIST_APPEND | 5,011,440 | 8.6% |
| POP_JUMP_IF_FALSE | 1,717,016 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 23,900,257 | 41.0% |
| FOR_ITER_TUPLE | 4,235,114 | 7.3% |
| LOAD_ATTR_METHOD_NO_DICT | 3,998,811 | 6.9% |
| CALL | 3,328,752 | 5.7% |
| RESUME_CHECK | 2,936,891 | 5.0% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 4,527,340 | 37.7% |
| GET_ITER | 2,309,300 | 19.2% |
| ENTER_EXECUTOR | 713,240 | 5.9% |
| LOAD_ATTR_SLOT | 627,020 | 5.2% |
| TO_BOOL_ALWAYS_TRUE | 487,160 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,759,500 | 56.2% |
| FOR_ITER | 1,586,060 | 13.2% |
| FOR_ITER_LIST | 1,325,380 | 11.0% |
| POP_JUMP_IF_NONE | 1,217,980 | 10.1% |
| JUMP_FORWARD | 623,140 | 5.2% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 7,262,235 | 77.8% |
| EXTENDED_ARG | 1,586,060 | 17.0% |
| SWAP | 364,080 | 3.9% |
| JUMP_BACKWARD | 54,644 | 0.6% |
| LOAD_FAST | 42,460 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 2,891,675 | 31.0% |
| RETURN_CONST | 2,194,441 | 23.5% |
| STORE_FAST | 1,932,422 | 20.7% |
| LOAD_FAST | 1,133,443 | 12.1% |
| LOAD_GLOBAL_BUILTIN | 279,720 | 3.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 913,400 | 75.2% |
| STORE_FAST | 300,320 | 24.7% |
| STORE_NAME | 840 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,213,280 | 99.9% |
| STORE_NAME | 1,280 | 0.1% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 979,900 | 98.8% |
| ENTER_EXECUTOR | 11,940 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 913,400 | 92.1% |
| STORE_FAST | 78,240 | 7.9% |
| STORE_DEREF | 160 | 0.0% |
| STORE_NAME | 40 | 0.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 20,791,560 | 73.3% |
| LOAD_CONST | 3,542,440 | 12.5% |
| LOAD_FAST | 3,498,000 | 12.3% |
| LOAD_FAST_LOAD_FAST | 445,120 | 1.6% |
| LOAD_ATTR | 47,960 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 19,064,900 | 67.2% |
| POP_JUMP_IF_TRUE | 5,792,320 | 20.4% |
| RETURN_VALUE | 2,006,560 | 7.1% |
| LOAD_FAST | 818,720 | 2.9% |
| COPY | 400,740 | 1.4% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 608,789 | 67.9% |
| POP_TOP | 81,280 | 9.1% |
| CALL_LIST_APPEND | 65,400 | 7.3% |
| LIST_APPEND | 43,980 | 4.9% |
| EXTENDED_ARG | 23,820 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_GEN | 615,420 | 68.6% |
| FOR_ITER_LIST | 153,960 | 17.2% |
| FOR_ITER | 54,644 | 6.1% |
| EXTENDED_ARG | 31,380 | 3.5% |
| ENTER_EXECUTOR | 15,140 | 1.7% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 181,500 | 95.9% |
| POP_EXCEPT | 7,320 | 3.9% |
| EXTENDED_ARG | 320 | 0.2% |
| RESUME | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 181,520 | 95.9% |
| LOAD_FAST | 5,080 | 2.7% |
| NOP | 2,240 | 1.2% |
| LOAD_FAST_LOAD_FAST | 160 | 0.1% |
| LOAD_GLOBAL_MODULE | 120 | 0.1% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NONE | 7,009,120 | 28.8% |
| LOAD_ATTR_SLOT | 6,820,340 | 28.0% |
| LOAD_FAST | 3,303,000 | 13.6% |
| STORE_ATTR_SLOT | 2,753,340 | 11.3% |
| STORE_FAST | 1,805,708 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,466,368 | 51.2% |
| STORE_FAST | 7,290,720 | 29.9% |
| MAP_ADD | 3,137,760 | 12.9% |
| LOAD_CONST | 513,280 | 2.1% |
| LOAD_GLOBAL_MODULE | 481,062 | 2.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,565,260 | 59.7% |
| CALL | 3,514,360 | 27.7% |
| LOAD_FAST | 771,756 | 6.1% |
| BINARY_SUBSCR_LIST_INT | 168,300 | 1.3% |
| LOAD_ATTR_SLOT | 154,640 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 12,636,056 | 99.7% |
| JUMP_BACKWARD | 43,980 | 0.3% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,020 | 81.0% |
| RETURN_VALUE | 9,440 | 12.5% |
| BINARY_SLICE | 4,480 | 5.9% |
| LOAD_CONST | 160 | 0.2% |
| STORE_FAST | 160 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 75,180 | 99.8% |
| LOAD_CONST | 160 | 0.2% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 37,203,103 | 66.8% |
| LOAD_GLOBAL_MODULE | 13,883,100 | 24.9% |
| LOAD_ATTR_INSTANCE_VALUE | 1,309,620 | 2.4% |
| LOAD_FAST_LOAD_FAST | 982,020 | 1.8% |
| CALL_TYPE_1 | 721,960 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 24,813,912 | 44.5% |
| LOAD_FAST_LOAD_FAST | 5,521,600 | 9.9% |
| TO_BOOL | 4,707,640 | 8.5% |
| PUSH_NULL | 4,204,780 | 7.5% |
| CALL_PY_EXACT_ARGS | 3,335,540 | 6.0% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 84,645,340 | 24.5% |
| LOAD_FAST | 76,467,519 | 22.2% |
| LOAD_CONST | 26,735,640 | 7.7% |
| LOAD_ATTR_INSTANCE_VALUE | 13,812,300 | 4.0% |
| MAP_ADD | 13,695,200 | 4.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 140,029,840 | 40.6% |
| BINARY_SUBSCR_DICT | 50,556,380 | 14.6% |
| CALL_KW | 37,421,240 | 10.8% |
| LOAD_CONST | 26,735,640 | 7.7% |
| COMPARE_OP_STR | 15,472,516 | 4.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 46,031,900 | 71.2% |
| LOAD_DEREF | 6,472,140 | 10.0% |
| LOAD_FAST | 2,717,180 | 4.2% |
| LOAD_GLOBAL_MODULE | 2,447,080 | 3.8% |
| POP_JUMP_IF_FALSE | 1,297,357 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 44,051,819 | 68.1% |
| LOAD_DEREF | 6,472,140 | 10.0% |
| LOAD_ATTR_SLOT | 3,885,740 | 6.0% |
| LOAD_CONST | 2,153,847 | 3.3% |
| LOAD_FAST_LOAD_FAST | 1,759,440 | 2.7% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 187,798,718 | 13.0% |
| RESUME_CHECK | 150,584,697 | 10.4% |
| LOAD_CONST | 140,029,840 | 9.7% |
| POP_JUMP_IF_FALSE | 124,176,427 | 8.6% |
| STORE_FAST | 120,089,730 | 8.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 217,327,781 | 15.0% |
| STORE_ATTR_SLOT | 179,530,299 | 12.4% |
| LOAD_GLOBAL_MODULE | 133,064,751 | 9.2% |
| LOAD_ATTR_METHOD_NO_DICT | 94,137,682 | 6.5% |
| CALL_PY_EXACT_ARGS | 80,412,339 | 5.5% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 13,269,820 | 95.5% |
| LOAD_FAST_AND_CLEAR | 623,940 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 13,264,380 | 95.5% |
| LOAD_FAST_AND_CLEAR | 623,940 | 4.5% |
| MAKE_CELL | 5,440 | 0.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,078,160 | 76.4% |
| POP_JUMP_IF_FALSE | 152,800 | 10.8% |
| LOAD_GLOBAL_BUILTIN | 134,640 | 9.5% |
| POP_JUMP_IF_TRUE | 12,320 | 0.9% |
| LOAD_FAST_CHECK | 10,720 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_NOT_NONE | 1,004,400 | 71.2% |
| LOAD_ATTR_SLOT | 88,760 | 6.3% |
| EXTENDED_ARG | 81,440 | 5.8% |
| LOAD_ATTR_METHOD_WITH_VALUES | 76,040 | 5.4% |
| TO_BOOL_BOOL | 50,000 | 3.5% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 70,357,660 | 25.1% |
| LOAD_SUPER_ATTR_METHOD | 35,810,960 | 12.8% |
| RESUME_CHECK | 30,206,540 | 10.8% |
| LOAD_GLOBAL_MODULE | 22,881,620 | 8.2% |
| STORE_FAST | 20,697,751 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 124,049,340 | 44.2% |
| CALL_PY_EXACT_ARGS | 51,162,000 | 18.2% |
| STORE_ATTR_INSTANCE_VALUE | 22,102,080 | 7.9% |
| LOAD_FAST | 19,246,809 | 6.9% |
| CONTAINS_OP | 8,654,405 | 3.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 45,600 | 18.8% |
| POP_JUMP_IF_FALSE | 44,590 | 18.4% |
| STORE_FAST | 38,322 | 15.8% |
| RESUME_CHECK | 12,440 | 5.1% |
| RESUME | 12,340 | 5.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 75,380 | 31.0% |
| LOAD_FAST | 52,660 | 21.7% |
| LOAD_GLOBAL_BUILTIN | 46,100 | 19.0% |
| CALL | 26,740 | 11.0% |
| LOAD_ATTR | 11,600 | 4.8% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,080 | 51.4% |
| LOAD_NAME | 580 | 27.6% |
| STORE_NAME | 200 | 9.5% |
| STORE_SUBSCR | 100 | 4.8% |
| SETUP_ANNOTATIONS | 40 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 580 | 27.6% |
| LOAD_NAME | 580 | 27.6% |
| BUILD_TUPLE | 380 | 18.1% |
| BINARY_SUBSCR | 300 | 14.3% |
| GET_ITER | 80 | 3.8% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,820 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 2,400 | 49.8% |
| CALL | 1,040 | 21.6% |
| LOAD_FAST | 680 | 14.1% |
| LOAD_FAST_LOAD_FAST | 420 | 8.7% |
| LOAD_GLOBAL | 180 | 3.7% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 10,918,760 | 65.8% |
| CALL_KW | 2,435,400 | 14.7% |
| CALL_PY_EXACT_ARGS | 2,428,480 | 14.6% |
| BINARY_SUBSCR_GETITEM | 470,380 | 2.8% |
| CALL_PY_WITH_DEFAULTS | 292,600 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| MAKE_CELL | 10,918,760 | 65.8% |
| RESUME_CHECK | 5,670,760 | 34.2% |
| SWAP | 5,440 | 0.0% |
| RESUME | 1,640 | 0.0% |
| RETURN_GENERATOR | 1,280 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 10,557,100 | 71.4% |
| JUMP_FORWARD | 3,137,760 | 21.2% |
| CALL_BUILTIN_CLASS | 807,480 | 5.5% |
| LOAD_FAST | 128,320 | 0.9% |
| RETURN_VALUE | 80,220 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,695,200 | 92.6% |
| CALL_FUNCTION_EX | 805,600 | 5.4% |
| ENTER_EXECUTOR | 276,828 | 1.9% |
| JUMP_BACKWARD | 4,240 | 0.0% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 138,134,325 | 51.5% |
| CONTAINS_OP | 39,389,511 | 14.7% |
| IS_OP | 19,064,900 | 7.1% |
| TO_BOOL_ALWAYS_TRUE | 12,570,771 | 4.7% |
| TO_BOOL_NONE | 11,557,849 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 124,176,427 | 46.3% |
| LOAD_GLOBAL_BUILTIN | 65,430,109 | 24.4% |
| LOAD_GLOBAL_MODULE | 23,041,420 | 8.6% |
| LOAD_FAST_LOAD_FAST | 13,882,029 | 5.2% |
| POP_TOP | 10,313,024 | 3.8% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,363,320 | 48.9% |
| LOAD_ATTR_SLOT | 15,204,780 | 38.4% |
| LOAD_ATTR | 2,024,300 | 5.1% |
| EXTENDED_ARG | 1,217,980 | 3.1% |
| BINARY_SUBSCR_DICT | 1,046,200 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 18,875,340 | 47.6% |
| RETURN_CONST | 7,931,660 | 20.0% |
| JUMP_FORWARD | 7,009,120 | 17.7% |
| LOAD_CONST | 2,261,380 | 5.7% |
| LOAD_GLOBAL_BUILTIN | 1,491,170 | 3.8% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 41,245,400 | 87.4% |
| LOAD_ATTR_SLOT | 2,407,440 | 5.1% |
| BINARY_SUBSCR_DICT | 1,975,220 | 4.2% |
| LOAD_FAST_CHECK | 1,004,400 | 2.1% |
| BINARY_SUBSCR | 149,100 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 18,197,520 | 38.6% |
| LOAD_FAST | 9,714,340 | 20.6% |
| LOAD_CONST | 6,937,160 | 14.7% |
| LOAD_FAST_LOAD_FAST | 5,298,280 | 11.2% |
| RETURN_CONST | 2,321,120 | 4.9% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 50,313,766 | 46.3% |
| TO_BOOL_LIST | 17,346,660 | 16.0% |
| COMPARE_OP_STR | 13,452,832 | 12.4% |
| COMPARE_OP_INT | 5,824,319 | 5.4% |
| IS_OP | 5,792,320 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 48,737,708 | 44.8% |
| ENTER_EXECUTOR | 15,111,942 | 13.9% |
| LOAD_GLOBAL_MODULE | 10,947,280 | 10.1% |
| POP_TOP | 8,672,052 | 8.0% |
| NOP | 7,043,520 | 6.5% |


</details>

### RAISE_VARARGS

<details>
<summary> Successors and predecessors for RAISE_VARARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 100,640 | 59.3% |
| RETURN_VALUE | 36,960 | 21.8% |
| CALL | 25,840 | 15.2% |
| LOAD_CONST | 6,080 | 3.6% |
| POP_TOP | 160 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100,640 | 59.3% |
| PUSH_EXC_INFO | 62,880 | 37.0% |
| COPY | 6,240 | 3.7% |


</details>

### RERAISE

<details>
<summary> Successors and predecessors for RERAISE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_EXCEPT | 128,320 | 47.2% |
| DELETE_FAST | 100,640 | 37.0% |
| CALL_INTRINSIC_1 | 21,440 | 7.9% |
| POP_JUMP_IF_FALSE | 21,440 | 7.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 122,080 | 48.8% |
| PUSH_EXC_INFO | 106,720 | 42.6% |
| CALL_INTRINSIC_1 | 21,440 | 8.6% |


</details>

### RETURN_CONST

<details>
<summary> Successors and predecessors for RETURN_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 60,343,400 | 40.3% |
| RESUME_CHECK | 33,811,860 | 22.6% |
| POP_TOP | 11,525,120 | 7.7% |
| POP_JUMP_IF_FALSE | 8,937,960 | 6.0% |
| POP_JUMP_IF_NONE | 7,931,660 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 52,750,020 | 35.2% |
| INTERPRETER_EXIT | 30,999,340 | 20.7% |
| LOAD_FAST | 30,810,880 | 20.6% |
| RETURN_VALUE | 21,376,660 | 14.3% |
| TO_BOOL_BOOL | 5,710,880 | 3.8% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 80 | 66.7% |
| JUMP_BACKWARD_NO_INTERRUPT | 40 | 33.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 60 | 50.0% |
| SEND_GEN | 60 | 50.0% |


</details>

### SET_ADD

<details>
<summary> Successors and predecessors for SET_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP_ADD_UNICODE | 641,040 | 91.5% |
| LOAD_ATTR_INSTANCE_VALUE | 31,660 | 4.5% |
| STORE_FAST_LOAD_FAST | 20,180 | 2.9% |
| LOAD_FAST | 3,630 | 0.5% |
| RETURN_VALUE | 3,200 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 696,110 | 99.3% |
| JUMP_BACKWARD | 4,620 | 0.7% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 1,985,800 | 77.2% |
| SET_FUNCTION_ATTRIBUTE | 585,780 | 22.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 856,340 | 33.3% |
| SET_FUNCTION_ATTRIBUTE | 585,780 | 22.8% |
| STORE_FAST | 511,260 | 19.9% |
| LOAD_FAST | 226,380 | 8.8% |
| STORE_DEREF | 212,480 | 8.3% |


</details>

### SET_UPDATE

<details>
<summary> Successors and predecessors for SET_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 160 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 160 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 4,712,600 | 80.7% |
| LOAD_FAST | 1,043,640 | 17.9% |
| SWAP | 59,400 | 1.0% |
| STORE_ATTR | 20,280 | 0.3% |
| LOAD_ATTR_SLOT | 4,900 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,696,580 | 46.1% |
| RETURN_CONST | 1,590,540 | 27.2% |
| LOAD_FAST | 1,197,300 | 20.5% |
| LOAD_CONST | 133,040 | 2.3% |
| LOAD_GLOBAL_MODULE | 128,920 | 2.2% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,944,320 | 82.3% |
| SET_FUNCTION_ATTRIBUTE | 212,480 | 9.0% |
| RETURN_VALUE | 80,440 | 3.4% |
| LOAD_ATTR_SLOT | 51,480 | 2.2% |
| FOR_ITER_LIST | 19,340 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,464,560 | 62.0% |
| LOAD_FAST | 565,920 | 24.0% |
| LOAD_GLOBAL_BUILTIN | 129,580 | 5.5% |
| LOAD_CONST | 94,600 | 4.0% |
| LOAD_DEREF | 88,520 | 3.7% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 44,701,023 | 18.3% |
| FOR_ITER_LIST | 26,557,685 | 10.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 25,888,372 | 10.6% |
| LOAD_ATTR_SLOT | 22,174,660 | 9.1% |
| BUILD_LIST | 16,125,260 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 120,089,730 | 49.1% |
| LOAD_GLOBAL_BUILTIN | 35,845,511 | 14.7% |
| LOAD_GLOBAL_MODULE | 29,108,358 | 11.9% |
| LOAD_FAST_LOAD_FAST | 20,697,751 | 8.5% |
| LOAD_CONST | 9,423,180 | 3.9% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 2,655,548 | 70.0% |
| FOR_ITER_TUPLE | 878,760 | 23.2% |
| FOR_ITER_RANGE | 167,600 | 4.4% |
| FOR_ITER | 90,140 | 2.4% |
| CALL_LEN | 1,000 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,489,920 | 39.3% |
| LOAD_CONST | 861,368 | 22.7% |
| LOAD_ATTR_INSTANCE_VALUE | 623,600 | 16.4% |
| LOAD_ATTR_METHOD_NO_DICT | 263,060 | 6.9% |
| LOAD_FAST | 211,960 | 5.6% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_LIST | 7,221,420 | 58.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 3,885,275 | 31.4% |
| UNPACK_SEQUENCE_TUPLE | 793,340 | 6.4% |
| COPY | 304,900 | 2.5% |
| BINARY_SUBSCR_LIST_INT | 47,420 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,287,775 | 75.1% |
| LOAD_FAST_LOAD_FAST | 1,130,700 | 9.1% |
| STORE_FAST | 861,095 | 7.0% |
| LOAD_GLOBAL_BUILTIN | 652,540 | 5.3% |
| LOAD_GLOBAL_MODULE | 175,340 | 1.4% |


</details>

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 1,280 | 57.1% |
| SET_FUNCTION_ATTRIBUTE | 560 | 25.0% |
| LOAD_CONST | 120 | 5.4% |
| CALL | 80 | 3.6% |
| BUILD_STRING | 60 | 2.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| IMPORT_FROM | 840 | 37.5% |
| LOAD_CONST | 620 | 27.7% |
| POP_TOP | 440 | 19.6% |
| LOAD_NAME | 200 | 8.9% |
| RETURN_CONST | 60 | 2.7% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_AND_CLEAR | 13,264,380 | 30.3% |
| BUILD_LIST | 12,068,800 | 27.6% |
| FOR_ITER_LIST | 8,931,460 | 20.4% |
| LOAD_FAST | 2,412,440 | 5.5% |
| CALL_LEN | 1,790,200 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_LIST | 12,068,800 | 27.6% |
| FOR_ITER_LIST | 11,185,020 | 25.6% |
| STORE_FAST | 10,709,800 | 24.5% |
| COPY | 1,791,960 | 4.1% |
| POP_TOP | 1,759,060 | 4.0% |


</details>

### UNPACK_EX

<details>
<summary> Successors and predecessors for UNPACK_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 380 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 380 | 100.0% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 45,280 | 60.5% |
| COPY | 13,280 | 17.7% |
| FOR_ITER_LIST | 4,599 | 6.1% |
| FOR_ITER | 4,540 | 6.1% |
| RETURN_VALUE | 3,680 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 49,699 | 66.4% |
| STORE_FAST_STORE_FAST | 19,040 | 25.4% |
| UNPACK_SEQUENCE_TWO_TUPLE | 4,120 | 5.5% |
| UNPACK_SEQUENCE_TUPLE | 980 | 1.3% |
| UNPACK_SEQUENCE | 740 | 1.0% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,262,480 | 22.4% |
| LOAD_CONST | 942,720 | 16.8% |
| ENTER_EXECUTOR | 880,640 | 15.7% |
| LOAD_FAST | 571,420 | 10.2% |
| CALL_ISINSTANCE | 399,700 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| INTERPRETER_EXIT | 4,806,360 | 85.4% |
| STORE_FAST | 448,760 | 8.0% |
| UNPACK_SEQUENCE_TUPLE | 188,040 | 3.3% |
| YIELD_VALUE | 181,560 | 3.2% |
| UNPACK_SEQUENCE | 60 | 0.0% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 19,880 | 48.6% |
| CACHE | 5,500 | 13.5% |
| CALL_PY_EXACT_ARGS | 5,500 | 13.5% |
| COPY_FREE_VARS | 3,080 | 7.5% |
| POP_TOP | 2,420 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 19,400 | 47.5% |
| LOAD_GLOBAL | 12,340 | 30.2% |
| LOAD_FAST_LOAD_FAST | 2,060 | 5.0% |
| LOAD_CONST | 1,920 | 4.7% |
| POP_TOP | 1,820 | 4.5% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 118,140 | 82.6% |
| ENTER_EXECUTOR | 24,560 | 17.2% |
| BINARY_OP_ADD_INT | 380 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 142,720 | 99.7% |
| BINARY_OP_ADD_INT | 360 | 0.3% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,027,949 | 55.1% |
| CALL_LEN | 755,560 | 20.5% |
| CALL_METHOD_DESCRIPTOR_O | 733,880 | 19.9% |
| LOAD_FAST_LOAD_FAST | 79,499 | 2.2% |
| LOAD_FAST | 76,580 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,581,660 | 43.0% |
| LOAD_FAST | 984,029 | 26.7% |
| SWAP | 478,280 | 13.0% |
| LOAD_FAST_LOAD_FAST | 295,180 | 8.0% |
| LOAD_CONST | 106,900 | 2.9% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 981,640 | 35.8% |
| LOAD_FAST | 509,560 | 18.6% |
| CALL_METHOD_DESCRIPTOR_O | 492,280 | 17.9% |
| LOAD_FAST_LOAD_FAST | 492,220 | 17.9% |
| LOAD_ATTR | 180,080 | 6.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 773,440 | 28.2% |
| RETURN_VALUE | 673,140 | 24.5% |
| SET_ADD | 641,040 | 23.3% |
| STORE_FAST | 346,640 | 12.6% |
| BINARY_OP_INPLACE_ADD_UNICODE | 164,520 | 6.0% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 600 | 96.8% |
| BINARY_OP | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 600 | 96.8% |
| CALL | 20 | 3.2% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,600 | 80.2% |
| BINARY_SUBSCR_TUPLE_INT | 640 | 19.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 2,240 | 69.1% |
| BINARY_OP_ADD_INT | 640 | 19.8% |
| LOAD_CONST | 180 | 5.6% |
| CALL_BUILTIN_O | 180 | 5.6% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 89,280 | 61.0% |
| LOAD_FAST_LOAD_FAST | 56,640 | 38.7% |
| BINARY_OP | 380 | 0.3% |
| LOAD_ATTR_WITH_HINT | 120 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 117,680 | 80.4% |
| LOAD_FAST_LOAD_FAST | 28,260 | 19.3% |
| LOAD_GLOBAL_BUILTIN | 240 | 0.2% |
| LOAD_FAST | 140 | 0.1% |
| BINARY_OP | 60 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,761,479 | 93.6% |
| LOAD_FAST | 61,830 | 3.3% |
| CALL_LEN | 50,500 | 2.7% |
| LOAD_FAST_LOAD_FAST | 3,760 | 0.2% |
| LOAD_ATTR_SLOT | 1,880 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 924,880 | 49.2% |
| BINARY_SLICE | 445,100 | 23.7% |
| SWAP | 145,000 | 7.7% |
| STORE_FAST | 138,360 | 7.4% |
| BINARY_SUBSCR_LIST_INT | 131,700 | 7.0% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 50,556,380 | 86.3% |
| LOAD_FAST | 4,410,613 | 7.5% |
| BINARY_SUBSCR_DICT | 1,517,419 | 2.6% |
| BINARY_SUBSCR_LIST_INT | 910,680 | 1.6% |
| LOAD_DEREF | 751,600 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,883,220 | 18.6% |
| LOAD_CONST | 9,943,220 | 17.0% |
| STORE_FAST | 9,915,511 | 16.9% |
| GET_ITER | 6,242,220 | 10.7% |
| CALL_PY_EXACT_ARGS | 4,758,320 | 8.1% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 766,520 | 54.8% |
| ENTER_EXECUTOR | 424,660 | 30.4% |
| LOAD_FAST_LOAD_FAST | 199,420 | 14.3% |
| LOAD_CONST | 6,860 | 0.5% |
| LOAD_FAST | 420 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 927,280 | 66.3% |
| MAKE_CELL | 470,380 | 33.6% |
| LOAD_ATTR_SLOT | 320 | 0.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,153,540 | 46.0% |
| LOAD_FAST | 2,591,580 | 28.7% |
| LOAD_FAST_LOAD_FAST | 2,098,120 | 23.2% |
| BINARY_OP_SUBTRACT_INT | 131,700 | 1.5% |
| BINARY_OP_ADD_INT | 23,800 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,312,280 | 14.5% |
| LOAD_FAST | 1,206,000 | 13.4% |
| LOAD_GLOBAL_MODULE | 1,127,160 | 12.5% |
| BINARY_SUBSCR_DICT | 910,680 | 10.1% |
| LOAD_ATTR_INSTANCE_VALUE | 736,600 | 8.2% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 374,140 | 80.6% |
| BINARY_OP_ADD_INT | 58,680 | 12.6% |
| BINARY_OP_SUBTRACT_INT | 18,400 | 4.0% |
| LOAD_FAST_LOAD_FAST | 10,939 | 2.4% |
| LOAD_FAST | 1,700 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 317,200 | 68.3% |
| LOAD_FAST | 70,099 | 15.1% |
| CALL_BUILTIN_O | 33,900 | 7.3% |
| LOAD_FAST_LOAD_FAST | 16,920 | 3.6% |
| COMPARE_OP_STR | 16,880 | 3.6% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 835,640 | 99.6% |
| LOAD_FAST_LOAD_FAST | 2,160 | 0.3% |
| BINARY_SUBSCR | 1,440 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 153,680 | 18.3% |
| FORMAT_SIMPLE | 140,800 | 16.8% |
| LOAD_FAST_LOAD_FAST | 105,300 | 12.5% |
| STORE_FAST | 101,680 | 12.1% |
| CALL | 77,740 | 9.3% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,562,660 | 46.9% |
| LOAD_FAST | 902,560 | 27.1% |
| LOAD_GLOBAL_MODULE | 327,580 | 9.8% |
| CALL | 216,600 | 6.5% |
| RETURN_VALUE | 182,760 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 3,103,900 | 93.1% |
| COPY_FREE_VARS | 225,240 | 6.8% |
| CALL_PY_EXACT_ARGS | 3,200 | 0.1% |
| STORE_FAST | 1,280 | 0.0% |
| MAKE_CELL | 140 | 0.0% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,616,040 | 58.9% |
| BINARY_SUBSCR_DICT | 3,226,120 | 24.9% |
| LOAD_CONST | 1,345,980 | 10.4% |
| ENTER_EXECUTOR | 461,220 | 3.6% |
| RETURN_VALUE | 140,080 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 11,545,700 | 89.3% |
| POP_TOP | 1,311,880 | 10.1% |
| CALL_PY_EXACT_ARGS | 50,520 | 0.4% |
| CALL_BOUND_METHOD_EXACT_ARGS | 24,640 | 0.2% |
| RESUME | 980 | 0.0% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,913,080 | 29.5% |
| LOAD_GLOBAL_BUILTIN | 3,561,520 | 17.8% |
| LOAD_ATTR_SLOT | 2,257,986 | 11.3% |
| LOAD_ATTR_CLASS | 1,894,480 | 9.5% |
| CALL_LEN | 1,536,780 | 7.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,501,680 | 47.4% |
| LOAD_FAST | 5,260,200 | 26.3% |
| STORE_FAST | 1,886,260 | 9.4% |
| RETURN_VALUE | 1,272,480 | 6.4% |
| MAP_ADD | 807,480 | 4.0% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 2,946,559 | 46.1% |
| LOAD_ATTR_INSTANCE_VALUE | 2,329,880 | 36.4% |
| LOAD_FAST_LOAD_FAST | 922,720 | 14.4% |
| LOAD_FAST | 99,840 | 1.6% |
| LOAD_GLOBAL_BUILTIN | 45,000 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,448,300 | 22.7% |
| RETURN_VALUE | 1,162,840 | 18.2% |
| PUSH_EXC_INFO | 1,143,320 | 17.9% |
| TO_BOOL_BOOL | 1,020,340 | 16.0% |
| POP_TOP | 819,560 | 12.8% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,597,760 | 83.1% |
| RETURN_GENERATOR | 206,240 | 10.7% |
| CALL_BUILTIN_CLASS | 70,840 | 3.7% |
| RETURN_VALUE | 24,360 | 1.3% |
| LOAD_CONST | 13,060 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,318,640 | 68.6% |
| COPY | 167,680 | 8.7% |
| LOAD_CONST | 152,140 | 7.9% |
| PUSH_EXC_INFO | 88,420 | 4.6% |
| RETURN_VALUE | 85,420 | 4.4% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 2,834,875 | 35.8% |
| RETURN_GENERATOR | 2,372,800 | 30.0% |
| LOAD_FAST | 1,062,720 | 13.4% |
| LOAD_GLOBAL_MODULE | 602,364 | 7.6% |
| LOAD_ATTR_INSTANCE_VALUE | 326,720 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 3,484,914 | 44.1% |
| LOAD_FAST | 2,478,159 | 31.3% |
| TO_BOOL_BOOL | 849,000 | 10.7% |
| CALL_PY_EXACT_ARGS | 452,260 | 5.7% |
| STORE_FAST | 229,580 | 2.9% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 114,689,090 | 84.3% |
| LOAD_GLOBAL_BUILTIN | 17,546,400 | 12.9% |
| BUILD_TUPLE | 2,260,840 | 1.7% |
| LOAD_ATTR | 948,840 | 0.7% |
| LOAD_ATTR_MODULE | 470,451 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 133,033,603 | 97.7% |
| COPY | 2,057,800 | 1.5% |
| YIELD_VALUE | 399,700 | 0.3% |
| RETURN_VALUE | 373,258 | 0.3% |
| STORE_FAST | 197,740 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,027,860 | 56.6% |
| LOAD_ATTR_SLOT | 5,536,820 | 31.3% |
| LOAD_DEREF | 950,280 | 5.4% |
| LOAD_ATTR_INSTANCE_VALUE | 949,080 | 5.4% |
| LOAD_ATTR | 108,320 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,681,680 | 26.4% |
| COMPARE_OP_INT | 2,944,020 | 16.6% |
| LOAD_GLOBAL_BUILTIN | 2,281,860 | 12.9% |
| SWAP | 1,790,200 | 10.1% |
| CALL_BUILTIN_CLASS | 1,536,780 | 8.7% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,322,855 | 76.7% |
| RETURN_VALUE | 1,294,300 | 8.1% |
| ENTER_EXECUTOR | 945,304 | 5.9% |
| LOAD_CONST | 283,720 | 1.8% |
| BUILD_TUPLE | 273,981 | 1.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,763,100 | 54.5% |
| ENTER_EXECUTOR | 5,011,440 | 31.2% |
| NOP | 1,217,640 | 7.6% |
| LOAD_CONST | 340,240 | 2.1% |
| LOAD_GLOBAL_BUILTIN | 238,680 | 1.5% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,155,499 | 54.6% |
| LOAD_ATTR_METHOD_NO_DICT | 10,081,817 | 32.1% |
| LOAD_CONST | 1,359,800 | 4.3% |
| ENTER_EXECUTOR | 946,180 | 3.0% |
| LOAD_GLOBAL_MODULE | 611,430 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 25,888,372 | 82.4% |
| POP_TOP | 2,371,877 | 7.6% |
| LOAD_FAST | 1,338,413 | 4.3% |
| CALL_PY_EXACT_ARGS | 436,080 | 1.4% |
| LOAD_ATTR_METHOD_NO_DICT | 310,340 | 1.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,235,500 | 89.0% |
| LOAD_FAST | 93,640 | 6.7% |
| LOAD_ATTR_MODULE | 46,200 | 3.3% |
| LOAD_ATTR_METHOD_NO_DICT | 12,840 | 0.9% |
| CALL | 680 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,053,820 | 75.9% |
| LOAD_CONST | 125,000 | 9.0% |
| GET_ITER | 94,180 | 6.8% |
| CONTAINS_OP | 46,220 | 3.3% |
| RETURN_VALUE | 45,860 | 3.3% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 1,486,920 | 98.0% |
| ENTER_EXECUTOR | 22,540 | 1.5% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 3,080 | 0.2% |
| LOAD_ATTR | 2,760 | 0.2% |
| CALL | 1,540 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 863,820 | 56.9% |
| LOAD_FAST | 287,380 | 18.9% |
| POP_TOP | 160,140 | 10.6% |
| CALL_BUILTIN_CLASS | 119,760 | 7.9% |
| LOAD_ATTR_METHOD_NO_DICT | 44,760 | 3.0% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 3,258,200 | 55.2% |
| LOAD_FAST | 1,853,119 | 31.4% |
| RETURN_VALUE | 315,360 | 5.3% |
| BUILD_TUPLE | 121,560 | 2.1% |
| LOAD_ATTR_SLOT | 104,580 | 1.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,538,780 | 43.0% |
| POP_TOP | 2,008,699 | 34.0% |
| BINARY_OP_ADD_INT | 733,880 | 12.4% |
| BINARY_OP_ADD_UNICODE | 492,280 | 8.3% |
| STORE_FAST | 85,860 | 1.5% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80,412,339 | 37.2% |
| LOAD_FAST_LOAD_FAST | 51,162,000 | 23.7% |
| LOAD_ATTR_METHOD_NO_DICT | 37,184,112 | 17.2% |
| LOAD_ATTR_SLOT | 6,884,329 | 3.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 5,450,400 | 2.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 187,249,916 | 86.6% |
| COPY_FREE_VARS | 23,723,100 | 11.0% |
| MAKE_CELL | 2,428,480 | 1.1% |
| RETURN_GENERATOR | 2,111,440 | 1.0% |
| CALL_PY_EXACT_ARGS | 358,895 | 0.2% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 3,965,600 | 38.3% |
| LOAD_FAST | 3,368,547 | 32.5% |
| LOAD_FAST_LOAD_FAST | 918,740 | 8.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 577,060 | 5.6% |
| LOAD_ATTR_SLOT | 322,200 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 9,944,340 | 96.0% |
| MAKE_CELL | 292,600 | 2.8% |
| COPY_FREE_VARS | 116,240 | 1.1% |
| CALL_PY_EXACT_ARGS | 3,960 | 0.0% |
| RETURN_GENERATOR | 460 | 0.0% |


</details>

### CALL_STR_1

<details>
<summary> Successors and predecessors for CALL_STR_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 609,700 | 100.0% |
| UNARY_NOT | 120 | 0.0% |
| CALL | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 491,820 | 80.6% |
| CALL_BUILTIN_O | 93,740 | 15.4% |
| STORE_FAST | 16,660 | 2.7% |
| CALL | 7,520 | 1.2% |
| BUILD_TUPLE | 140 | 0.0% |


</details>

### CALL_TUPLE_1

<details>
<summary> Successors and predecessors for CALL_TUPLE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,409,420 | 92.5% |
| LOAD_ATTR_SLOT | 732,236 | 7.2% |
| RETURN_VALUE | 11,340 | 0.1% |
| LOAD_FAST_CHECK | 9,720 | 0.1% |
| RETURN_GENERATOR | 4,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,480,180 | 93.2% |
| LOAD_GLOBAL_BUILTIN | 381,080 | 3.7% |
| BUILD_TUPLE | 265,516 | 2.6% |
| CALL_PY_EXACT_ARGS | 16,760 | 0.2% |
| RETURN_VALUE | 12,440 | 0.1% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,556,540 | 100.0% |
| LOAD_CONST | 300 | 0.0% |
| CALL | 200 | 0.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,475,160 | 62.5% |
| STORE_FAST | 769,500 | 13.8% |
| LOAD_ATTR | 721,960 | 13.0% |
| PUSH_NULL | 445,160 | 8.0% |
| LOAD_GLOBAL_MODULE | 60,000 | 1.1% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 440 | 84.6% |
| LOAD_ATTR_INSTANCE_VALUE | 60 | 11.5% |
| COMPARE_OP | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 460 | 88.5% |
| POP_JUMP_IF_FALSE | 60 | 11.5% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 7,344,142 | 39.3% |
| CALL_LEN | 2,944,020 | 15.8% |
| LOAD_GLOBAL_MODULE | 1,792,320 | 9.6% |
| COPY | 1,790,160 | 9.6% |
| LOAD_ATTR_CLASS | 1,777,400 | 9.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 10,703,570 | 57.3% |
| POP_JUMP_IF_TRUE | 5,824,319 | 31.2% |
| COPY | 1,052,812 | 5.6% |
| RETURN_VALUE | 639,596 | 3.4% |
| EXTENDED_ARG | 302,920 | 1.6% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 15,472,516 | 71.4% |
| LOAD_FAST | 4,532,012 | 20.9% |
| RETURN_VALUE | 478,820 | 2.2% |
| LOAD_ATTR_INSTANCE_VALUE | 419,326 | 1.9% |
| LOAD_ATTR_MODULE | 316,800 | 1.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 13,452,832 | 62.1% |
| POP_JUMP_IF_FALSE | 5,628,420 | 26.0% |
| COPY | 1,547,764 | 7.1% |
| RETURN_VALUE | 614,514 | 2.8% |
| EXTENDED_ARG | 389,260 | 1.8% |


</details>

### FOR_ITER_GEN

<details>
<summary> Successors and predecessors for FOR_ITER_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD | 615,420 | 92.7% |
| GET_ITER | 48,380 | 7.3% |
| FOR_ITER | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 615,440 | 92.7% |
| POP_TOP | 48,380 | 7.3% |
| RESUME | 80 | 0.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 23,900,257 | 38.9% |
| GET_ITER | 22,327,527 | 36.3% |
| SWAP | 11,185,020 | 18.2% |
| LOAD_FAST | 2,579,740 | 4.2% |
| EXTENDED_ARG | 1,325,380 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 26,557,685 | 43.2% |
| LOAD_FAST | 13,557,373 | 22.0% |
| SWAP | 8,931,460 | 14.5% |
| RETURN_CONST | 7,250,396 | 11.8% |
| STORE_FAST_LOAD_FAST | 2,655,548 | 4.3% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 2,976,620 | 63.2% |
| ENTER_EXECUTOR | 1,224,539 | 26.0% |
| SWAP | 395,200 | 8.4% |
| EXTENDED_ARG | 106,920 | 2.3% |
| JUMP_BACKWARD | 6,980 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,425,839 | 30.3% |
| RETURN_CONST | 1,399,480 | 29.7% |
| LOAD_FAST | 1,101,940 | 23.4% |
| LOAD_GLOBAL_MODULE | 412,760 | 8.8% |
| STORE_FAST_LOAD_FAST | 167,600 | 3.6% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 9,469,933 | 62.7% |
| ENTER_EXECUTOR | 4,235,114 | 28.0% |
| SWAP | 1,325,520 | 8.8% |
| EXTENDED_ARG | 34,520 | 0.2% |
| FOR_ITER_LIST | 17,421 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,752,302 | 57.9% |
| STORE_FAST | 3,186,744 | 21.1% |
| SWAP | 1,315,800 | 8.7% |
| STORE_FAST_LOAD_FAST | 878,760 | 5.8% |
| LOAD_FAST_LOAD_FAST | 538,880 | 3.6% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 6,576,140 | 88.3% |
| LOAD_FAST | 772,000 | 10.4% |
| COPY | 52,720 | 0.7% |
| ENTER_EXECUTOR | 37,800 | 0.5% |
| LOAD_ATTR_CLASS | 3,240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 1,894,480 | 25.4% |
| COMPARE_OP_INT | 1,777,400 | 23.9% |
| LOAD_ATTR_METHOD_NO_DICT | 1,351,560 | 18.2% |
| CALL | 1,283,100 | 17.2% |
| LOAD_ATTR_MODULE | 772,000 | 10.4% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 61,938,168 | 80.5% |
| LOAD_FAST_LOAD_FAST | 6,277,701 | 8.2% |
| LOAD_ATTR_INSTANCE_VALUE | 2,973,960 | 3.9% |
| LOAD_GLOBAL_MODULE | 2,087,280 | 2.7% |
| LOAD_DEREF | 901,580 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 14,379,678 | 18.7% |
| LOAD_CONST | 13,812,300 | 17.9% |
| LOAD_ATTR_METHOD_NO_DICT | 7,074,890 | 9.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,466,220 | 8.4% |
| CONTAINS_OP | 3,905,799 | 5.1% |


</details>

### LOAD_ATTR_METHOD_LAZY_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_LAZY_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,400 | 99.8% |
| LOAD_ATTR | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,300 | 99.1% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 120 | 0.7% |
| CALL | 20 | 0.1% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 94,137,682 | 72.2% |
| LOAD_ATTR_SLOT | 13,083,796 | 10.0% |
| LOAD_ATTR_INSTANCE_VALUE | 7,074,890 | 5.4% |
| LOAD_GLOBAL_MODULE | 5,009,720 | 3.8% |
| ENTER_EXECUTOR | 3,998,811 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 57,853,862 | 44.4% |
| CALL_PY_EXACT_ARGS | 37,184,112 | 28.5% |
| LOAD_CONST | 12,268,736 | 9.4% |
| CALL_METHOD_DESCRIPTOR_FAST | 10,081,817 | 7.7% |
| LOAD_GLOBAL_MODULE | 8,979,769 | 6.9% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 46,059,646 | 81.7% |
| LOAD_ATTR_INSTANCE_VALUE | 6,466,220 | 11.5% |
| LOAD_DEREF | 1,261,300 | 2.2% |
| LOAD_ATTR_WITH_HINT | 678,200 | 1.2% |
| LOAD_FAST_LOAD_FAST | 640,480 | 1.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 39,478,231 | 70.0% |
| LOAD_FAST_LOAD_FAST | 7,865,420 | 13.9% |
| CALL_PY_EXACT_ARGS | 5,450,400 | 9.7% |
| LOAD_CONST | 1,350,840 | 2.4% |
| LOAD_DEREF | 1,062,980 | 1.9% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 8,803,331 | 66.7% |
| LOAD_ATTR_MODULE | 2,897,340 | 21.9% |
| LOAD_ATTR_CLASS | 772,000 | 5.8% |
| LOAD_FAST_LOAD_FAST | 617,400 | 4.7% |
| LOAD_FAST | 101,200 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 2,926,880 | 22.2% |
| LOAD_ATTR_MODULE | 2,897,340 | 21.9% |
| LOAD_FAST | 2,050,720 | 15.5% |
| COMPARE_OP | 1,253,300 | 9.5% |
| LOAD_GLOBAL_MODULE | 803,120 | 6.1% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 534,760 | 100.0% |
| LOAD_ATTR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 491,820 | 92.0% |
| LOAD_FAST | 21,600 | 4.0% |
| IS_OP | 21,420 | 4.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 344,560 | 64.6% |
| LOAD_FAST | 184,200 | 34.5% |
| LOAD_FAST_LOAD_FAST | 1,680 | 0.3% |
| BINARY_SUBSCR_DICT | 980 | 0.2% |
| ENTER_EXECUTOR | 900 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 345,600 | 64.8% |
| CALL_LEN | 68,920 | 12.9% |
| RETURN_VALUE | 47,840 | 9.0% |
| LOAD_FAST | 47,720 | 8.9% |
| POP_JUMP_IF_NONE | 18,520 | 3.5% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,534,203 | 54.7% |
| LOAD_ATTR_SLOT | 3,228,546 | 23.5% |
| ENTER_EXECUTOR | 2,583,496 | 18.8% |
| LOAD_ATTR_INSTANCE_VALUE | 241,480 | 1.8% |
| CALL | 46,680 | 0.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 12,867,487 | 93.5% |
| RETURN_VALUE | 531,952 | 3.9% |
| LOAD_FAST | 119,280 | 0.9% |
| STORE_FAST | 117,800 | 0.9% |
| LOAD_CONST | 52,260 | 0.4% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 217,327,781 | 88.1% |
| LOAD_ATTR_SLOT | 17,337,421 | 7.0% |
| LOAD_DEREF | 3,885,740 | 1.6% |
| LOAD_FAST_LOAD_FAST | 3,275,748 | 1.3% |
| STORE_FAST_LOAD_FAST | 1,489,920 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 29,775,212 | 12.1% |
| GET_ITER | 23,940,916 | 9.7% |
| STORE_FAST | 22,174,660 | 9.0% |
| RETURN_VALUE | 18,246,975 | 7.4% |
| LOAD_ATTR_SLOT | 17,337,421 | 7.0% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,741,200 | 57.2% |
| LOAD_FAST_LOAD_FAST | 3,171,700 | 20.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,105,920 | 20.3% |
| LOAD_ATTR_WITH_HINT | 249,500 | 1.6% |
| LOAD_ATTR | 9,540 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 4,799,420 | 31.4% |
| LOAD_ATTR_METHOD_NO_DICT | 1,811,720 | 11.9% |
| TO_BOOL_BOOL | 1,765,640 | 11.6% |
| COPY | 1,394,600 | 9.1% |
| LOAD_FAST | 1,196,140 | 7.8% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 84,035,264 | 31.0% |
| POP_JUMP_IF_FALSE | 65,430,109 | 24.1% |
| STORE_FAST | 35,845,511 | 13.2% |
| LOAD_FAST | 19,766,760 | 7.3% |
| POP_JUMP_IF_NOT_NONE | 18,197,520 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 187,798,718 | 69.3% |
| LOAD_DEREF | 46,031,900 | 17.0% |
| CALL_ISINSTANCE | 17,546,400 | 6.5% |
| CALL_BUILTIN_CLASS | 3,561,520 | 1.3% |
| LOAD_CONST | 3,140,760 | 1.2% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 133,064,751 | 44.3% |
| STORE_FAST | 29,108,358 | 9.7% |
| RESUME_CHECK | 26,429,680 | 8.8% |
| POP_JUMP_IF_FALSE | 23,041,420 | 7.7% |
| LOAD_GLOBAL_MODULE | 16,341,960 | 5.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 114,689,090 | 38.2% |
| LOAD_FAST | 57,269,389 | 19.1% |
| LOAD_FAST_LOAD_FAST | 22,881,620 | 7.6% |
| IS_OP | 20,791,560 | 6.9% |
| LOAD_GLOBAL_MODULE | 16,341,960 | 5.4% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 541,500 | 100.0% |
| LOAD_SUPER_ATTR | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 538,680 | 99.5% |
| STORE_FAST | 2,880 | 0.5% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 43,007,140 | 100.0% |
| LOAD_SUPER_ATTR | 2,400 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 35,810,960 | 83.3% |
| CALL_PY_WITH_DEFAULTS | 3,965,600 | 9.2% |
| CALL_PY_EXACT_ARGS | 1,630,880 | 3.8% |
| LOAD_FAST | 1,037,240 | 2.4% |
| LOAD_GLOBAL_MODULE | 344,600 | 0.8% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 187,249,916 | 54.3% |
| COPY_FREE_VARS | 46,507,260 | 13.5% |
| CACHE | 34,891,867 | 10.1% |
| CALL_KW | 21,713,260 | 6.3% |
| LOAD_ATTR_PROPERTY | 12,867,487 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 150,584,697 | 43.7% |
| LOAD_GLOBAL_BUILTIN | 84,035,264 | 24.4% |
| RETURN_CONST | 33,811,860 | 9.8% |
| LOAD_FAST_LOAD_FAST | 30,206,540 | 8.8% |
| LOAD_GLOBAL_MODULE | 26,429,680 | 7.7% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 181,520 | 79.1% |
| LOAD_CONST | 47,920 | 20.9% |
| SEND | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 181,520 | 79.1% |
| POP_TOP | 47,940 | 20.9% |
| RESUME | 40 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 22,102,080 | 56.7% |
| LOAD_FAST | 16,248,820 | 41.7% |
| SWAP | 397,040 | 1.0% |
| BINARY_SUBSCR | 224,720 | 0.6% |
| STORE_ATTR_INSTANCE_VALUE | 15,960 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 18,308,380 | 46.9% |
| RETURN_CONST | 6,846,760 | 17.6% |
| LOAD_FAST | 6,501,540 | 16.7% |
| LOAD_GLOBAL_BUILTIN | 2,566,180 | 6.6% |
| LOAD_GLOBAL_MODULE | 1,833,380 | 4.7% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 179,530,299 | 58.8% |
| LOAD_FAST_LOAD_FAST | 124,049,340 | 40.6% |
| STORE_ATTR_SLOT | 1,241,759 | 0.4% |
| LOAD_ATTR_SLOT | 391,500 | 0.1% |
| STORE_ATTR | 12,720 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 84,645,340 | 27.7% |
| LOAD_FAST_LOAD_FAST | 70,357,660 | 23.1% |
| RETURN_CONST | 60,343,400 | 19.8% |
| LOAD_FAST | 56,436,999 | 18.5% |
| LOAD_GLOBAL_BUILTIN | 15,842,020 | 5.2% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 471,280 | 57.3% |
| LOAD_FAST_LOAD_FAST | 349,080 | 42.5% |
| STORE_ATTR | 600 | 0.1% |
| SWAP | 360 | 0.0% |
| STORE_ATTR_WITH_HINT | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 256,100 | 31.2% |
| LOAD_GLOBAL_MODULE | 224,040 | 27.3% |
| RETURN_CONST | 172,260 | 21.0% |
| LOAD_FAST | 128,900 | 15.7% |
| LOAD_GLOBAL_BUILTIN | 39,320 | 4.8% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,808,518 | 76.0% |
| LOAD_ATTR_SLOT | 179,580 | 7.5% |
| LOAD_FAST_LOAD_FAST | 177,340 | 7.4% |
| SWAP | 166,360 | 7.0% |
| LOAD_ATTR_INSTANCE_VALUE | 23,560 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,248,660 | 52.4% |
| ENTER_EXECUTOR | 568,940 | 23.9% |
| LOAD_FAST | 452,918 | 19.0% |
| LOAD_GLOBAL_BUILTIN | 43,360 | 1.8% |
| LOAD_DEREF | 31,660 | 1.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 216,440 | 99.7% |
| LOAD_FAST | 640 | 0.3% |
| STORE_SUBSCR | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 215,720 | 99.3% |
| LOAD_FAST | 520 | 0.2% |
| JUMP_BACKWARD | 320 | 0.1% |
| RETURN_CONST | 320 | 0.1% |
| EXTENDED_ARG | 280 | 0.1% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,806,735 | 74.5% |
| LOAD_ATTR_SLOT | 2,776,420 | 19.1% |
| LOAD_ATTR_INSTANCE_VALUE | 276,080 | 1.9% |
| ENTER_EXECUTOR | 269,700 | 1.9% |
| COPY | 116,960 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 12,570,771 | 86.6% |
| POP_JUMP_IF_TRUE | 1,418,140 | 9.8% |
| EXTENDED_ARG | 487,160 | 3.4% |
| TO_BOOL_NONE | 18,024 | 0.1% |
| TO_BOOL_ALWAYS_TRUE | 16,063 | 0.1% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_ISINSTANCE | 133,033,603 | 65.1% |
| COPY | 19,175,948 | 9.4% |
| LOAD_FAST | 17,080,080 | 8.4% |
| RETURN_VALUE | 12,626,140 | 6.2% |
| LOAD_ATTR_SLOT | 5,798,780 | 2.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 138,134,325 | 67.6% |
| POP_JUMP_IF_TRUE | 50,313,766 | 24.6% |
| UNARY_NOT | 11,412,180 | 5.6% |
| EXTENDED_ARG | 4,527,340 | 2.2% |
| TO_BOOL_STR | 320 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 592,681 | 62.4% |
| LOAD_ATTR_INSTANCE_VALUE | 178,000 | 18.8% |
| RETURN_VALUE | 74,160 | 7.8% |
| LOAD_ATTR_SLOT | 69,440 | 7.3% |
| BINARY_OP | 28,400 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 677,241 | 71.4% |
| POP_JUMP_IF_TRUE | 201,280 | 21.2% |
| UNARY_NOT | 69,840 | 7.4% |
| TO_BOOL_STR | 640 | 0.1% |
| TO_BOOL_BOOL | 160 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,337,420 | 75.9% |
| LOAD_ATTR_SLOT | 3,252,920 | 14.2% |
| LOAD_ATTR_INSTANCE_VALUE | 1,297,340 | 5.7% |
| COPY | 443,760 | 1.9% |
| BINARY_SUBSCR_LIST_INT | 196,560 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 17,346,660 | 75.9% |
| POP_JUMP_IF_FALSE | 3,838,140 | 16.8% |
| UNARY_NOT | 1,262,660 | 5.5% |
| EXTENDED_ARG | 395,360 | 1.7% |
| TO_BOOL | 2,140 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,192,705 | 63.5% |
| LOAD_ATTR_SLOT | 4,014,660 | 25.0% |
| COPY | 898,620 | 5.6% |
| LOAD_ATTR_INSTANCE_VALUE | 291,800 | 1.8% |
| LOAD_ATTR_MODULE | 259,440 | 1.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 11,557,849 | 72.0% |
| POP_JUMP_IF_TRUE | 4,123,080 | 25.7% |
| EXTENDED_ARG | 355,400 | 2.2% |
| TO_BOOL_ALWAYS_TRUE | 18,393 | 0.1% |
| TO_BOOL | 2,980 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,329,720 | 72.6% |
| COPY | 752,600 | 16.4% |
| LOAD_ATTR_SLOT | 219,000 | 4.8% |
| LOAD_ATTR_INSTANCE_VALUE | 174,560 | 3.8% |
| STORE_FAST_LOAD_FAST | 94,340 | 2.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,672,720 | 58.3% |
| POP_JUMP_IF_TRUE | 1,726,800 | 37.6% |
| UNARY_NOT | 184,780 | 4.0% |
| TO_BOOL_NONE | 2,440 | 0.1% |
| TO_BOOL_INT | 780 | 0.0% |


</details>

### UNPACK_SEQUENCE_LIST

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_KW | 7,090,880 | 98.2% |
| RETURN_VALUE | 116,360 | 1.6% |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 8,160 | 0.1% |
| LOAD_FAST | 7,920 | 0.1% |
| LOAD_ATTR_SLOT | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 7,221,420 | 100.0% |
| STORE_FAST | 2,860 | 0.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 388,440 | 40.6% |
| YIELD_VALUE | 188,040 | 19.6% |
| STORE_FAST | 146,440 | 15.3% |
| FOR_ITER | 115,300 | 12.0% |
| LOAD_ATTR_INSTANCE_VALUE | 46,520 | 4.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 793,340 | 82.8% |
| LOAD_FAST | 93,420 | 9.8% |
| STORE_FAST | 70,780 | 7.4% |
| STORE_DEREF | 40 | 0.0% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER | 2,891,675 | 66.8% |
| RETURN_VALUE | 736,380 | 17.0% |
| FOR_ITER_LIST | 253,920 | 5.9% |
| RETURN_CONST | 145,080 | 3.4% |
| STORE_FAST | 128,460 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 3,885,275 | 89.7% |
| STORE_FAST | 429,180 | 9.9% |
| UNPACK_SEQUENCE_TWO_TUPLE | 14,560 | 0.3% |
| UNPACK_SEQUENCE | 20 | 0.0% |


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
|     deferred | 2,370,548 | 21.1% |
|          hit | 8,848,117 | 78.7% |
|         miss | 39,640 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,840 | 32.8% |
| Failure | 11,940 | 67.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| add other | 5,560 | 46.6% |
| multiply different types | 2,900 | 24.3% |
| or | 1,040 | 8.7% |
| remainder | 860 | 7.2% |
| subtract other | 760 | 6.4% |
| and int | 340 | 2.8% |
| and different types | 160 | 1.3% |
| subtract different types | 140 | 1.2% |
| true divide different types | 120 | 1.0% |
| and other | 40 | 0.3% |
| add different types | 20 | 0.2% |


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
|     deferred | 20,139,635 | 22.3% |
|          hit | 70,317,451 | 77.7% |
|         miss | 1,260 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 12,320 | 36.2% |
| Failure | 21,718 | 63.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| out of range | 13,218 | 60.9% |
| other | 4,660 | 21.5% |
| code complex parameters | 3,580 | 16.5% |
| buffer int | 200 | 0.9% |
| tuple slice | 60 | 0.3% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 63,706,260 | 11.6% |
|          hit | 486,594,031 | 88.3% |
|         miss | 30,058,115 | 5.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 679,615 | 88.0% |
| Failure | 92,260 | 12.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| no dict | 31,600 | 34.3% |
| code complex parameters | 23,160 | 25.1% |
| meth descr varargs | 11,000 | 11.9% |
| class no vectorcall | 7,700 | 8.3% |
| cfunc noargs | 4,500 | 4.9% |
| class mutable | 4,380 | 4.7% |
| cfunc varargs keywords | 2,160 | 2.3% |
| meth descr varargs keywords | 1,300 | 1.4% |
| wrong number arguments | 1,220 | 1.3% |
| init not simple | 1,140 | 1.2% |
| meth descr method fastcall keywords | 1,020 | 1.1% |
| bound method | 900 | 1.0% |
| other | 800 | 0.9% |
| init not python | 480 | 0.5% |
| cfunc varargs | 440 | 0.5% |
| cmethod | 360 | 0.4% |
| operator wrapper | 100 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 21,444,584 | 34.9% |
|          hit | 39,895,899 | 65.0% |
|         miss | 465,561 | 0.8% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 21,793 | 29.9% |
| Failure | 51,145 | 70.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| big int | 25,565 | 50.0% |
| baseobject | 10,580 | 20.7% |
| other | 4,840 | 9.5% |
| different types | 3,600 | 7.0% |
| tuple | 2,180 | 4.3% |
| bool | 2,080 | 4.1% |
| list | 1,780 | 3.5% |
| set | 280 | 0.5% |
| string | 240 | 0.5% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 11,219,106 | 12.3% |
|          hit | 80,025,842 | 87.6% |
|         miss | 1,957,326 | 2.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 49,202 | 64.3% |
| Failure | 27,294 | 35.7% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| enumerate | 6,740 | 24.7% |
| zip | 5,580 | 20.4% |
| set | 5,354 | 19.6% |
| dict items | 3,500 | 12.8% |
| reversed list | 3,000 | 11.0% |
| dict keys | 1,660 | 6.1% |
| dict values | 860 | 3.2% |
| itertools | 360 | 1.3% |
| map | 160 | 0.6% |
| other | 80 | 0.3% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 98,834,178 | 16.0% |
|        deopt | 780 | 0.0% |
|          hit | 516,749,200 | 83.8% |
|         miss | 44,272,782 | 7.2% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 989,527 | 86.2% |
| Failure | 158,980 | 13.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 75,340 | 47.4% |
| not managed dict | 32,140 | 20.2% |
| shadowed | 21,980 | 13.8% |
| non overriding descriptor | 6,180 | 3.9% |
| class method obj | 6,140 | 3.9% |
| metaclass attribute | 6,000 | 3.8% |
| method | 4,660 | 2.9% |
| class attr simple | 3,520 | 2.2% |
| module attr not found | 2,520 | 1.6% |
| builtin class method | 300 | 0.2% |
| class attr descriptor | 120 | 0.1% |
| mutable class | 80 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 127,880 | 0.0% |
|        deopt | 920 | 0.0% |
|          hit | 571,604,622 | 100.0% |
|         miss | 6,660 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 121,620 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 2,360 | 0.0% |
|          hit | 43,551,100 | 100.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 2,460 | 100.0% |
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
|     deferred | 60 | 0.0% |
|          hit | 229,500 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 60 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 71,268,008 | 20.3% |
|          hit | 278,328,111 | 79.3% |
|         miss | 66,726,347 | 19.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,281,139 | 98.4% |
| Failure | 20,360 | 1.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 14,320 | 70.3% |
| not in dict | 4,720 | 23.2% |
| not in keys | 720 | 3.5% |
| overridden | 600 | 2.9% |


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
|     deferred | 1,884,980 | 42.0% |
|          hit | 2,598,138 | 57.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 1,500 | 45.7% |
| Failure | 1,780 | 54.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| dict subclass no override | 1,200 | 67.4% |
| out of range | 580 | 32.6% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,707,995 | 5.0% |
|          hit | 259,693,117 | 94.9% |
|         miss | 3,652,395 | 1.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 128,100 | 78.9% |
| Failure | 34,340 | 21.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| number | 16,140 | 47.0% |
| tuple | 10,120 | 29.5% |
| dict | 3,820 | 11.1% |
| set | 1,780 | 5.2% |
| other | 1,260 | 3.7% |
| mapping | 1,220 | 3.6% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 68,779 | 0.5% |
|          hit | 12,510,895 | 99.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 5,380 | 88.2% |
| Failure | 720 | 11.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| sequence | 540 | 75.0% |
| iterator | 180 | 25.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 3,532,236,308 | 50.4% |
| Not specialized | 628,019,597 | 9.0% |
| Specialized hits | 2,704,292,104 | 38.6% |
| Specialized misses | 147,180,106 | 2.1% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 98,834,178 | 32.4% |
| STORE_ATTR | 71,268,008 | 23.4% |
| CALL | 63,706,260 | 20.9% |
| COMPARE_OP | 21,444,584 | 7.0% |
| BINARY_SUBSCR | 20,139,635 | 6.6% |
| TO_BOOL | 13,707,995 | 4.5% |
| FOR_ITER | 11,219,106 | 3.7% |
| BINARY_OP | 2,370,548 | 0.8% |
| STORE_SUBSCR | 1,884,980 | 0.6% |
| LOAD_GLOBAL | 127,880 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 65,833,867 | 44.7% |
| LOAD_ATTR_METHOD_NO_DICT | 28,563,702 | 19.4% |
| CALL_PY_EXACT_ARGS | 22,231,115 | 15.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 7,210,941 | 4.9% |
| LOAD_ATTR_SLOT | 4,289,361 | 2.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 4,014,960 | 2.7% |
| LOAD_ATTR_INSTANCE_VALUE | 2,811,220 | 1.9% |
| CALL_METHOD_DESCRIPTOR_FAST | 2,762,380 | 1.9% |
| TO_BOOL_ALWAYS_TRUE | 1,913,014 | 1.3% |
| TO_BOOL_NONE | 1,340,501 | 0.9% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 60,510,107 | 17.5% |
| Calls to Python functions inlined | 284,930,263 | 82.5% |
| Calls via PyEval_EvalFrame (total) | 60,510,107 | 17.5% |
| Calls via PyEval_EvalFrame (vector) | 53,289,627 | 15.4% |
| Calls via PyEval_EvalFrame (generator) | 7,220,480 | 2.1% |
| Calls via PyEval_EvalFrame (legacy) | 100 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 53,289,487 | 15.4% |
| Calls via PyEval_EvalFrame (build class) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 6,954,190 | 2.0% |
| Calls via PyEval_EvalFrame (function ex) | 1,237,660 | 0.4% |
| Calls via PyEval_EvalFrame (api) | 11,829,737 | 3.4% |
| Calls via PyEval_EvalFrame (method) | 100 | 0.0% |
| Frame objects created | 2,373,920 | 0.7% |
| Frames pushed | 243,612,615 | 70.5% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 153,543,603 | 28.5% |
| Frees to freelist | 153,588,915 |  |
| Allocations | 384,721,466 | 71.5% |
| Allocations to 512 bytes | 384,192,776 | 71.4% |
| Allocations to 4 kbytes | 369,287 | 0.1% |
| Allocations over 4 kbytes | 159,403 | 0.0% |
| Frees | 379,279,598 |  |
| New values | 4,435,060 |  |
| Interpreter increfs | 3,657,088,306 | 74.1% |
| Interpreter decrefs | 4,027,290,455 | 75.1% |
| Increfs | 1,278,311,442 | 25.9% |
| Decrefs | 1,332,829,893 | 24.9% |
| Materialize dict (on request) | 340 | 0.0% |
| Materialize dict (new key) | 1,160 | 0.0% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 220 | 0.0% |
| Method cache hits | 210,450,974 |  |
| Method cache misses | 4,600,779 |  |
| Method cache collisions | 5,323,894 |  |
| Method cache dunder hits | 178,291,021 |  |
| Method cache dunder misses | 747,987 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 180 | 216,040 | 430,867,640 |
| 1 | 20 | 10,536,020 | 223,597,280 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 16,300 |  |
| Traces created | 15,140 | 92.9% |
| Trace stack overflow | 80 | 0.5% |
| Trace stack underflow | 80 | 0.5% |
| Trace too long | 120 | 0.7% |
| Trace too short | 1,160 | 7.1% |
| Inner loop found | 627 | 3.8% |
| Recursive call | 380 | 2.3% |
| Low confidence | 477 | 2.9% |
| Traces executed | 58,237,672 |  |
| Uops executed | 871,504,958 | 14.96 |

### Trace length histogram

<details>
<summary> trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 0 | 0.0% |
| <= 8 | 0 | 0.0% |
| <= 16 | 140 | 0.9% |
| <= 32 | 4,844 | 32.0% |
| <= 64 | 4,612 | 30.5% |
| <= 128 | 2,871 | 19.0% |
| <= 256 | 2,038 | 13.5% |
| <= 512 | 635 | 4.2% |


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 0 | 0.0% |
| <= 4 | 20 | 0.1% |
| <= 8 | 520 | 3.4% |
| <= 16 | 3,984 | 26.3% |
| <= 32 | 4,695 | 31.0% |
| <= 64 | 2,944 | 19.4% |
| <= 128 | 2,142 | 14.1% |
| <= 256 | 692 | 4.6% |
| <= 512 | 143 | 0.9% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 1,130,677 | 1.9% |
| <= 2 | 28,026,914 | 48.1% |
| <= 4 | 954,299 | 1.6% |
| <= 8 | 7,506,816 | 12.9% |
| <= 16 | 6,164,973 | 10.6% |
| <= 32 | 7,559,176 | 13.0% |
| <= 64 | 5,666,133 | 9.7% |
| <= 128 | 840,769 | 1.4% |
| <= 256 | 199,154 | 0.3% |
| <= 512 | 150,876 | 0.3% |
| <= 1,024 | 17,205 | 0.0% |
| <= 2,048 | 4,540 | 0.0% |
| <= 4,096 | 7,820 | 0.0% |
| <= 8,192 | 8,020 | 0.0% |
| <= 16,384 | 300 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 105,122,336 | 12.1% | 12.1% |  |
| _SET_IP | 90,206,098 | 10.4% | 22.4% |  |
| _CHECK_VALIDITY | 71,295,553 | 8.2% | 30.6% |  |
| STORE_FAST | 49,490,260 | 5.7% | 36.3% |  |
| _ITER_CHECK_LIST | 48,464,145 | 5.6% | 41.8% | 0.6% |
| _GUARD_NOT_EXHAUSTED_LIST | 48,162,192 | 5.5% | 47.4% | 49.8% |
| _GUARD_GLOBALS_VERSION | 37,283,939 | 4.3% | 51.6% | 0.8% |
| _GUARD_TYPE_VERSION | 33,234,843 | 3.8% | 55.5% | 17.0% |
| _ITER_NEXT_LIST | 24,200,685 | 2.8% | 58.2% |  |
| _LOAD_GLOBAL_MODULE | 20,388,250 | 2.3% | 60.6% |  |
| _GUARD_BUILTINS_VERSION | 16,594,069 | 1.9% | 62.5% |  |
| _LOAD_GLOBAL_BUILTINS | 16,594,069 | 1.9% | 64.4% |  |
| _LOAD_CONST_INLINE_BORROW | 14,695,358 | 1.7% | 66.1% |  |
| _GUARD_IS_TRUE_POP | 12,706,854 | 1.5% | 67.5% | 10.5% |
| _GUARD_IS_FALSE_POP | 12,691,439 | 1.5% | 69.0% | 11.0% |
| _EXIT_TRACE | 12,669,816 | 1.5% | 70.4% | 100.0% |
| _JUMP_TO_TOP | 11,285,624 | 1.3% | 71.7% |  |
| _LOAD_ATTR_SLOT | 10,928,683 | 1.3% | 73.0% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 10,669,272 | 1.2% | 74.2% | 8.5% |
| TO_BOOL_BOOL | 10,500,789 | 1.2% | 75.4% |  |
| CALL_ISINSTANCE | 9,928,769 | 1.1% | 76.5% |  |
| _CHECK_STACK_SPACE | 9,759,572 | 1.1% | 77.7% | 0.0% |
| _INIT_CALL_PY_EXACT_ARGS | 9,758,772 | 1.1% | 78.8% |  |
| _PUSH_FRAME | 9,758,772 | 1.1% | 79.9% |  |
| _SAVE_RETURN_OFFSET | 9,758,772 | 1.1% | 81.0% |  |
| _FOR_ITER_TIER_TWO | 9,644,508 | 1.1% | 82.1% | 42.2% |
| _LOAD_ATTR_METHOD_NO_DICT | 7,998,972 | 0.9% | 83.1% |  |
| _LOAD_CONST_INLINE | 7,253,280 | 0.8% | 83.9% |  |
| BINARY_SUBSCR_LIST_INT | 7,095,000 | 0.8% | 84.7% |  |
| _ITER_CHECK_TUPLE | 7,080,160 | 0.8% | 85.5% | 11.8% |
| RESUME_CHECK | 6,689,161 | 0.8% | 86.3% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 6,246,816 | 0.7% | 87.0% | 59.3% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 6,181,279 | 0.7% | 87.7% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 6,181,279 | 0.7% | 88.4% |  |
| COMPARE_OP_STR | 6,094,980 | 0.7% | 89.1% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 5,553,325 | 0.6% | 89.7% |  |
| _GUARD_IS_NOT_NONE_POP | 4,876,300 | 0.6% | 90.3% | 2.2% |
| BINARY_SUBSCR_TUPLE_INT | 4,809,300 | 0.6% | 90.9% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 4,046,099 | 0.5% | 91.3% | 23.4% |
| CONTAINS_OP | 4,040,824 | 0.5% | 91.8% |  |
| _LOAD_ATTR | 3,072,581 | 0.4% | 92.1% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 3,027,400 | 0.3% | 92.5% | 42.0% |
| _ITER_CHECK_RANGE | 3,027,400 | 0.3% | 92.8% |  |
| POP_TOP | 3,017,064 | 0.3% | 93.2% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 2,926,020 | 0.3% | 93.5% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 2,926,020 | 0.3% | 93.9% |  |
| COMPARE_OP_INT | 2,759,673 | 0.3% | 94.2% |  |
| _GUARD_IS_NONE_POP | 2,556,280 | 0.3% | 94.5% | 8.0% |
| _ITER_NEXT_TUPLE | 2,542,506 | 0.3% | 94.8% |  |
| PUSH_NULL | 2,256,641 | 0.3% | 95.0% |  |
| LIST_APPEND | 1,975,924 | 0.2% | 95.2% |  |
| _GUARD_BOTH_UNICODE | 1,947,060 | 0.2% | 95.5% |  |
| _BINARY_OP_ADD_UNICODE | 1,947,060 | 0.2% | 95.7% |  |
| _GUARD_KEYS_VERSION | 1,874,749 | 0.2% | 95.9% | 6.9% |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 1,874,749 | 0.2% | 96.1% |  |
| _CHECK_ATTR_MODULE | 1,860,589 | 0.2% | 96.3% |  |
| _LOAD_ATTR_MODULE | 1,860,589 | 0.2% | 96.5% |  |
| BINARY_SUBSCR_DICT | 1,791,448 | 0.2% | 96.8% |  |
| TO_BOOL_NONE | 1,774,280 | 0.2% | 97.0% | 4.8% |
| _ITER_NEXT_RANGE | 1,754,901 | 0.2% | 97.2% |  |
| _GUARD_NOS_INT | 1,739,586 | 0.2% | 97.4% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 1,700,229 | 0.2% | 97.5% |  |
| _BINARY_OP_SUBTRACT_INT | 1,628,031 | 0.2% | 97.7% |  |
| LOAD_DEREF | 1,504,193 | 0.2% | 97.9% |  |
| SET_ADD | 1,357,910 | 0.2% | 98.1% |  |
| CALL_BUILTIN_FAST | 1,342,781 | 0.2% | 98.2% |  |
| TO_BOOL_STR | 1,182,700 | 0.1% | 98.4% |  |
| CALL_STR_1 | 1,133,040 | 0.1% | 98.5% |  |
| CALL_BUILTIN_O | 1,132,380 | 0.1% | 98.6% |  |
| BUILD_LIST | 1,023,805 | 0.1% | 98.7% |  |
| _POP_FRAME | 1,008,557 | 0.1% | 98.8% |  |
| GET_ITER | 978,421 | 0.1% | 99.0% |  |
| MAP_ADD | 636,772 | 0.1% | 99.0% |  |
| FORMAT_SIMPLE | 537,820 | 0.1% | 99.1% |  |
| BUILD_TUPLE | 490,419 | 0.1% | 99.2% |  |
| _COMPARE_OP | 479,400 | 0.1% | 99.2% |  |
| BUILD_STRING | 476,660 | 0.1% | 99.3% |  |
| CALL_LEN | 377,960 | 0.0% | 99.3% |  |
| _STORE_ATTR_SLOT | 375,140 | 0.0% | 99.3% |  |
| TO_BOOL_LIST | 370,340 | 0.0% | 99.4% |  |
| _BINARY_OP_ADD_INT | 369,912 | 0.0% | 99.4% |  |
| TO_BOOL_ALWAYS_TRUE | 334,780 | 0.0% | 99.5% | 73.9% |
| SWAP | 286,240 | 0.0% | 99.5% |  |
| _BINARY_SUBSCR | 277,085 | 0.0% | 99.5% |  |
| COPY | 248,401 | 0.0% | 99.6% |  |
| STORE_SUBSCR_DICT | 247,882 | 0.0% | 99.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 246,780 | 0.0% | 99.6% |  |
| IS_OP | 241,580 | 0.0% | 99.6% |  |
| BINARY_SLICE | 241,200 | 0.0% | 99.7% |  |
| CALL_TYPE_1 | 240,320 | 0.0% | 99.7% |  |
| _LOAD_ATTR_WITH_HINT | 209,980 | 0.0% | 99.7% | 0.0% |
| _CHECK_ATTR_WITH_HINT | 209,980 | 0.0% | 99.8% |  |
| MAKE_FUNCTION | 177,300 | 0.0% | 99.8% |  |
| CALL_METHOD_DESCRIPTOR_O | 177,141 | 0.0% | 99.8% |  |
| BINARY_SUBSCR_STR_INT | 176,121 | 0.0% | 99.8% | 0.1% |
| CALL_BUILTIN_CLASS | 167,740 | 0.0% | 99.8% |  |
| UNARY_NOT | 166,280 | 0.0% | 99.9% |  |
| _GUARD_BOTH_INT | 159,211 | 0.0% | 99.9% | 17.5% |
| BUILD_MAP | 158,041 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_TUPLE | 144,120 | 0.0% | 99.9% |  |
| LOAD_FAST_AND_CLEAR | 125,020 | 0.0% | 99.9% |  |
| _BINARY_OP | 110,772 | 0.0% | 99.9% |  |
| UNPACK_SEQUENCE_LIST | 89,040 | 0.0% | 99.9% |  |
| TO_BOOL_INT | 72,779 | 0.0% | 99.9% |  |
| SET_FUNCTION_ATTRIBUTE | 70,020 | 0.0% | 100.0% |  |
| COPY_FREE_VARS | 46,400 | 0.0% | 100.0% |  |
| MAKE_CELL | 44,500 | 0.0% | 100.0% |  |
| _LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 44,420 | 0.0% | 100.0% |  |
| _CHECK_ATTR_CLASS | 43,140 | 0.0% | 100.0% | 87.6% |
| LOAD_SUPER_ATTR_METHOD | 41,440 | 0.0% | 100.0% |  |
| _TO_BOOL | 39,360 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 28,600 | 0.0% | 100.0% | 78.8% |
| STORE_DEREF | 18,720 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 15,980 | 0.0% | 100.0% |  |
| DELETE_SUBSCR | 8,640 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 8,400 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 8,400 | 0.0% | 100.0% |  |
| _LOAD_ATTR_CLASS | 5,340 | 0.0% | 100.0% |  |
| BUILD_SET | 3,360 | 0.0% | 100.0% |  |
| _UNPACK_SEQUENCE | 3,181 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 2,560 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 2,400 | 0.0% | 100.0% |  |
| _STORE_SUBSCR | 1,180 | 0.0% | 100.0% |  |
| FORMAT_WITH_SPEC | 680 | 0.0% | 100.0% |  |
| _STORE_ATTR | 520 | 0.0% | 100.0% |  |
| UNARY_INVERT | 260 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 220 | 0.0% | 100.0% |  |
| _GUARD_TOS_INT | 140 | 0.0% | 100.0% |  |
| UNPACK_EX | 100 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| CALL | 1,777 |
| FOR_ITER_GEN | 1,160 |
| CALL_LIST_APPEND | 1,140 |
| CALL_KW | 940 |
| CALL_PY_WITH_DEFAULTS | 800 |
| LOAD_ATTR_PROPERTY | 780 |
| YIELD_VALUE | 760 |
| CALL_ALLOC_AND_ENTER_INIT | 363 |
| IMPORT_NAME | 20 |
| BINARY_SUBSCR_GETITEM | 20 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 40 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 40 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-01
