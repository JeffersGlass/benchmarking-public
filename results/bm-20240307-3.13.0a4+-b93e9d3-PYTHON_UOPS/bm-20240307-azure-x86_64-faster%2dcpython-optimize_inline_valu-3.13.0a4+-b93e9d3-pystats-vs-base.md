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
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">12,024,039</td>
<td align="right">11,341,283</td>
<td align="right">-5.7%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">13,578,641</td>
<td align="right">12,822,759</td>
<td align="right">-5.6%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_LIST</td>
<td align="right">9,246,537</td>
<td align="right">8,753,739</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">83,384,955</td>
<td align="right">80,958,276</td>
<td align="right">-2.9%</td>
</tr>
<tr>
<td align="left">UNARY_INVERT</td>
<td align="right">2,741,725</td>
<td align="right">2,819,829</td>
<td align="right">2.8%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">76,296,202</td>
<td align="right">74,555,331</td>
<td align="right">-2.3%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">342,313,019</td>
<td align="right">335,078,756</td>
<td align="right">-2.1%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">632,730,807</td>
<td align="right">622,705,595</td>
<td align="right">-1.6%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">551,513,403</td>
<td align="right">544,912,799</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">257,301,514</td>
<td align="right">254,725,919</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">73,083,905</td>
<td align="right">72,368,508</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">557,641,450</td>
<td align="right">552,813,687</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">4,728,134,214</td>
<td align="right">4,688,009,655</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">183,047,697</td>
<td align="right">181,579,513</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,164,127,587</td>
<td align="right">1,155,693,432</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">507,303,929</td>
<td align="right">503,659,281</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">179,332,081</td>
<td align="right">178,070,344</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">500,015,337</td>
<td align="right">496,571,253</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">211,972,110</td>
<td align="right">210,640,814</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">161,684,236</td>
<td align="right">160,675,230</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">1,594,166,356</td>
<td align="right">1,584,951,181</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">160,427,754</td>
<td align="right">159,551,155</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">73,367,052</td>
<td align="right">72,986,732</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">221,764,607</td>
<td align="right">220,615,808</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">271,885,930</td>
<td align="right">270,502,204</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">348,673,499</td>
<td align="right">346,964,933</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">425,853,572</td>
<td align="right">423,849,266</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_TUPLE</td>
<td align="right">21,562,888</td>
<td align="right">21,468,839</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">153,755,255</td>
<td align="right">153,094,985</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">147,734,183</td>
<td align="right">147,106,668</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">332,391,833</td>
<td align="right">331,082,960</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">244,935,412</td>
<td align="right">243,991,036</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">7,559,313,302</td>
<td align="right">7,530,520,348</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">486,117,778</td>
<td align="right">484,268,698</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">8,633,451,219</td>
<td align="right">8,601,123,373</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">184,083,154</td>
<td align="right">183,440,508</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">1,659,889,724</td>
<td align="right">1,654,097,763</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">8,303,670,930</td>
<td align="right">8,275,524,913</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">590,247,057</td>
<td align="right">588,286,206</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">2,088,029,278</td>
<td align="right">2,081,101,417</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">1,269,916,369</td>
<td align="right">1,265,745,400</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">30,258,071,370</td>
<td align="right">30,159,209,510</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">350,538,646</td>
<td align="right">349,418,831</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">139,603,031</td>
<td align="right">139,157,290</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">222,957,042</td>
<td align="right">222,265,593</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">433,414,580</td>
<td align="right">432,071,065</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">1,818,193,952</td>
<td align="right">1,812,575,779</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">143,493,299</td>
<td align="right">143,060,054</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">149,673,868</td>
<td align="right">149,228,483</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">75,775,910</td>
<td align="right">75,553,304</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">2,281,933,863</td>
<td align="right">2,275,717,101</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">283,860,645</td>
<td align="right">283,091,461</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">254,876,462</td>
<td align="right">254,236,565</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">3,611,034,268</td>
<td align="right">3,602,114,989</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">828,108,758</td>
<td align="right">826,081,090</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">337,156,915</td>
<td align="right">336,356,382</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">94,924,494</td>
<td align="right">94,700,722</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">97,212,716</td>
<td align="right">96,988,944</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">1,769,586,620</td>
<td align="right">1,765,684,341</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,473,346,128</td>
<td align="right">1,470,150,848</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">704,458,419</td>
<td align="right">702,959,512</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">10,036,435</td>
<td align="right">10,057,645</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">331,380,375</td>
<td align="right">330,713,016</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">851,121,533</td>
<td align="right">849,413,311</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">4,484,059,713</td>
<td align="right">4,475,181,469</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">7,508,482,708</td>
<td align="right">7,494,093,231</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">ENTER_EXECUTOR</td>
<td align="right">2,858,838,414</td>
<td align="right">2,853,537,610</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">6,582,436,356</td>
<td align="right">6,570,511,291</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">370,747,500</td>
<td align="right">370,100,213</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">4,388,054,064</td>
<td align="right">4,380,732,444</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,544,386,538</td>
<td align="right">4,537,108,898</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">72,504,392</td>
<td align="right">72,619,760</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_DICT</td>
<td align="right">319,563,924</td>
<td align="right">319,127,940</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">780,607,154</td>
<td align="right">779,627,834</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">888,345,911</td>
<td align="right">887,297,004</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">315,227,869</td>
<td align="right">314,885,902</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">82,974</td>
<td align="right">83,059</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">4,015,630,301</td>
<td align="right">4,011,571,493</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">763,198,219</td>
<td align="right">762,482,059</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">5,193,799,065</td>
<td align="right">5,189,028,827</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">280,725,812</td>
<td align="right">280,483,923</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">1,199,147,369</td>
<td align="right">1,198,153,028</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">10,012</td>
<td align="right">10,004</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">1,090,645,799</td>
<td align="right">1,089,780,070</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,259,219,444</td>
<td align="right">1,258,251,830</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">567,386,331</td>
<td align="right">566,962,872</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">29,834,212</td>
<td align="right">29,855,654</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">11,372</td>
<td align="right">11,364</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">166,427,852</td>
<td align="right">166,320,600</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">44,579,708</td>
<td align="right">44,607,782</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">127,114,939</td>
<td align="right">127,193,194</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">13,452</td>
<td align="right">13,444</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">800,942,749</td>
<td align="right">800,546,691</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">559,661,484</td>
<td align="right">559,397,409</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">164,038,710</td>
<td align="right">164,112,505</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">361,110,608</td>
<td align="right">360,949,731</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">84,533,786</td>
<td align="right">84,567,764</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">5,271,759</td>
<td align="right">5,269,675</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">611,312,994</td>
<td align="right">611,076,348</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">1,764,835,675</td>
<td align="right">1,764,188,753</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,408,542,742</td>
<td align="right">1,408,062,485</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">371,589,247</td>
<td align="right">371,468,955</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">957,427,909</td>
<td align="right">957,168,805</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">866,466,381</td>
<td align="right">866,699,068</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,521,570,687</td>
<td align="right">1,521,176,066</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">83,850,725</td>
<td align="right">83,829,962</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">339,763,087</td>
<td align="right">339,688,204</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">23,523</td>
<td align="right">23,528</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">343,722</td>
<td align="right">343,787</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">566,524</td>
<td align="right">566,631</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">2,298,629</td>
<td align="right">2,298,204</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">132,131,176</td>
<td align="right">132,155,170</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">669,364,921</td>
<td align="right">669,248,198</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">157,346,524</td>
<td align="right">157,370,820</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">84,313,486</td>
<td align="right">84,325,664</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">90,185,709</td>
<td align="right">90,197,105</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">50,154,194</td>
<td align="right">50,148,540</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">70,369,075</td>
<td align="right">70,361,962</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">13,106,892</td>
<td align="right">13,107,973</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">79,189,677</td>
<td align="right">79,195,199</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">12,435,774</td>
<td align="right">12,436,638</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,323,251,823</td>
<td align="right">2,323,401,578</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">151,914</td>
<td align="right">151,923</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">24,534,142</td>
<td align="right">24,532,730</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">173,399,898</td>
<td align="right">173,391,716</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">25,045,682</td>
<td align="right">25,044,546</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">25,045,532</td>
<td align="right">25,044,399</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">505,594,358</td>
<td align="right">505,616,944</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">44,546,001</td>
<td align="right">44,544,186</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">123,740,095</td>
<td align="right">123,736,045</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">1,119,409,276</td>
<td align="right">1,119,445,060</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">113,400,582</td>
<td align="right">113,397,022</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">6,185,985</td>
<td align="right">6,185,798</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_SET</td>
<td align="right">118,408,996</td>
<td align="right">118,406,481</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">2,322,490</td>
<td align="right">2,322,535</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">54,798,013</td>
<td align="right">54,797,180</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,803,079</td>
<td align="right">20,803,362</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">199,964,655</td>
<td align="right">199,962,050</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">95,450,359</td>
<td align="right">95,451,602</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">WITH_EXCEPT_START</td>
<td align="right">233,564</td>
<td align="right">233,561</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">193,643,894</td>
<td align="right">193,641,573</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">7,752,586</td>
<td align="right">7,752,509</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">118,675,426</td>
<td align="right">118,674,270</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">141,826,433</td>
<td align="right">141,827,703</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">272,816,062</td>
<td align="right">272,814,004</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">155,025,668</td>
<td align="right">155,024,696</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">29,357,527</td>
<td align="right">29,357,395</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">19,338,509</td>
<td align="right">19,338,594</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,519,819,827</td>
<td align="right">1,519,826,006</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,864,433</td>
<td align="right">229,865,093</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">344,922,286</td>
<td align="right">344,923,171</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">176,518,947</td>
<td align="right">176,519,362</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">202,872,864</td>
<td align="right">202,872,466</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">787,214,028</td>
<td align="right">787,215,354</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">402,689,517</td>
<td align="right">402,690,175</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">140,875,723</td>
<td align="right">140,875,895</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">173,868,065</td>
<td align="right">173,868,257</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">231,109,944</td>
<td align="right">231,110,119</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">387,727,303</td>
<td align="right">387,727,049</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">556,770,395</td>
<td align="right">556,770,081</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">64,709,654</td>
<td align="right">64,709,677</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">82,349,630</td>
<td align="right">82,349,615</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">47,505,562</td>
<td align="right">47,505,563</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP_STR</td>
<td align="right">60,075,026</td>
<td align="right">60,075,027</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">250,156,090</td>
<td align="right">250,156,086</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_FALSE</td>
<td align="right">38,888,640</td>
<td align="right">38,888,640</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RESUME</td>
<td align="right">38,866,420</td>
<td align="right">38,866,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_VALUE</td>
<td align="right">38,857,520</td>
<td align="right">38,857,520</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_NAME</td>
<td align="right">12,328,327</td>
<td align="right">12,328,327</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_ANEXT</td>
<td align="right">8,000,960</td>
<td align="right">8,000,960</td>
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
<td align="left">STORE_GLOBAL</td>
<td align="right">6,944,700</td>
<td align="right">6,944,700</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,695,518</td>
<td align="right">6,695,518</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RERAISE</td>
<td align="right">3,847,445</td>
<td align="right">3,847,445</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BEFORE_ASYNC_WITH</td>
<td align="right">3,005,920</td>
<td align="right">3,005,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_EX</td>
<td align="right">1,129,926</td>
<td align="right">1,129,926</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">965,583</td>
<td align="right">965,583</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">546,276</td>
<td align="right">546,276</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">200,448</td>
<td align="right">200,448</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_GETATTRIBUTE_OVERRIDDEN</td>
<td align="right">92,500</td>
<td align="right">92,500</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_BUILD_CLASS</td>
<td align="right">28,886</td>
<td align="right">28,886</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_RETURN_CONST</td>
<td align="right">7,200</td>
<td align="right">7,200</td>
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
<td align="left">SETUP_ANNOTATIONS</td>
<td align="right">1,424</td>
<td align="right">1,424</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">1,080</td>
<td align="right">1,080</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_NAME</td>
<td align="right">980</td>
<td align="right">980</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NONE</td>
<td align="right">720</td>
<td align="right">720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_FORWARD</td>
<td align="right">400</td>
<td align="right">400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NOT_NONE</td>
<td align="right">400</td>
<td align="right">400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_2</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,626,006,375</td>
<td align="right">74.7%</td>
<td align="right">2,618,573,145</td>
<td align="right">74.7%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">886,985,322</td>
<td align="right">25.2%</td>
<td align="right">887,217,892</td>
<td align="right">25.3%</td>
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
<td align="right">22,219,660</td>
<td align="right">0.6%</td>
<td align="right">22,219,653</td>
<td align="right">0.6%</td>
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
<td align="left">Success</td>
<td align="right">473,107</td>
<td align="right">27.8%</td>
<td align="right">473,194</td>
<td align="right">27.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,227,612</td>
<td align="right">72.2%</td>
<td align="right">1,227,635</td>
<td align="right">72.2%</td>
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
<td align="left">power</td>
<td align="right">5,680</td>
<td align="right">0.5%</td>
<td align="right">5,692</td>
<td align="right">0.5%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">or</td>
<td align="right">19,400</td>
<td align="right">1.6%</td>
<td align="right">19,431</td>
<td align="right">1.6%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">14,064</td>
<td align="right">1.1%</td>
<td align="right">14,046</td>
<td align="right">1.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">lshift</td>
<td align="right">7,304</td>
<td align="right">0.6%</td>
<td align="right">7,312</td>
<td align="right">0.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">2,014</td>
<td align="right">0.2%</td>
<td align="right">2,016</td>
<td align="right">0.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">56,314</td>
<td align="right">4.6%</td>
<td align="right">56,275</td>
<td align="right">4.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">and int</td>
<td align="right">59,476</td>
<td align="right">4.8%</td>
<td align="right">59,516</td>
<td align="right">4.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">71,643</td>
<td align="right">5.8%</td>
<td align="right">71,598</td>
<td align="right">5.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">13,141</td>
<td align="right">1.1%</td>
<td align="right">13,149</td>
<td align="right">1.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,492</td>
<td align="right">0.3%</td>
<td align="right">3,490</td>
<td align="right">0.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">70,325</td>
<td align="right">5.7%</td>
<td align="right">70,362</td>
<td align="right">5.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">68,216</td>
<td align="right">5.6%</td>
<td align="right">68,188</td>
<td align="right">5.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">5,944</td>
<td align="right">0.5%</td>
<td align="right">5,946</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">46,236</td>
<td align="right">3.8%</td>
<td align="right">46,244</td>
<td align="right">3.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">26,704</td>
<td align="right">2.2%</td>
<td align="right">26,706</td>
<td align="right">2.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">737,986</td>
<td align="right">60.1%</td>
<td align="right">737,991</td>
<td align="right">60.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">13,834</td>
<td align="right">1.1%</td>
<td align="right">13,834</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,260</td>
<td align="right">0.4%</td>
<td align="right">5,260</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and different types</td>
<td align="right">579</td>
<td align="right">0.0%</td>
<td align="right">579</td>
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
<td align="right">556,316,076</td>
<td align="right">21.8%</td>
<td align="right">549,717,614</td>
<td align="right">21.7%</td>
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
<td align="right">1,996,376,101</td>
<td align="right">78.2%</td>
<td align="right">1,982,476,303</td>
<td align="right">78.3%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">5,235,393</td>
<td align="right">0.2%</td>
<td align="right">5,235,498</td>
<td align="right">0.2%</td>
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
<td align="right">224,335</td>
<td align="right">51.8%</td>
<td align="right">222,283</td>
<td align="right">51.6%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">208,385</td>
<td align="right">48.2%</td>
<td align="right">208,400</td>
<td align="right">48.4%</td>
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
<td align="left">buffer slice</td>
<td align="right">980</td>
<td align="right">0.4%</td>
<td align="right">900</td>
<td align="right">0.4%</td>
<td align="right">-8.2%</td>
</tr>
<tr>
<td align="left">list slice</td>
<td align="right">720</td>
<td align="right">0.3%</td>
<td align="right">680</td>
<td align="right">0.3%</td>
<td align="right">-5.6%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">31,160</td>
<td align="right">13.9%</td>
<td align="right">30,360</td>
<td align="right">13.7%</td>
<td align="right">-2.6%</td>
</tr>
<tr>
<td align="left">tuple slice</td>
<td align="right">184</td>
<td align="right">0.1%</td>
<td align="right">186</td>
<td align="right">0.1%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">84,969</td>
<td align="right">37.9%</td>
<td align="right">84,047</td>
<td align="right">37.8%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">buffer int</td>
<td align="right">38,923</td>
<td align="right">17.4%</td>
<td align="right">38,740</td>
<td align="right">17.4%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">57,963</td>
<td align="right">25.8%</td>
<td align="right">57,934</td>
<td align="right">26.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">5,036</td>
<td align="right">2.2%</td>
<td align="right">5,036</td>
<td align="right">2.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,300</td>
<td align="right">1.9%</td>
<td align="right">4,300</td>
<td align="right">1.9%</td>
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
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">258,597,887</td>
<td align="right">2.2%</td>
<td align="right">255,424,747</td>
<td align="right">2.2%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">1,511,297,260</td>
<td align="right">12.7%</td>
<td align="right">1,507,217,279</td>
<td align="right">12.7%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">10,339,915,215</td>
<td align="right">87.2%</td>
<td align="right">10,322,416,079</td>
<td align="right">87.2%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">39,400</td>
<td align="right">0.0%</td>
<td align="right">39,400</td>
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
<td align="right">5,504,405</td>
<td align="right">84.4%</td>
<td align="right">5,444,556</td>
<td align="right">84.3%</td>
<td align="right">-1.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">1,015,666</td>
<td align="right">15.6%</td>
<td align="right">1,014,742</td>
<td align="right">15.7%</td>
<td align="right">-0.1%</td>
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
<td align="left">metaclass</td>
<td align="right">43,414</td>
<td align="right">4.3%</td>
<td align="right">43,060</td>
<td align="right">4.2%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">str</td>
<td align="right">3,200</td>
<td align="right">0.3%</td>
<td align="right">3,180</td>
<td align="right">0.3%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">operator wrapper</td>
<td align="right">10,180</td>
<td align="right">1.0%</td>
<td align="right">10,136</td>
<td align="right">1.0%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">8,250</td>
<td align="right">0.8%</td>
<td align="right">8,224</td>
<td align="right">0.8%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">21,671</td>
<td align="right">2.1%</td>
<td align="right">21,725</td>
<td align="right">2.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">74,540</td>
<td align="right">7.3%</td>
<td align="right">74,410</td>
<td align="right">7.3%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">79,626</td>
<td align="right">7.8%</td>
<td align="right">79,515</td>
<td align="right">7.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">71,014</td>
<td align="right">7.0%</td>
<td align="right">71,100</td>
<td align="right">7.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">11,837</td>
<td align="right">1.2%</td>
<td align="right">11,851</td>
<td align="right">1.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">207,563</td>
<td align="right">20.4%</td>
<td align="right">207,338</td>
<td align="right">20.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">25,242</td>
<td align="right">2.5%</td>
<td align="right">25,216</td>
<td align="right">2.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">64,427</td>
<td align="right">6.3%</td>
<td align="right">64,376</td>
<td align="right">6.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">186,303</td>
<td align="right">18.3%</td>
<td align="right">186,242</td>
<td align="right">18.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">cfunc varargs keywords</td>
<td align="right">32,162</td>
<td align="right">3.2%</td>
<td align="right">32,155</td>
<td align="right">3.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">14,343</td>
<td align="right">1.4%</td>
<td align="right">14,340</td>
<td align="right">1.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">105,236</td>
<td align="right">10.4%</td>
<td align="right">105,216</td>
<td align="right">10.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,406</td>
<td align="right">1.6%</td>
<td align="right">16,406</td>
<td align="right">1.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">cmethod</td>
<td align="right">14,100</td>
<td align="right">1.4%</td>
<td align="right">14,100</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">13,894</td>
<td align="right">1.4%</td>
<td align="right">13,894</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not simple</td>
<td align="right">12,258</td>
<td align="right">1.2%</td>
<td align="right">12,258</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,128,033,919</td>
<td align="right">92.9%</td>
<td align="right">2,111,583,300</td>
<td align="right">92.8%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">163,409,169</td>
<td align="right">7.1%</td>
<td align="right">162,399,153</td>
<td align="right">7.1%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,089,350</td>
<td align="right">0.1%</td>
<td align="right">2,088,210</td>
<td align="right">0.1%</td>
<td align="right">-0.1%</td>
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
<td align="right">245,595</td>
<td align="right">67.4%</td>
<td align="right">245,467</td>
<td align="right">67.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">118,822</td>
<td align="right">32.6%</td>
<td align="right">118,820</td>
<td align="right">32.6%</td>
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
<td align="left">bytes</td>
<td align="right">4,400</td>
<td align="right">1.8%</td>
<td align="right">4,280</td>
<td align="right">1.7%</td>
<td align="right">-2.7%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">1,640</td>
<td align="right">0.7%</td>
<td align="right">1,600</td>
<td align="right">0.7%</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">55,707</td>
<td align="right">22.7%</td>
<td align="right">55,147</td>
<td align="right">22.5%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">big int</td>
<td align="right">74,757</td>
<td align="right">30.4%</td>
<td align="right">75,457</td>
<td align="right">30.7%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">14,589</td>
<td align="right">5.9%</td>
<td align="right">14,504</td>
<td align="right">5.9%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">35,376</td>
<td align="right">14.4%</td>
<td align="right">35,294</td>
<td align="right">14.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">13,080</td>
<td align="right">5.3%</td>
<td align="right">13,110</td>
<td align="right">5.3%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">24,609</td>
<td align="right">10.0%</td>
<td align="right">24,641</td>
<td align="right">10.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">4,024</td>
<td align="right">1.6%</td>
<td align="right">4,020</td>
<td align="right">1.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">2,342</td>
<td align="right">1.0%</td>
<td align="right">2,343</td>
<td align="right">1.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">10,720</td>
<td align="right">4.4%</td>
<td align="right">10,720</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">4,351</td>
<td align="right">1.8%</td>
<td align="right">4,351</td>
<td align="right">1.8%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### CONTAINS_OP

