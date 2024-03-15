
# Pystats results

- benchmark: asyncio_tcp_ssl
- fork: mdboom
- ref: pystats-test2
- commit hash: 28e6201
- commit date: 2024-02-07T11:00:47-05:00

## Execution counts

<details>
<summary> execution counts for all instructions </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| LOAD_FAST | 104,827,401 | 22.2% | 22.2% |  |
| POP_JUMP_IF_FALSE | 26,967,020 | 5.7% | 27.9% |  |
| STORE_FAST | 26,209,190 | 5.6% | 33.5% |  |
| LOAD_ATTR_INSTANCE_VALUE | 23,185,888 | 4.9% | 38.4% |  |
| RESUME_CHECK | 21,542,705 | 4.6% | 43.0% |  |
| TO_BOOL_BOOL | 19,287,325 | 4.1% | 47.1% |  |
| LOAD_ATTR_METHOD_NO_DICT | 14,408,368 | 3.1% | 50.1% |  |
| LOAD_CONST | 14,240,484 | 3.0% | 53.1% |  |
| POP_TOP | 13,798,985 | 2.9% | 56.0% |  |
| POP_JUMP_IF_TRUE | 11,507,837 | 2.4% | 58.5% |  |
| CALL_PY_EXACT_ARGS | 11,131,868 | 2.4% | 60.8% | 0.0% |
| LOAD_ATTR | 10,931,510 | 2.3% | 63.2% |  |
| RETURN_VALUE | 10,579,402 | 2.2% | 65.4% |  |
| LOAD_ATTR_WITH_HINT | 10,468,883 | 2.2% | 67.6% |  |
| RETURN_CONST | 10,058,258 | 2.1% | 69.8% |  |
| CALL | 8,850,312 | 1.9% | 71.6% |  |
| ENTER_EXECUTOR | 7,535,683 | 1.6% | 73.2% |  |
| TO_BOOL | 7,521,607 | 1.6% | 74.8% |  |
| LOAD_FAST_LOAD_FAST | 7,439,961 | 1.6% | 76.4% |  |
| POP_JUMP_IF_NONE | 7,405,028 | 1.6% | 78.0% |  |
| LOAD_ATTR_METHOD_WITH_VALUES | 6,869,478 | 1.5% | 79.4% | 0.0% |
| LOAD_GLOBAL_MODULE | 6,434,074 | 1.4% | 80.8% | 0.0% |
| CALL_PY_WITH_DEFAULTS | 5,451,602 | 1.2% | 81.9% |  |
| LOAD_FAST_CHECK | 5,120,320 | 1.1% | 83.0% |  |
| CALL_LIST_APPEND | 4,846,137 | 1.0% | 84.1% |  |
| STORE_ATTR_SLOT | 4,664,637 | 1.0% | 85.0% | 0.1% |
| COMPARE_OP_INT | 4,662,072 | 1.0% | 86.0% | 0.0% |
| LOAD_GLOBAL_BUILTIN | 4,170,371 | 0.9% | 86.9% | 0.0% |
| LOAD_ATTR_SLOT | 4,133,967 | 0.9% | 87.8% | 0.1% |
| NOP | 4,005,274 | 0.8% | 88.6% |  |
| TO_BOOL_INT | 3,099,165 | 0.7% | 89.3% |  |
| CALL_LEN | 2,961,267 | 0.6% | 89.9% |  |
| LOAD_ATTR_MODULE | 2,397,546 | 0.5% | 90.4% | 0.0% |
| INTERPRETER_EXIT | 2,345,305 | 0.5% | 90.9% |  |
| BINARY_OP | 2,124,983 | 0.5% | 91.4% |  |
| CALL_METHOD_DESCRIPTOR_O | 2,051,703 | 0.4% | 91.8% | 0.0% |
| PUSH_NULL | 2,045,068 | 0.4% | 92.2% |  |
| LOAD_DEREF | 1,652,105 | 0.4% | 92.6% |  |
| STORE_ATTR_INSTANCE_VALUE | 1,638,963 | 0.3% | 92.9% |  |
| SEND_GEN | 1,637,725 | 0.3% | 93.3% |  |
| JUMP_BACKWARD_NO_INTERRUPT | 1,629,265 | 0.3% | 93.6% |  |
| POP_JUMP_IF_NOT_NONE | 1,367,544 | 0.3% | 93.9% |  |
| BUILD_TUPLE | 1,349,922 | 0.3% | 94.2% |  |
| JUMP_FORWARD | 1,321,985 | 0.3% | 94.5% |  |
| YIELD_VALUE | 1,308,564 | 0.3% | 94.8% |  |
| TO_BOOL_NONE | 1,305,782 | 0.3% | 95.0% | 0.0% |
| FOR_ITER_LIST | 1,287,944 | 0.3% | 95.3% |  |
| COPY | 1,022,282 | 0.2% | 95.5% |  |
| CALL_FUNCTION_EX | 1,019,061 | 0.2% | 95.8% |  |
| COMPARE_OP | 989,063 | 0.2% | 96.0% |  |
| END_SEND | 987,823 | 0.2% | 96.2% |  |
| GET_AWAITABLE | 987,823 | 0.2% | 96.4% |  |
| GET_ITER | 976,643 | 0.2% | 96.6% |  |
| STORE_FAST_STORE_FAST | 973,624 | 0.2% | 96.8% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 973,064 | 0.2% | 97.0% |  |
| BUILD_LIST | 968,104 | 0.2% | 97.2% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 700,340 | 0.1% | 97.4% | 0.2% |
| STORE_ATTR_WITH_HINT | 691,080 | 0.1% | 97.5% |  |
| BINARY_SLICE | 688,601 | 0.1% | 97.6% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 661,083 | 0.1% | 97.8% |  |
| BINARY_OP_ADD_INT | 659,762 | 0.1% | 97.9% |  |
| SEND | 659,602 | 0.1% | 98.1% |  |
| RETURN_GENERATOR | 659,322 | 0.1% | 98.2% |  |
| TO_BOOL_LIST | 645,542 | 0.1% | 98.3% |  |
| FOR_ITER_RANGE | 644,802 | 0.1% | 98.5% |  |
| CONTAINS_OP | 644,561 | 0.1% | 98.6% |  |
| CALL_BUILTIN_CLASS | 384,721 | 0.1% | 98.7% |  |
| COPY_FREE_VARS | 349,983 | 0.1% | 98.8% |  |
| SWAP | 342,862 | 0.1% | 98.8% |  |
| CALL_KW | 341,202 | 0.1% | 98.9% |  |
| CALL_BOUND_METHOD_EXACT_ARGS | 329,422 | 0.1% | 99.0% | 0.1% |
| DELETE_SUBSCR | 328,721 | 0.1% | 99.1% |  |
| CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS | 323,281 | 0.1% | 99.1% | 0.0% |
| LIST_EXTEND | 322,841 | 0.1% | 99.2% |  |
| CALL_INTRINSIC_1 | 322,781 | 0.1% | 99.3% |  |
| BINARY_OP_ADD_FLOAT | 322,141 | 0.1% | 99.3% |  |
| CHECK_EXC_MATCH | 321,941 | 0.1% | 99.4% |  |
| POP_EXCEPT | 321,941 | 0.1% | 99.5% |  |
| PUSH_EXC_INFO | 321,941 | 0.1% | 99.5% |  |
| MAKE_CELL | 321,920 | 0.1% | 99.6% |  |
| LOAD_ATTR_PROPERTY | 321,821 | 0.1% | 99.7% |  |
| MAKE_FUNCTION | 321,780 | 0.1% | 99.7% |  |
| SET_FUNCTION_ATTRIBUTE | 321,140 | 0.1% | 99.8% |  |
| BINARY_OP_MULTIPLY_INT | 320,961 | 0.1% | 99.9% |  |
| BUILD_SLICE | 320,721 | 0.1% | 99.9% |  |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 54,119 | 0.0% | 100.0% | 0.2% |
| CALL_ISINSTANCE | 28,882 | 0.0% | 100.0% |  |
| EXTENDED_ARG | 16,740 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_INT | 16,540 | 0.0% | 100.0% |  |
| LOAD_GLOBAL | 13,980 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_LIST_INT | 13,198 | 0.0% | 100.0% |  |
| MAP_ADD | 12,920 | 0.0% | 100.0% |  |
| STORE_ATTR | 12,580 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 9,821 | 0.0% | 100.0% |  |
| FOR_ITER | 9,820 | 0.0% | 100.0% |  |
| FOR_ITER_TUPLE | 9,680 | 0.0% | 100.0% |  |
| STORE_SUBSCR_DICT | 9,381 | 0.0% | 100.0% |  |
| BINARY_SUBSCR | 8,680 | 0.0% | 100.0% |  |
| COMPARE_OP_FLOAT | 6,539 | 0.0% | 100.0% |  |
| RESUME | 5,620 | 0.0% | 100.0% |  |
| JUMP_BACKWARD | 4,919 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_METHOD | 3,520 | 0.0% | 100.0% |  |
| IS_OP | 2,280 | 0.0% | 100.0% |  |
| BUILD_MAP | 2,180 | 0.0% | 100.0% |  |
| CALL_BUILTIN_FAST | 1,780 | 0.0% | 100.0% | 1.1% |
| TO_BOOL_STR | 1,200 | 0.0% | 100.0% | 5.0% |
| STORE_NAME | 1,160 | 0.0% | 100.0% |  |
| CALL_BUILTIN_O | 1,140 | 0.0% | 100.0% | 5.3% |
| CALL_TYPE_1 | 1,040 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR | 1,020 | 0.0% | 100.0% |  |
| COMPARE_OP_STR | 980 | 0.0% | 100.0% | 2.0% |
| LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES | 880 | 0.0% | 100.0% | 13.6% |
| UNARY_INVERT | 880 | 0.0% | 100.0% |  |
| STORE_DEREF | 880 | 0.0% | 100.0% |  |
| STORE_SUBSCR | 860 | 0.0% | 100.0% |  |
| LOAD_SUPER_ATTR_ATTR | 820 | 0.0% | 100.0% |  |
| DICT_UPDATE | 760 | 0.0% | 100.0% |  |
| LOAD_NAME | 760 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE | 760 | 0.0% | 100.0% |  |
| BINARY_OP_ADD_UNICODE | 700 | 0.0% | 100.0% |  |
| LIST_APPEND | 680 | 0.0% | 100.0% |  |
| LOAD_FAST_AND_CLEAR | 680 | 0.0% | 100.0% |  |
| STORE_FAST_LOAD_FAST | 620 | 0.0% | 100.0% |  |
| CALL_ALLOC_AND_ENTER_INIT | 600 | 0.0% | 100.0% | 3.3% |
| EXIT_INIT_CHECK | 580 | 0.0% | 100.0% |  |
| BEFORE_WITH | 560 | 0.0% | 100.0% |  |
| UNARY_NOT | 520 | 0.0% | 100.0% |  |
| DICT_MERGE | 460 | 0.0% | 100.0% |  |
| TO_BOOL_ALWAYS_TRUE | 400 | 0.0% | 100.0% | 10.0% |
| BUILD_SET | 400 | 0.0% | 100.0% |  |
| LOAD_ATTR_CLASS | 380 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_TUPLE_INT | 360 | 0.0% | 100.0% |  |
| UNPACK_SEQUENCE_TUPLE | 280 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 220 | 0.0% | 100.0% | 63.6% |
| IMPORT_NAME | 200 | 0.0% | 100.0% |  |
| BINARY_OP_SUBTRACT_FLOAT | 200 | 0.0% | 100.0% |  |
| BINARY_OP_MULTIPLY_FLOAT | 140 | 0.0% | 100.0% |  |
| CALL_STR_1 | 120 | 0.0% | 100.0% |  |
| LOAD_BUILD_CLASS | 100 | 0.0% | 100.0% |  |
| BUILD_CONST_KEY_MAP | 100 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_GETITEM | 100 | 0.0% | 100.0% |  |
| CALL_TUPLE_1 | 100 | 0.0% | 100.0% |  |
| BEFORE_ASYNC_WITH | 80 | 0.0% | 100.0% |  |
| RAISE_VARARGS | 80 | 0.0% | 100.0% |  |
| RERAISE | 80 | 0.0% | 100.0% |  |
| IMPORT_FROM | 60 | 0.0% | 100.0% |  |
| STORE_SLICE | 40 | 0.0% | 100.0% |  |
| UNARY_NEGATIVE | 40 | 0.0% | 100.0% |  |
| STORE_SUBSCR_LIST_INT | 40 | 0.0% | 100.0% |  |
| STORE_GLOBAL | 20 | 0.0% | 100.0% |  |


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 pairs </summary>

