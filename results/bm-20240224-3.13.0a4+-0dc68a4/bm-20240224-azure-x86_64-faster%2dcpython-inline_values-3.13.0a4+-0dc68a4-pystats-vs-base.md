## Execution counts

<details>
<summary> Execution counts for Tier 1 instructions. </summary>


The "miss ratio" column shows the percentage of times the instruction
executed that it deoptimized. When this happens, the base unspecialized
instruction is not counted.

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">235,853,331</td>
<td align="right">206,324,272</td>
<td align="right">-12.5%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">67,295,489</td>
<td align="right">71,855,938</td>
<td align="right">6.8%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">91,209,872</td>
<td align="right">96,717,279</td>
<td align="right">6.0%</td>
</tr>
<tr>
<td align="left">WITH_EXCEPT_START</td>
<td align="right">5,880</td>
<td align="right">5,560</td>
<td align="right">-5.4%</td>
</tr>
<tr>
<td align="left">UNARY_INVERT</td>
<td align="right">15,058,917</td>
<td align="right">14,311,699</td>
<td align="right">-5.0%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">6,925,097</td>
<td align="right">6,638,918</td>
<td align="right">-4.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,663,075,219</td>
<td align="right">1,691,503,751</td>
<td align="right">1.7%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">11,198,876</td>
<td align="right">11,059,531</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">2,813,366,920</td>
<td align="right">2,791,426,699</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">338,531,900</td>
<td align="right">336,186,509</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">5,307,042</td>
<td align="right">5,272,558</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">122,906,649</td>
<td align="right">122,157,653</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">208,315,772</td>
<td align="right">207,278,383</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">89,078,801</td>
<td align="right">88,650,508</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,205,467,382</td>
<td align="right">1,199,741,128</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">80,015,272</td>
<td align="right">79,693,329</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">197,229,105</td>
<td align="right">196,583,477</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">101,761,373</td>
<td align="right">102,027,645</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,171,748,179</td>
<td align="right">1,168,748,639</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">112,610,060</td>
<td align="right">112,351,480</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">1,391,933,119</td>
<td align="right">1,388,800,953</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">350,798,506</td>
<td align="right">350,021,328</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">268,841,803</td>
<td align="right">268,301,965</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">602,453,472</td>
<td align="right">601,250,326</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">741,329,839</td>
<td align="right">739,910,876</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">116,051,632</td>
<td align="right">115,838,888</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">222,711,402</td>
<td align="right">222,358,657</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">234,899,105</td>
<td align="right">234,529,512</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">443,972,903</td>
<td align="right">443,329,487</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">4,451,407,802</td>
<td align="right">4,445,053,145</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">2,030,883,382</td>
<td align="right">2,028,019,353</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">249,619,249</td>
<td align="right">249,283,929</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">2,078,376,054</td>
<td align="right">2,075,664,874</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">178,106,833</td>
<td align="right">177,887,960</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">4,091,466,872</td>
<td align="right">4,086,445,456</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,603,096,783</td>
<td align="right">4,597,625,840</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">90,302,043</td>
<td align="right">90,195,106</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">27,981,108</td>
<td align="right">27,948,341</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">4,197,716,072</td>
<td align="right">4,193,027,204</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">1,811,949,024</td>
<td align="right">1,809,982,882</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">7,937,510,553</td>
<td align="right">7,929,002,513</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">515,424,297</td>
<td align="right">514,886,935</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">843,957,405</td>
<td align="right">843,175,400</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">429,830,674</td>
<td align="right">429,463,128</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,075,621,381</td>
<td align="right">2,073,964,789</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,113,886</td>
<td align="right">6,109,089</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">1,780,277,588</td>
<td align="right">1,778,892,119</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">640,241,784</td>
<td align="right">639,753,148</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">310,221</td>
<td align="right">310,449</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">993,229,028</td>
<td align="right">992,507,470</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">42,756,678,884</td>
<td align="right">42,727,378,038</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">455,253,682</td>
<td align="right">454,945,267</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">6,064,850,105</td>
<td align="right">6,068,903,127</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">22,162,747</td>
<td align="right">22,148,300</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">22,162,887</td>
<td align="right">22,148,440</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">21,672,294</td>
<td align="right">21,658,303</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,878,914,719</td>
<td align="right">1,877,779,401</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">175,496,759</td>
<td align="right">175,392,957</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">427,571,692</td>
<td align="right">427,328,144</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">1,570,121,721</td>
<td align="right">1,569,229,241</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">2,149,286,284</td>
<td align="right">2,148,078,300</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">1,304,719,823</td>
<td align="right">1,304,005,378</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">238,862,514</td>
<td align="right">238,732,209</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">5,729,059,818</td>
<td align="right">5,725,988,153</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">494,475,707</td>
<td align="right">494,230,524</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">14,508,834,528</td>
<td align="right">14,501,667,968</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">385,919,344</td>
<td align="right">385,728,944</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">12,368,447,337</td>
<td align="right">12,362,400,228</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">1,091,598,339</td>
<td align="right">1,091,066,027</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">252,306,647</td>
<td align="right">252,189,666</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">1,151,293,878</td>
<td align="right">1,150,791,503</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">11,474,243,138</td>
<td align="right">11,469,319,519</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RERAISE</td>
<td align="right">2,256,803</td>
<td align="right">2,255,843</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">4,920,668,979</td>
<td align="right">4,918,620,143</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">839,113,501</td>
<td align="right">838,789,957</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">501,919,145</td>
<td align="right">502,112,359</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">4,873,473,954</td>
<td align="right">4,871,608,623</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">2,105,832,245</td>
<td align="right">2,106,612,198</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">1,779,373</td>
<td align="right">1,780,030</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">2,204,978,887</td>
<td align="right">2,204,195,687</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">407,190,310</td>
<td align="right">407,049,958</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">335,672,862</td>
<td align="right">335,565,497</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">244,492</td>
<td align="right">244,568</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">127,408,823</td>
<td align="right">127,370,517</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">9,626,421</td>
<td align="right">9,623,810</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">263,878,611</td>
<td align="right">263,811,905</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">459,256,435</td>
<td align="right">459,149,038</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">177,956,542</td>
<td align="right">177,915,293</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">10,275,026</td>
<td align="right">10,272,660</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">929,034,747</td>
<td align="right">928,824,035</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">14,451,584,640</td>
<td align="right">14,448,393,826</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">2,676,498,932</td>
<td align="right">2,675,969,155</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">16,544</td>
<td align="right">16,547</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">818,932,907</td>
<td align="right">819,076,543</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">665,788,767</td>
<td align="right">665,681,238</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">1,118,566</td>
<td align="right">1,118,746</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">828,021,261</td>
<td align="right">827,903,496</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">1,498,052,709</td>
<td align="right">1,497,841,546</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,385,804,981</td>
<td align="right">1,385,627,652</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">8,620,277</td>
<td align="right">8,619,317</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">767,153,027</td>
<td align="right">767,087,805</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">2,120,686,631</td>
<td align="right">2,120,508,678</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">471,185,306</td>
<td align="right">471,148,888</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">3,554,740,317</td>
<td align="right">3,554,466,019</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">1,518,507,937</td>
<td align="right">1,518,623,043</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">35,048,504</td>
<td align="right">35,046,036</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">93,445,192</td>
<td align="right">93,440,812</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">95,727,494</td>
<td align="right">95,723,114</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">5,731,607</td>
<td align="right">5,731,347</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">96,589,452</td>
<td align="right">96,585,150</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">76,904,888</td>
<td align="right">76,902,008</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">127,855,214</td>
<td align="right">127,859,770</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">97,768,067</td>
<td align="right">97,764,649</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">154,799,323</td>
<td align="right">154,794,523</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">591,366,692</td>
<td align="right">591,348,712</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">139,472,686</td>
<td align="right">139,468,846</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">550,875,540</td>
<td align="right">550,861,262</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">635,385,722</td>
<td align="right">635,371,031</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,607,308,080</td>
<td align="right">1,607,273,950</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">176,305,447</td>
<td align="right">176,302,249</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,398,510</td>
<td align="right">20,398,868</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">1,257,285,042</td>
<td align="right">1,257,266,644</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">96,882,516</td>
<td align="right">96,881,236</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">59,536,039</td>
<td align="right">59,536,794</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">151,079,919</td>
<td align="right">151,081,764</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">2,416,463,121</td>
<td align="right">2,416,435,583</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">1,382,309,140</td>
<td align="right">1,382,293,775</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">3,155,402,214</td>
<td align="right">3,155,367,775</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">363,159,232</td>
<td align="right">363,155,419</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">1,674,318,364</td>
<td align="right">1,674,303,004</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">485,070,925</td>
<td align="right">485,075,329</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">76,203,255</td>
<td align="right">76,202,590</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">178,814,636</td>
<td align="right">178,813,305</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">818,374,133</td>
<td align="right">818,368,420</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">109,427,934</td>
<td align="right">109,427,294</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">443,623,803</td>
<td align="right">443,621,672</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">344,329,673</td>
<td align="right">344,328,090</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">585,024,240</td>
<td align="right">585,021,936</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">240,174,340</td>
<td align="right">240,175,066</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">249,369,255</td>
<td align="right">249,368,606</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">12,004,593</td>
<td align="right">12,004,563</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">284,442,988</td>
<td align="right">284,442,316</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">480,179,075</td>
<td align="right">480,179,869</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">36,720,299</td>
<td align="right">36,720,347</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">170,944,133</td>
<td align="right">170,944,279</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">779,600,123</td>
<td align="right">779,599,710</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">360,729,982</td>
<td align="right">360,730,147</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">193,735,909</td>
<td align="right">193,735,929</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">351,453,292</td>
<td align="right">351,453,321</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">65,805,648</td>
<td align="right">65,805,650</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">211,724,785</td>
<td align="right">211,724,791</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,269,608</td>
<td align="right">229,269,614</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">164,809,252</td>
<td align="right">164,809,256</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">391,471,923</td>
<td align="right">391,471,929</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">162,423,035</td>
<td align="right">162,423,035</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_ANEXT</td>
<td align="right">133,515,680</td>
<td align="right">133,515,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">98,816,261</td>
<td align="right">98,816,261</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RESUME</td>
<td align="right">38,846,240</td>
<td align="right">38,846,240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_FALSE</td>
<td align="right">38,846,080</td>
<td align="right">38,846,080</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_VALUE</td>
<td align="right">38,845,680</td>
<td align="right">38,845,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_NAME</td>
<td align="right">14,039,527</td>
<td align="right">14,039,527</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_GLOBAL</td>
<td align="right">8,204,540</td>
<td align="right">8,204,540</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_ASYNC_FOR</td>
<td align="right">8,000,000</td>
<td align="right">8,000,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AITER</td>
<td align="right">8,000,000</td>
<td align="right">8,000,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BEFORE_ASYNC_WITH</td>
<td align="right">2,995,200</td>
<td align="right">2,995,200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">2,172,606</td>
<td align="right">2,172,606</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_EX</td>
<td align="right">1,041,926</td>
<td align="right">1,041,926</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">965,696</td>
<td align="right">965,696</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">28,680</td>
<td align="right">28,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_BUILD_CLASS</td>
<td align="right">18,886</td>
<td align="right">18,886</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_LOCALS</td>
<td align="right">2,260</td>
<td align="right">2,260</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FROM_DICT_OR_DEREF</td>
<td align="right">2,240</td>
<td align="right">2,240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">1,440</td>
<td align="right">1,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_NAME</td>
<td align="right">900</td>
<td align="right">900</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">648</td>
<td align="right">648</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">640</td>
<td align="right">640</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">400</td>
<td align="right">400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_CONST</td>
<td align="right">240</td>
<td align="right">240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">240</td>
<td align="right">240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">160</td>
<td align="right">160</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SETUP_ANNOTATIONS</td>
<td align="right">84</td>
<td align="right">84</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_2</td>
<td align="right">80</td>
<td align="right">80</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NOT_NONE</td>
<td align="right">80</td>
<td align="right">80</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