<details>
<summary> specialization stats for CONTAINS_OP family </summary>

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
<td align="right">509,586,918</td>
<td align="right">100.0%</td>
<td align="right">505,943,626</td>
<td align="right">100.0%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">2,525,364</td>
<td align="right">0.5%</td>
<td align="right">2,525,364</td>
<td align="right">0.5%</td>
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
<td align="right">164,652</td>
<td align="right">67.9%</td>
<td align="right">163,296</td>
<td align="right">67.8%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">77,723</td>
<td align="right">32.1%</td>
<td align="right">77,723</td>
<td align="right">32.2%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">293,759,739</td>
<td align="right">17.5%</td>
<td align="right">292,905,897</td>
<td align="right">17.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,383,610,760</td>
<td align="right">82.3%</td>
<td align="right">1,380,986,852</td>
<td align="right">82.4%</td>
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
<td align="right">142,987,190</td>
<td align="right">8.5%</td>
<td align="right">142,780,875</td>
<td align="right">8.5%</td>
<td align="right">-0.1%</td>
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
<td align="right">218,428</td>
<td align="right">7.3%</td>
<td align="right">209,573</td>
<td align="right">7.1%</td>
<td align="right">-4.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,764,278</td>
<td align="right">92.7%</td>
<td align="right">2,760,390</td>
<td align="right">92.9%</td>
<td align="right">-0.1%</td>
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
<td align="left">dict items</td>
<td align="right">85,201</td>
<td align="right">39.0%</td>
<td align="right">76,415</td>
<td align="right">36.5%</td>
<td align="right">-10.3%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">8,171</td>
<td align="right">3.7%</td>
<td align="right">8,073</td>
<td align="right">3.9%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">28,153</td>
<td align="right">12.9%</td>
<td align="right">28,182</td>
<td align="right">13.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">21,109</td>
<td align="right">9.7%</td>
<td align="right">21,109</td>
<td align="right">10.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">15,119</td>
<td align="right">6.9%</td>
<td align="right">15,119</td>
<td align="right">7.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">14,898</td>
<td align="right">6.8%</td>
<td align="right">14,898</td>
<td align="right">7.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">14,734</td>
<td align="right">6.7%</td>
<td align="right">14,734</td>
<td align="right">7.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">seq iter</td>
<td align="right">10,560</td>
<td align="right">4.8%</td>
<td align="right">10,560</td>
<td align="right">5.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">7,651</td>
<td align="right">3.5%</td>
<td align="right">7,651</td>
<td align="right">3.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">7,050</td>
<td align="right">3.2%</td>
<td align="right">7,050</td>
<td align="right">3.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">3,180</td>
<td align="right">1.5%</td>
<td align="right">3,180</td>
<td align="right">1.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,620</td>
<td align="right">0.7%</td>
<td align="right">1,620</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">660</td>
<td align="right">0.3%</td>
<td align="right">660</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">callable</td>
<td align="right">282</td>
<td align="right">0.1%</td>
<td align="right">282</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">40</td>
<td align="right">0.0%</td>
<td align="right">40</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">11,248,966,462</td>
<td align="right">83.2%</td>
<td align="right">11,190,308,250</td>
<td align="right">83.2%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">2,246,975,750</td>
<td align="right">16.6%</td>
<td align="right">2,243,826,868</td>
<td align="right">16.7%</td>
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
<td align="right">2,135,928</td>
<td align="right">0.0%</td>
<td align="right">2,136,638</td>
<td align="right">0.0%</td>
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
<td align="right">790,958,071</td>
<td align="right">5.9%</td>
<td align="right">791,003,477</td>
<td align="right">5.9%</td>
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
<td align="right">1,536,855</td>
<td align="right">8.9%</td>
<td align="right">1,534,962</td>
<td align="right">8.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">15,791,594</td>
<td align="right">91.1%</td>
<td align="right">15,792,495</td>
<td align="right">91.1%</td>
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
<td align="left">method</td>
<td align="right">145,514</td>
<td align="right">9.5%</td>
<td align="right">144,134</td>
<td align="right">9.4%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">26,365</td>
<td align="right">1.7%</td>
<td align="right">26,191</td>
<td align="right">1.7%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">21,128</td>
<td align="right">1.4%</td>
<td align="right">21,093</td>
<td align="right">1.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">82,231</td>
<td align="right">5.4%</td>
<td align="right">82,171</td>
<td align="right">5.4%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">116,009</td>
<td align="right">7.5%</td>
<td align="right">116,092</td>
<td align="right">7.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">216,349</td>
<td align="right">14.1%</td>
<td align="right">216,198</td>
<td align="right">14.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">non overriding descriptor</td>
<td align="right">13,750</td>
<td align="right">0.9%</td>
<td align="right">13,741</td>
<td align="right">0.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">non object slot</td>
<td align="right">3,622</td>
<td align="right">0.2%</td>
<td align="right">3,620</td>
<td align="right">0.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">metaclass attribute</td>
<td align="right">260,943</td>
<td align="right">17.0%</td>
<td align="right">260,844</td>
<td align="right">17.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">30,206</td>
<td align="right">2.0%</td>
<td align="right">30,200</td>
<td align="right">2.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">has managed dict</td>
<td align="right">550,697</td>
<td align="right">35.8%</td>
<td align="right">550,637</td>
<td align="right">35.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">27,603</td>
<td align="right">1.8%</td>
<td align="right">27,603</td>
<td align="right">1.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">17,602</td>
<td align="right">1.1%</td>
<td align="right">17,602</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">13,440</td>
<td align="right">0.9%</td>
<td align="right">13,440</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">3,916</td>
<td align="right">0.3%</td>
<td align="right">3,916</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">non string or split</td>
<td align="right">3,620</td>
<td align="right">0.2%</td>
<td align="right">3,620</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">2,360</td>
<td align="right">0.2%</td>
<td align="right">2,360</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">1,100</td>
<td align="right">0.1%</td>
<td align="right">1,100</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">property</td>
<td align="right">60</td>
<td align="right">0.0%</td>
<td align="right">60</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">expected error</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">20</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">366,127</td>
<td align="right">0.0%</td>
<td align="right">365,124</td>
<td align="right">0.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">9,677,492,651</td>
<td align="right">99.8%</td>
<td align="right">9,663,845,172</td>
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
<td align="right">20,500,127</td>
<td align="right">0.2%</td>
<td align="right">20,499,351</td>
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
<td align="right">12,962</td>
<td align="right">0.0%</td>
<td align="right">12,962</td>
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
<td align="right">669,079</td>
<td align="right">100.0%</td>
<td align="right">669,135</td>
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
<td align="right">134,867,525</td>
<td align="right">100.0%</td>
<td align="right">134,945,703</td>
<td align="right">100.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">11,826</td>
<td align="right">0.0%</td>
<td align="right">11,831</td>
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
<td align="right">11,697</td>
<td align="right">100.0%</td>
<td align="right">11,697</td>
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
<td align="right">787,183,128</td>
<td align="right">81.9%</td>
<td align="right">787,184,454</td>
<td align="right">81.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">173,830,042</td>
<td align="right">18.1%</td>
<td align="right">173,830,239</td>
<td align="right">18.1%</td>
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
<td align="right">30,900</td>
<td align="right">0.0%</td>
<td align="right">30,900</td>
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
<td align="right">7,174</td>
<td align="right">10.4%</td>
<td align="right">7,173</td>
<td align="right">10.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">61,749</td>
<td align="right">89.6%</td>
<td align="right">61,745</td>
<td align="right">89.6%</td>
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
<td align="right">16,129</td>
<td align="right">26.1%</td>
<td align="right">16,125</td>
<td align="right">26.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">53.7%</td>
<td align="right">33,180</td>
<td align="right">53.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">9,980</td>
<td align="right">16.2%</td>
<td align="right">9,980</td>
<td align="right">16.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">2,220</td>
<td align="right">3.6%</td>
<td align="right">2,220</td>
<td align="right">3.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">240</td>
<td align="right">0.4%</td>
<td align="right">240</td>
<td align="right">0.4%</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">2,578,606,202</td>
<td align="right">91.4%</td>
<td align="right">2,570,206,601</td>
<td align="right">91.4%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">239,637,865</td>
<td align="right">8.5%</td>
<td align="right">238,894,947</td>
<td align="right">8.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">170,050,866</td>
<td align="right">6.0%</td>
<td align="right">170,022,514</td>
<td align="right">6.0%</td>
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
<td align="right">131,797</td>
<td align="right">3.8%</td>
<td align="right">131,481</td>
<td align="right">3.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">3,365,109</td>
<td align="right">96.2%</td>
<td align="right">3,364,594</td>
<td align="right">96.2%</td>
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
<td align="left">property</td>
<td align="right">5,720</td>
<td align="right">4.3%</td>
<td align="right">5,580</td>
<td align="right">4.2%</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,820</td>
<td align="right">8.2%</td>
<td align="right">10,660</td>
<td align="right">8.1%</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">3,440</td>
<td align="right">2.6%</td>
<td align="right">3,420</td>
<td align="right">2.6%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">28,510</td>
<td align="right">21.6%</td>
<td align="right">28,514</td>
<td align="right">21.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">50,315</td>
<td align="right">38.2%</td>
<td align="right">50,315</td>
<td align="right">38.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">15,765</td>
<td align="right">12.0%</td>
<td align="right">15,765</td>
<td align="right">12.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">8,201</td>
<td align="right">6.2%</td>
<td align="right">8,201</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">6,832</td>
<td align="right">5.2%</td>
<td align="right">6,832</td>
<td align="right">5.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">1,560</td>
<td align="right">1.2%</td>
<td align="right">1,560</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">594</td>
<td align="right">0.5%</td>
<td align="right">594</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">40</td>
<td align="right">0.0%</td>
<td align="right">40</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">415,376,349</td>
<td align="right">69.3%</td>
<td align="right">413,559,378</td>
<td align="right">69.3%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">183,970,807</td>
<td align="right">30.7%</td>
<td align="right">183,328,318</td>
<td align="right">30.7%</td>
<td align="right">-0.3%</td>
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
<td align="left">Failure</td>
<td align="right">96,562</td>
<td align="right">83.8%</td>
<td align="right">96,399</td>
<td align="right">83.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">18,665</td>
<td align="right">16.2%</td>
<td align="right">18,671</td>
<td align="right">16.2%</td>
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
<td align="left">array int</td>
<td align="right">15,300</td>
<td align="right">15.8%</td>
<td align="right">15,140</td>
<td align="right">15.7%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">29,935</td>
<td align="right">31.0%</td>
<td align="right">29,931</td>
<td align="right">31.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">43,579</td>
<td align="right">45.1%</td>
<td align="right">43,580</td>
<td align="right">45.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,828</td>
<td align="right">4.0%</td>
<td align="right">3,828</td>
<td align="right">4.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">2,080</td>
<td align="right">2.2%</td>
<td align="right">2,080</td>
<td align="right">2.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">1,840</td>
<td align="right">1.9%</td>
<td align="right">1,840</td>
<td align="right">1.9%</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">434,585,853</td>
<td align="right">7.5%</td>
<td align="right">433,246,114</td>
<td align="right">7.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">5,359,255,916</td>
<td align="right">92.5%</td>
<td align="right">5,350,823,884</td>
<td align="right">92.5%</td>
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
<td align="right">105,159,112</td>
<td align="right">1.8%</td>
<td align="right">105,127,262</td>
<td align="right">1.8%</td>
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
<td align="right">695,761</td>
<td align="right">23.5%</td>
<td align="right">695,340</td>
<td align="right">23.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,269,331</td>
<td align="right">76.5%</td>
<td align="right">2,268,768</td>
<td align="right">76.5%</td>
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
<td align="left">sequence</td>
<td align="right">18,423</td>
<td align="right">2.6%</td>
<td align="right">18,262</td>
<td align="right">2.6%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">40,231</td>
<td align="right">5.8%</td>
<td align="right">40,110</td>
<td align="right">5.8%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">19,041</td>
<td align="right">2.7%</td>
<td align="right">18,995</td>
<td align="right">2.7%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">99,766</td>
<td align="right">14.3%</td>
<td align="right">99,666</td>
<td align="right">14.3%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">175,598</td>
<td align="right">25.2%</td>
<td align="right">175,568</td>
<td align="right">25.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">45,092</td>
<td align="right">6.5%</td>
<td align="right">45,098</td>
<td align="right">6.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">109,636</td>
<td align="right">15.8%</td>
<td align="right">109,648</td>
<td align="right">15.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">183,694</td>
<td align="right">26.4%</td>
<td align="right">183,713</td>
<td align="right">26.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">float</td>
<td align="right">2,620</td>
<td align="right">0.4%</td>
<td align="right">2,620</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray</td>
<td align="right">1,240</td>
<td align="right">0.2%</td>
<td align="right">1,240</td>
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
<td align="right">988,059,188</td>
<td align="right">99.9%</td>
<td align="right">987,410,728</td>
<td align="right">99.9%</td>
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
<td align="right">933,655</td>
<td align="right">0.1%</td>
<td align="right">933,735</td>
<td align="right">0.1%</td>
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
<td align="right">426,660</td>
<td align="right">0.0%</td>
<td align="right">426,660</td>
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
<td align="right">3,577</td>
<td align="right">6.0%</td>
<td align="right">3,579</td>
<td align="right">6.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">55,952</td>
<td align="right">94.0%</td>
<td align="right">55,977</td>
<td align="right">94.0%</td>
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
<td align="right">2,436</td>
<td align="right">68.1%</td>
<td align="right">2,438</td>
<td align="right">68.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">761</td>
<td align="right">21.3%</td>
<td align="right">761</td>
<td align="right">21.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">10.6%</td>
<td align="right">380</td>
<td align="right">10.6%</td>
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
Not specialized
<details>
<summary>ⓘ</summary>