|Pair | Count | Self | Cumulative | 
|---|---:|---:|---:|
| LOAD_FAST LOAD_ATTR_INSTANCE_VALUE | 23,161,106 | 4.9% | 4.9% |
| STORE_FAST LOAD_FAST | 17,568,502 | 3.7% | 8.6% |
| RESUME_CHECK LOAD_FAST | 16,819,911 | 3.6% | 12.2% |
| TO_BOOL_BOOL POP_JUMP_IF_FALSE | 16,597,757 | 3.5% | 15.7% |
| POP_JUMP_IF_FALSE LOAD_FAST | 13,871,142 | 2.9% | 18.7% |
| LOAD_ATTR_METHOD_NO_DICT LOAD_FAST | 12,310,523 | 2.6% | 21.3% |
| LOAD_FAST TO_BOOL_BOOL | 10,570,723 | 2.2% | 23.5% |
| CALL_PY_EXACT_ARGS RESUME_CHECK | 10,463,546 | 2.2% | 25.7% |
| POP_JUMP_IF_TRUE LOAD_FAST | 9,153,228 | 1.9% | 27.7% |
| RETURN_CONST POP_TOP | 8,365,775 | 1.8% | 29.4% |
| RETURN_VALUE STORE_FAST | 7,784,390 | 1.6% | 31.1% |
| LOAD_FAST LOAD_ATTR_WITH_HINT | 7,548,039 | 1.6% | 32.7% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_NO_DICT | 7,467,306 | 1.6% | 34.3% |
| TO_BOOL POP_JUMP_IF_TRUE | 7,163,725 | 1.5% | 35.8% |
| LOAD_FAST RETURN_VALUE | 7,120,230 | 1.5% | 37.3% |
| POP_JUMP_IF_NONE LOAD_FAST | 7,080,647 | 1.5% | 38.8% |
| CALL STORE_FAST | 6,817,026 | 1.4% | 40.2% |
| LOAD_FAST TO_BOOL | 6,430,126 | 1.4% | 41.6% |
| LOAD_FAST POP_JUMP_IF_NONE | 6,423,905 | 1.4% | 43.0% |
| LOAD_FAST CALL | 6,107,424 | 1.3% | 44.3% |
| LOAD_FAST LOAD_ATTR | 5,703,459 | 1.2% | 45.5% |
| CALL_PY_WITH_DEFAULTS RESUME_CHECK | 5,451,482 | 1.2% | 46.6% |
| ENTER_EXECUTOR CALL_PY_WITH_DEFAULTS | 5,119,680 | 1.1% | 47.7% |
| LOAD_CONST LOAD_FAST | 4,972,795 | 1.1% | 48.8% |
| CALL_LIST_APPEND ENTER_EXECUTOR | 4,845,037 | 1.0% | 49.8% |
| POP_TOP RETURN_CONST | 4,693,985 | 1.0% | 50.8% |
| LOAD_CONST STORE_FAST | 4,570,855 | 1.0% | 51.7% |
| LOAD_FAST CALL_LIST_APPEND | 4,479,077 | 0.9% | 52.7% |
| POP_JUMP_IF_FALSE LOAD_FAST_CHECK | 4,478,897 | 0.9% | 53.6% |
| LOAD_FAST_CHECK LOAD_ATTR_METHOD_NO_DICT | 4,478,857 | 0.9% | 54.6% |
| POP_TOP LOAD_FAST | 4,349,993 | 0.9% | 55.5% |
| COMPARE_OP_INT POP_JUMP_IF_FALSE | 4,340,271 | 0.9% | 56.4% |
| LOAD_FAST LOAD_ATTR_SLOT | 4,117,408 | 0.9% | 57.3% |
| LOAD_ATTR CALL_PY_EXACT_ARGS | 3,922,827 | 0.8% | 58.1% |
| LOAD_ATTR_INSTANCE_VALUE TO_BOOL_BOOL | 3,921,031 | 0.8% | 59.0% |
| LOAD_FAST LOAD_ATTR_METHOD_WITH_VALUES | 3,824,166 | 0.8% | 59.8% |
| LOAD_GLOBAL_BUILTIN LOAD_FAST | 3,690,010 | 0.8% | 60.6% |
| LOAD_ATTR_METHOD_WITH_VALUES CALL_PY_EXACT_ARGS | 3,490,647 | 0.7% | 61.3% |
| NOP LOAD_FAST | 3,343,130 | 0.7% | 62.0% |
| TO_BOOL_BOOL POP_JUMP_IF_TRUE | 2,689,128 | 0.6% | 62.6% |
| LOAD_FAST_LOAD_FAST STORE_ATTR_SLOT | 2,640,548 | 0.6% | 63.1% |
| POP_JUMP_IF_FALSE LOAD_CONST | 2,637,089 | 0.6% | 63.7% |
| LOAD_ATTR_WITH_HINT TO_BOOL_BOOL | 2,614,545 | 0.6% | 64.3% |
| LOAD_FAST CALL_PY_EXACT_ARGS | 2,405,788 | 0.5% | 64.8% |
| LOAD_GLOBAL_MODULE LOAD_ATTR_MODULE | 2,395,066 | 0.5% | 65.3% |
| LOAD_GLOBAL_MODULE LOAD_ATTR | 2,262,024 | 0.5% | 65.8% |
| LOAD_ATTR_METHOD_WITH_VALUES LOAD_FAST | 2,074,467 | 0.4% | 66.2% |
| LOAD_FAST STORE_ATTR_SLOT | 2,023,469 | 0.4% | 66.6% |
| CACHE RESUME_CHECK | 2,020,845 | 0.4% | 67.0% |
| POP_TOP LOAD_CONST | 1,984,223 | 0.4% | 67.5% |
| STORE_ATTR_SLOT LOAD_FAST_LOAD_FAST | 1,979,866 | 0.4% | 67.9% |
| LOAD_FAST_LOAD_FAST LOAD_ATTR_WITH_HINT | 1,949,244 | 0.4% | 68.3% |
| LOAD_ATTR_WITH_HINT COMPARE_OP_INT | 1,949,124 | 0.4% | 68.7% |
| TO_BOOL_INT POP_JUMP_IF_FALSE | 1,768,362 | 0.4% | 69.1% |
| CALL_METHOD_DESCRIPTOR_O POP_TOP | 1,722,141 | 0.4% | 69.5% |
| LOAD_FAST LOAD_GLOBAL_MODULE | 1,703,563 | 0.4% | 69.8% |
| LOAD_ATTR_MODULE PUSH_NULL | 1,692,384 | 0.4% | 70.2% |
| POP_JUMP_IF_FALSE RETURN_CONST | 1,680,046 | 0.4% | 70.5% |
| LOAD_FAST LOAD_CONST | 1,656,889 | 0.4% | 70.9% |
| LOAD_FAST STORE_ATTR_INSTANCE_VALUE | 1,629,743 | 0.3% | 71.2% |
| LOAD_ATTR_WITH_HINT LOAD_GLOBAL_MODULE | 1,614,103 | 0.3% | 71.6% |
| LOAD_ATTR_INSTANCE_VALUE CALL_LEN | 1,606,604 | 0.3% | 71.9% |
| STORE_FAST LOAD_FAST_LOAD_FAST | 1,387,923 | 0.3% | 72.2% |
| LOAD_FAST CALL_METHOD_DESCRIPTOR_O | 1,370,782 | 0.3% | 72.5% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR_METHOD_WITH_VALUES | 1,358,745 | 0.3% | 72.8% |
| STORE_FAST LOAD_GLOBAL_BUILTIN | 1,355,923 | 0.3% | 73.1% |
| RETURN_CONST INTERPRETER_EXIT | 1,353,462 | 0.3% | 73.4% |
| RESUME_CHECK LOAD_GLOBAL_MODULE | 1,353,222 | 0.3% | 73.6% |
| STORE_FAST RETURN_CONST | 1,339,662 | 0.3% | 73.9% |
| TO_BOOL_INT POP_JUMP_IF_TRUE | 1,330,723 | 0.3% | 74.2% |
| POP_JUMP_IF_FALSE NOP | 1,329,861 | 0.3% | 74.5% |
| STORE_ATTR_SLOT LOAD_CONST | 1,329,185 | 0.3% | 74.8% |
| STORE_FAST JUMP_FORWARD | 1,312,847 | 0.3% | 75.1% |
| RESUME_CHECK JUMP_BACKWARD_NO_INTERRUPT | 1,307,844 | 0.3% | 75.3% |
| TO_BOOL_NONE POP_JUMP_IF_FALSE | 1,305,722 | 0.3% | 75.6% |
| LOAD_CONST COMPARE_OP_INT | 1,304,186 | 0.3% | 75.9% |
| LOAD_ATTR_SLOT TO_BOOL_NONE | 1,303,202 | 0.3% | 76.2% |
| LOAD_ATTR_INSTANCE_VALUE LOAD_ATTR | 1,301,282 | 0.3% | 76.4% |
| LOAD_ATTR_SLOT TO_BOOL_BOOL | 1,124,120 | 0.2% | 76.7% |
| LOAD_FAST LOAD_ATTR_METHOD_NO_DICT | 1,112,600 | 0.2% | 76.9% |
| POP_TOP ENTER_EXECUTOR | 1,077,960 | 0.2% | 77.1% |
| LOAD_FAST POP_JUMP_IF_NOT_NONE | 1,043,603 | 0.2% | 77.4% |
| LOAD_ATTR_INSTANCE_VALUE RETURN_VALUE | 1,040,745 | 0.2% | 77.6% |
| LOAD_FAST CALL_LEN | 1,033,362 | 0.2% | 77.8% |
| LOAD_FAST_LOAD_FAST LOAD_FAST | 1,031,222 | 0.2% | 78.0% |
| CALL_FUNCTION_EX POP_TOP | 1,017,961 | 0.2% | 78.2% |
| COPY TO_BOOL_INT | 1,010,402 | 0.2% | 78.4% |
| LOAD_GLOBAL_MODULE BINARY_OP | 1,010,362 | 0.2% | 78.7% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR_METHOD_WITH_VALUES | 995,962 | 0.2% | 78.9% |
| LOAD_ATTR LOAD_FAST | 995,724 | 0.2% | 79.1% |
| POP_JUMP_IF_FALSE LOAD_FAST_LOAD_FAST | 988,703 | 0.2% | 79.3% |
| GET_AWAITABLE LOAD_CONST | 987,823 | 0.2% | 79.5% |
| COMPARE_OP POP_JUMP_IF_FALSE | 985,303 | 0.2% | 79.7% |
| LOAD_ATTR COMPARE_OP | 983,043 | 0.2% | 79.9% |
| LOAD_ATTR_WITH_HINT LOAD_ATTR | 979,762 | 0.2% | 80.1% |
| LOAD_ATTR_INSTANCE_VALUE POP_JUMP_IF_NONE | 979,423 | 0.2% | 80.3% |
| YIELD_VALUE YIELD_VALUE | 979,343 | 0.2% | 80.5% |
| JUMP_BACKWARD_NO_INTERRUPT SEND_GEN | 979,043 | 0.2% | 80.7% |
| SEND_GEN RESUME_CHECK | 978,943 | 0.2% | 81.0% |
| UNPACK_SEQUENCE_TWO_TUPLE STORE_FAST_STORE_FAST | 972,904 | 0.2% | 81.2% |


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each opcode </summary>

### BINARY_SLICE

<details>
<summary> Successors and predecessors for BINARY_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 641,682 | 93.2% |
| LOAD_CONST | 46,759 | 6.8% |
| BINARY_OP_ADD_INT | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_O | 358,319 | 52.0% |
| CALL | 320,741 | 46.6% |
| STORE_FAST | 8,661 | 1.3% |
| LIST_EXTEND | 240 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 200 | 0.0% |


</details>

### STORE_SLICE

<details>
<summary> Successors and predecessors for STORE_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |


</details>

### CACHE

<details>
<summary> Successors and predecessors for CACHE </summary>

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 2,020,845 | 86.2% |
| COPY_FREE_VARS | 322,660 | 13.8% |
| RESUME | 920 | 0.0% |
| POP_TOP | 480 | 0.0% |
| RETURN_GENERATOR | 320 | 0.0% |


</details>

### BEFORE_ASYNC_WITH

<details>
<summary> Successors and predecessors for BEFORE_ASYNC_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 80 | 100.0% |


</details>

### BEFORE_WITH

<details>
<summary> Successors and predecessors for BEFORE_WITH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 240 | 42.9% |
| RETURN_VALUE | 120 | 21.4% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 21.4% |
| LOAD_GLOBAL | 40 | 7.1% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 40 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 520 | 92.9% |
| STORE_FAST | 40 | 7.1% |


</details>

### BINARY_SUBSCR

<details>
<summary> Successors and predecessors for BINARY_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 8,280 | 95.4% |
| BINARY_SUBSCR | 180 | 2.1% |
| LOAD_FAST | 120 | 1.4% |
| BUILD_SLICE | 60 | 0.7% |
| RETURN_VALUE | 40 | 0.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,080 | 93.1% |
| BINARY_SUBSCR | 180 | 2.1% |
| BINARY_SUBSCR_LIST_INT | 100 | 1.2% |
| BINARY_SUBSCR_DICT | 80 | 0.9% |
| LOAD_ATTR | 60 | 0.7% |


</details>

### CHECK_EXC_MATCH

<details>
<summary> Successors and predecessors for CHECK_EXC_MATCH </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 321,001 | 99.7% |
| LOAD_GLOBAL_BUILTIN | 680 | 0.2% |
| BUILD_TUPLE | 160 | 0.0% |
| LOAD_GLOBAL | 100 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 321,941 | 100.0% |


</details>

### DELETE_SUBSCR

<details>
<summary> Successors and predecessors for DELETE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_SLICE | 320,661 | 97.5% |
| LOAD_CONST | 8,000 | 2.4% |
| LOAD_FAST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 328,661 | 100.0% |
| LOAD_GLOBAL_MODULE | 60 | 0.0% |


</details>

### END_SEND

<details>
<summary> Successors and predecessors for END_SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 337,141 | 34.1% |
| SEND | 328,981 | 33.3% |
| RETURN_VALUE | 321,701 | 32.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 666,282 | 67.4% |
| STORE_FAST | 321,141 | 32.5% |
| UNPACK_SEQUENCE | 120 | 0.0% |
| UNPACK_SEQUENCE_TWO_TUPLE | 120 | 0.0% |
| RETURN_VALUE | 80 | 0.0% |


</details>

### EXIT_INIT_CHECK

<details>
<summary> Successors and predecessors for EXIT_INIT_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 580 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 580 | 100.0% |


</details>

### GET_ITER

<details>
<summary> Successors and predecessors for GET_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 645,842 | 66.1% |
| CALL_BUILTIN_CLASS | 322,101 | 33.0% |
| LOAD_ATTR_INSTANCE_VALUE | 8,140 | 0.8% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 180 | 0.0% |
| BINARY_SLICE | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 644,602 | 66.0% |
| FOR_ITER_RANGE | 322,021 | 33.0% |
| FOR_ITER | 8,640 | 0.9% |
| LOAD_FAST_AND_CLEAR | 680 | 0.1% |
| FOR_ITER_TUPLE | 460 | 0.0% |


</details>

### INTERPRETER_EXIT

<details>
<summary> Successors and predecessors for INTERPRETER_EXIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 1,353,462 | 57.7% |
| RETURN_VALUE | 662,222 | 28.2% |
| YIELD_VALUE | 329,221 | 14.0% |
| RETURN_GENERATOR | 400 | 0.0% |


</details>

### LOAD_BUILD_CLASS

<details>
<summary> Successors and predecessors for LOAD_BUILD_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 100 | 100.0% |


</details>

### MAKE_FUNCTION

<details>
<summary> Successors and predecessors for MAKE_FUNCTION </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 321,780 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SET_FUNCTION_ATTRIBUTE | 321,140 | 99.8% |
| STORE_NAME | 500 | 0.2% |
| LOAD_CONST | 100 | 0.0% |
| CALL_BUILTIN_FAST | 40 | 0.0% |


</details>

### NOP

<details>
<summary> Successors and predecessors for NOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,329,861 | 33.2% |
| POP_JUMP_IF_TRUE | 658,404 | 16.4% |
| STORE_FAST | 645,622 | 16.1% |
| NOP | 641,862 | 16.0% |
| RESUME_CHECK | 358,764 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,343,130 | 83.5% |
| NOP | 641,862 | 16.0% |
| LOAD_GLOBAL_MODULE | 18,982 | 0.5% |
| LOAD_GLOBAL_BUILTIN | 340 | 0.0% |
| LOAD_CONST | 300 | 0.0% |


</details>

### POP_EXCEPT