## Pair counts

<details>
<summary> Pair counts for top 100 Tier 1 instructions </summary>


Pairs of specialized operations that deoptimize and are then followed by
the corresponding unspecialized instruction are not counted as pairs.

Not included in comparative output.


</details>

## Predecessor/Successor Pairs

<details>
<summary> Top 5 predecessors and successors of each Tier 1 opcode. </summary>


This does not include the unspecialized instructions that occur after a
specialized instruction deoptimizes.

Not included in comparative output.


</details>

## Specialization stats

<details>
<summary> Specialization stats by family </summary>

### BINARY_OP

<details>
<summary> specialization stats for BINARY_OP family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,439,641,821</td>
<td align="right">17.2%</td>
<td align="right">1,436,510,289</td>
<td align="right">17.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,906,605,807</td>
<td align="right">82.7%</td>
<td align="right">6,906,221,237</td>
<td align="right">82.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">50,404,785</td>
<td align="right">0.6%</td>
<td align="right">50,404,785</td>
<td align="right">0.6%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">1,701,064</td>
<td align="right">63.1%</td>
<td align="right">1,700,304</td>
<td align="right">63.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">995,019</td>
<td align="right">36.9%</td>
<td align="right">995,145</td>
<td align="right">36.9%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">or</td>
<td align="right">16,671</td>
<td align="right">1.0%</td>
<td align="right">16,394</td>
<td align="right">1.0%</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">and int</td>
<td align="right">70,106</td>
<td align="right">4.1%</td>
<td align="right">69,663</td>
<td align="right">4.1%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">power</td>
<td align="right">13,481</td>
<td align="right">0.8%</td>
<td align="right">13,509</td>
<td align="right">0.8%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">1,633</td>
<td align="right">0.1%</td>
<td align="right">1,635</td>
<td align="right">0.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">66,385</td>
<td align="right">3.9%</td>
<td align="right">66,337</td>
<td align="right">3.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">68,848</td>
<td align="right">4.0%</td>
<td align="right">68,825</td>
<td align="right">4.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">52,252</td>
<td align="right">3.1%</td>
<td align="right">52,268</td>
<td align="right">3.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">17,763</td>
<td align="right">1.0%</td>
<td align="right">17,767</td>
<td align="right">1.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">215,655</td>
<td align="right">12.7%</td>
<td align="right">215,612</td>
<td align="right">12.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">27,703</td>
<td align="right">1.6%</td>
<td align="right">27,707</td>
<td align="right">1.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">29,103</td>
<td align="right">1.7%</td>
<td align="right">29,107</td>
<td align="right">1.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">37,147</td>
<td align="right">2.2%</td>
<td align="right">37,152</td>
<td align="right">2.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">lshift</td>
<td align="right">29,167</td>
<td align="right">1.7%</td>
<td align="right">29,169</td>
<td align="right">1.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">251,235</td>
<td align="right">14.8%</td>
<td align="right">251,238</td>
<td align="right">14.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">778,882</td>
<td align="right">45.8%</td>
<td align="right">778,888</td>
<td align="right">45.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">15,954</td>
<td align="right">0.9%</td>
<td align="right">15,954</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,500</td>
<td align="right">0.3%</td>
<td align="right">5,500</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,060</td>
<td align="right">0.2%</td>
<td align="right">3,060</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and different types</td>
<td align="right">519</td>
<td align="right">0.0%</td>
<td align="right">519</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### BINARY_SLICE