Instructions that could be specialized but aren't, e.g. `LOAD_ATTR`, `BINARY_SLICE`.
</details>
</td>
<td align="right">16,576,688,266</td>
<td align="right">10.2%</td>
<td align="right">16,520,154,554</td>
<td align="right">10.2%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">57,619,235,379</td>
<td align="right">35.5%</td>
<td align="right">57,453,609,680</td>
<td align="right">35.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">86,706,395,711</td>
<td align="right">53.4%</td>
<td align="right">86,488,290,277</td>
<td align="right">53.4%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,501,167,982</td>
<td align="right">0.9%</td>
<td align="right">1,497,770,671</td>
<td align="right">0.9%</td>
<td align="right">-0.2%</td>
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
<td align="left">BINARY_SUBSCR</td>
<td align="right">556,316,076</td>
<td align="right">7.7%</td>
<td align="right">549,717,614</td>
<td align="right">7.6%</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">509,586,918</td>
<td align="right">7.1%</td>
<td align="right">505,943,626</td>
<td align="right">7.0%</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">183,970,807</td>
<td align="right">2.5%</td>
<td align="right">183,328,318</td>
<td align="right">2.5%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">239,637,865</td>
<td align="right">3.3%</td>
<td align="right">238,894,947</td>
<td align="right">3.3%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">434,585,853</td>
<td align="right">6.0%</td>
<td align="right">433,246,114</td>
<td align="right">6.0%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">293,759,739</td>
<td align="right">4.1%</td>
<td align="right">292,905,897</td>
<td align="right">4.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,511,297,260</td>
<td align="right">20.9%</td>
<td align="right">1,507,217,279</td>
<td align="right">20.9%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">2,246,975,750</td>
<td align="right">31.1%</td>
<td align="right">2,243,826,868</td>
<td align="right">31.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">886,985,322</td>
<td align="right">12.3%</td>
<td align="right">887,217,892</td>
<td align="right">12.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">173,830,042</td>
<td align="right">2.4%</td>
<td align="right">173,830,239</td>
<td align="right">2.4%</td>
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
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">133,485,291</td>
<td align="right">8.9%</td>
<td align="right">130,916,024</td>
<td align="right">8.7%</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">71,422,749</td>
<td align="right">4.8%</td>
<td align="right">71,279,705</td>
<td align="right">4.8%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">71,327,441</td>
<td align="right">4.7%</td>
<td align="right">71,264,170</td>
<td align="right">4.8%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">49,300,666</td>
<td align="right">3.3%</td>
<td align="right">49,284,541</td>
<td align="right">3.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">99,144,233</td>
<td align="right">6.6%</td>
<td align="right">99,117,791</td>
<td align="right">6.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">252,916,060</td>
<td align="right">16.8%</td>
<td align="right">252,961,607</td>
<td align="right">16.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">70,741,822</td>
<td align="right">4.7%</td>
<td align="right">70,738,293</td>
<td align="right">4.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">70,852,708</td>
<td align="right">4.7%</td>
<td align="right">70,850,788</td>
<td align="right">4.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">108,747,591</td>
<td align="right">7.2%</td>
<td align="right">108,746,222</td>
<td align="right">7.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">289,317,131</td>
<td align="right">19.3%</td>
<td align="right">289,316,811</td>
<td align="right">19.3%</td>
<td align="right">-0.0%</td>
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
<td align="left">Calls to Python functions inlined</td>
<td align="right">5,726,724,865</td>
<td align="right">71.1%</td>
<td align="right">5,712,208,571</td>
<td align="right">71.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">5,042,920,989</td>
<td align="right">62.6%</td>
<td align="right">5,032,430,693</td>
<td align="right">62.6%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">254,906,365</td>
<td align="right">3.2%</td>
<td align="right">254,728,470</td>
<td align="right">3.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">883,077,030</td>
<td align="right">11.0%</td>
<td align="right">883,287,734</td>
<td align="right">11.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,326,918,698</td>
<td align="right">28.9%</td>
<td align="right">2,327,068,470</td>
<td align="right">28.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,326,918,698</td>
<td align="right">28.9%</td>
<td align="right">2,327,068,470</td>
<td align="right">28.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,438,514,398</td>
<td align="right">17.9%</td>
<td align="right">1,438,453,466</td>
<td align="right">17.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,443,841,668</td>
<td align="right">17.9%</td>
<td align="right">1,443,780,736</td>
<td align="right">18.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">474,625,435</td>
<td align="right">5.9%</td>
<td align="right">474,614,419</td>
<td align="right">5.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">38,685,649</td>
<td align="right">0.5%</td>
<td align="right">38,684,803</td>
<td align="right">0.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">88,589,458</td>
<td align="right">1.1%</td>
<td align="right">88,587,973</td>
<td align="right">1.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">213,355,252</td>
<td align="right">2.6%</td>
<td align="right">213,357,047</td>
<td align="right">2.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">5,298,384</td>
<td align="right">0.1%</td>
<td align="right">5,298,384</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (build class)</td>
<td align="right">28,886</td>
<td align="right">0.0%</td>
<td align="right">28,886</td>
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
<td align="left">Method cache misses</td>
<td align="right">81,969,626</td>
<td align="right"></td>
<td align="right">77,916,926</td>
<td align="right"></td>
<td align="right">-4.9%</td>
</tr>
<tr>
<td align="left">Method cache collisions</td>
<td align="right">87,918,368</td>
<td align="right"></td>
<td align="right">83,679,799</td>
<td align="right"></td>
<td align="right">-4.8%</td>
</tr>
<tr>
<td align="left">Method cache dunder misses</td>
<td align="right">13,702,669</td>
<td align="right"></td>
<td align="right">13,516,832</td>
<td align="right"></td>
<td align="right">-1.4%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,917,299,518</td>
<td align="right">36.3%</td>
<td align="right">6,846,703,470</td>
<td align="right">36.2%</td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,925,219,422</td>
<td align="right"></td>
<td align="right">6,854,628,869</td>
<td align="right"></td>
<td align="right">-1.0%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">12,018,016,392</td>
<td align="right">63.0%</td>
<td align="right">11,955,072,653</td>
<td align="right">63.2%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">12,144,656,246</td>
<td align="right">63.7%</td>
<td align="right">12,081,565,166</td>
<td align="right">63.8%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">109,455,989,771</td>
<td align="right">78.4%</td>
<td align="right">108,910,269,468</td>
<td align="right">78.4%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">12,469,018,420</td>
<td align="right"></td>
<td align="right">12,407,529,177</td>
<td align="right"></td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">27,066,424,022</td>
<td align="right">22.2%</td>
<td align="right">26,942,847,396</td>
<td align="right">22.2%</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">94,694,555,039</td>
<td align="right">77.8%</td>
<td align="right">94,282,517,392</td>
<td align="right">77.8%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">30,108,523,753</td>
<td align="right">21.6%</td>
<td align="right">29,990,220,167</td>
<td align="right">21.6%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">105,488,944</td>
<td align="right">0.6%</td>
<td align="right">105,347,496</td>
<td align="right">0.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">New values</td>
<td align="right">90,988,734</td>
<td align="right"></td>
<td align="right">91,025,357</td>
<td align="right"></td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">21,150,910</td>
<td align="right">0.1%</td>
<td align="right">21,145,017</td>
<td align="right">0.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,604,490,032</td>
<td align="right"></td>
<td align="right">3,603,522,278</td>
<td align="right"></td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,330,142,588</td>
<td align="right"></td>
<td align="right">3,329,950,620</td>
<td align="right"></td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,704,847</td>
<td align="right">3.0%</td>
<td align="right">2,704,848</td>
<td align="right">3.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">4,273,412</td>
<td align="right">4.7%</td>
<td align="right">4,273,413</td>
<td align="right">4.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (new key)</td>
<td align="right">215,335</td>
<td align="right">0.2%</td>
<td align="right">215,335</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (too big)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left">Materialize dict (str subclass)</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
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
<td align="right">749,207</td>
<td align="right">47,225,608</td>
<td align="right">6,192,183,626</td>
<td align="right">747,651</td>
<td align="right">47,227,645</td>
<td align="right">6,183,399,676</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">67,043</td>
<td align="right">36,518,316</td>
<td align="right">5,060,015,064</td>
<td align="right">66,904</td>
<td align="right">36,517,762</td>
<td align="right">5,053,511,900</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">21,016</td>
<td align="right">53,583,558</td>
<td align="right">18,410,319,538</td>
<td align="right">21,017</td>
<td align="right">53,583,532</td>
<td align="right">18,412,438,596</td>
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
Trace stack overflow
<details>
<summary>ⓘ</summary>