<details>
<summary> Successors and predecessors for POP_EXCEPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 321,261 | 99.8% |
| SWAP | 420 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| COPY | 80 | 0.0% |
| STORE_ATTR_INSTANCE_VALUE | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 320,941 | 99.7% |
| RETURN_VALUE | 420 | 0.1% |
| RETURN_CONST | 340 | 0.1% |
| POP_TOP | 80 | 0.0% |
| RERAISE | 80 | 0.0% |


</details>

### POP_TOP

<details>
<summary> Successors and predecessors for POP_TOP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 8,365,775 | 60.6% |
| CALL_METHOD_DESCRIPTOR_O | 1,722,141 | 12.5% |
| CALL_FUNCTION_EX | 1,017,961 | 7.4% |
| END_SEND | 666,282 | 4.8% |
| SEND_GEN | 658,382 | 4.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_CONST | 4,693,985 | 34.0% |
| LOAD_FAST | 4,349,993 | 31.5% |
| LOAD_CONST | 1,984,223 | 14.4% |
| ENTER_EXECUTOR | 1,077,960 | 7.8% |
| RESUME_CHECK | 658,842 | 4.8% |


</details>

### PUSH_EXC_INFO

<details>
<summary> Successors and predecessors for PUSH_EXC_INFO </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 320,801 | 99.6% |
| BINARY_SUBSCR_DICT | 520 | 0.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 360 | 0.1% |
| RERAISE | 80 | 0.0% |
| CALL_METHOD_DESCRIPTOR_O | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 320,941 | 99.7% |
| LOAD_GLOBAL_BUILTIN | 720 | 0.2% |
| LOAD_GLOBAL | 280 | 0.1% |


</details>

### PUSH_NULL

<details>
<summary> Successors and predecessors for PUSH_NULL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 1,692,384 | 82.8% |
| LOAD_ATTR | 324,541 | 15.9% |
| LOAD_DEREF | 24,243 | 1.2% |
| LOAD_FAST | 3,220 | 0.2% |
| LOAD_NAME | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 717,563 | 35.1% |
| LOAD_FAST_LOAD_FAST | 669,983 | 32.8% |
| CALL | 655,542 | 32.1% |
| LOAD_CONST | 840 | 0.0% |
| LOAD_GLOBAL_MODULE | 240 | 0.0% |


</details>

### RETURN_GENERATOR

<details>
<summary> Successors and predecessors for RETURN_GENERATOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 337,521 | 51.2% |
| ENTER_EXECUTOR | 320,261 | 48.6% |
| CALL_KW | 400 | 0.1% |
| CACHE | 320 | 0.0% |
| CALL | 300 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_AWAITABLE | 658,442 | 99.9% |
| INTERPRETER_EXIT | 400 | 0.1% |
| STORE_FAST | 160 | 0.0% |
| CALL | 120 | 0.0% |
| LIST_APPEND | 80 | 0.0% |


</details>

### RETURN_VALUE

<details>
<summary> Successors and predecessors for RETURN_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,120,230 | 67.3% |
| LOAD_ATTR_INSTANCE_VALUE | 1,040,745 | 9.8% |
| CALL | 690,501 | 6.5% |
| LOAD_ATTR | 641,401 | 6.1% |
| BINARY_OP_ADD_INT | 337,441 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 7,784,390 | 73.6% |
| TO_BOOL_BOOL | 694,243 | 6.6% |
| LOAD_FAST | 690,061 | 6.5% |
| INTERPRETER_EXIT | 662,222 | 6.3% |
| POP_TOP | 339,302 | 3.2% |


</details>

### STORE_SUBSCR

<details>
<summary> Successors and predecessors for STORE_SUBSCR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 240 | 27.9% |
| LOAD_ATTR_INSTANCE_VALUE | 140 | 16.3% |
| LOAD_CONST | 120 | 14.0% |
| LOAD_FAST | 120 | 14.0% |
| LOAD_ATTR | 100 | 11.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 220 | 25.6% |
| RETURN_CONST | 180 | 20.9% |
| STORE_SUBSCR_DICT | 160 | 18.6% |
| ENTER_EXECUTOR | 80 | 9.3% |
| JUMP_FORWARD | 80 | 9.3% |


</details>

### TO_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,430,126 | 85.5% |
| LOAD_ATTR_INSTANCE_VALUE | 743,440 | 9.9% |
| LOAD_ATTR_WITH_HINT | 336,981 | 4.5% |
| TO_BOOL | 4,760 | 0.1% |
| LOAD_ATTR | 2,560 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 7,163,725 | 95.2% |
| POP_JUMP_IF_FALSE | 349,082 | 4.6% |
| TO_BOOL | 4,760 | 0.1% |
| TO_BOOL_BOOL | 2,860 | 0.0% |
| TO_BOOL_INT | 460 | 0.0% |


</details>

### UNARY_INVERT

<details>
<summary> Successors and predecessors for UNARY_INVERT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 440 | 50.0% |
| BINARY_OP | 400 | 45.5% |
| LOAD_ATTR | 40 | 4.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 880 | 100.0% |


</details>

### UNARY_NEGATIVE

<details>
<summary> Successors and predecessors for UNARY_NEGATIVE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 40 | 100.0% |


</details>

### UNARY_NOT

<details>
<summary> Successors and predecessors for UNARY_NOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 340 | 65.4% |
| TO_BOOL | 80 | 15.4% |
| TO_BOOL_INT | 80 | 15.4% |
| TO_BOOL_LIST | 20 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 260 | 50.0% |
| RETURN_VALUE | 160 | 30.8% |
| STORE_FAST | 80 | 15.4% |
| CALL_PY_EXACT_ARGS | 20 | 3.8% |


</details>

### BINARY_OP

<details>
<summary> Successors and predecessors for BINARY_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 1,010,362 | 47.5% |
| LOAD_ATTR_MODULE | 695,602 | 32.7% |
| LOAD_ATTR | 366,740 | 17.3% |
| POP_JUMP_IF_FALSE | 45,999 | 2.2% |
| BINARY_OP | 2,600 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COPY | 688,821 | 32.4% |
| TO_BOOL_INT | 688,221 | 32.4% |
| STORE_FAST | 368,780 | 17.4% |
| BUILD_TUPLE | 366,580 | 17.3% |
| LOAD_FAST_LOAD_FAST | 7,941 | 0.4% |


</details>

### BUILD_CONST_KEY_MAP

<details>
<summary> Successors and predecessors for BUILD_CONST_KEY_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 40 | 40.0% |
| STORE_FAST | 40 | 40.0% |
| DICT_UPDATE | 20 | 20.0% |


</details>

### BUILD_LIST

<details>
<summary> Successors and predecessors for BUILD_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 322,121 | 33.3% |
| LOAD_ATTR_SLOT | 322,001 | 33.3% |
| LOAD_FAST | 321,542 | 33.2% |
| SWAP | 680 | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 643,383 | 66.5% |
| LOAD_FAST | 323,321 | 33.4% |
| SWAP | 680 | 0.1% |
| RETURN_VALUE | 240 | 0.0% |
| STORE_DEREF | 160 | 0.0% |


</details>

### BUILD_MAP

<details>
<summary> Successors and predecessors for BUILD_MAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| DICT_UPDATE | 720 | 33.0% |
| LOAD_FAST | 540 | 24.8% |
| BUILD_TUPLE | 240 | 11.0% |
| STORE_ATTR_INSTANCE_VALUE | 180 | 8.3% |
| STORE_FAST | 120 | 5.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 780 | 35.8% |
| EXTENDED_ARG | 580 | 26.6% |
| CALL_FUNCTION_EX | 320 | 14.7% |
| STORE_FAST | 280 | 12.8% |
| LOAD_CONST | 180 | 8.3% |


</details>

### BUILD_SET

<details>
<summary> Successors and predecessors for BUILD_SET </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 360 | 90.0% |
| LOAD_ATTR | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 400 | 100.0% |


</details>

### BUILD_SLICE

<details>
<summary> Successors and predecessors for BUILD_SLICE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 320,661 | 100.0% |
| LOAD_CONST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| DELETE_SUBSCR | 320,661 | 100.0% |
| BINARY_SUBSCR | 60 | 0.0% |


</details>

### BUILD_TUPLE

<details>
<summary> Successors and predecessors for BUILD_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 641,701 | 47.5% |
| BINARY_OP | 366,580 | 27.2% |
| LOAD_FAST | 322,220 | 23.9% |
| LOAD_FAST_LOAD_FAST | 9,141 | 0.7% |
| LOAD_GLOBAL_BUILTIN | 9,060 | 0.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CONTAINS_OP | 641,701 | 47.5% |
| CALL_LIST_APPEND | 366,660 | 27.2% |
| LOAD_CONST | 321,100 | 23.8% |
| CALL_ISINSTANCE | 8,920 | 0.7% |
| CALL_PY_EXACT_ARGS | 8,621 | 0.6% |


</details>

### CALL

<details>
<summary> Successors and predecessors for CALL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,107,424 | 69.0% |
| LOAD_FAST_LOAD_FAST | 660,942 | 7.5% |
| PUSH_NULL | 655,542 | 7.4% |
| LOAD_ATTR_INSTANCE_VALUE | 650,643 | 7.4% |
| LOAD_CONST | 339,642 | 3.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 6,817,026 | 77.0% |
| RETURN_VALUE | 690,501 | 7.8% |
| POP_TOP | 332,981 | 3.8% |
| RESUME_CHECK | 332,961 | 3.8% |
| LOAD_CONST | 320,861 | 3.6% |


</details>

### CALL_FUNCTION_EX

<details>
<summary> Successors and predecessors for CALL_FUNCTION_EX </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 695,620 | 68.3% |
| CALL_INTRINSIC_1 | 322,421 | 31.6% |
| DICT_MERGE | 460 | 0.0% |
| BUILD_MAP | 320 | 0.0% |
| LOAD_FAST | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,017,961 | 99.9% |
| STORE_FAST | 360 | 0.0% |
| RESUME_CHECK | 260 | 0.0% |
| GET_AWAITABLE | 160 | 0.0% |
| RETURN_VALUE | 140 | 0.0% |


</details>

### CALL_INTRINSIC_1

<details>
<summary> Successors and predecessors for CALL_INTRINSIC_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LIST_EXTEND | 322,781 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 322,421 | 99.9% |
| LOAD_CONST | 320 | 0.1% |
| BUILD_MAP | 40 | 0.0% |


</details>

### CALL_KW

<details>
<summary> Successors and predecessors for CALL_KW </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 341,202 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 329,081 | 96.4% |
| COPY_FREE_VARS | 8,021 | 2.4% |
| RESUME_CHECK | 1,360 | 0.4% |
| STORE_FAST | 1,200 | 0.4% |
| POP_TOP | 480 | 0.1% |


</details>

### COMPARE_OP

<details>
<summary> Successors and predecessors for COMPARE_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 983,043 | 99.4% |
| COMPARE_OP | 2,380 | 0.2% |
| LOAD_CONST | 1,400 | 0.1% |
| LOAD_ATTR_MODULE | 940 | 0.1% |
| LOAD_GLOBAL_MODULE | 240 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 985,303 | 99.6% |
| COMPARE_OP | 2,380 | 0.2% |
| COMPARE_OP_INT | 760 | 0.1% |
| POP_JUMP_IF_TRUE | 420 | 0.0% |
| COMPARE_OP_STR | 80 | 0.0% |


</details>

### CONTAINS_OP

<details>
<summary> Successors and predecessors for CONTAINS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BUILD_TUPLE | 641,701 | 99.6% |
| LOAD_FAST | 900 | 0.1% |
| LOAD_ATTR_INSTANCE_VALUE | 440 | 0.1% |
| BUILD_SET | 400 | 0.1% |
| LOAD_GLOBAL_MODULE | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 643,761 | 99.9% |
| POP_JUMP_IF_TRUE | 720 | 0.1% |
| STORE_FAST | 60 | 0.0% |
| EXTENDED_ARG | 20 | 0.0% |


</details>

### COPY

<details>
<summary> Successors and predecessors for COPY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| BINARY_OP | 688,821 | 67.4% |
| CALL_LEN | 321,841 | 31.5% |
| LOAD_FAST | 9,840 | 1.0% |
| SWAP | 720 | 0.1% |
| UNARY_NOT | 260 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_INT | 1,010,402 | 98.8% |
| LOAD_ATTR_WITH_HINT | 8,440 | 0.8% |
| LOAD_ATTR_INSTANCE_VALUE | 840 | 0.1% |
| COMPARE_OP_INT | 600 | 0.1% |
| TO_BOOL | 500 | 0.0% |


</details>

### COPY_FREE_VARS

<details>
<summary> Successors and predecessors for COPY_FREE_VARS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CACHE | 322,660 | 92.2% |
| CALL_PY_EXACT_ARGS | 10,181 | 2.9% |
| CALL_KW | 8,021 | 2.3% |
| CALL_BOUND_METHOD_EXACT_ARGS | 8,001 | 2.3% |
| LOAD_ATTR_PROPERTY | 580 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 349,083 | 99.7% |
| RESUME | 660 | 0.2% |
| RETURN_GENERATOR | 160 | 0.0% |
| MAKE_CELL | 80 | 0.0% |


</details>

### DICT_MERGE

<details>
<summary> Successors and predecessors for DICT_MERGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 420 | 91.3% |
| CALL | 40 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_FUNCTION_EX | 460 | 100.0% |


</details>

### DICT_UPDATE

<details>
<summary> Successors and predecessors for DICT_UPDATE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 740 | 97.4% |
| BUILD_CONST_KEY_MAP | 20 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| BUILD_MAP | 720 | 94.7% |
| EXTENDED_ARG | 20 | 2.6% |
| STORE_NAME | 20 | 2.6% |


</details>

### ENTER_EXECUTOR

<details>
<summary> Successors and predecessors for ENTER_EXECUTOR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_LIST_APPEND | 4,845,037 | 64.3% |
| POP_TOP | 1,077,960 | 14.3% |
| JUMP_FORWARD | 641,043 | 8.5% |
| POP_JUMP_IF_FALSE | 321,461 | 4.3% |
| POP_JUMP_IF_TRUE | 321,081 | 4.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_WITH_DEFAULTS | 5,119,680 | 67.9% |
| CALL_FUNCTION_EX | 695,620 | 9.2% |
| FOR_ITER_LIST | 641,362 | 8.5% |
| FOR_ITER_RANGE | 321,781 | 4.3% |
| RESUME_CHECK | 321,561 | 4.3% |


</details>

### EXTENDED_ARG