<details>
<summary> specialization stats for BINARY_SLICE family </summary>


</details>

### BINARY_SUBSCR

<details>
<summary> specialization stats for BINARY_SUBSCR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,522,681,570</td>
<td align="right">25.1%</td>
<td align="right">1,522,796,682</td>
<td align="right">25.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">4,542,835,067</td>
<td align="right">74.9%</td>
<td align="right">4,542,599,011</td>
<td align="right">74.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">4,805,280</td>
<td align="right">0.1%</td>
<td align="right">4,805,307</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">185,238</td>
<td align="right">29.3%</td>
<td align="right">185,257</td>
<td align="right">29.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">446,409</td>
<td align="right">70.7%</td>
<td align="right">446,411</td>
<td align="right">70.7%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">tuple slice</td>
<td align="right">83</td>
<td align="right">0.0%</td>
<td align="right">87</td>
<td align="right">0.0%</td>
<td align="right">4.8%</td>
</tr>
<tr>
<td align="left">buffer int</td>
<td align="right">46,063</td>
<td align="right">10.3%</td>
<td align="right">46,023</td>
<td align="right">10.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">118,158</td>
<td align="right">26.5%</td>
<td align="right">118,196</td>
<td align="right">26.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">157,600</td>
<td align="right">35.3%</td>
<td align="right">157,600</td>
<td align="right">35.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">80,809</td>
<td align="right">18.1%</td>
<td align="right">80,809</td>
<td align="right">18.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list slice</td>
<td align="right">34,620</td>
<td align="right">7.8%</td>
<td align="right">34,620</td>
<td align="right">7.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,280</td>
<td align="right">1.0%</td>
<td align="right">4,280</td>
<td align="right">1.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">3,736</td>
<td align="right">0.8%</td>
<td align="right">3,736</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">buffer slice</td>
<td align="right">960</td>
<td align="right">0.2%</td>
<td align="right">960</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string slice</td>
<td align="right">100</td>
<td align="right">0.0%</td>
<td align="right">100</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### CALL