A trace is truncated because it would require more than 5 stack frames.
</details>
</td>
<td align="right">394</td>
<td align="right">0.1%</td>
<td align="right">389</td>
<td align="right">0.1%</td>
<td align="right">-1.3%</td>
</tr>
<tr>
<td align="left">
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">298,425</td>
<td align="right">101.9%</td>
<td align="right">301,341</td>
<td align="right">103.0%</td>
<td align="right">1.0%</td>
</tr>
<tr>
<td align="left">
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">144,291,654,999</td>
<td align="right">2,729.7%</td>
<td align="right">142,976,499,464</td>
<td align="right">2,708.5%</td>
<td align="right">-0.9%</td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">6,570</td>
<td align="right">2.2%</td>
<td align="right">6,548</td>
<td align="right">2.2%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">5,512,971</td>
<td align="right">1,882.6%</td>
<td align="right">5,500,225</td>
<td align="right">1,880.9%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">292,838</td>
<td align="right"></td>
<td align="right">292,432</td>
<td align="right"></td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">5,286,007,705</td>
<td align="right"></td>
<td align="right">5,278,790,906</td>
<td align="right"></td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">35,127,532</td>
<td align="right">11,995.6%</td>
<td align="right">35,095,076</td>
<td align="right">12,001.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">2,208,641</td>
<td align="right">754.2%</td>
<td align="right">2,208,336</td>
<td align="right">755.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">751,942</td>
<td align="right">256.8%</td>
<td align="right">751,943</td>
<td align="right">257.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Trace too long
<details>
<summary>ⓘ</summary>