<details>
<summary> Successors and predecessors for EXTENDED_ARG </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAP_ADD | 9,480 | 56.6% |
| LOAD_CONST | 5,420 | 32.4% |
| BUILD_MAP | 580 | 3.5% |
| STORE_NAME | 360 | 2.2% |
| PUSH_NULL | 200 | 1.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 16,080 | 96.1% |
| FOR_ITER | 200 | 1.2% |
| JUMP_BACKWARD | 120 | 0.7% |
| POP_JUMP_IF_FALSE | 120 | 0.7% |
| FOR_ITER_LIST | 120 | 0.7% |


</details>

### FOR_ITER

<details>
<summary> Successors and predecessors for FOR_ITER </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 8,640 | 88.0% |
| JUMP_BACKWARD | 620 | 6.3% |
| FOR_ITER | 260 | 2.6% |
| EXTENDED_ARG | 200 | 2.0% |
| LOAD_FAST | 80 | 0.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,420 | 85.7% |
| RETURN_CONST | 480 | 4.9% |
| FOR_ITER_LIST | 280 | 2.9% |
| FOR_ITER | 260 | 2.6% |
| LOAD_FAST | 200 | 2.0% |


</details>

### GET_AWAITABLE

<details>
<summary> Successors and predecessors for GET_AWAITABLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_GENERATOR | 658,442 | 66.7% |
| LOAD_ATTR_INSTANCE_VALUE | 320,561 | 32.5% |
| LOAD_FAST | 8,160 | 0.8% |
| RETURN_VALUE | 240 | 0.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 987,823 | 100.0% |


</details>

### IMPORT_FROM

<details>
<summary> Successors and predecessors for IMPORT_FROM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| IMPORT_NAME | 60 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_NAME | 40 | 66.7% |
| STORE_FAST | 20 | 33.3% |


</details>

### IMPORT_NAME

<details>
<summary> Successors and predecessors for IMPORT_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 200 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 80 | 40.0% |
| IMPORT_FROM | 60 | 30.0% |
| STORE_NAME | 60 | 30.0% |


</details>

### IS_OP

<details>
<summary> Successors and predecessors for IS_OP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 820 | 36.0% |
| LOAD_FAST | 800 | 35.1% |
| LOAD_CONST | 560 | 24.6% |
| LOAD_FAST_LOAD_FAST | 80 | 3.5% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,600 | 70.2% |
| RETURN_VALUE | 400 | 17.5% |
| LOAD_DEREF | 160 | 7.0% |
| POP_JUMP_IF_TRUE | 120 | 5.3% |


</details>

### JUMP_BACKWARD

<details>
<summary> Successors and predecessors for JUMP_BACKWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,800 | 36.6% |
| POP_JUMP_IF_FALSE | 839 | 17.1% |
| CALL_LIST_APPEND | 600 | 12.2% |
| STORE_FAST | 580 | 11.8% |
| POP_JUMP_IF_TRUE | 340 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 1,520 | 30.9% |
| LOAD_FAST | 1,199 | 24.4% |
| FOR_ITER_RANGE | 900 | 18.3% |
| FOR_ITER | 620 | 12.6% |
| FOR_ITER_TUPLE | 360 | 7.3% |


</details>

### JUMP_BACKWARD_NO_INTERRUPT

<details>
<summary> Successors and predecessors for JUMP_BACKWARD_NO_INTERRUPT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 1,307,844 | 80.3% |
| POP_EXCEPT | 320,941 | 19.7% |
| RESUME | 480 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SEND_GEN | 979,043 | 60.1% |
| SEND | 329,281 | 20.2% |
| LOAD_FAST | 320,861 | 19.7% |
| LOAD_CONST | 80 | 0.0% |


</details>

### JUMP_FORWARD

<details>
<summary> Successors and predecessors for JUMP_FORWARD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,312,847 | 99.3% |
| POP_JUMP_IF_FALSE | 6,399 | 0.5% |
| POP_TOP | 1,219 | 0.1% |
| STORE_ATTR_INSTANCE_VALUE | 480 | 0.0% |
| STORE_ATTR | 320 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 641,043 | 48.5% |
| LOAD_FAST | 351,002 | 26.6% |
| LOAD_GLOBAL_BUILTIN | 328,460 | 24.8% |
| LOAD_FAST_LOAD_FAST | 500 | 0.0% |
| LOAD_GLOBAL | 240 | 0.0% |


</details>

### LIST_APPEND

<details>
<summary> Successors and predecessors for LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_METHOD_DESCRIPTOR_FAST | 560 | 82.4% |
| RETURN_GENERATOR | 80 | 11.8% |
| CALL_BUILTIN_CLASS | 40 | 5.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 600 | 88.2% |
| JUMP_BACKWARD | 80 | 11.8% |


</details>

### LIST_EXTEND

<details>
<summary> Successors and predecessors for LIST_EXTEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 322,001 | 99.7% |
| LOAD_FAST | 520 | 0.2% |
| BINARY_SLICE | 240 | 0.1% |
| LOAD_CONST | 60 | 0.0% |
| LOAD_ATTR | 20 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_INTRINSIC_1 | 322,781 | 100.0% |
| LOAD_NAME | 60 | 0.0% |


</details>

### LOAD_ATTR

<details>
<summary> Successors and predecessors for LOAD_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 5,703,459 | 52.2% |
| LOAD_GLOBAL_MODULE | 2,262,024 | 20.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,301,282 | 11.9% |
| LOAD_ATTR_WITH_HINT | 979,762 | 9.0% |
| LOAD_ATTR_SLOT | 322,401 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,922,827 | 35.9% |
| LOAD_FAST | 995,724 | 9.1% |
| COMPARE_OP | 983,043 | 9.0% |
| LOAD_CONST | 651,642 | 6.0% |
| LOAD_GLOBAL_MODULE | 643,021 | 5.9% |


</details>

### LOAD_CONST

<details>
<summary> Successors and predecessors for LOAD_CONST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 2,637,089 | 18.5% |
| POP_TOP | 1,984,223 | 13.9% |
| LOAD_FAST | 1,656,889 | 11.6% |
| STORE_ATTR_SLOT | 1,329,185 | 9.3% |
| GET_AWAITABLE | 987,823 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,972,795 | 34.9% |
| STORE_FAST | 4,570,855 | 32.1% |
| COMPARE_OP_INT | 1,304,186 | 9.2% |
| SEND_GEN | 658,222 | 4.6% |
| CALL_PY_EXACT_ARGS | 641,962 | 4.5% |


</details>

### LOAD_DEREF

<details>
<summary> Successors and predecessors for LOAD_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 649,141 | 39.3% |
| STORE_FAST | 328,981 | 19.9% |
| POP_JUMP_IF_FALSE | 321,160 | 19.4% |
| LOAD_CONST | 320,480 | 19.4% |
| LOAD_ATTR | 16,082 | 1.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 961,320 | 58.2% |
| LOAD_ATTR | 321,360 | 19.5% |
| STORE_ATTR_WITH_HINT | 320,360 | 19.4% |
| PUSH_NULL | 24,243 | 1.5% |
| LOAD_FAST | 13,041 | 0.8% |


</details>

### LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 17,568,502 | 16.8% |
| RESUME_CHECK | 16,819,911 | 16.0% |
| POP_JUMP_IF_FALSE | 13,871,142 | 13.2% |
| LOAD_ATTR_METHOD_NO_DICT | 12,310,523 | 11.7% |
| POP_JUMP_IF_TRUE | 9,153,228 | 8.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 23,161,106 | 22.1% |
| TO_BOOL_BOOL | 10,570,723 | 10.1% |
| LOAD_ATTR_WITH_HINT | 7,548,039 | 7.2% |
| RETURN_VALUE | 7,120,230 | 6.8% |
| TO_BOOL | 6,430,126 | 6.1% |


</details>

### LOAD_FAST_AND_CLEAR

<details>
<summary> Successors and predecessors for LOAD_FAST_AND_CLEAR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 680 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 680 | 100.0% |


</details>

### LOAD_FAST_CHECK

<details>
<summary> Successors and predecessors for LOAD_FAST_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,478,897 | 87.5% |
| STORE_FAST | 320,522 | 6.3% |
| LOAD_ATTR_METHOD_NO_DICT | 320,522 | 6.3% |
| POP_TOP | 240 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 4,478,857 | 87.5% |
| LOAD_FAST | 320,542 | 6.3% |
| CALL_METHOD_DESCRIPTOR_O | 320,482 | 6.3% |
| POP_JUMP_IF_NOT_NONE | 240 | 0.0% |
| CALL | 80 | 0.0% |


</details>

### LOAD_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for LOAD_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 1,979,866 | 26.6% |
| STORE_FAST | 1,387,923 | 18.7% |
| POP_JUMP_IF_FALSE | 988,703 | 13.3% |
| LOAD_ATTR_METHOD_NO_DICT | 742,981 | 10.0% |
| PUSH_NULL | 669,983 | 9.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_SLOT | 2,640,548 | 35.5% |
| LOAD_ATTR_WITH_HINT | 1,949,244 | 26.2% |
| LOAD_FAST | 1,031,222 | 13.9% |
| CALL | 660,942 | 8.9% |
| LOAD_FAST_LOAD_FAST | 654,481 | 8.8% |


</details>

### LOAD_GLOBAL

<details>
<summary> Successors and predecessors for LOAD_GLOBAL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,960 | 14.0% |
| LOAD_ATTR | 1,460 | 10.4% |
| RESUME_CHECK | 1,100 | 7.9% |
| RESUME | 1,080 | 7.7% |
| STORE_FAST | 1,040 | 7.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 4,740 | 33.9% |
| LOAD_ATTR | 3,100 | 22.2% |
| LOAD_GLOBAL_BUILTIN | 2,260 | 16.2% |
| LOAD_FAST | 1,140 | 8.2% |
| CALL | 620 | 4.4% |


</details>

### LOAD_NAME

<details>
<summary> Successors and predecessors for LOAD_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 200 | 26.3% |
| STORE_NAME | 120 | 15.8% |
| LOAD_CONST | 100 | 13.2% |
| RESUME | 100 | 13.2% |
| BINARY_OP | 80 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 480 | 63.2% |
| LOAD_ATTR | 140 | 18.4% |
| STORE_NAME | 100 | 13.2% |
| LOAD_NAME | 40 | 5.3% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 96.1% |
| LOAD_GLOBAL | 20 | 2.0% |
| LOAD_GLOBAL_MODULE | 20 | 2.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_SUPER_ATTR_METHOD | 440 | 43.1% |
| LOAD_FAST | 200 | 19.6% |
| CALL | 160 | 15.7% |
| LOAD_FAST_LOAD_FAST | 100 | 9.8% |
| LOAD_SUPER_ATTR_ATTR | 60 | 5.9% |


</details>

### MAKE_CELL

<details>
<summary> Successors and predecessors for MAKE_CELL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 320,600 | 99.6% |
| MAKE_CELL | 880 | 0.3% |
| CALL_KW | 160 | 0.0% |
| CACHE | 80 | 0.0% |
| CALL_FUNCTION_EX | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 320,720 | 99.6% |
| MAKE_CELL | 880 | 0.3% |
| RETURN_GENERATOR | 240 | 0.1% |
| RESUME | 80 | 0.0% |


</details>

### MAP_ADD

<details>
<summary> Successors and predecessors for MAP_ADD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 12,920 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| EXTENDED_ARG | 9,480 | 73.4% |
| LOAD_CONST | 2,680 | 20.7% |
| DICT_UPDATE | 740 | 5.7% |
| BUILD_MAP | 20 | 0.2% |


</details>

### POP_JUMP_IF_FALSE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_FALSE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 16,597,757 | 61.5% |
| COMPARE_OP_INT | 4,340,271 | 16.1% |
| TO_BOOL_INT | 1,768,362 | 6.6% |
| TO_BOOL_NONE | 1,305,722 | 4.8% |
| COMPARE_OP | 985,303 | 3.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 13,871,142 | 51.4% |
| LOAD_FAST_CHECK | 4,478,897 | 16.6% |
| LOAD_CONST | 2,637,089 | 9.8% |
| RETURN_CONST | 1,680,046 | 6.2% |
| NOP | 1,329,861 | 4.9% |


</details>

### POP_JUMP_IF_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,423,905 | 86.8% |
| LOAD_ATTR_INSTANCE_VALUE | 979,423 | 13.2% |
| LOAD_ATTR | 960 | 0.0% |
| LOAD_ATTR_WITH_HINT | 280 | 0.0% |
| CALL | 160 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,080,647 | 95.6% |
| LOAD_CONST | 321,121 | 4.3% |
| RETURN_CONST | 1,520 | 0.0% |
| LOAD_GLOBAL_MODULE | 440 | 0.0% |
| LOAD_FAST_LOAD_FAST | 400 | 0.0% |


</details>

### POP_JUMP_IF_NOT_NONE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_NOT_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,043,603 | 76.3% |
| LOAD_ATTR_INSTANCE_VALUE | 321,901 | 23.5% |
| LOAD_ATTR_WITH_HINT | 600 | 0.0% |
| LOAD_GLOBAL_MODULE | 480 | 0.0% |
| CALL_BUILTIN_FAST | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 702,582 | 51.4% |
| LOAD_GLOBAL_MODULE | 331,741 | 24.3% |
| LOAD_FAST_LOAD_FAST | 330,421 | 24.2% |
| RETURN_CONST | 620 | 0.0% |
| LOAD_GLOBAL | 600 | 0.0% |


</details>

### POP_JUMP_IF_TRUE

<details>
<summary> Successors and predecessors for POP_JUMP_IF_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL | 7,163,725 | 62.3% |
| TO_BOOL_BOOL | 2,689,128 | 23.4% |
| TO_BOOL_INT | 1,330,723 | 11.6% |
| COMPARE_OP_INT | 321,701 | 2.8% |
| TO_BOOL_STR | 840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 9,153,228 | 79.5% |
| NOP | 658,404 | 5.7% |
| RETURN_CONST | 367,280 | 3.2% |
| LOAD_CONST | 362,522 | 3.2% |
| STORE_FAST | 321,861 | 2.8% |


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
| POP_TOP | 4,693,985 | 46.7% |
| POP_JUMP_IF_FALSE | 1,680,046 | 16.7% |
| STORE_FAST | 1,339,662 | 13.3% |
| STORE_ATTR_SLOT | 669,603 | 6.7% |
| STORE_ATTR_INSTANCE_VALUE | 643,821 | 6.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 8,365,775 | 83.2% |
| INTERPRETER_EXIT | 1,353,462 | 13.5% |
| END_SEND | 337,141 | 3.4% |
| EXIT_INIT_CHECK | 580 | 0.0% |
| STORE_FAST | 460 | 0.0% |


</details>

### SEND