<details>
<summary> specialization stats for CALL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,414,986,214</td>
<td align="right">10.8%</td>
<td align="right">1,412,197,556</td>
<td align="right">10.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">249,215,227</td>
<td align="right">1.9%</td>
<td align="right">249,427,683</td>
<td align="right">1.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">11,723,819,650</td>
<td align="right">89.2%</td>
<td align="right">11,714,325,300</td>
<td align="right">89.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">31,040</td>
<td align="right">0.0%</td>
<td align="right">31,040</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">813,923</td>
<td align="right">13.6%</td>
<td align="right">811,518</td>
<td align="right">13.6%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">5,163,269</td>
<td align="right">86.4%</td>
<td align="right">5,167,248</td>
<td align="right">86.4%</td>
<td align="right">0.1%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">8,034</td>
<td align="right">1.0%</td>
<td align="right">7,793</td>
<td align="right">1.0%</td>
<td align="right">-3.0%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">14,399</td>
<td align="right">1.8%</td>
<td align="right">14,192</td>
<td align="right">1.7%</td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left">operator wrapper</td>
<td align="right">5,414</td>
<td align="right">0.7%</td>
<td align="right">5,352</td>
<td align="right">0.7%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">53,150</td>
<td align="right">6.5%</td>
<td align="right">52,568</td>
<td align="right">6.5%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">7,947</td>
<td align="right">1.0%</td>
<td align="right">7,867</td>
<td align="right">1.0%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">20,335</td>
<td align="right">2.5%</td>
<td align="right">20,167</td>
<td align="right">2.5%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">10,634</td>
<td align="right">1.3%</td>
<td align="right">10,558</td>
<td align="right">1.3%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">metaclass</td>
<td align="right">36,139</td>
<td align="right">4.4%</td>
<td align="right">35,913</td>
<td align="right">4.4%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">cfunc varargs keywords</td>
<td align="right">25,349</td>
<td align="right">3.1%</td>
<td align="right">25,201</td>
<td align="right">3.1%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">57,518</td>
<td align="right">7.1%</td>
<td align="right">57,258</td>
<td align="right">7.1%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">7,691</td>
<td align="right">0.9%</td>
<td align="right">7,658</td>
<td align="right">0.9%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">142,110</td>
<td align="right">17.5%</td>
<td align="right">141,501</td>
<td align="right">17.4%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">33,537</td>
<td align="right">4.1%</td>
<td align="right">33,453</td>
<td align="right">4.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">196,015</td>
<td align="right">24.1%</td>
<td align="right">195,955</td>
<td align="right">24.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">52,891</td>
<td align="right">6.5%</td>
<td align="right">52,901</td>
<td align="right">6.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">100,936</td>
<td align="right">12.4%</td>
<td align="right"></td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,326</td>
<td align="right">2.0%</td>
<td align="right">16,326</td>
<td align="right">2.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">cmethod</td>
<td align="right">12,880</td>
<td align="right">1.6%</td>
<td align="right">12,880</td>
<td align="right">1.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not simple</td>
<td align="right">9,778</td>
<td align="right">1.2%</td>
<td align="right">9,778</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">2,840</td>
<td align="right">0.3%</td>
<td align="right">2,840</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">120</td>
<td align="right">0.0%</td>
<td align="right">120</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not inline values</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">101,357</td>
<td align="right">12.5%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### COMPARE_OP

<details>
<summary> specialization stats for COMPARE_OP family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,903,912</td>
<td align="right">0.0%</td>
<td align="right">1,874,977</td>
<td align="right">0.0%</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">240,432,633</td>
<td align="right">5.1%</td>
<td align="right">240,275,349</td>
<td align="right">5.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">4,517,438,258</td>
<td align="right">94.9%</td>
<td align="right">4,516,080,607</td>
<td align="right">94.9%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">240,119</td>
<td align="right">71.9%</td>
<td align="right">238,685</td>
<td align="right">71.9%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">93,674</td>
<td align="right">28.1%</td>
<td align="right">93,152</td>
<td align="right">28.1%</td>
<td align="right">-0.6%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">big int</td>
<td align="right">62,031</td>
<td align="right">25.8%</td>
<td align="right">60,682</td>
<td align="right">25.4%</td>
<td align="right">-2.2%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">19,086</td>
<td align="right">7.9%</td>
<td align="right">19,025</td>
<td align="right">8.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">5,162</td>
<td align="right">2.1%</td>
<td align="right">5,172</td>
<td align="right">2.2%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">23,854</td>
<td align="right">9.9%</td>
<td align="right">23,888</td>
<td align="right">10.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">14,664</td>
<td align="right">6.1%</td>
<td align="right">14,644</td>
<td align="right">6.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">52,339</td>
<td align="right">21.8%</td>
<td align="right">52,291</td>
<td align="right">21.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">34,346</td>
<td align="right">14.3%</td>
<td align="right">34,346</td>
<td align="right">14.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">10,600</td>
<td align="right">4.4%</td>
<td align="right">10,600</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">9,843</td>
<td align="right">4.1%</td>
<td align="right">9,843</td>
<td align="right">4.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">4,340</td>
<td align="right">1.8%</td>
<td align="right">4,340</td>
<td align="right">1.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,274</td>
<td align="right">1.4%</td>
<td align="right">3,274</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">580</td>
<td align="right">0.2%</td>
<td align="right">580</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### FOR_ITER

<details>
<summary> specialization stats for FOR_ITER family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">3,290,005,438</td>
<td align="right">82.9%</td>
<td align="right">3,287,331,412</td>
<td align="right">82.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">673,413,333</td>
<td align="right">17.0%</td>
<td align="right">673,618,362</td>
<td align="right">17.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">175,135,181</td>
<td align="right">4.4%</td>
<td align="right">175,148,796</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">288,808</td>
<td align="right">7.9%</td>
<td align="right">290,316</td>
<td align="right">8.0%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">3,352,185</td>
<td align="right">92.1%</td>
<td align="right">3,352,477</td>
<td align="right">92.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">callable</td>
<td align="right">522</td>
<td align="right">0.2%</td>
<td align="right">502</td>
<td align="right">0.2%</td>
<td align="right">-3.8%</td>
</tr>
<tr>
<td align="left">dict items</td>
<td align="right">106,650</td>
<td align="right">36.9%</td>
<td align="right">108,192</td>
<td align="right">37.3%</td>
<td align="right">1.4%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">6,708</td>
<td align="right">2.3%</td>
<td align="right">6,688</td>
<td align="right">2.3%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">27,333</td>
<td align="right">9.5%</td>
<td align="right">27,374</td>
<td align="right">9.4%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">19,660</td>
<td align="right">6.8%</td>
<td align="right">19,640</td>
<td align="right">6.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">43,308</td>
<td align="right">15.0%</td>
<td align="right">43,293</td>
<td align="right">14.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">seq iter</td>
<td align="right">29,760</td>
<td align="right">10.3%</td>
<td align="right">29,760</td>
<td align="right">10.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">19,304</td>
<td align="right">6.7%</td>
<td align="right">19,304</td>
<td align="right">6.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">12,310</td>
<td align="right">4.3%</td>
<td align="right">12,310</td>
<td align="right">4.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">8,072</td>
<td align="right">2.8%</td>
<td align="right">8,072</td>
<td align="right">2.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">8,021</td>
<td align="right">2.8%</td>
<td align="right">8,021</td>
<td align="right">2.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">5,700</td>
<td align="right">2.0%</td>
<td align="right">5,700</td>
<td align="right">2.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,000</td>
<td align="right">0.3%</td>
<td align="right">1,000</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">440</td>
<td align="right">0.2%</td>
<td align="right">440</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### LOAD_ATTR