A trace is truncated because it is longer than the instruction buffer.
</details>
</td>
<td align="right">280</td>
<td align="right">0.1%</td>
<td align="right">280</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Executors invalidated
<details>
<summary>ⓘ</summary>

The number of executors that were invalidated due to watched dictionary changes.
</details>
</td>
<td align="right">5,500</td>
<td align="right">0.2%</td>
<td align="right">5,500</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
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
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">3,039</td>
<td align="right">0.1%</td>
<td align="right">3,047</td>
<td align="right">0.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">779,306</td>
<td align="right">35.3%</td>
<td align="right">780,037</td>
<td align="right">35.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">167,362</td>
<td align="right">7.6%</td>
<td align="right">167,300</td>
<td align="right">7.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">764,111</td>
<td align="right">34.6%</td>
<td align="right">763,135</td>
<td align="right">34.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">486,732</td>
<td align="right">22.0%</td>
<td align="right">486,738</td>
<td align="right">22.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">7,089</td>
<td align="right">0.3%</td>
<td align="right">7,077</td>
<td align="right">0.3%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">1,002</td>
<td align="right">0.0%</td>
<td align="right">1,002</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">2,080</td>
<td align="right">0.1%</td>
<td align="right">2,088</td>
<td align="right">0.1%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">23,649</td>
<td align="right">1.1%</td>
<td align="right">23,673</td>
<td align="right">1.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">31,108</td>
<td align="right">1.4%</td>
<td align="right">31,059</td>
<td align="right">1.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">19,368</td>
<td align="right">0.9%</td>
<td align="right">19,336</td>
<td align="right">0.9%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">9,347</td>
<td align="right">0.4%</td>
<td align="right">9,352</td>
<td align="right">0.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">2,593</td>
<td align="right">0.1%</td>
<td align="right">2,573</td>
<td align="right">0.1%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">740</td>
<td align="right">0.0%</td>
<td align="right">740</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
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
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 2</td>
<td align="right">22,692,640</td>
<td align="right">0.4%</td>
<td align="right">22,692,640</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">640,194,391</td>
<td align="right">12.1%</td>
<td align="right">639,653,021</td>
<td align="right">12.1%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">746,705,815</td>
<td align="right">14.1%</td>
<td align="right">746,711,420</td>
<td align="right">14.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">1,055,330,850</td>
<td align="right">20.0%</td>
<td align="right">1,054,026,498</td>
<td align="right">20.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">964,054,378</td>
<td align="right">18.2%</td>
<td align="right">960,177,188</td>
<td align="right">18.2%</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">320,498,498</td>
<td align="right">6.1%</td>
<td align="right">325,638,320</td>
<td align="right">6.2%</td>
<td align="right">1.6%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">205,529,907</td>
<td align="right">3.9%</td>
<td align="right">200,620,766</td>
<td align="right">3.8%</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">93,954,858</td>
<td align="right">1.8%</td>
<td align="right">93,913,327</td>
<td align="right">1.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">24,754,195</td>
<td align="right">0.5%</td>
<td align="right">24,740,254</td>
<td align="right">0.5%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">7,017,329</td>
<td align="right">0.1%</td>
<td align="right">7,032,041</td>
<td align="right">0.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">17,734,691</td>
<td align="right">0.3%</td>
<td align="right">17,079,972</td>
<td align="right">0.3%</td>
<td align="right">-3.7%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">1,942,481</td>
<td align="right">0.0%</td>
<td align="right">1,942,482</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">133,482</td>
<td align="right">0.0%</td>
<td align="right">133,464</td>
<td align="right">0.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left"><= 16,384</td>
<td align="right">74,940</td>
<td align="right">0.0%</td>
<td align="right">74,940</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 32,768</td>
<td align="right">40,960</td>
<td align="right">0.0%</td>
<td align="right">40,960</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 65,536</td>
<td align="right">12,960</td>
<td align="right">0.0%</td>
<td align="right">12,960</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 131,072</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 262,144</td>
<td align="right">1,920</td>
<td align="right">0.0%</td>
<td align="right">1,920</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 524,288</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">320</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 1,048,576</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">400</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 2,097,152</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 4,194,304</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 8,388,608</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right"></td>
</tr>
<tr>
<td align="left"><= 16,777,216</td>
<td align="right">240</td>
<td align="right">0.0%</td>
<td align="right">240</td>
<td align="right">0.0%</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Uop execution stats