<details>
<summary> Successors and predecessors for SEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 329,601 | 50.0% |
| JUMP_BACKWARD_NO_INTERRUPT | 329,281 | 49.9% |
| SEND | 720 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| END_SEND | 328,981 | 49.9% |
| YIELD_VALUE | 328,981 | 49.9% |
| SEND | 720 | 0.1% |
| POP_TOP | 460 | 0.1% |
| SEND_GEN | 460 | 0.1% |


</details>

### SET_FUNCTION_ATTRIBUTE

<details>
<summary> Successors and predecessors for SET_FUNCTION_ATTRIBUTE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 321,140 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 320,940 | 99.9% |
| LOAD_FAST_LOAD_FAST | 80 | 0.0% |
| LOAD_GLOBAL_MODULE | 80 | 0.0% |
| STORE_NAME | 40 | 0.0% |


</details>

### STORE_ATTR

<details>
<summary> Successors and predecessors for STORE_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,340 | 66.3% |
| LOAD_FAST_LOAD_FAST | 2,520 | 20.0% |
| STORE_ATTR | 680 | 5.4% |
| SWAP | 400 | 3.2% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 2.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_ATTR_INSTANCE_VALUE | 3,560 | 28.3% |
| LOAD_FAST | 2,760 | 21.9% |
| LOAD_CONST | 1,760 | 14.0% |
| RETURN_CONST | 1,000 | 7.9% |
| STORE_ATTR | 680 | 5.4% |


</details>

### STORE_DEREF

<details>
<summary> Successors and predecessors for STORE_DEREF </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 320 | 36.4% |
| BUILD_LIST | 160 | 18.2% |
| CALL_KW | 160 | 18.2% |
| BINARY_OP_ADD_INT | 120 | 13.6% |
| CALL | 80 | 9.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 54.5% |
| LOAD_CONST | 160 | 18.2% |
| BUILD_LIST | 80 | 9.1% |
| LOAD_DEREF | 80 | 9.1% |
| LOAD_FAST_LOAD_FAST | 80 | 9.1% |


</details>

### STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 7,784,390 | 29.7% |
| CALL | 6,817,026 | 26.0% |
| LOAD_CONST | 4,570,855 | 17.4% |
| CALL_LEN | 697,140 | 2.7% |
| LOAD_ATTR_INSTANCE_VALUE | 689,021 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 17,568,502 | 67.0% |
| LOAD_FAST_LOAD_FAST | 1,387,923 | 5.3% |
| LOAD_GLOBAL_BUILTIN | 1,355,923 | 5.2% |
| RETURN_CONST | 1,339,662 | 5.1% |
| JUMP_FORWARD | 1,312,847 | 5.0% |


</details>

### STORE_FAST_LOAD_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_LOAD_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_TUPLE | 560 | 90.3% |
| CALL_LEN | 40 | 6.5% |
| COPY | 20 | 3.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_STR | 560 | 90.3% |
| PUSH_NULL | 40 | 6.5% |
| LOAD_ATTR | 20 | 3.2% |


</details>

### STORE_FAST_STORE_FAST

<details>
<summary> Successors and predecessors for STORE_FAST_STORE_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 972,904 | 99.9% |
| UNPACK_SEQUENCE | 300 | 0.0% |
| UNPACK_SEQUENCE_TUPLE | 160 | 0.0% |
| COPY | 100 | 0.0% |
| POP_TOP | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 972,224 | 99.9% |
| LOAD_FAST_LOAD_FAST | 340 | 0.0% |
| LOAD_GLOBAL_MODULE | 320 | 0.0% |
| STORE_FAST | 180 | 0.0% |
| NOP | 160 | 0.0% |


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

### STORE_NAME

<details>
<summary> Successors and predecessors for STORE_NAME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| MAKE_FUNCTION | 500 | 43.1% |
| CALL | 220 | 19.0% |
| LOAD_CONST | 160 | 13.8% |
| LOAD_NAME | 100 | 8.6% |
| IMPORT_NAME | 60 | 5.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 400 | 34.5% |
| EXTENDED_ARG | 360 | 31.0% |
| LOAD_NAME | 120 | 10.3% |
| RETURN_CONST | 120 | 10.3% |
| LOAD_BUILD_CLASS | 100 | 8.6% |


</details>

### SWAP

<details>
<summary> Successors and predecessors for SWAP </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 329,562 | 96.1% |
| BINARY_OP_SUBTRACT_INT | 8,400 | 2.4% |
| BINARY_OP_ADD_INT | 1,080 | 0.3% |
| BUILD_LIST | 680 | 0.2% |
| LOAD_FAST_AND_CLEAR | 680 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 330,162 | 96.3% |
| STORE_ATTR_WITH_HINT | 8,440 | 2.5% |
| STORE_ATTR_INSTANCE_VALUE | 840 | 0.2% |
| COPY | 720 | 0.2% |
| BUILD_LIST | 680 | 0.2% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 160 | 21.1% |
| STORE_FAST | 160 | 21.1% |
| END_SEND | 120 | 15.8% |
| LOAD_FAST | 80 | 10.5% |
| FOR_ITER_LIST | 80 | 10.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 320 | 42.1% |
| STORE_FAST_STORE_FAST | 300 | 39.5% |
| UNPACK_SEQUENCE_TUPLE | 60 | 7.9% |
| STORE_FAST | 40 | 5.3% |
| POP_TOP | 20 | 2.6% |


</details>

### YIELD_VALUE

<details>
<summary> Successors and predecessors for YIELD_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 979,343 | 74.8% |
| SEND | 328,981 | 25.1% |
| LOAD_CONST | 160 | 0.0% |
| CALL | 80 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| YIELD_VALUE | 979,343 | 74.8% |
| INTERPRETER_EXIT | 329,221 | 25.2% |


</details>

### RESUME

<details>
<summary> Successors and predecessors for RESUME </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL | 2,940 | 52.3% |
| CACHE | 920 | 16.4% |
| COPY_FREE_VARS | 660 | 11.7% |
| POP_TOP | 480 | 8.5% |
| SEND_GEN | 400 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 2,940 | 52.3% |
| LOAD_GLOBAL | 1,080 | 19.2% |
| JUMP_BACKWARD_NO_INTERRUPT | 480 | 8.5% |
| LOAD_CONST | 340 | 6.0% |
| NOP | 260 | 4.6% |


</details>

### BINARY_OP_ADD_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 321,821 | 99.9% |
| LOAD_FAST | 280 | 0.1% |
| BINARY_OP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 321,841 | 99.9% |
| LOAD_FAST | 300 | 0.1% |


</details>

### BINARY_OP_ADD_INT

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 337,421 | 51.1% |
| CALL_LEN | 320,901 | 48.6% |
| LOAD_CONST | 1,240 | 0.2% |
| BINARY_OP | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 337,441 | 51.1% |
| STORE_FAST | 320,761 | 48.6% |
| SWAP | 1,080 | 0.2% |
| BINARY_SLICE | 160 | 0.0% |
| LOAD_FAST | 120 | 0.0% |


</details>

### BINARY_OP_ADD_UNICODE

<details>
<summary> Successors and predecessors for BINARY_OP_ADD_UNICODE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 600 | 85.7% |
| BINARY_SUBSCR_LIST_INT | 80 | 11.4% |
| BINARY_OP | 20 | 2.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 480 | 68.6% |
| CALL | 120 | 17.1% |
| STORE_FAST | 80 | 11.4% |
| LOAD_GLOBAL | 20 | 2.9% |


</details>

### BINARY_OP_MULTIPLY_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 120 | 85.7% |
| BINARY_OP | 20 | 14.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_O | 120 | 85.7% |
| CALL | 20 | 14.3% |


</details>

### BINARY_OP_MULTIPLY_INT

<details>
<summary> Successors and predecessors for BINARY_OP_MULTIPLY_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,541 | 99.9% |
| LOAD_CONST | 320 | 0.1% |
| BINARY_OP | 60 | 0.0% |
| LOAD_ATTR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| COMPARE_OP_INT | 320,581 | 99.9% |
| STORE_FAST | 300 | 0.1% |
| COMPARE_OP | 40 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 40 | 0.0% |


</details>

### BINARY_OP_SUBTRACT_FLOAT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 120 | 60.0% |
| BINARY_OP | 40 | 20.0% |
| LOAD_FAST | 40 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 100.0% |


</details>

### BINARY_OP_SUBTRACT_INT

<details>
<summary> Successors and predecessors for BINARY_OP_SUBTRACT_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,040 | 48.6% |
| LOAD_FAST_LOAD_FAST | 7,960 | 48.1% |
| LOAD_CONST | 400 | 2.4% |
| BINARY_OP | 100 | 0.6% |
| CALL_LEN | 40 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| SWAP | 8,400 | 50.8% |
| STORE_FAST | 8,000 | 48.4% |
| LOAD_FAST | 60 | 0.4% |
| RETURN_VALUE | 40 | 0.2% |
| LOAD_FAST_LOAD_FAST | 40 | 0.2% |


</details>

### BINARY_SUBSCR_DICT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 8,061 | 82.1% |
| LOAD_FAST | 1,580 | 16.1% |
| BINARY_SUBSCR | 80 | 0.8% |
| LOAD_CONST | 80 | 0.8% |
| BUILD_TUPLE | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 8,201 | 83.5% |
| RETURN_VALUE | 940 | 9.6% |
| PUSH_EXC_INFO | 520 | 5.3% |
| LOAD_FAST | 120 | 1.2% |
| CALL_BUILTIN_CLASS | 40 | 0.4% |


</details>

### BINARY_SUBSCR_GETITEM

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_GETITEM </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 80 | 80.0% |
| LOAD_FAST | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 100 | 100.0% |


</details>

### BINARY_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 13,078 | 99.1% |
| BINARY_SUBSCR | 100 | 0.8% |
| LOAD_FAST | 20 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 6,659 | 50.5% |
| STORE_FAST | 6,279 | 47.6% |
| BINARY_OP_ADD_UNICODE | 80 | 0.6% |
| LOAD_ATTR | 60 | 0.5% |
| RETURN_VALUE | 40 | 0.3% |


</details>

### BINARY_SUBSCR_STR_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_STR_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 80 | 36.4% |
| LOAD_CONST | 80 | 36.4% |
| LOAD_FAST | 60 | 27.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 100 | 45.5% |
| STORE_FAST | 100 | 45.5% |
| PUSH_EXC_INFO | 20 | 9.1% |


</details>

### BINARY_SUBSCR_TUPLE_INT

<details>
<summary> Successors and predecessors for BINARY_SUBSCR_TUPLE_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 360 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 200 | 55.6% |
| RETURN_VALUE | 80 | 22.2% |
| LOAD_GLOBAL_MODULE | 80 | 22.2% |


</details>

### CALL_ALLOC_AND_ENTER_INIT

<details>
<summary> Successors and predecessors for CALL_ALLOC_AND_ENTER_INIT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 300 | 50.0% |
| LOAD_FAST_LOAD_FAST | 160 | 26.7% |
| CALL | 80 | 13.3% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 6.7% |
| LOAD_GLOBAL_MODULE | 20 | 3.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 580 | 96.7% |
| STORE_FAST | 20 | 3.3% |


</details>

### CALL_BOUND_METHOD_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_BOUND_METHOD_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 320,861 | 97.4% |
| CALL_BUILTIN_CLASS | 7,981 | 2.4% |
| LOAD_CONST | 360 | 0.1% |
| LOAD_FAST | 120 | 0.0% |
| PUSH_NULL | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 321,181 | 97.5% |
| COPY_FREE_VARS | 8,001 | 2.4% |
| POP_TOP | 240 | 0.1% |


</details>

### CALL_BUILTIN_CLASS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 330,222 | 85.8% |
| LOAD_ATTR_INSTANCE_VALUE | 53,559 | 13.9% |
| CALL | 280 | 0.1% |
| LOAD_GLOBAL_BUILTIN | 220 | 0.1% |
| LOAD_CONST | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 322,101 | 83.7% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 53,399 | 13.9% |
| CALL_BOUND_METHOD_EXACT_ARGS | 7,981 | 2.1% |
| STORE_FAST | 540 | 0.1% |
| LOAD_FAST | 240 | 0.1% |


</details>

### CALL_BUILTIN_FAST

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 1,060 | 59.6% |
| LOAD_FAST | 320 | 18.0% |
| LOAD_ATTR_SLOT | 180 | 10.1% |
| CALL | 120 | 6.7% |
| LOAD_FAST_LOAD_FAST | 60 | 3.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 560 | 31.5% |
| TO_BOOL_BOOL | 520 | 29.2% |
| POP_JUMP_IF_NOT_NONE | 360 | 20.2% |
| COPY | 220 | 12.4% |
| TO_BOOL | 60 | 3.4% |


</details>

### CALL_BUILTIN_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_BUILTIN_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_BUILTIN_CLASS | 53,399 | 98.7% |
| LOAD_FAST | 400 | 0.7% |
| LOAD_CONST | 120 | 0.2% |
| RETURN_GENERATOR | 80 | 0.1% |
| CALL_STR_1 | 40 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RETURN_VALUE | 53,779 | 99.4% |
| STORE_FAST | 260 | 0.5% |
| BEFORE_WITH | 40 | 0.1% |
| BUILD_TUPLE | 20 | 0.0% |
| LOAD_GLOBAL_BUILTIN | 20 | 0.0% |


</details>

### CALL_BUILTIN_O

<details>
<summary> Successors and predecessors for CALL_BUILTIN_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 440 | 38.6% |
| LOAD_ATTR_INSTANCE_VALUE | 280 | 24.6% |
| CALL | 120 | 10.5% |
| BINARY_OP_MULTIPLY_FLOAT | 120 | 10.5% |
| LOAD_CONST | 80 | 7.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 500 | 43.9% |
| STORE_FAST | 300 | 26.3% |
| LOAD_CONST | 140 | 12.3% |
| BUILD_TUPLE | 80 | 7.0% |
| TO_BOOL_INT | 60 | 5.3% |


</details>

### CALL_ISINSTANCE

<details>
<summary> Successors and predecessors for CALL_ISINSTANCE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_BUILTIN | 19,022 | 65.9% |
| BUILD_TUPLE | 8,920 | 30.9% |
| CALL | 380 | 1.3% |
| LOAD_GLOBAL_MODULE | 360 | 1.2% |
| LOAD_ATTR_MODULE | 160 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 28,442 | 98.5% |
| TO_BOOL | 380 | 1.3% |
| RETURN_VALUE | 40 | 0.1% |
| LOAD_FAST | 20 | 0.1% |


</details>

### CALL_LEN