<details>
<summary> specialization stats for LOAD_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,460,249</td>
<td align="right">0.0%</td>
<td align="right">2,029</td>
<td align="right">0.0%</td>
<td align="right">-99.9%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">855,373,274</td>
<td align="right">5.1%</td>
<td align="right">948,467,382</td>
<td align="right">5.7%</td>
<td align="right">10.9%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">2,500,576,447</td>
<td align="right">14.9%</td>
<td align="right">2,619,050,504</td>
<td align="right">15.6%</td>
<td align="right">4.7%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">14,271,024,200</td>
<td align="right">85.0%</td>
<td align="right">14,135,123,692</td>
<td align="right">84.3%</td>
<td align="right">-1.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">1,094,947</td>
<td align="right">6.1%</td>
<td align="right">2,389,217</td>
<td align="right">11.4%</td>
<td align="right">118.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">16,777,099</td>
<td align="right">93.9%</td>
<td align="right">18,531,412</td>
<td align="right">88.6%</td>
<td align="right">10.5%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">has managed dict</td>
<td align="right">300,331</td>
<td align="right">27.4%</td>
<td align="right">1,560,912</td>
<td align="right">65.3%</td>
<td align="right">419.7%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">98,021</td>
<td align="right">9.0%</td>
<td align="right">114,374</td>
<td align="right">4.8%</td>
<td align="right">16.7%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,180</td>
<td align="right">0.7%</td>
<td align="right">6,880</td>
<td align="right">0.3%</td>
<td align="right">-4.2%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">132,586</td>
<td align="right">12.1%</td>
<td align="right">129,125</td>
<td align="right">5.4%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">non overriding descriptor</td>
<td align="right">10,456</td>
<td align="right">1.0%</td>
<td align="right">10,288</td>
<td align="right">0.4%</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">non object slot</td>
<td align="right">2,760</td>
<td align="right">0.3%</td>
<td align="right">2,720</td>
<td align="right">0.1%</td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">6,076</td>
<td align="right">0.6%</td>
<td align="right">6,025</td>
<td align="right">0.3%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">15,360</td>
<td align="right">1.4%</td>
<td align="right">15,260</td>
<td align="right">0.6%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">23,643</td>
<td align="right">2.2%</td>
<td align="right">23,563</td>
<td align="right">1.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">143,808</td>
<td align="right">13.1%</td>
<td align="right">143,496</td>
<td align="right">6.0%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">18,763</td>
<td align="right">1.7%</td>
<td align="right">18,754</td>
<td align="right">0.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">metaclass attribute</td>
<td align="right">254,982</td>
<td align="right">23.3%</td>
<td align="right">254,943</td>
<td align="right">10.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">67,424</td>
<td align="right">6.2%</td>
<td align="right">67,416</td>
<td align="right">2.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">8,382</td>
<td align="right">0.8%</td>
<td align="right">8,382</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">2,817</td>
<td align="right">0.3%</td>
<td align="right">2,817</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">2,358</td>
<td align="right">0.2%</td>
<td align="right">2,358</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">non string or split</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">21,604</td>
<td align="right">0.9%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">300</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### LOAD_GLOBAL

<details>
<summary> specialization stats for LOAD_GLOBAL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">303,543</td>
<td align="right">0.0%</td>
<td align="right">299,861</td>
<td align="right">0.0%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">10,180,164,077</td>
<td align="right">99.8%</td>
<td align="right">10,170,741,437</td>
<td align="right">99.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">20,211,652</td>
<td align="right">0.2%</td>
<td align="right">20,208,280</td>
<td align="right">0.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">8,322</td>
<td align="right">0.0%</td>
<td align="right">8,322</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">490,401</td>
<td align="right">100.0%</td>
<td align="right">490,449</td>
<td align="right">100.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### LOAD_SUPER_ATTR

<details>
<summary> specialization stats for LOAD_SUPER_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">128,213,691</td>
<td align="right">100.0%</td>
<td align="right">127,430,211</td>
<td align="right">100.0%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">8,367</td>
<td align="right">0.0%</td>
<td align="right">8,370</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">8,177</td>
<td align="right">100.0%</td>
<td align="right">8,177</td>
<td align="right">100.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


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

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">779,569,463</td>
<td align="right">82.5%</td>
<td align="right">779,569,050</td>
<td align="right">82.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">164,784,832</td>
<td align="right">17.4%</td>
<td align="right">164,784,836</td>
<td align="right">17.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">30,660</td>
<td align="right">0.0%</td>
<td align="right">30,660</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">4,620</td>
<td align="right">8.4%</td>
<td align="right">4,620</td>
<td align="right">8.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">50,460</td>
<td align="right">91.6%</td>
<td align="right">50,460</td>
<td align="right">91.6%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">65.8%</td>
<td align="right">33,180</td>
<td align="right">65.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">14,020</td>
<td align="right">27.8%</td>
<td align="right">14,020</td>
<td align="right">27.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,260</td>
<td align="right">6.5%</td>
<td align="right">3,260</td>
<td align="right">6.5%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### STORE_ATTR