<details>
<summary> uop execution stats </summary>

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
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_1</td>
<td align="right">6,115,032</td>
<td align="right">3,373,352</td>
<td align="right">-44.8%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES</td>
<td align="right">103,186,059</td>
<td align="right">75,924,590</td>
<td align="right">-26.4%</td>
</tr>
<tr>
<td align="left">_CHECK_MANAGED_OBJECT_HAS_VALUES</td>
<td align="right">1,590,331,919</td>
<td align="right">1,248,960,791</td>
<td align="right">-21.5%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_LIST</td>
<td align="right">23,336,252</td>
<td align="right">19,899,498</td>
<td align="right">-14.7%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR</td>
<td align="right">1,116,379,885</td>
<td align="right">1,022,245,371</td>
<td align="right">-8.4%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_FLOAT</td>
<td align="right">489,054,520</td>
<td align="right">457,694,520</td>
<td align="right">-6.4%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">51,797,866</td>
<td align="right">49,056,186</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">_CHECK_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">51,857,706</td>
<td align="right">49,116,026</td>
<td align="right">-5.3%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_RANGE</td>
<td align="right">672,138,723</td>
<td align="right">640,160,476</td>
<td align="right">-4.8%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_RANGE</td>
<td align="right">714,268,287</td>
<td align="right">681,661,647</td>
<td align="right">-4.6%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_RANGE</td>
<td align="right">715,626,047</td>
<td align="right">683,019,407</td>
<td align="right">-4.6%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_FLOAT</td>
<td align="right">1,464,732,296</td>
<td align="right">1,402,012,432</td>
<td align="right">-4.3%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">1,100,461,940</td>
<td align="right">1,069,101,940</td>
<td align="right">-2.8%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS</td>
<td align="right">423,934</td>
<td align="right">435,056</td>
<td align="right">2.6%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_5</td>
<td align="right">1,405,440,183</td>
<td align="right">1,373,603,342</td>
<td align="right">-2.3%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST</td>
<td align="right">4,295,875,640</td>
<td align="right">4,201,763,059</td>
<td align="right">-2.2%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_4</td>
<td align="right">1,534,712,380</td>
<td align="right">1,502,605,127</td>
<td align="right">-2.1%</td>
</tr>
<tr>
<td align="left">_TO_BOOL</td>
<td align="right">177,883,464</td>
<td align="right">174,446,264</td>
<td align="right">-1.9%</td>
</tr>
<tr>
<td align="left">_JUMP_TO_TOP</td>
<td align="right">1,884,845,744</td>
<td align="right">1,853,413,647</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_2</td>
<td align="right">1,882,190,436</td>
<td align="right">1,851,032,839</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY_AND_SET_IP</td>
<td align="right">2,064,375,029</td>
<td align="right">2,032,413,599</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">_STORE_FAST</td>
<td align="right">4,159,730,406</td>
<td align="right">4,095,669,793</td>
<td align="right">-1.5%</td>
</tr>
<tr>
<td align="left">_CALL_ISINSTANCE</td>
<td align="right">5,227,334</td>
<td align="right">5,286,980</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY</td>
<td align="right">17,403,815,961</td>
<td align="right">17,267,788,503</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_0</td>
<td align="right">1,584,116,367</td>
<td align="right">1,572,208,313</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_3</td>
<td align="right">5,576,113</td>
<td align="right">5,617,407</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">_SET_IP</td>
<td align="right">14,852,694,472</td>
<td align="right">14,750,554,298</td>
<td align="right">-0.7%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_2</td>
<td align="right">33,141,509</td>
<td align="right">33,352,480</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_AND_CLEAR</td>
<td align="right">13,741,735</td>
<td align="right">13,660,135</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP</td>
<td align="right">98,328,039</td>
<td align="right">97,768,161</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">137,224,498</td>
<td align="right">136,533,058</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_CHECK</td>
<td align="right">76,065</td>
<td align="right">76,394</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_TYPE_VERSION</td>
<td align="right">4,155,147,155</td>
<td align="right">4,140,152,775</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_CLASS</td>
<td align="right">6,511,882</td>
<td align="right">6,534,766</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_MAKE_CELL</td>
<td align="right">108,332</td>
<td align="right">108,686</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION_EXACT_ARGS</td>
<td align="right">861,605,960</td>
<td align="right">859,041,281</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_0</td>
<td align="right">3,886,087,100</td>
<td align="right">3,875,944,117</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_FALSE_POP</td>
<td align="right">4,154,823,914</td>
<td align="right">4,145,467,290</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_COPY_FREE_VARS</td>
<td align="right">96,955</td>
<td align="right">96,751</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_CLASS</td>
<td align="right">19,466,687</td>
<td align="right">19,506,953</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE</td>
<td align="right">315,032,177</td>
<td align="right">314,534,307</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_START_EXECUTOR</td>
<td align="right">4,100,675,815</td>
<td align="right">4,094,493,693</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">542,173,719</td>
<td align="right">541,437,852</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_BOOL</td>
<td align="right">685,028,613</td>
<td align="right">684,128,582</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_DEREF</td>
<td align="right">418,795,762</td>
<td align="right">419,193,457</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_COLD_EXIT</td>
<td align="right">1,185,331,890</td>
<td align="right">1,184,297,213</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">207,745,220</td>
<td align="right">207,911,800</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_BINARY_OP</td>
<td align="right">650,775,909</td>
<td align="right">650,284,869</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_POP_FRAME</td>
<td align="right">361,573,537</td>
<td align="right">361,843,030</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_6</td>
<td align="right">1,057,513,013</td>
<td align="right">1,056,795,142</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">597,754,700</td>
<td align="right">598,146,175</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_EXIT_TRACE</td>
<td align="right">1,591,782,967</td>
<td align="right">1,590,771,493</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_BUILD_LIST</td>
<td align="right">127,485,012</td>
<td align="right">127,404,548</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">648,993,951</td>
<td align="right">649,400,030</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION</td>
<td align="right">995,986,954</td>
<td align="right">995,367,646</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_TRUE_POP</td>
<td align="right">1,580,151,776</td>
<td align="right">1,581,068,993</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_KEYS_VERSION</td>
<td align="right">728,810,803</td>
<td align="right">729,217,009</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES_INST_ATTR_FROM_DICT</td>
<td align="right">728,817,289</td>
<td align="right">729,223,495</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">8,785,261</td>
<td align="right">8,780,895</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_6</td>
<td align="right">633,663,658</td>
<td align="right">633,383,800</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_MODULE</td>
<td align="right">7,722,997</td>
<td align="right">7,719,731</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_MODULE</td>
<td align="right">7,722,997</td>
<td align="right">7,719,731</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GET_ITER</td>
<td align="right">57,961,213</td>
<td align="right">57,984,968</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_LIST</td>
<td align="right">1,365,886,907</td>
<td align="right">1,365,377,343</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_3</td>
<td align="right">2,395,473,705</td>
<td align="right">2,394,615,189</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_TUPLE</td>
<td align="right">2,418,380</td>
<td align="right">2,417,553</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_TUPLE</td>
<td align="right">408,488,350</td>
<td align="right">408,348,697</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_TUPLE</td>
<td align="right">153,133,094</td>
<td align="right">153,178,894</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_TUPLE</td>
<td align="right">258,932,429</td>
<td align="right">258,855,927</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_TUPLE</td>
<td align="right">479,766,504</td>
<td align="right">479,627,785</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_LEN</td>
<td align="right">48,772,899</td>
<td align="right">48,785,517</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_1</td>
<td align="right">272,044,686</td>
<td align="right">271,975,943</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_STACK_SPACE</td>
<td align="right">811,366,781</td>
<td align="right">811,563,036</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_RESUME_CHECK</td>
<td align="right">811,282,959</td>
<td align="right">811,479,127</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_PUSH_FRAME</td>
<td align="right">811,326,304</td>
<td align="right">811,522,268</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SAVE_RETURN_OFFSET</td>
<td align="right">811,326,304</td>
<td align="right">811,522,268</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NOT_NONE_POP</td>
<td align="right">103,681,936</td>
<td align="right">103,705,206</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_3</td>
<td align="right">516,311,341</td>
<td align="right">516,424,249</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_DICT</td>
<td align="right">218,839,703</td>
<td align="right">218,886,963</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP</td>
<td align="right">1,298,739,109</td>
<td align="right">1,298,465,663</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_CLASS_0</td>
<td align="right">18,321,987</td>
<td align="right">18,325,593</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_2</td>
<td align="right">633,260,662</td>
<td align="right">633,370,812</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL</td>
<td align="right">104,012,711</td>
<td align="right">104,030,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_7</td>
<td align="right">1,344,533,229</td>
<td align="right">1,344,760,713</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_LIST</td>
<td align="right">1,349,608,639</td>
<td align="right">1,349,382,252</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP</td>
<td align="right">273,694,837</td>
<td align="right">273,738,181</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SWAP</td>
<td align="right">1,031,371,800</td>
<td align="right">1,031,209,143</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_INT</td>
<td align="right">169,976,547</td>
<td align="right">169,951,011</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW_WITH_NULL</td>
<td align="right">152,414,397</td>
<td align="right">152,437,281</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NONE_POP</td>
<td align="right">38,766,240</td>
<td align="right">38,771,490</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_REPLACE_WITH_TRUE</td>
<td align="right">27,258,639</td>
<td align="right">27,262,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_1</td>
<td align="right">1,836,824,247</td>
<td align="right">1,837,030,082</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">14,466,201</td>
<td align="right">14,464,638</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_7</td>
<td align="right">3,064,896,161</td>
<td align="right">3,065,209,205</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_LIST</td>
<td align="right">1,116,574,438</td>
<td align="right">1,116,475,519</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_1</td>
<td align="right">5,229,999,481</td>
<td align="right">5,229,593,762</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR</td>
<td align="right">479,403,305</td>
<td align="right">479,437,569</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_FOR_ITER_TIER_TWO</td>
<td align="right">404,599,792</td>
<td align="right">404,626,510</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAP_ADD</td>
<td align="right">15,931,198</td>
<td align="right">15,932,044</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_PUSH_NULL</td>
<td align="right">488,688,261</td>
<td align="right">488,707,899</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BEFORE_WITH</td>
<td align="right">113,207</td>
<td align="right">113,203</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_SET</td>
<td align="right">73,173,587</td>
<td align="right">73,175,956</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_O</td>
<td align="right">156,461,136</td>
<td align="right">156,456,459</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW</td>
<td align="right">6,479,413,629</td>
<td align="right">6,479,599,084</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_SLOT</td>
<td align="right">115,442,994</td>
<td align="right">115,439,705</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_LIST_INT</td>
<td align="right">950,056,533</td>
<td align="right">950,078,353</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_MAKE_FUNCTION</td>
<td align="right">1,882,885</td>
<td align="right">1,882,908</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR</td>
<td align="right">267,693,666</td>
<td align="right">267,696,759</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">102,490,119</td>
<td align="right">102,488,959</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_WITH_NULL</td>
<td align="right">416,985,956</td>
<td align="right">416,981,565</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_LIST</td>
<td align="right">77,416,880</td>
<td align="right">77,416,320</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CALL_INTRINSIC_1</td>
<td align="right">97,608,052</td>
<td align="right">97,608,674</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LIST_EXTEND</td>
<td align="right">98,527,092</td>
<td align="right">98,527,714</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_0</td>
<td align="right">212,130,095</td>
<td align="right">212,131,418</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SLICE</td>
<td align="right">69,712,884</td>
<td align="right">69,712,564</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LIST_APPEND</td>
<td align="right">169,241,556</td>
<td align="right">169,242,083</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_FLOAT</td>
<td align="right">57,693,176</td>
<td align="right">57,693,312</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_INT</td>
<td align="right">719,635,715</td>
<td align="right">719,634,049</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE</td>
<td align="right">4,164,677</td>
<td align="right">4,164,668</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_DICT</td>
<td align="right">208,170,385</td>
<td align="right">208,169,937</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_INT</td>
<td align="right">326,031,591</td>
<td align="right">326,032,170</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_DICT</td>
<td align="right">27,953,902</td>
<td align="right">27,953,855</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_5</td>
<td align="right">817,251,473</td>
<td align="right">817,252,777</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_INT</td>
<td align="right">1,925,515,313</td>
<td align="right">1,925,513,057</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COPY</td>
<td align="right">1,007,927,665</td>
<td align="right">1,007,926,514</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_INT</td>
<td align="right">2,593,049,859</td>
<td align="right">2,593,047,224</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_WITH_HINT</td>
<td align="right">86,426,706</td>
<td align="right">86,426,622</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_WITH_HINT</td>
<td align="right">86,427,266</td>
<td align="right">86,427,182</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_IS_OP</td>
<td align="right">54,615,291</td>
<td align="right">54,615,331</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_NONE</td>
<td align="right">68,854,255</td>
<td align="right">68,854,303</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_UNICODE</td>
<td align="right">954,286,203</td>
<td align="right">954,285,603</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">138,643,886</td>
<td align="right">138,643,801</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL_STR</td>
<td align="right">21,457,799</td>
<td align="right">21,457,791</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_0</td>
<td align="right">658,067,692</td>
<td align="right">658,067,936</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_4</td>
<td align="right">547,848,946</td>
<td align="right">547,849,142</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_UNICODE</td>
<td align="right">22,697,241</td>
<td align="right">22,697,233</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_MAP</td>
<td align="right">2,907,121</td>
<td align="right">2,907,122</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR_STR_INT</td>
<td align="right">1,175,683,966</td>
<td align="right">1,175,683,570</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP_STR</td>
<td align="right">1,813,345,650</td>
<td align="right">1,813,345,050</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NEGATIVE</td>
<td align="right">30,182,077</td>
<td align="right">30,182,083</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST</td>
<td align="right">391,120,892</td>
<td align="right">391,120,830</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_STR</td>
<td align="right">28,150,105</td>
<td align="right">28,150,108</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONTAINS_OP_LIST</td>
<td align="right">50,311,508</td>
<td align="right">50,311,506</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_4</td>
<td align="right">288,009,967</td>
<td align="right">288,009,964</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR_LIST_INT</td>
<td align="right">446,386,480</td>
<td align="right">446,386,480</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE_TUPLE</td>
<td align="right">443,337,445</td>
<td align="right">443,337,445</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">368,976,020</td>
<td align="right">368,976,020</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_TYPE_1</td>
<td align="right">144,224,323</td>
<td align="right">144,224,323</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SLICE</td>
<td align="right">143,141,120</td>
<td align="right">143,141,120</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_SLICE</td>
<td align="right">138,499,780</td>
<td align="right">138,499,780</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GET_ANEXT</td>
<td align="right">125,514,720</td>
<td align="right">125,514,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_INT</td>
<td align="right">96,155,640</td>
<td align="right">96,155,640</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">78,411,090</td>
<td align="right">78,411,090</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_GLOBALS_VERSION</td>
<td align="right">63,840,560</td>
<td align="right">63,840,560</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,536,180</td>
<td align="right">57,536,180</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,536,180</td>
<td align="right">57,536,180</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_MODULE</td>
<td align="right">57,391,240</td>
<td align="right">57,391,240</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR</td>
<td align="right">49,553,205</td>
<td align="right">49,553,205</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_0</td>
<td align="right">40,187,629</td>
<td align="right">40,187,629</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_INVERT</td>
<td align="right">12,537,420</td>
<td align="right">12,537,420</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">8,992,706</td>
<td align="right">8,992,706</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_FORMAT_SIMPLE</td>
<td align="right">8,828,681</td>
<td align="right">8,828,681</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">8,761,321</td>
<td align="right">8,761,321</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_BUILTINS</td>
<td align="right">4,589,720</td>
<td align="right">4,589,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_STRING</td>
<td align="right">3,283,036</td>
<td align="right">3,283,036</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_STR_1</td>
<td align="right">2,997,300</td>
<td align="right">2,997,300</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_DEREF</td>
<td align="right">2,861,908</td>
<td align="right">2,861,908</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_NAME</td>
<td align="right">1,810,080</td>
<td align="right">1,810,080</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SET_ADD</td>
<td align="right">1,449,343</td>
<td align="right">1,449,343</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_DELETE_SUBSCR</td>
<td align="right">1,416,700</td>
<td align="right">1,416,700</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_GLOBAL</td>
<td align="right">1,260,560</td>
<td align="right">1,260,560</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_POP_TOP_LOAD_CONST_INLINE_BORROW</td>
<td align="right">676,034</td>
<td align="right">676,034</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_NAME</td>
<td align="right">581,900</td>
<td align="right">581,900</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNARY_NOT</td>
<td align="right">426,290</td>
<td align="right">426,290</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_DICT_MERGE</td>
<td align="right">360,540</td>
<td align="right">360,540</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CONVERT_VALUE</td>
<td align="right">82,800</td>
<td align="right">82,800</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SET_FUNCTION_ATTRIBUTE</td>
<td align="right">22,680</td>
<td align="right">22,680</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_SET</td>
<td align="right">6,861</td>
<td align="right">6,861</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CALL_TUPLE_1</td>
<td align="right">2,020</td>
<td align="right">2,020</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BUILD_CONST_KEY_MAP</td>
<td align="right">987</td>
<td align="right">987</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_FORMAT_WITH_SPEC</td>
<td align="right">680</td>
<td align="right">680</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