<details>
<summary> Successors and predecessors for CALL_LEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 1,606,604 | 54.3% |
| LOAD_FAST | 1,033,362 | 34.9% |
| LOAD_ATTR_WITH_HINT | 320,861 | 10.8% |
| CALL | 320 | 0.0% |
| BINARY_SUBSCR | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 697,140 | 23.5% |
| TO_BOOL_INT | 650,262 | 22.0% |
| LOAD_FAST | 641,341 | 21.7% |
| COPY | 321,841 | 10.9% |
| LOAD_CONST | 321,181 | 10.8% |


</details>

### CALL_LIST_APPEND

<details>
<summary> Successors and predecessors for CALL_LIST_APPEND </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,479,077 | 92.4% |
| BUILD_TUPLE | 366,660 | 7.6% |
| CALL | 120 | 0.0% |
| LOAD_ATTR_MODULE | 120 | 0.0% |
| LOAD_CONST | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 4,845,037 | 100.0% |
| JUMP_BACKWARD | 600 | 0.0% |
| JUMP_FORWARD | 140 | 0.0% |
| NOP | 80 | 0.0% |
| LOAD_CONST | 80 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 329,541 | 49.8% |
| LOAD_FAST | 321,261 | 48.6% |
| LOAD_FAST_LOAD_FAST | 8,941 | 1.4% |
| LOAD_GLOBAL_MODULE | 680 | 0.1% |
| RETURN_VALUE | 360 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 651,082 | 98.5% |
| RETURN_VALUE | 9,101 | 1.4% |
| LIST_APPEND | 560 | 0.1% |
| POP_TOP | 220 | 0.0% |
| LOAD_FAST | 60 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 321,821 | 99.5% |
| LOAD_FAST | 480 | 0.1% |
| LOAD_ATTR | 360 | 0.1% |
| LOAD_CONST | 280 | 0.1% |
| CALL | 220 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 322,001 | 99.6% |
| POP_TOP | 1,020 | 0.3% |
| RETURN_VALUE | 140 | 0.0% |
| LOAD_CONST | 40 | 0.0% |
| LOAD_ATTR_METHOD_NO_DICT | 40 | 0.0% |


</details>

### CALL_METHOD_DESCRIPTOR_NOARGS

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_NOARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 369,879 | 52.8% |
| LOAD_ATTR | 329,221 | 47.0% |
| CALL | 840 | 0.1% |
| LOAD_FAST | 360 | 0.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 367,619 | 52.5% |
| TO_BOOL_BOOL | 329,341 | 47.0% |
| POP_TOP | 920 | 0.1% |
| RETURN_VALUE | 700 | 0.1% |
| LOAD_FAST | 460 | 0.1% |


</details>

### CALL_METHOD_DESCRIPTOR_O

<details>
<summary> Successors and predecessors for CALL_METHOD_DESCRIPTOR_O </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,370,782 | 66.8% |
| BINARY_SLICE | 358,319 | 17.5% |
| LOAD_FAST_CHECK | 320,482 | 15.6% |
| CALL | 820 | 0.0% |
| LOAD_CONST | 600 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_TOP | 1,722,141 | 83.9% |
| CALL_PY_EXACT_ARGS | 320,482 | 15.6% |
| RETURN_VALUE | 8,560 | 0.4% |
| LOAD_CONST | 280 | 0.0% |
| STORE_FAST | 80 | 0.0% |


</details>

### CALL_PY_EXACT_ARGS

<details>
<summary> Successors and predecessors for CALL_PY_EXACT_ARGS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 3,922,827 | 35.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 3,490,647 | 31.4% |
| LOAD_FAST | 2,405,788 | 21.6% |
| LOAD_CONST | 641,962 | 5.8% |
| LOAD_ATTR_METHOD_NO_DICT | 330,842 | 3.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 10,463,546 | 94.0% |
| RETURN_GENERATOR | 337,521 | 3.0% |
| MAKE_CELL | 320,600 | 2.9% |
| COPY_FREE_VARS | 10,181 | 0.1% |
| RESUME | 20 | 0.0% |


</details>

### CALL_PY_WITH_DEFAULTS

<details>
<summary> Successors and predecessors for CALL_PY_WITH_DEFAULTS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 5,119,680 | 93.9% |
| LOAD_ATTR | 321,341 | 5.9% |
| LOAD_FAST | 9,161 | 0.2% |
| LOAD_ATTR_METHOD_NO_DICT | 360 | 0.0% |
| LOAD_ATTR_METHOD_WITH_VALUES | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 5,451,482 | 100.0% |
| RETURN_GENERATOR | 120 | 0.0% |


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
| LOAD_GLOBAL_MODULE | 80 | 80.0% |
| LOAD_FAST | 20 | 20.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL | 80 | 80.0% |
| CALL_BUILTIN_FAST_WITH_KEYWORDS | 20 | 20.0% |


</details>

### CALL_TYPE_1

<details>
<summary> Successors and predecessors for CALL_TYPE_1 </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 980 | 94.2% |
| LOAD_GLOBAL_MODULE | 40 | 3.8% |
| CALL | 20 | 1.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 740 | 71.2% |
| LOAD_GLOBAL_MODULE | 200 | 19.2% |
| PUSH_NULL | 40 | 3.8% |
| LOAD_FAST_LOAD_FAST | 40 | 3.8% |
| LOAD_GLOBAL | 20 | 1.9% |


</details>

### COMPARE_OP_FLOAT

<details>
<summary> Successors and predecessors for COMPARE_OP_FLOAT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 6,259 | 95.7% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 1.8% |
| LOAD_ATTR_SLOT | 120 | 1.8% |
| COMPARE_OP | 40 | 0.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 6,399 | 97.9% |
| RETURN_VALUE | 140 | 2.1% |


</details>

### COMPARE_OP_INT

<details>
<summary> Successors and predecessors for COMPARE_OP_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_WITH_HINT | 1,949,124 | 41.8% |
| LOAD_CONST | 1,304,186 | 28.0% |
| LOAD_GLOBAL_MODULE | 321,861 | 6.9% |
| LOAD_FAST | 321,581 | 6.9% |
| BINARY_OP_MULTIPLY_INT | 320,581 | 6.9% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 4,340,271 | 93.1% |
| POP_JUMP_IF_TRUE | 321,701 | 6.9% |
| RETURN_VALUE | 60 | 0.0% |
| STORE_FAST | 40 | 0.0% |


</details>

### COMPARE_OP_STR

<details>
<summary> Successors and predecessors for COMPARE_OP_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_CONST | 740 | 75.5% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 12.2% |
| COMPARE_OP | 80 | 8.2% |
| LOAD_FAST | 40 | 4.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 840 | 85.7% |
| COPY | 60 | 6.1% |
| STORE_FAST | 60 | 6.1% |
| EXTENDED_ARG | 20 | 2.0% |


</details>

### FOR_ITER_LIST

<details>
<summary> Successors and predecessors for FOR_ITER_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 644,602 | 50.0% |
| ENTER_EXECUTOR | 641,362 | 49.8% |
| JUMP_BACKWARD | 1,520 | 0.1% |
| FOR_ITER | 280 | 0.0% |
| EXTENDED_ARG | 120 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| UNPACK_SEQUENCE_TWO_TUPLE | 642,422 | 49.9% |
| RETURN_CONST | 322,041 | 25.0% |
| LOAD_FAST | 321,941 | 25.0% |
| STORE_FAST | 1,020 | 0.1% |
| LOAD_DEREF | 140 | 0.0% |


</details>

### FOR_ITER_RANGE

<details>
<summary> Successors and predecessors for FOR_ITER_RANGE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| GET_ITER | 322,021 | 49.9% |
| ENTER_EXECUTOR | 321,781 | 49.9% |
| JUMP_BACKWARD | 900 | 0.1% |
| FOR_ITER | 60 | 0.0% |
| SWAP | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 322,761 | 50.1% |
| LOAD_CONST | 321,861 | 49.9% |
| LOAD_FAST | 100 | 0.0% |
| SWAP | 40 | 0.0% |
| LOAD_GLOBAL_MODULE | 40 | 0.0% |


</details>

### FOR_ITER_TUPLE

<details>
<summary> Successors and predecessors for FOR_ITER_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 8,260 | 85.3% |
| SWAP | 560 | 5.8% |
| GET_ITER | 460 | 4.8% |
| JUMP_BACKWARD | 360 | 3.7% |
| FOR_ITER | 40 | 0.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| NOP | 8,000 | 82.6% |
| STORE_FAST_LOAD_FAST | 560 | 5.8% |
| SWAP | 560 | 5.8% |
| STORE_FAST | 460 | 4.8% |
| LOAD_GLOBAL | 40 | 0.4% |


</details>

### LOAD_ATTR_CLASS

<details>
<summary> Successors and predecessors for LOAD_ATTR_CLASS </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 360 | 94.7% |
| LOAD_ATTR | 20 | 5.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 380 | 100.0% |


</details>

### LOAD_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for LOAD_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 23,161,106 | 99.9% |
| LOAD_FAST_LOAD_FAST | 9,501 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 9,041 | 0.0% |
| LOAD_ATTR | 4,880 | 0.0% |
| COPY | 840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_METHOD_NO_DICT | 7,467,306 | 32.2% |
| TO_BOOL_BOOL | 3,921,031 | 16.9% |
| CALL_LEN | 1,606,604 | 6.9% |
| LOAD_ATTR_METHOD_WITH_VALUES | 1,358,745 | 5.9% |
| LOAD_ATTR | 1,301,282 | 5.6% |


</details>

### LOAD_ATTR_METHOD_NO_DICT

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_NO_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 7,467,306 | 51.8% |
| LOAD_FAST_CHECK | 4,478,857 | 31.1% |
| LOAD_FAST | 1,112,600 | 7.7% |
| LOAD_ATTR_WITH_HINT | 650,922 | 4.5% |
| LOAD_ATTR | 376,901 | 2.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 12,310,523 | 85.4% |
| LOAD_FAST_LOAD_FAST | 742,981 | 5.2% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 369,879 | 2.6% |
| CALL_PY_EXACT_ARGS | 330,842 | 2.3% |
| CALL_METHOD_DESCRIPTOR_FAST | 329,541 | 2.3% |


</details>

### LOAD_ATTR_METHOD_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_METHOD_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,824,166 | 55.7% |
| LOAD_ATTR_INSTANCE_VALUE | 1,358,745 | 19.8% |
| LOAD_ATTR_WITH_HINT | 995,962 | 14.5% |
| LOAD_ATTR_SLOT | 677,284 | 9.9% |
| RETURN_VALUE | 9,021 | 0.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 3,490,647 | 50.8% |
| LOAD_FAST | 2,074,467 | 30.2% |
| LOAD_FAST_LOAD_FAST | 660,082 | 9.6% |
| LOAD_CONST | 641,323 | 9.3% |
| CALL | 1,820 | 0.0% |


</details>

### LOAD_ATTR_MODULE

<details>
<summary> Successors and predecessors for LOAD_ATTR_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 2,395,066 | 99.9% |
| LOAD_ATTR | 2,280 | 0.1% |
| LOAD_FAST | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| PUSH_NULL | 1,692,384 | 70.6% |
| BINARY_OP | 695,602 | 29.0% |
| CALL | 1,280 | 0.1% |
| LOAD_FAST | 1,080 | 0.0% |
| LOAD_CONST | 1,040 | 0.0% |


</details>

### LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES

<details>
<summary> Successors and predecessors for LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 740 | 84.1% |
| LOAD_ATTR | 120 | 13.6% |
| LOAD_FAST_LOAD_FAST | 20 | 2.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 580 | 65.9% |
| CALL | 140 | 15.9% |
| BINARY_OP | 120 | 13.6% |
| CALL_ISINSTANCE | 20 | 2.3% |
| LOAD_GLOBAL_BUILTIN | 20 | 2.3% |


</details>

### LOAD_ATTR_PROPERTY

<details>
<summary> Successors and predecessors for LOAD_ATTR_PROPERTY </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 321,401 | 99.9% |
| LOAD_ATTR | 220 | 0.1% |
| LOAD_DEREF | 120 | 0.0% |
| LOAD_FAST_LOAD_FAST | 40 | 0.0% |
| LOAD_ATTR_INSTANCE_VALUE | 40 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 321,241 | 99.8% |
| COPY_FREE_VARS | 580 | 0.2% |


</details>

### LOAD_ATTR_SLOT

<details>
<summary> Successors and predecessors for LOAD_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 4,117,408 | 99.6% |
| LOAD_FAST_LOAD_FAST | 7,980 | 0.2% |
| BINARY_SUBSCR_LIST_INT | 6,659 | 0.2% |
| LOAD_ATTR | 940 | 0.0% |
| LOAD_ATTR_MODULE | 820 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_NONE | 1,303,202 | 31.5% |
| TO_BOOL_BOOL | 1,124,120 | 27.2% |
| LOAD_ATTR_METHOD_WITH_VALUES | 677,284 | 16.4% |
| LOAD_ATTR | 322,401 | 7.8% |
| BUILD_LIST | 322,001 | 7.8% |


</details>

### LOAD_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for LOAD_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 7,548,039 | 72.1% |
| LOAD_FAST_LOAD_FAST | 1,949,244 | 18.6% |
| LOAD_DEREF | 961,320 | 9.2% |
| COPY | 8,440 | 0.1% |
| LOAD_ATTR | 1,840 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| TO_BOOL_BOOL | 2,614,545 | 25.0% |
| COMPARE_OP_INT | 1,949,124 | 18.6% |
| LOAD_GLOBAL_MODULE | 1,614,103 | 15.4% |
| LOAD_ATTR_METHOD_WITH_VALUES | 995,962 | 9.5% |
| LOAD_ATTR | 979,762 | 9.4% |


</details>

### LOAD_GLOBAL_BUILTIN

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_BUILTIN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST | 1,355,923 | 32.5% |
| POP_JUMP_IF_FALSE | 636,482 | 15.3% |
| LOAD_GLOBAL_BUILTIN | 445,299 | 10.7% |
| RESUME_CHECK | 406,382 | 9.7% |
| LOAD_FAST | 348,503 | 8.4% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,690,010 | 88.5% |
| LOAD_GLOBAL_BUILTIN | 445,299 | 10.7% |
| CALL_ISINSTANCE | 19,022 | 0.5% |
| BUILD_TUPLE | 9,060 | 0.2% |
| LOAD_DEREF | 4,200 | 0.1% |


</details>

### LOAD_GLOBAL_MODULE