<details>
<summary> specialization stats for STORE_ATTR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">269,887,185</td>
<td align="right">9.2%</td>
<td align="right">275,051,809</td>
<td align="right">9.3%</td>
<td align="right">1.9%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">206,693,383</td>
<td align="right">7.0%</td>
<td align="right">207,319,335</td>
<td align="right">7.0%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,671,887,727</td>
<td align="right">90.7%</td>
<td align="right">2,665,501,393</td>
<td align="right">90.5%</td>
<td align="right">-0.2%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">89,838</td>
<td align="right">2.2%</td>
<td align="right">105,366</td>
<td align="right">2.6%</td>
<td align="right">17.3%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">4,011,849</td>
<td align="right">97.8%</td>
<td align="right">4,018,098</td>
<td align="right">97.4%</td>
<td align="right">0.2%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">no dict</td>
<td align="right">3,020</td>
<td align="right">3.4%</td>
<td align="right">4,540</td>
<td align="right">4.3%</td>
<td align="right">50.3%</td>
</tr>
<tr>
<td align="left">property</td>
<td align="right">2,720</td>
<td align="right">3.0%</td>
<td align="right">2,620</td>
<td align="right">2.5%</td>
<td align="right">-3.7%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">2,508</td>
<td align="right">2.8%</td>
<td align="right">2,516</td>
<td align="right">2.4%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,341</td>
<td align="right">8.2%</td>
<td align="right">7,321</td>
<td align="right">6.9%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">45,678</td>
<td align="right">50.8%</td>
<td align="right">45,638</td>
<td align="right">43.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">12,545</td>
<td align="right">14.0%</td>
<td align="right">12,545</td>
<td align="right">11.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,500</td>
<td align="right">11.7%</td>
<td align="right">10,500</td>
<td align="right">10.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">4,092</td>
<td align="right">4.6%</td>
<td align="right">4,092</td>
<td align="right">3.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">800</td>
<td align="right">0.9%</td>
<td align="right">800</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">614</td>
<td align="right">0.7%</td>
<td align="right">614</td>
<td align="right">0.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">non string or split</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">14,160</td>
<td align="right">13.4%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### STORE_SLICE

<details>
<summary> specialization stats for STORE_SLICE family </summary>


</details>

### STORE_SUBSCR

<details>
<summary> specialization stats for STORE_SUBSCR family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">853,863,163</td>
<td align="right">65.8%</td>
<td align="right">853,321,021</td>
<td align="right">65.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">443,458,282</td>
<td align="right">34.2%</td>
<td align="right">443,456,195</td>
<td align="right">34.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,880</td>
<td align="right">0.0%</td>
<td align="right">2,880</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Success</td>
<td align="right">12,589</td>
<td align="right">7.5%</td>
<td align="right">12,585</td>
<td align="right">7.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">155,812</td>
<td align="right">92.5%</td>
<td align="right">155,772</td>
<td align="right">92.5%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">other</td>
<td align="right">780</td>
<td align="right">0.5%</td>
<td align="right">760</td>
<td align="right">0.5%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">42,060</td>
<td align="right">27.0%</td>
<td align="right">42,040</td>
<td align="right">27.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">66,240</td>
<td align="right">42.5%</td>
<td align="right">66,240</td>
<td align="right">42.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">33,744</td>
<td align="right">21.7%</td>
<td align="right">33,744</td>
<td align="right">21.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">9,320</td>
<td align="right">6.0%</td>
<td align="right">9,320</td>
<td align="right">6.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,668</td>
<td align="right">2.4%</td>
<td align="right">3,668</td>
<td align="right">2.4%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### TO_BOOL

<details>
<summary> specialization stats for TO_BOOL family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,318,268,470</td>
<td align="right">92.3%</td>
<td align="right">6,313,640,078</td>
<td align="right">92.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">520,128,952</td>
<td align="right">7.6%</td>
<td align="right">519,938,634</td>
<td align="right">7.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">137,684,213</td>
<td align="right">2.0%</td>
<td align="right">137,684,142</td>
<td align="right">2.0%</td>
<td align="right">-0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">668,845</td>
<td align="right">19.2%</td>
<td align="right">668,642</td>
<td align="right">19.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,805,760</td>
<td align="right">80.8%</td>
<td align="right">2,805,810</td>
<td align="right">80.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">sequence</td>
<td align="right">16,080</td>
<td align="right">2.4%</td>
<td align="right">16,040</td>
<td align="right">2.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">27,052</td>
<td align="right">4.0%</td>
<td align="right">27,015</td>
<td align="right">4.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">97,696</td>
<td align="right">14.6%</td>
<td align="right">97,615</td>
<td align="right">14.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">109,399</td>
<td align="right">16.4%</td>
<td align="right">109,373</td>
<td align="right">16.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">173,415</td>
<td align="right">25.9%</td>
<td align="right">173,392</td>
<td align="right">25.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">183,137</td>
<td align="right">27.4%</td>
<td align="right">183,141</td>
<td align="right">27.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">30,710</td>
<td align="right">4.6%</td>
<td align="right">30,710</td>
<td align="right">4.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">28,156</td>
<td align="right">4.2%</td>
<td align="right">28,156</td>
<td align="right">4.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">float</td>
<td align="right">1,740</td>
<td align="right">0.3%</td>
<td align="right">1,740</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray</td>
<td align="right">1,040</td>
<td align="right">0.2%</td>
<td align="right">1,040</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">memory view</td>
<td align="right">420</td>
<td align="right">0.1%</td>
<td align="right">420</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### UNPACK_SEQUENCE

<details>
<summary> specialization stats for UNPACK_SEQUENCE family </summary>

<table>
<thead>
<tr>
<th align="left">Kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,044,668,826</td>
<td align="right">99.8%</td>
<td align="right">2,044,392,921</td>
<td align="right">99.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">3,184,734</td>
<td align="right">0.2%</td>
<td align="right">3,184,932</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,972,240</td>
<td align="right">0.1%</td>
<td align="right">2,972,240</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Success</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Failure</td>
<td align="right">2,198</td>
<td align="right">2.2%</td>
<td align="right">2,200</td>
<td align="right">2.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">95,529</td>
<td align="right">97.8%</td>
<td align="right">95,557</td>
<td align="right">97.7%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th align="left">Failure kind</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">sequence</td>
<td align="right">1,457</td>
<td align="right">66.3%</td>
<td align="right">1,459</td>
<td align="right">66.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">17.3%</td>
<td align="right">380</td>
<td align="right">17.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">361</td>
<td align="right">16.4%</td>
<td align="right">361</td>
<td align="right">16.4%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>


</details>

## Specialization effectiveness

<details>
<summary> specialization effectiveness </summary>


All entries are execution counts. Should add up to the total number of
Tier 1 instructions executed.

<table>
<thead>
<tr>
<th align="left">Instructions</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,685,034,031</td>
<td align="right">0.7%</td>
<td align="right">1,778,974,576</td>
<td align="right">0.8%</td>
<td align="right">5.6%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">75,906,211,975</td>
<td align="right">33.2%</td>
<td align="right">75,725,656,891</td>
<td align="right">33.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Not specialized
<details>
<summary>ⓘ</summary>