### Unsupported opcodes

<details>
<summary> unsupported opcodes </summary>

<table>
<thead>
<tr>
<th align="left">Opcode</th>
<th align="right">Base Count</th>
<th align="right">Head Count</th>
<th align="right">Change</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">93,385</td>
<td align="right">93,065</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">1,636</td>
<td align="right">1,633</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">13,745,908</td>
<td align="right">13,724,289</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">88,516</td>
<td align="right">88,476</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">5,694</td>
<td align="right">5,695</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">8,100,437</td>
<td align="right">8,099,735</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">12,808</td>
<td align="right">12,807</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">44,859</td>
<td align="right">44,856</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">3,065,006</td>
<td align="right">3,065,023</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">3,922,400</td>
<td align="right">3,922,400</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">219,017</td>
<td align="right">219,017</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">74,041</td>
<td align="right">74,041</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">415</td>
<td align="right">415</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">140</td>
<td align="right">140</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">80</td>
<td align="right">80</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


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
<td align="right">261</td>
<td align="right">261</td>
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
<td align="right">441</td>
<td align="right">441</td>
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
<td align="right">1,060</td>
<td align="right">1,060</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
watched globals modification
<details>
<summary>ⓘ</summary>

A watched `globals()` dict has been modified
</details>
</td>
<td align="right">1,060</td>
<td align="right">1,060</td>
<td align="right">0.0%</td>
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
<td align="right">2,020</td>
<td align="right">2,020</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

---
Stats gathered on: 2024-03-07