<details>
<summary> Successors and predecessors for LOAD_GLOBAL_MODULE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,703,563 | 26.5% |
| LOAD_ATTR_WITH_HINT | 1,614,103 | 25.1% |
| RESUME_CHECK | 1,353,222 | 21.0% |
| LOAD_ATTR | 643,021 | 10.0% |
| POP_TOP | 375,841 | 5.8% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_MODULE | 2,395,066 | 37.2% |
| LOAD_ATTR | 2,262,024 | 35.2% |
| BINARY_OP | 1,010,362 | 15.7% |
| COMPARE_OP_INT | 321,861 | 5.0% |
| CHECK_EXC_MATCH | 321,001 | 5.0% |


</details>

### LOAD_SUPER_ATTR_ATTR

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_ATTR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 640 | 78.0% |
| LOAD_GLOBAL_MODULE | 120 | 14.6% |
| LOAD_SUPER_ATTR | 60 | 7.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_GLOBAL_MODULE | 640 | 78.0% |
| LOAD_ATTR_METHOD_NO_DICT | 120 | 14.6% |
| LOAD_GLOBAL | 40 | 4.9% |
| LOAD_ATTR | 20 | 2.4% |


</details>

### LOAD_SUPER_ATTR_METHOD

<details>
<summary> Successors and predecessors for LOAD_SUPER_ATTR_METHOD </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 3,080 | 87.5% |
| LOAD_SUPER_ATTR | 440 | 12.5% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,400 | 39.8% |
| LOAD_FAST_LOAD_FAST | 1,220 | 34.7% |
| CALL_PY_EXACT_ARGS | 760 | 21.6% |
| CALL | 140 | 4.0% |


</details>

### RESUME_CHECK

<details>
<summary> Successors and predecessors for RESUME_CHECK </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| CALL_PY_EXACT_ARGS | 10,463,546 | 48.6% |
| CALL_PY_WITH_DEFAULTS | 5,451,482 | 25.3% |
| CACHE | 2,020,845 | 9.4% |
| SEND_GEN | 978,943 | 4.5% |
| POP_TOP | 658,842 | 3.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 16,819,911 | 78.1% |
| LOAD_GLOBAL_MODULE | 1,353,222 | 6.3% |
| JUMP_BACKWARD_NO_INTERRUPT | 1,307,844 | 6.1% |
| LOAD_DEREF | 649,141 | 3.0% |
| LOAD_CONST | 644,061 | 3.0% |


</details>

### SEND_GEN

<details>
<summary> Successors and predecessors for SEND_GEN </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| JUMP_BACKWARD_NO_INTERRUPT | 979,043 | 59.8% |
| LOAD_CONST | 658,222 | 40.2% |
| SEND | 460 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| RESUME_CHECK | 978,943 | 59.8% |
| POP_TOP | 658,382 | 40.2% |
| RESUME | 400 | 0.0% |


</details>

### STORE_ATTR_INSTANCE_VALUE

<details>
<summary> Successors and predecessors for STORE_ATTR_INSTANCE_VALUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 1,629,743 | 99.4% |
| LOAD_FAST_LOAD_FAST | 4,200 | 0.3% |
| STORE_ATTR | 3,560 | 0.2% |
| SWAP | 840 | 0.1% |
| LOAD_DEREF | 360 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 661,561 | 40.4% |
| RETURN_CONST | 643,821 | 39.3% |
| NOP | 320,621 | 19.6% |
| LOAD_CONST | 6,200 | 0.4% |
| LOAD_FAST_LOAD_FAST | 2,140 | 0.1% |


</details>

### STORE_ATTR_SLOT

<details>
<summary> Successors and predecessors for STORE_ATTR_SLOT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 2,640,548 | 56.6% |
| LOAD_FAST | 2,023,469 | 43.4% |
| STORE_ATTR | 560 | 0.0% |
| STORE_ATTR_SLOT | 60 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 1,979,866 | 42.4% |
| LOAD_CONST | 1,329,185 | 28.5% |
| LOAD_FAST | 669,963 | 14.4% |
| RETURN_CONST | 669,603 | 14.4% |
| NOP | 15,960 | 0.3% |


</details>

### STORE_ATTR_WITH_HINT

<details>
<summary> Successors and predecessors for STORE_ATTR_WITH_HINT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 353,120 | 51.1% |
| LOAD_DEREF | 320,360 | 46.4% |
| SWAP | 8,440 | 1.2% |
| ENTER_EXECUTOR | 7,600 | 1.1% |
| LOAD_FAST_LOAD_FAST | 1,120 | 0.2% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 337,320 | 48.8% |
| RETURN_CONST | 329,420 | 47.7% |
| NOP | 15,800 | 2.3% |
| ENTER_EXECUTOR | 7,660 | 1.1% |
| LOAD_CONST | 420 | 0.1% |


</details>

### STORE_SUBSCR_DICT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_DICT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR | 8,341 | 88.9% |
| LOAD_FAST | 480 | 5.1% |
| LOAD_CONST | 280 | 3.0% |
| STORE_SUBSCR | 160 | 1.7% |
| LOAD_ATTR_INSTANCE_VALUE | 120 | 1.3% |

|Successors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 8,681 | 92.5% |
| NOP | 220 | 2.3% |
| LOAD_CONST | 140 | 1.5% |
| RETURN_CONST | 140 | 1.5% |
| LOAD_GLOBAL_MODULE | 120 | 1.3% |


</details>

### STORE_SUBSCR_LIST_INT

<details>
<summary> Successors and predecessors for STORE_SUBSCR_LIST_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST_LOAD_FAST | 40 | 100.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| ENTER_EXECUTOR | 20 | 50.0% |
| RETURN_CONST | 20 | 50.0% |


</details>

### TO_BOOL_ALWAYS_TRUE

<details>
<summary> Successors and predecessors for TO_BOOL_ALWAYS_TRUE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 280 | 70.0% |
| TO_BOOL | 80 | 20.0% |
| TO_BOOL_NONE | 40 | 10.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 260 | 65.0% |
| POP_JUMP_IF_TRUE | 140 | 35.0% |


</details>

### TO_BOOL_BOOL

<details>
<summary> Successors and predecessors for TO_BOOL_BOOL </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 10,570,723 | 54.8% |
| LOAD_ATTR_INSTANCE_VALUE | 3,921,031 | 20.3% |
| LOAD_ATTR_WITH_HINT | 2,614,545 | 13.6% |
| LOAD_ATTR_SLOT | 1,124,120 | 5.8% |
| RETURN_VALUE | 694,243 | 3.6% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 16,597,757 | 86.1% |
| POP_JUMP_IF_TRUE | 2,689,128 | 13.9% |
| UNARY_NOT | 340 | 0.0% |
| EXTENDED_ARG | 100 | 0.0% |


</details>

### TO_BOOL_INT

<details>
<summary> Successors and predecessors for TO_BOOL_INT </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| COPY | 1,010,402 | 32.6% |
| BINARY_OP | 688,221 | 22.2% |
| CALL_LEN | 650,262 | 21.0% |
| LOAD_FAST | 375,020 | 12.1% |
| LOAD_ATTR_INSTANCE_VALUE | 374,700 | 12.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,768,362 | 57.1% |
| POP_JUMP_IF_TRUE | 1,330,723 | 42.9% |
| UNARY_NOT | 80 | 0.0% |


</details>

### TO_BOOL_LIST

<details>
<summary> Successors and predecessors for TO_BOOL_LIST </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_INSTANCE_VALUE | 644,982 | 99.9% |
| LOAD_FAST | 360 | 0.1% |
| TO_BOOL | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 645,242 | 100.0% |
| POP_JUMP_IF_TRUE | 280 | 0.0% |
| UNARY_NOT | 20 | 0.0% |


</details>

### TO_BOOL_NONE

<details>
<summary> Successors and predecessors for TO_BOOL_NONE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_ATTR_SLOT | 1,303,202 | 99.8% |
| LOAD_FAST | 1,700 | 0.1% |
| LOAD_ATTR | 600 | 0.0% |
| TO_BOOL | 280 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_FALSE | 1,305,722 | 100.0% |
| TO_BOOL_ALWAYS_TRUE | 40 | 0.0% |
| POP_JUMP_IF_TRUE | 20 | 0.0% |


</details>

### TO_BOOL_STR

<details>
<summary> Successors and predecessors for TO_BOOL_STR </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_LOAD_FAST | 560 | 46.7% |
| LOAD_FAST | 400 | 33.3% |
| COPY | 160 | 13.3% |
| TO_BOOL | 80 | 6.7% |

|Successors | Count | Percentage | 
|---|---:|---:|
| POP_JUMP_IF_TRUE | 840 | 70.0% |
| POP_JUMP_IF_FALSE | 360 | 30.0% |


</details>

### UNPACK_SEQUENCE_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| LOAD_FAST | 80 | 28.6% |
| CALL_METHOD_DESCRIPTOR_O | 80 | 28.6% |
| UNPACK_SEQUENCE | 60 | 21.4% |
| BINARY_SUBSCR_LIST_INT | 40 | 14.3% |
| RETURN_VALUE | 20 | 7.1% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 160 | 57.1% |
| POP_TOP | 60 | 21.4% |
| STORE_FAST | 60 | 21.4% |


</details>

### UNPACK_SEQUENCE_TWO_TUPLE

<details>
<summary> Successors and predecessors for UNPACK_SEQUENCE_TWO_TUPLE </summary>

|Predecessors | Count | Percentage | 
|---|---:|---:|
| FOR_ITER_LIST | 642,422 | 66.0% |
| STORE_FAST | 329,402 | 33.9% |
| RETURN_VALUE | 480 | 0.0% |
| UNPACK_SEQUENCE | 320 | 0.0% |
| BINARY_SLICE | 200 | 0.0% |

|Successors | Count | Percentage | 
|---|---:|---:|
| STORE_FAST_STORE_FAST | 972,904 | 100.0% |
| STORE_FAST | 100 | 0.0% |
| LOAD_FAST | 60 | 0.0% |


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
|     deferred | 2,121,943 | 61.6% |
|          hit | 1,320,444 | 38.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 480 | 15.8% |
| Failure | 2,560 | 84.2% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| and int | 1,760 | 68.8% |
| or | 600 | 23.4% |
| floor divide | 120 | 4.7% |
| multiply different types | 60 | 2.3% |
| add different types | 20 | 0.8% |


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
|     deferred | 8,460 | 26.1% |
|          hit | 23,559 | 72.8% |
|         miss | 140 | 0.4% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 180 | 50.0% |
| Failure | 180 | 50.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| buffer int | 140 | 77.8% |
| out of range | 20 | 11.1% |
| buffer slice | 20 | 11.1% |


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 8,836,672 | 23.2% |
|          hit | 29,255,567 | 76.8% |
|         miss | 2,820 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 8,380 | 50.9% |
| Failure | 8,080 | 49.1% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| meth descr varargs | 1,960 | 24.3% |
| class no vectorcall | 1,340 | 16.6% |
| code complex parameters | 920 | 11.4% |
| cfunc noargs | 800 | 9.9% |
| meth descr method fastcall keywords | 760 | 9.4% |
| no dict | 640 | 7.9% |
| other | 380 | 4.7% |
| cfunc varargs keywords | 340 | 4.2% |
| meth descr varargs keywords | 260 | 3.2% |
| class mutable | 220 | 2.7% |
| operator wrapper | 140 | 1.7% |
| metaclass | 140 | 1.7% |
| cfunc varargs | 100 | 1.2% |
| wrong number arguments | 40 | 0.5% |
| cmethod | 40 | 0.5% |


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 985,983 | 17.4% |
|          hit | 4,669,411 | 82.5% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 880 | 27.0% |
| Failure | 2,380 | 73.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| baseobject | 1,780 | 74.8% |
| other | 220 | 9.2% |
| tuple | 140 | 5.9% |
| different types | 120 | 5.0% |
| float long | 80 | 3.4% |
| bool | 40 | 1.7% |


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 9,180 | 0.5% |
|          hit | 1,942,426 | 99.5% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 59.4% |
| Failure | 260 | 40.6% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 140 | 53.8% |
| dict items | 80 | 30.8% |
| set | 40 | 15.4% |


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 10,903,290 | 15.0% |
|          hit | 61,783,571 | 85.0% |
|         miss | 3,640 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 15,760 | 49.5% |
| Failure | 16,100 | 50.5% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| has managed dict | 7,720 | 48.0% |
| metaclass attribute | 3,440 | 21.4% |
| not managed dict | 2,620 | 16.3% |
| method | 1,200 | 7.5% |
| shadowed | 720 | 4.5% |
| class method obj | 180 | 1.1% |
| non object slot | 80 | 0.5% |
| class attr descriptor | 60 | 0.4% |
| class attr simple | 40 | 0.2% |
| module attr not found | 20 | 0.1% |
| builtin class method | 20 | 0.1% |


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,160 | 0.1% |
|        deopt | 80 | 0.0% |
|          hit | 10,604,265 | 99.9% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 7,000 | 100.0% |
| Failure | 0 | 0.0% |


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 520 | 9.7% |
|          hit | 4,340 | 81.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 500 | 100.0% |
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
|     deferred | 658,422 | 28.7% |
|          hit | 1,637,725 | 71.3% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 460 | 39.0% |
| Failure | 720 | 61.0% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| other | 720 | 100.0% |


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 13,540 | 0.2% |
|          hit | 6,988,420 | 99.7% |
|         miss | 6,260 | 0.1% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,620 | 87.2% |
| Failure | 680 | 12.8% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| class attr simple | 320 | 47.1% |
| overridden | 80 | 11.8% |
| overriding descriptor | 80 | 11.8% |
| not in dict | 80 | 11.8% |
| no dict | 40 | 5.9% |
| property | 40 | 5.9% |
| not in keys | 40 | 5.9% |


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
|     deferred | 640 | 6.2% |
|          hit | 9,421 | 91.6% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 160 | 72.7% |
| Failure | 60 | 27.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| py simple | 40 | 66.7% |
| bytearray int | 20 | 33.3% |


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 7,513,027 | 23.6% |
|          hit | 24,339,234 | 76.4% |
|         miss | 180 | 0.0% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 4,000 | 45.7% |
| Failure | 4,760 | 54.3% |

|Failure kind | Count | Ratio | 
|---|---:|---:|
| bytes | 2,420 | 50.8% |
| sequence | 1,380 | 29.0% |
| bytearray | 260 | 5.5% |
| mapping | 260 | 5.5% |
| dict | 160 | 3.4% |
| memory view | 140 | 2.9% |
| set | 100 | 2.1% |
| float | 20 | 0.4% |
| tuple | 20 | 0.4% |


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

|Kind | Count | Ratio | 
|---|---:|---:|
|     deferred | 380 | 0.0% |
|          hit | 973,344 | 99.9% |

| | Count | Ratio | 
|---|---:|---:|
| Success | 380 | 100.0% |
| Failure | 0 | 0.0% |


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>