Instructions that could be specialized but aren't, e.g. `LOAD_ATTR`, `BINARY_SLICE`.
</details>
</td>
<td align="right">23,845,181,729</td>
<td align="right">10.4%</td>
<td align="right">23,863,465,811</td>
<td align="right">10.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">126,869,651,284</td>
<td align="right">55.6%</td>
<td align="right">126,794,230,856</td>
<td align="right">55.6%</td>
<td align="right">-0.1%</td>
</tr>
</tbody>
</table>

### Deferred by instruction

<details>
<summary> Breakdown of deferred (not specialized) instruction counts by family </summary>

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">2,500,576,447</td>
<td align="right">27.1%</td>
<td align="right">2,619,050,504</td>
<td align="right">28.1%</td>
<td align="right">4.7%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">269,887,185</td>
<td align="right">2.9%</td>
<td align="right">275,051,809</td>
<td align="right">2.9%</td>
<td align="right">1.9%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">1,439,641,821</td>
<td align="right">15.6%</td>
<td align="right">1,436,510,289</td>
<td align="right">15.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,414,986,214</td>
<td align="right">15.4%</td>
<td align="right">1,412,197,556</td>
<td align="right">15.1%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">240,432,633</td>
<td align="right">2.6%</td>
<td align="right">240,275,349</td>
<td align="right">2.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">520,128,952</td>
<td align="right">5.6%</td>
<td align="right">519,938,634</td>
<td align="right">5.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">673,413,333</td>
<td align="right">7.3%</td>
<td align="right">673,618,362</td>
<td align="right">7.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">1,522,681,570</td>
<td align="right">16.5%</td>
<td align="right">1,522,796,682</td>
<td align="right">16.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">443,458,282</td>
<td align="right">4.8%</td>
<td align="right">443,456,195</td>
<td align="right">4.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">164,784,832</td>
<td align="right">1.8%</td>
<td align="right">164,784,836</td>
<td align="right">1.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Misses by instruction

<details>
<summary> Breakdown of misses (specialized deopts) instruction counts by family </summary>

<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">254,657,004</td>
<td align="right">15.1%</td>
<td align="right">336,601,369</td>
<td align="right">18.9%</td>
<td align="right">32.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">348,155,559</td>
<td align="right">20.7%</td>
<td align="right">367,061,730</td>
<td align="right">20.6%</td>
<td align="right">5.4%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">108,671,031</td>
<td align="right">6.4%</td>
<td align="right">109,280,668</td>
<td align="right">6.1%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">87,338,168</td>
<td align="right">5.2%</td>
<td align="right">87,356,727</td>
<td align="right">4.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">97,967,791</td>
<td align="right">5.8%</td>
<td align="right">97,984,106</td>
<td align="right">5.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">87,726,453</td>
<td align="right">5.2%</td>
<td align="right">87,721,509</td>
<td align="right">4.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">111,168,509</td>
<td align="right">6.6%</td>
<td align="right">111,173,395</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">125,318,784</td>
<td align="right">7.4%</td>
<td align="right">125,320,563</td>
<td align="right">7.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">67,271,805</td>
<td align="right">4.0%</td>
<td align="right">67,271,873</td>
<td align="right">3.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">69,565,988</td>
<td align="right">4.1%</td>
<td align="right"></td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right"></td>
<td align="right"></td>
<td align="right">61,949,865</td>
<td align="right">3.5%</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>


</details>

## Call stats

<details>
<summary> Inlined calls and frame stats </summary>


This shows what fraction of calls to Python functions are inlined (i.e.
not having a call at the C level) and for those that are not, where the
call comes from.  The various categories overlap.

Also includes the count of frame objects created.

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,224,324,277</td>
<td align="right">14.5%</td>
<td align="right">1,222,493,125</td>
<td align="right">14.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,229,637,327</td>
<td align="right">14.5%</td>
<td align="right">1,227,806,175</td>
<td align="right">14.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">4,957,285,894</td>
<td align="right">58.6%</td>
<td align="right">4,951,051,680</td>
<td align="right">58.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls to Python functions inlined</td>
<td align="right">6,383,136,972</td>
<td align="right">75.4%</td>
<td align="right">6,376,290,307</td>
<td align="right">75.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">230,152,373</td>
<td align="right">2.7%</td>
<td align="right">229,929,547</td>
<td align="right">2.7%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,078,549,237</td>
<td align="right">24.6%</td>
<td align="right">2,076,892,342</td>
<td align="right">24.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,078,549,237</td>
<td align="right">24.6%</td>
<td align="right">2,076,892,342</td>
<td align="right">24.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">848,911,910</td>
<td align="right">10.0%</td>
<td align="right">849,086,167</td>
<td align="right">10.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">84,491,602</td>
<td align="right">1.0%</td>
<td align="right">84,476,498</td>
<td align="right">1.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">338,007,189</td>
<td align="right">4.0%</td>
<td align="right">337,970,131</td>
<td align="right">4.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">21,974,507</td>
<td align="right">0.3%</td>
<td align="right">21,973,554</td>
<td align="right">0.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">211,357,009</td>
<td align="right">2.5%</td>
<td align="right">211,357,166</td>
<td align="right">2.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">5,294,164</td>
<td align="right">0.1%</td>
<td align="right">5,294,164</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (build class)</td>
<td align="right">18,886</td>
<td align="right">0.0%</td>
<td align="right">18,886</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

## Object stats

<details>
<summary> Allocations, frees and dict materializatons </summary>


Below, "allocations" means "allocations that are not from a freelist".
Total allocations = "Allocations from freelist" + "Allocations".

"New values" is the number of values arrays created for objects with
managed dicts.

The cache hit/miss numbers are for the MRO cache, split into dunder and
other names.

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">New values</td>
<td align="right">74,699,704</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">-100.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (new key)</td>
<td align="right">189,835</td>
<td align="right">0.3%</td>
<td align="right">89,695</td>
<td align="right">89,695 / 0 !!</td>
<td align="right">-52.8%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">3,650,505</td>
<td align="right">4.9%</td>
<td align="right">2,946,063</td>
<td align="right">2,946,063 / 0 !!</td>
<td align="right">-19.3%</td>
</tr>
<tr>
<td align="left">Method cache dunder misses</td>
<td align="right">12,576,674</td>
<td align="right"></td>
<td align="right">13,330,572</td>
<td align="right"></td>
<td align="right">6.0%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,033,863,181</td>
<td align="right"></td>
<td align="right">3,158,240,663</td>
<td align="right"></td>
<td align="right">4.1%</td>
</tr>
<tr>
<td align="left">Method cache collisions</td>
<td align="right">96,489,854</td>
<td align="right"></td>
<td align="right">98,653,150</td>
<td align="right"></td>
<td align="right">2.2%</td>
</tr>
<tr>
<td align="left">Method cache misses</td>
<td align="right">91,622,644</td>
<td align="right"></td>
<td align="right">93,037,338</td>
<td align="right"></td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">11,500,110,725</td>
<td align="right">63.1%</td>
<td align="right">11,333,119,821</td>
<td align="right">62.8%</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">11,623,992,068</td>
<td align="right">63.8%</td>
<td align="right">11,456,896,347</td>
<td align="right">63.5%</td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">11,963,943,481</td>
<td align="right"></td>
<td align="right">11,798,655,277</td>
<td align="right"></td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">25,597,592,165</td>
<td align="right">22.8%</td>
<td align="right">25,857,921,488</td>
<td align="right">23.0%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">28,567,063,792</td>
<td align="right">22.1%</td>
<td align="right">28,725,820,527</td>
<td align="right">22.2%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">20,708,780</td>
<td align="right">0.1%</td>
<td align="right">20,640,480</td>
<td align="right">0.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">86,684,267,006</td>
<td align="right">77.2%</td>
<td align="right">86,523,287,050</td>
<td align="right">77.0%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,267,988,904</td>
<td align="right"></td>
<td align="right">3,264,456,350</td>
<td align="right"></td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,589,499,496</td>
<td align="right">36.2%</td>
<td align="right">6,583,529,554</td>
<td align="right">36.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,596,885,197</td>
<td align="right"></td>
<td align="right">6,591,127,841</td>
<td align="right"></td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">100,807,169,005</td>
<td align="right">77.9%</td>
<td align="right">100,743,280,911</td>
<td align="right">77.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">103,172,563</td>
<td align="right">0.6%</td>
<td align="right">103,136,046</td>
<td align="right">0.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (too big)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">Materialize dict (str subclass)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,343,620</td>
<td align="right">3.1%</td>
<td align="right"></td>
<td align="right"></td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

## GC stats

<details>
<summary> GC collections and effectiveness </summary>


Collected/visits gives some measure of efficiency.

<table>
<thead>
<tr>
<th align="right">Generation</th>
<th align="right">Base Collections</th>
<th align="right">Base Objects collected</th>
<th align="right">Base Object visits</th>
<th align="right">Head Collections</th>
<th align="right">Head Objects collected</th>
<th align="right">Head Object visits</th>
</tr>
</thead>
<tbody>
<tr>
<td align="right">0</td>
<td align="right">727,276</td>
<td align="right">46,027,369</td>
<td align="right">6,015,799,266</td>
<td align="right">733,671</td>
<td align="right">45,730,449</td>
<td align="right">6,032,612,790</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">65,072</td>
<td align="right">36,610,154</td>
<td align="right">4,937,660,744</td>
<td align="right">65,705</td>
<td align="right">36,638,934</td>
<td align="right">4,959,639,760</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">20,826</td>
<td align="right">53,177,840</td>
<td align="right">18,063,737,056</td>
<td align="right">20,890</td>
<td align="right">55,881,400</td>
<td align="right">18,286,621,090</td>
</tr>
</tbody>
</table>


</details>

## Optimization (Tier 2) stats

<details>
<summary> statistics about the Tier 2 optimizer </summary>

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Trace stack overflow
<details>
<summary>ⓘ</summary>

A trace is truncated because it would require more than 5 stack frames.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Trace too long
<details>
<summary>ⓘ</summary>

A trace is truncated because it is longer than the instruction buffer.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Executors invalidated
<details>
<summary>ⓘ</summary>

The number of executors that were invalidated due to watched dictionary changes.
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
</tbody>
</table>

### Trace length histogram

<details>
<summary> trace length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### Optimized trace length histogram

<details>
<summary> optimized trace length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### Trace run length histogram

<details>
<summary> trace run length histogram </summary>

<table>
<thead>
<tr>
<th align="left">Range</th>
<th align="right">Base Count</th>
<th align="right">Base Ratio</th>
<th align="right">Head Count</th>
<th align="right">Head Ratio</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left"><= 1</td>
<td align="right">0</td>
<td align="right"></td>
<td align="right">0</td>
<td align="right"></td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>


</details>


</details>

## Rare events

<details>
<summary> Counts of rare/unlikely events </summary>

<table>
<thead>
<tr>
<th align="left">Event</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">
set class
<details>
<summary>ⓘ</summary>

Setting an object's class, `obj.__class__ = ...`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
set bases
<details>
<summary>ⓘ</summary>

Setting the bases of a class, `cls.__bases__ = ...`
</details>
</td>
<td align="right">41</td>
<td align="right">41</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
set eval frame func
<details>
<summary>ⓘ</summary>

Setting the PEP 523 frame eval function `_PyInterpreterState_SetFrameEvalFunc()`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
builtin dict
<details>
<summary>ⓘ</summary>

Modifying the builtins, `__builtins__.__dict__[var] = ...`
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
func modification
<details>
<summary>ⓘ</summary>

Modifying a function, e.g. `func.__defaults__ = ...`, etc.
</details>
</td>
<td align="right">181</td>
<td align="right">181</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
watched dict modification
<details>
<summary>ⓘ</summary>

A watched dict has been modified
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">
watched globals modification
<details>
<summary>ⓘ</summary>

A watched `globals()` dict has been modified
</details>
</td>
<td align="right">0</td>
<td align="right">0</td>
<td align="right"></td>
</tr>
</tbody>
</table>


</details>

## Meta stats

<details>
<summary> Meta statistics </summary>

<table>
<thead>
<tr>
<th align="left"></th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">Number of data files</td>
<td align="right">1,900</td>
<td align="right">1,900</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

---
Stats gathered on: 2024-02-29