|Instructions | Count | Ratio | 
|---|---:|---:|
| Basic | 228,020,548 | 48.3% |
| Not specialized | 79,060,847 | 16.8% |
| Specialized hits | 164,765,250 | 34.9% |
| Specialized misses | 13,400 | 0.0% |

### Deferred by instruction

<details>
<summary> deferred by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| LOAD_ATTR | 10,903,290 | 35.1% |
| CALL | 8,836,672 | 28.5% |
| TO_BOOL | 7,513,027 | 24.2% |
| BINARY_OP | 2,121,943 | 6.8% |
| COMPARE_OP | 985,983 | 3.2% |
| SEND | 658,422 | 2.1% |
| STORE_ATTR | 13,540 | 0.0% |
| FOR_ITER | 9,180 | 0.0% |
| BINARY_SUBSCR | 8,460 | 0.0% |
| LOAD_GLOBAL | 7,160 | 0.0% |


</details>

### Misses by instruction

<details>
<summary> misses by instruction </summary>

|Name | Count | Ratio | 
|---|---:|---:|
| STORE_ATTR_SLOT | 6,260 | 46.7% |
| LOAD_ATTR_SLOT | 3,000 | 22.4% |
| CALL_METHOD_DESCRIPTOR_NOARGS | 1,420 | 10.6% |
| CALL_METHOD_DESCRIPTOR_O | 540 | 4.0% |
| CALL_PY_EXACT_ARGS | 280 | 2.1% |
| LOAD_ATTR_METHOD_WITH_VALUES | 280 | 2.1% |
| CALL_BOUND_METHOD_EXACT_ARGS | 240 | 1.8% |
| LOAD_ATTR_MODULE | 240 | 1.8% |
| COMPARE_OP_INT | 160 | 1.2% |
| BINARY_SUBSCR_STR_INT | 140 | 1.0% |


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>

| | Count | Ratio | 
|---|---:|---:|
| Calls to PyEval_EvalDefault | 2,345,305 | 10.9% |
| Calls to Python functions inlined | 19,220,520 | 89.1% |
| Calls via PyEval_EvalFrame (total) | 2,345,305 | 10.9% |
| Calls via PyEval_EvalFrame (vector) | 2,015,604 | 9.3% |
| Calls via PyEval_EvalFrame (generator) | 329,701 | 1.5% |
| Calls via PyEval_EvalFrame (legacy) | 40 | 0.0% |
| Calls via PyEval_EvalFrame (function vectorcall) | 2,015,464 | 9.3% |
| Calls via PyEval_EvalFrame (build class) | 100 | 0.0% |
| Calls via PyEval_EvalFrame (slot) | 360 | 0.0% |
| Calls via PyEval_EvalFrame (function ex) | 440 | 0.0% |
| Calls via PyEval_EvalFrame (api) | 1,920 | 0.0% |
| Calls via PyEval_EvalFrame (method) | 659,802 | 3.1% |
| Frame objects created | 643,082 | 3.0% |
| Frames pushed | 18,595,855 | 86.2% |


</details>

## Object stats

<details>
<summary> allocations, frees and dict materializatons </summary>

| | Count | Ratio | 
|---|---:|---:|
| Allocations from freelist | 14,685,265 | 41.2% |
| Frees to freelist | 14,692,666 |  |
| Allocations | 20,964,620 | 58.8% |
| Allocations to 512 bytes | 14,550,842 | 40.8% |
| Allocations to 4 kbytes | 323,159 | 0.9% |
| Allocations over 4 kbytes | 6,090,619 | 17.1% |
| Frees | 21,343,759 |  |
| New values | 1,680 |  |
| Interpreter increfs | 231,004,222 | 76.6% |
| Interpreter decrefs | 255,714,305 | 76.3% |
| Increfs | 70,625,631 | 23.4% |
| Decrefs | 79,377,583 | 23.7% |
| Materialize dict (on request) | 0 | 0.0% |
| Materialize dict (new key) | 160 | 9.5% |
| Materialize dict (too big) | 0 | 0.0% |
| Materialize dict (str subclass) | 0 | 0.0% |
| Dematerialize dict | 0 | 0.0% |
| Method cache hits | 20,352,927 |  |
| Method cache misses | 120,609 |  |
| Method cache collisions | 130,662 |  |
| Method cache dunder hits | 1,036,103 |  |
| Method cache dunder misses | 11,740 |  |


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>

|Generation | Collections | Objects collected | Object visits | 
|---:|---:|---:|---:|
| 0 | 20 | 60 | 68,760 |
| 1 | 0 | 0 | 0 |
| 2 | 0 | 0 | 0 |


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

| | Count | Ratio | 
|---|---:|---:|
| Optimization attempts | 200 |  |
| Traces created | 200 | 100.0% |
| Trace stack overflow | 0 | 0.0% |
| Trace stack underflow | 0 | 0.0% |
| Trace too long | 0 | 0.0% |
| Trace too short | 0 | 0.0% |
| Inner loop found | 0 | 0.0% |
| Recursive call | 0 | 0.0% |
| Low confidence | 0 | 0.0% |
| Traces executed | 7,535,683 |  |
| Uops executed | 148,616,921 | 19.72 |

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
| <= 32 | 60 | 30.0% |
| <= 64 | 40 | 20.0% |
| <= 128 | 40 | 20.0% |
| <= 256 | 60 | 30.0% |


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
| <= 16 | 20 | 10.0% |
| <= 32 | 60 | 30.0% |
| <= 64 | 40 | 20.0% |
| <= 128 | 60 | 30.0% |
| <= 256 | 20 | 10.0% |


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

|Range | Count | Ratio | 
|---|---:|---:|
| <= 1 | 0 | 0.0% |
| <= 2 | 656,782 | 8.7% |
| <= 4 | 321,741 | 4.3% |
| <= 8 | 280 | 0.0% |
| <= 16 | 321,461 | 4.3% |
| <= 32 | 5,531,879 | 73.4% |
| <= 64 | 180 | 0.0% |
| <= 128 | 695,640 | 9.2% |
| <= 256 | 7,600 | 0.1% |
| <= 512 | 0 | 0.0% |
| <= 1,024 | 40 | 0.0% |
| <= 2,048 | 40 | 0.0% |
| <= 4,096 | 0 | 0.0% |
| <= 8,192 | 40 | 0.0% |


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

|Name | Count | Self | Cumulative | Miss ratio | 
|---|---:|---:|---:|---:|
| _SET_IP | 23,812,938 | 16.0% | 16.0% |  |
| _CHECK_VALIDITY | 23,038,918 | 15.5% | 31.5% |  |
| _GUARD_TYPE_VERSION | 16,553,941 | 11.1% | 42.7% |  |
| LOAD_FAST | 16,275,695 | 11.0% | 53.6% |  |
| _EXIT_TRACE | 6,465,342 | 4.4% | 58.0% | 100.0% |
| _LOAD_ATTR | 5,936,678 | 4.0% | 62.0% |  |
| _GUARD_DORV_VALUES_INST_ATTR_FROM_DICT | 5,776,682 | 3.9% | 65.8% |  |
| _GUARD_KEYS_VERSION | 5,776,682 | 3.9% | 69.7% |  |
| _LOAD_ATTR_METHOD_WITH_VALUES | 5,776,682 | 3.9% | 73.6% |  |
| _CHECK_ATTR_WITH_HINT | 5,142,480 | 3.5% | 77.1% |  |
| _LOAD_ATTR_WITH_HINT | 5,142,480 | 3.5% | 80.5% |  |
| _LOAD_ATTR_SLOT | 2,782,540 | 1.9% | 82.4% |  |
| STORE_FAST | 1,793,632 | 1.2% | 83.6% |  |
| _LOAD_ATTR_METHOD_NO_DICT | 1,445,079 | 1.0% | 84.6% |  |
| _GUARD_IS_FALSE_POP | 1,444,519 | 1.0% | 85.6% | 3.2% |
| _CHECK_MANAGED_OBJECT_HAS_VALUES | 1,407,120 | 0.9% | 86.5% |  |
| _LOAD_ATTR_INSTANCE_VALUE | 1,407,120 | 0.9% | 87.5% |  |
| TO_BOOL_BOOL | 1,399,000 | 0.9% | 88.4% |  |
| _CHECK_FUNCTION_EXACT_ARGS | 1,360,402 | 0.9% | 89.3% |  |
| _CHECK_STACK_SPACE | 1,360,402 | 0.9% | 90.2% |  |
| _INIT_CALL_PY_EXACT_ARGS | 1,360,402 | 0.9% | 91.1% |  |
| _PUSH_FRAME | 1,360,402 | 0.9% | 92.1% |  |
| _SAVE_RETURN_OFFSET | 1,360,402 | 0.9% | 93.0% |  |
| _GUARD_NOT_EXHAUSTED_RANGE | 1,036,381 | 0.7% | 93.7% | 31.0% |
| _ITER_CHECK_RANGE | 1,036,381 | 0.7% | 94.4% |  |
| _GUARD_NOT_EXHAUSTED_LIST | 733,100 | 0.5% | 94.9% | 87.5% |
| _ITER_CHECK_LIST | 733,100 | 0.5% | 95.4% |  |
| RESUME_CHECK | 718,580 | 0.5% | 95.8% |  |
| _ITER_NEXT_RANGE | 714,600 | 0.5% | 96.3% |  |
| PUSH_NULL | 696,940 | 0.5% | 96.8% |  |
| CALL_METHOD_DESCRIPTOR_NOARGS | 695,680 | 0.5% | 97.3% |  |
| BUILD_LIST | 695,620 | 0.5% | 97.7% |  |
| CALL_INTRINSIC_1 | 695,620 | 0.5% | 98.2% |  |
| LIST_EXTEND | 695,620 | 0.5% | 98.7% |  |
| _CHECK_GLOBALS | 427,759 | 0.3% | 99.0% |  |
| _LOAD_CONST_INLINE | 388,620 | 0.3% | 99.2% |  |
| UNPACK_SEQUENCE_TWO_TUPLE | 136,817 | 0.1% | 99.3% |  |
| _GUARD_IS_TRUE_POP | 117,038 | 0.1% | 99.4% | 38.9% |
| _BINARY_OP | 100,898 | 0.1% | 99.5% |  |
| _ITER_NEXT_LIST | 91,658 | 0.1% | 99.5% |  |
| TO_BOOL_INT | 90,898 | 0.1% | 99.6% |  |
| _LOAD_CONST_INLINE_BORROW | 90,619 | 0.1% | 99.6% |  |
| COPY | 53,059 | 0.0% | 99.7% |  |
| _TO_BOOL | 53,059 | 0.0% | 99.7% |  |
| SWAP | 53,039 | 0.0% | 99.7% |  |
| CALL_METHOD_DESCRIPTOR_FAST | 46,099 | 0.0% | 99.8% |  |
| _CHECK_ATTR_MODULE | 45,439 | 0.0% | 99.8% |  |
| _LOAD_ATTR_MODULE | 45,439 | 0.0% | 99.8% |  |
| BUILD_TUPLE | 22,800 | 0.0% | 99.9% |  |
| _GUARD_BOTH_INT | 18,940 | 0.0% | 99.9% |  |
| _BINARY_OP_ADD_INT | 17,700 | 0.0% | 99.9% |  |
| CONTAINS_OP | 17,680 | 0.0% | 99.9% |  |
| _GUARD_NOT_EXHAUSTED_TUPLE | 16,500 | 0.0% | 99.9% | 50.1% |
| _ITER_CHECK_TUPLE | 16,500 | 0.0% | 99.9% |  |
| _LOAD_CONST_INLINE_WITH_NULL | 15,840 | 0.0% | 99.9% |  |
| _CHECK_BUILTINS | 15,300 | 0.0% | 99.9% |  |
| _JUMP_TO_TOP | 11,960 | 0.0% | 99.9% |  |
| BINARY_SLICE | 11,320 | 0.0% | 99.9% |  |
| _STORE_SUBSCR | 10,120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_DICT | 10,000 | 0.0% | 100.0% |  |
| _ITER_NEXT_TUPLE | 8,240 | 0.0% | 100.0% |  |
| CALL_ISINSTANCE | 7,700 | 0.0% | 100.0% |  |
| _FOR_ITER_TIER_TWO | 7,680 | 0.0% | 100.0% | 100.0% |
| POP_TOP | 7,620 | 0.0% | 100.0% |  |
| GET_ITER | 7,600 | 0.0% | 100.0% |  |
| CALL_LEN | 7,600 | 0.0% | 100.0% |  |
| CALL_METHOD_DESCRIPTOR_O | 7,600 | 0.0% | 100.0% |  |
| LIST_APPEND | 1,880 | 0.0% | 100.0% |  |
| CALL_BUILTIN_CLASS | 1,240 | 0.0% | 100.0% |  |
| _BINARY_OP_SUBTRACT_INT | 1,240 | 0.0% | 100.0% |  |
| TO_BOOL_STR | 640 | 0.0% | 100.0% |  |
| _GUARD_BOTH_UNICODE | 360 | 0.0% | 100.0% |  |
| _BINARY_OP_ADD_UNICODE | 360 | 0.0% | 100.0% |  |
| _CHECK_CALL_BOUND_METHOD_EXACT_ARGS | 180 | 0.0% | 100.0% |  |
| _INIT_CALL_BOUND_METHOD_EXACT_ARGS | 180 | 0.0% | 100.0% |  |
| IS_OP | 120 | 0.0% | 100.0% |  |
| TO_BOOL_NONE | 120 | 0.0% | 100.0% |  |
| BINARY_SUBSCR_STR_INT | 100 | 0.0% | 100.0% | 80.0% |
| _GUARD_IS_NOT_NONE_POP | 40 | 0.0% | 100.0% | 50.0% |
| COMPARE_OP_STR | 40 | 0.0% | 100.0% |  |
| _POP_FRAME | 40 | 0.0% | 100.0% |  |
| _GUARD_DORV_VALUES | 40 | 0.0% | 100.0% |  |
| _STORE_ATTR_INSTANCE_VALUE | 40 | 0.0% | 100.0% |  |


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

|Opcode | Count | 
|---|---:|
| STORE_ATTR_WITH_HINT | 40 |
| RETURN_GENERATOR | 20 |
| CALL | 20 |
| CALL_FUNCTION_EX | 20 |
| CALL_LIST_APPEND | 20 |
| CALL_PY_WITH_DEFAULTS | 20 |


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

|Event | Count | 
|---|---:|
| set_class | 0 |
| set_bases | 0 |
| set_eval_frame_func | 0 |
| builtin_dict | 0 |
| func_modification | 0 |


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

| | Count | 
|---|---:|
| Number of data files | 20 |


</details>

---
Stats gathered on: 2024-02-07
