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
<td align="left">UNARY_INVERT</td>
<td align="right">1,893,373</td>
<td align="right">2,698,916</td>
<td align="right">42.5%</td>
</tr>
<tr>
<td align="left">EXTENDED_ARG</td>
<td align="right">111,744,935</td>
<td align="right">93,909,698</td>
<td align="right">-16.0%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">149,348,644</td>
<td align="right">135,171,115</td>
<td align="right">-9.5%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">326,414,914</td>
<td align="right">309,478,375</td>
<td align="right">-5.2%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NONE</td>
<td align="right">390,719,113</td>
<td align="right">373,298,810</td>
<td align="right">-4.5%</td>
</tr>
<tr>
<td align="left">JUMP_FORWARD</td>
<td align="right">457,603,260</td>
<td align="right">440,447,573</td>
<td align="right">-3.7%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">8,786,670</td>
<td align="right">9,089,991</td>
<td align="right">3.5%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">463,754,488</td>
<td align="right">449,550,532</td>
<td align="right">-3.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">1,275,759,870</td>
<td align="right">1,244,892,721</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">139,947,681</td>
<td align="right">142,468,129</td>
<td align="right">1.8%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">10,282,281</td>
<td align="right">10,429,760</td>
<td align="right">1.4%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">1,326,044,339</td>
<td align="right">1,309,747,402</td>
<td align="right">-1.2%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">27,196,860</td>
<td align="right">27,420,770</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">STORE_FAST</td>
<td align="right">6,739,818,886</td>
<td align="right">6,688,824,506</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">ENTER_EXECUTOR</td>
<td align="right">2,330,854,989</td>
<td align="right">2,346,399,345</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">122,803,307</td>
<td align="right">123,609,979</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_ATTR</td>
<td align="right">5,276,396</td>
<td align="right">5,310,948</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">137,687,291</td>
<td align="right">138,498,561</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">BINARY_OP</td>
<td align="right">604,762,578</td>
<td align="right">608,130,272</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">207,166,179</td>
<td align="right">208,291,010</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">67,288,322</td>
<td align="right">67,635,452</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">33,805,512</td>
<td align="right">33,971,724</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">4,089,292,368</td>
<td align="right">4,069,706,596</td>
<td align="right">-0.5%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">594,803,708</td>
<td align="right">597,630,818</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_CONST</td>
<td align="right">6,468,754,683</td>
<td align="right">6,439,776,261</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_FALSE</td>
<td align="right">5,717,101,502</td>
<td align="right">5,691,714,641</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">DICT_UPDATE</td>
<td align="right">71,950</td>
<td align="right">71,631</td>
<td align="right">-0.4%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">28,128,935</td>
<td align="right">28,244,411</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">146,249,094</td>
<td align="right">146,830,099</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,111,151,743</td>
<td align="right">1,115,102,246</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">LOAD_FAST</td>
<td align="right">25,179,967,808</td>
<td align="right">25,094,014,994</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">210,821,652</td>
<td align="right">211,508,335</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">488,136,433</td>
<td align="right">489,610,900</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">150,108,049</td>
<td align="right">150,551,304</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">NOP</td>
<td align="right">984,509,785</td>
<td align="right">987,351,599</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,190,189,497</td>
<td align="right">1,193,602,825</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">111,868,589</td>
<td align="right">112,135,335</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">352,641,588</td>
<td align="right">353,455,803</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">1,965,177,819</td>
<td align="right">1,969,453,087</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_MODULE</td>
<td align="right">3,484,747,876</td>
<td align="right">3,477,195,279</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">135,206,639</td>
<td align="right">135,493,842</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">463,559,502</td>
<td align="right">464,506,581</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">114,408,616</td>
<td align="right">114,638,285</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_FLOAT</td>
<td align="right">57,147,520</td>
<td align="right">57,260,653</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CLEANUP_THROW</td>
<td align="right">1,523</td>
<td align="right">1,520</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">59,312,350</td>
<td align="right">59,426,620</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">713,734,216</td>
<td align="right">715,096,646</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">188,821,476</td>
<td align="right">189,174,063</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_NOT_NONE</td>
<td align="right">663,622,352</td>
<td align="right">664,841,479</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">71,901,483</td>
<td align="right">72,032,052</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">WITH_EXCEPT_START</td>
<td align="right">183,983</td>
<td align="right">184,301</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_MODULE</td>
<td align="right">496,438,171</td>
<td align="right">497,265,732</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">353,765,606</td>
<td align="right">354,325,154</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">3,475,108,138</td>
<td align="right">3,480,388,274</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">RETURN_CONST</td>
<td align="right">1,982,268,135</td>
<td align="right">1,985,244,707</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">3,136,955,487</td>
<td align="right">3,141,570,239</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">256,844,480</td>
<td align="right">257,193,815</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">6,822,354,677</td>
<td align="right">6,831,139,624</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">722,282,148</td>
<td align="right">723,198,871</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">RETURN_VALUE</td>
<td align="right">4,159,816,372</td>
<td align="right">4,164,821,733</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">27,769,921</td>
<td align="right">27,802,822</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">1,056,360,025</td>
<td align="right">1,057,610,252</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">564,376,486</td>
<td align="right">565,016,289</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD</td>
<td align="right">280,707,889</td>
<td align="right">281,025,533</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">813,847,641</td>
<td align="right">814,719,862</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INTERPRETER_EXIT</td>
<td align="right">2,253,822,629</td>
<td align="right">2,256,182,063</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">680,631,699</td>
<td align="right">681,300,139</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">DELETE_FAST</td>
<td align="right">2,157,437</td>
<td align="right">2,155,419</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_LOAD_FAST</td>
<td align="right">5,548,973,852</td>
<td align="right">5,554,070,080</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">776,935,266</td>
<td align="right">777,606,995</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">1,207,985,594</td>
<td align="right">1,209,021,419</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL_BUILTIN</td>
<td align="right">3,381,033,353</td>
<td align="right">3,383,802,791</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_JUMP_BACKWARD</td>
<td align="right">10,012</td>
<td align="right">10,004</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">DELETE_ATTR</td>
<td align="right">6,117,448</td>
<td align="right">6,122,225</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">240,632,510</td>
<td align="right">240,820,159</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_RANGE</td>
<td align="right">147,335,667</td>
<td align="right">147,445,339</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_FOR_ITER</td>
<td align="right">11,372</td>
<td align="right">11,364</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">302,380,761</td>
<td align="right">302,568,162</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">832,064,020</td>
<td align="right">832,577,827</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_TRUE</td>
<td align="right">13,452</td>
<td align="right">13,444</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">187,208,843</td>
<td align="right">187,306,963</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">254,480,682</td>
<td align="right">254,604,288</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">POP_EXCEPT</td>
<td align="right">23,015,228</td>
<td align="right">23,024,862</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">PUSH_EXC_INFO</td>
<td align="right">23,015,375</td>
<td align="right">23,025,007</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CHECK_EXC_MATCH</td>
<td align="right">22,392,021</td>
<td align="right">22,401,391</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">340,895,835</td>
<td align="right">341,037,331</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">307,499,594</td>
<td align="right">307,619,504</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">9,825,081</td>
<td align="right">9,828,787</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RERAISE</td>
<td align="right">2,615,212</td>
<td align="right">2,616,165</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST_STORE_FAST</td>
<td align="right">1,726,699,953</td>
<td align="right">1,727,323,130</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_FROM</td>
<td align="right">10,474,688</td>
<td align="right">10,478,439</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">335,090,549</td>
<td align="right">335,207,121</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_CLASS</td>
<td align="right">160,158,724</td>
<td align="right">160,212,742</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">540,597,099</td>
<td align="right">540,772,634</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">109,215,924</td>
<td align="right">109,251,218</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">3,105,888,112</td>
<td align="right">3,106,883,204</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,204,515</td>
<td align="right">3,205,475</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">395,895,147</td>
<td align="right">396,011,845</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_SUBTRACT_INT</td>
<td align="right">432,834,982</td>
<td align="right">432,945,753</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">1,362,127,973</td>
<td align="right">1,362,438,653</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">295,142,575</td>
<td align="right">295,207,045</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">311,704,071</td>
<td align="right">311,771,189</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">129,415,122</td>
<td align="right">129,388,652</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">200,310,774</td>
<td align="right">200,341,946</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">150,739,578</td>
<td align="right">150,716,381</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE</td>
<td align="right">315,573</td>
<td align="right">315,610</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">134,603,453</td>
<td align="right">134,618,837</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR</td>
<td align="right">18,382</td>
<td align="right">18,384</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_FAST_LOAD_FAST</td>
<td align="right">42,343,929</td>
<td align="right">42,348,087</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">66,493,204</td>
<td align="right">66,499,674</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">7,453,872</td>
<td align="right">7,453,166</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">65,281,808</td>
<td align="right">65,287,391</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RESUME</td>
<td align="right">271,575</td>
<td align="right">271,552</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">POP_JUMP_IF_TRUE</td>
<td align="right">1,415,178,247</td>
<td align="right">1,415,060,594</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RAISE_VARARGS</td>
<td align="right">5,737,379</td>
<td align="right">5,737,806</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">101,728,285</td>
<td align="right">101,721,465</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">66,546,647</td>
<td align="right">66,542,248</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">26,370,704</td>
<td align="right">26,369,200</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">485,932,881</td>
<td align="right">485,911,591</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">90,233,622</td>
<td align="right">90,237,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_INT</td>
<td align="right">673,955,329</td>
<td align="right">673,982,721</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">49,883,115</td>
<td align="right">49,885,106</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">36,318,990</td>
<td align="right">36,320,368</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">152,367,655</td>
<td align="right">152,361,892</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">179,903,393</td>
<td align="right">179,896,773</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">97,355,767</td>
<td align="right">97,359,344</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">EXIT_INIT_CHECK</td>
<td align="right">93,509,720</td>
<td align="right">93,512,904</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">95,793,282</td>
<td align="right">95,796,466</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">463,056,638</td>
<td align="right">463,071,985</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">12,590,801</td>
<td align="right">12,590,486</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">114,782,518</td>
<td align="right">114,779,796</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">135,613,731</td>
<td align="right">135,611,017</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_ADD_UNICODE</td>
<td align="right">72,946,717</td>
<td align="right">72,947,991</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">1,726,064,955</td>
<td align="right">1,726,035,260</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">63,670,320</td>
<td align="right">63,669,231</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">142,873,656</td>
<td align="right">142,875,842</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">1,715,338</td>
<td align="right">1,715,363</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">416,051,647</td>
<td align="right">416,057,273</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">176,330,597</td>
<td align="right">176,332,961</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">JUMP_BACKWARD_NO_INTERRUPT</td>
<td align="right">551,647,414</td>
<td align="right">551,654,553</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">216,235,153</td>
<td align="right">216,237,947</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">38,703,620</td>
<td align="right">38,703,139</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">94,681,745</td>
<td align="right">94,682,788</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_AWAITABLE</td>
<td align="right">229,791,203</td>
<td align="right">229,788,952</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">71,656,336</td>
<td align="right">71,655,709</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">770,541,882</td>
<td align="right">770,535,171</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_FOR</td>
<td align="right">75,725,871</td>
<td align="right">75,726,505</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">497,682,828</td>
<td align="right">497,686,143</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_WITH_HINT</td>
<td align="right">355,114,914</td>
<td align="right">355,112,549</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">165,326,251</td>
<td align="right">165,325,265</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">END_SEND</td>
<td align="right">391,994,636</td>
<td align="right">391,992,387</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">899,642</td>
<td align="right">899,647</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
<td align="right">780,200,129</td>
<td align="right">780,195,912</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">172,790,109</td>
<td align="right">172,790,632</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">1,493,482,855</td>
<td align="right">1,493,479,056</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_GLOBAL</td>
<td align="right">20,555,838</td>
<td align="right">20,555,887</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BEFORE_ASYNC_WITH</td>
<td align="right">3,005,926</td>
<td align="right">3,005,920</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">235,749,398</td>
<td align="right">235,748,961</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">39,816,889</td>
<td align="right">39,816,826</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_MULTIPLY_INT</td>
<td align="right">161,269,831</td>
<td align="right">161,269,581</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">64,647,194</td>
<td align="right">64,647,118</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">36,536,627</td>
<td align="right">36,536,595</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">73,361,855</td>
<td align="right">73,361,865</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">272,661,126</td>
<td align="right">272,661,126</td>
<td align="right">0.0%</td>
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
<td align="right">10,248,367</td>
<td align="right">10,248,367</td>
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
<td align="right">6,944,440</td>
<td align="right">6,944,440</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_EX</td>
<td align="right">1,129,926</td>
<td align="right">1,129,926</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">401,536</td>
<td align="right">401,536</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_UPDATE</td>
<td align="right">88,668</td>
<td align="right">88,668</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_BUILD_CLASS</td>
<td align="right">19,866</td>
<td align="right">19,866</td>
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
<td align="left">DELETE_NAME</td>
<td align="right">900</td>
<td align="right">900</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
<td align="right">840</td>
<td align="right">840</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">INSTRUMENTED_POP_JUMP_IF_NONE</td>
<td align="right">720</td>
<td align="right">720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SETUP_ANNOTATIONS</td>
<td align="right">544</td>
<td align="right">544</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">624,965,616</td>
<td align="right">28.4%</td>
<td align="right">628,332,392</td>
<td align="right">28.5%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,573,474,559</td>
<td align="right">71.5%</td>
<td align="right">1,573,857,496</td>
<td align="right">71.4%</td>
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
<td align="right">21,800,138</td>
<td align="right">1.0%</td>
<td align="right">21,800,135</td>
<td align="right">1.0%</td>
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
<td align="right">1,137,271</td>
<td align="right">71.2%</td>
<td align="right">1,138,144</td>
<td align="right">71.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">459,829</td>
<td align="right">28.8%</td>
<td align="right">459,871</td>
<td align="right">28.8%</td>
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
<td align="right">16,384</td>
<td align="right">1.4%</td>
<td align="right">16,684</td>
<td align="right">1.5%</td>
<td align="right">1.8%</td>
</tr>
<tr>
<td align="left">and int</td>
<td align="right">39,263</td>
<td align="right">3.5%</td>
<td align="right">39,721</td>
<td align="right">3.5%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">power</td>
<td align="right">5,721</td>
<td align="right">0.5%</td>
<td align="right">5,728</td>
<td align="right">0.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">remainder</td>
<td align="right">52,538</td>
<td align="right">4.6%</td>
<td align="right">52,589</td>
<td align="right">4.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">add different types</td>
<td align="right">61,113</td>
<td align="right">5.4%</td>
<td align="right">61,150</td>
<td align="right">5.4%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">lshift</td>
<td align="right">5,463</td>
<td align="right">0.5%</td>
<td align="right">5,466</td>
<td align="right">0.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">rshift</td>
<td align="right">9,830</td>
<td align="right">0.9%</td>
<td align="right">9,834</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide other</td>
<td align="right">3,501</td>
<td align="right">0.3%</td>
<td align="right">3,500</td>
<td align="right">0.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">true divide float</td>
<td align="right">5,763</td>
<td align="right">0.5%</td>
<td align="right">5,764</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">add other</td>
<td align="right">60,906</td>
<td align="right">5.4%</td>
<td align="right">60,915</td>
<td align="right">5.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">floor divide</td>
<td align="right">32,552</td>
<td align="right">2.9%</td>
<td align="right">32,556</td>
<td align="right">2.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">xor</td>
<td align="right">9,443</td>
<td align="right">0.8%</td>
<td align="right">9,444</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">true divide different types</td>
<td align="right">11,563</td>
<td align="right">1.0%</td>
<td align="right">11,562</td>
<td align="right">1.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">multiply different types</td>
<td align="right">67,292</td>
<td align="right">5.9%</td>
<td align="right">67,296</td>
<td align="right">5.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">subtract different types</td>
<td align="right">736,432</td>
<td align="right">64.8%</td>
<td align="right">736,428</td>
<td align="right">64.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">subtract other</td>
<td align="right">12,074</td>
<td align="right">1.1%</td>
<td align="right">12,074</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">multiply other</td>
<td align="right">5,180</td>
<td align="right">0.5%</td>
<td align="right">5,180</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and other</td>
<td align="right">1,714</td>
<td align="right">0.2%</td>
<td align="right">1,714</td>
<td align="right">0.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">and different types</td>
<td align="right">539</td>
<td align="right">0.0%</td>
<td align="right">539</td>
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
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">1,796,746,207</td>
<td align="right">81.0%</td>
<td align="right">1,785,386,418</td>
<td align="right">80.9%</td>
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
<td align="right">420,462,363</td>
<td align="right">19.0%</td>
<td align="right">420,467,956</td>
<td align="right">19.1%</td>
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
<td align="right">4,774,100</td>
<td align="right">0.2%</td>
<td align="right">4,774,095</td>
<td align="right">0.2%</td>
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
<td align="right">173,988</td>
<td align="right">47.9%</td>
<td align="right">174,010</td>
<td align="right">47.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">189,396</td>
<td align="right">52.1%</td>
<td align="right">189,402</td>
<td align="right">52.1%</td>
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
<td align="right">84</td>
<td align="right">0.0%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">buffer int</td>
<td align="right">20,841</td>
<td align="right">12.0%</td>
<td align="right">20,868</td>
<td align="right">12.0%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">52,656</td>
<td align="right">30.3%</td>
<td align="right">52,652</td>
<td align="right">30.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">73,692</td>
<td align="right">42.4%</td>
<td align="right">73,690</td>
<td align="right">42.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">16,680</td>
<td align="right">9.6%</td>
<td align="right">16,680</td>
<td align="right">9.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">sequence int</td>
<td align="right">4,280</td>
<td align="right">2.5%</td>
<td align="right">4,280</td>
<td align="right">2.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">4,136</td>
<td align="right">2.4%</td>
<td align="right">4,136</td>
<td align="right">2.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">buffer slice</td>
<td align="right">880</td>
<td align="right">0.5%</td>
<td align="right">880</td>
<td align="right">0.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list slice</td>
<td align="right">640</td>
<td align="right">0.4%</td>
<td align="right">640</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string slice</td>
<td align="right">100</td>
<td align="right">0.1%</td>
<td align="right">100</td>
<td align="right">0.1%</td>
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
<td align="right">1,423,619,900</td>
<td align="right">15.0%</td>
<td align="right">1,426,900,792</td>
<td align="right">15.1%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">8,048,337,984</td>
<td align="right">84.9%</td>
<td align="right">8,039,764,674</td>
<td align="right">84.9%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">239,335,991</td>
<td align="right">2.5%</td>
<td align="right">239,203,527</td>
<td align="right">2.5%</td>
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
<td align="right">878,358</td>
<td align="right">14.9%</td>
<td align="right">880,812</td>
<td align="right">14.9%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">5,027,230</td>
<td align="right">85.1%</td>
<td align="right">5,024,748</td>
<td align="right">85.1%</td>
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
<td align="left">operator wrapper</td>
<td align="right">5,932</td>
<td align="right">0.7%</td>
<td align="right">6,000</td>
<td align="right">0.7%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">method wrapper</td>
<td align="right">7,678</td>
<td align="right">0.9%</td>
<td align="right">7,750</td>
<td align="right">0.9%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">class mutable</td>
<td align="right">20,887</td>
<td align="right">2.4%</td>
<td align="right">21,067</td>
<td align="right">2.4%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">bound method</td>
<td align="right">10,548</td>
<td align="right">1.2%</td>
<td align="right">10,636</td>
<td align="right">1.2%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">meth descr varargs keywords</td>
<td align="right">18,282</td>
<td align="right">2.1%</td>
<td align="right">18,421</td>
<td align="right">2.1%</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">cfunc noargs</td>
<td align="right">65,930</td>
<td align="right">7.5%</td>
<td align="right">66,419</td>
<td align="right">7.5%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">cfunc varargs</td>
<td align="right">11,738</td>
<td align="right">1.3%</td>
<td align="right">11,814</td>
<td align="right">1.3%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">161</td>
<td align="right">0.0%</td>
<td align="right">160</td>
<td align="right">0.0%</td>
<td align="right">-0.6%</td>
</tr>
<tr>
<td align="left">cfunc varargs keywords</td>
<td align="right">28,163</td>
<td align="right">3.2%</td>
<td align="right">28,323</td>
<td align="right">3.2%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">wrong number arguments</td>
<td align="right">9,094</td>
<td align="right">1.0%</td>
<td align="right">9,134</td>
<td align="right">1.0%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">metaclass</td>
<td align="right">37,594</td>
<td align="right">4.3%</td>
<td align="right">37,750</td>
<td align="right">4.3%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">code complex parameters</td>
<td align="right">157,460</td>
<td align="right">17.9%</td>
<td align="right">158,087</td>
<td align="right">17.9%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">class no vectorcall</td>
<td align="right">65,939</td>
<td align="right">7.5%</td>
<td align="right">66,140</td>
<td align="right">7.5%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">37,280</td>
<td align="right">4.2%</td>
<td align="right">37,389</td>
<td align="right">4.2%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">meth descr method fastcall keywords</td>
<td align="right">200,077</td>
<td align="right">22.8%</td>
<td align="right">200,129</td>
<td align="right">22.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">meth descr varargs</td>
<td align="right">57,116</td>
<td align="right">6.5%</td>
<td align="right">57,114</td>
<td align="right">6.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">102,756</td>
<td align="right">11.7%</td>
<td align="right">102,755</td>
<td align="right">11.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">init not python</td>
<td align="right">16,366</td>
<td align="right">1.9%</td>
<td align="right">16,366</td>
<td align="right">1.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">cmethod</td>
<td align="right">12,660</td>
<td align="right">1.4%</td>
<td align="right">12,660</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">init not simple</td>
<td align="right">10,018</td>
<td align="right">1.1%</td>
<td align="right">10,018</td>
<td align="right">1.1%</td>
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
<td align="right">1,756,190,882</td>
<td align="right">92.8%</td>
<td align="right">1,725,513,049</td>
<td align="right">92.6%</td>
<td align="right">-1.7%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,853,142</td>
<td align="right">0.1%</td>
<td align="right">1,844,607</td>
<td align="right">0.1%</td>
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
<td align="right">136,746,855</td>
<td align="right">7.2%</td>
<td align="right">137,026,033</td>
<td align="right">7.4%</td>
<td align="right">0.2%</td>
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
<td align="right">98,217</td>
<td align="right">31.4%</td>
<td align="right">98,037</td>
<td align="right">31.4%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">214,709</td>
<td align="right">68.6%</td>
<td align="right">214,379</td>
<td align="right">68.6%</td>
<td align="right">-0.2%</td>
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
<td align="right">61,112</td>
<td align="right">28.5%</td>
<td align="right">60,651</td>
<td align="right">28.3%</td>
<td align="right">-0.8%</td>
</tr>
<tr>
<td align="left">float long</td>
<td align="right">13,627</td>
<td align="right">6.3%</td>
<td align="right">13,680</td>
<td align="right">6.4%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">different types</td>
<td align="right">49,093</td>
<td align="right">22.9%</td>
<td align="right">49,172</td>
<td align="right">22.9%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">long float</td>
<td align="right">1,541</td>
<td align="right">0.7%</td>
<td align="right">1,539</td>
<td align="right">0.7%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">14,165</td>
<td align="right">6.6%</td>
<td align="right">14,171</td>
<td align="right">6.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bool</td>
<td align="right">3,356</td>
<td align="right">1.6%</td>
<td align="right">3,355</td>
<td align="right">1.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">23,034</td>
<td align="right">10.7%</td>
<td align="right">23,030</td>
<td align="right">10.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">baseobject</td>
<td align="right">29,607</td>
<td align="right">13.8%</td>
<td align="right">29,607</td>
<td align="right">13.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">string</td>
<td align="right">10,560</td>
<td align="right">4.9%</td>
<td align="right">10,560</td>
<td align="right">4.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">3,700</td>
<td align="right">1.7%</td>
<td align="right">3,700</td>
<td align="right">1.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,091</td>
<td align="right">1.4%</td>
<td align="right">3,091</td>
<td align="right">1.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">1,823</td>
<td align="right">0.8%</td>
<td align="right">1,823</td>
<td align="right">0.9%</td>
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
<td align="right">1,249,024,131</td>
<td align="right">81.8%</td>
<td align="right">1,250,838,230</td>
<td align="right">81.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">141,763,063</td>
<td align="right">9.3%</td>
<td align="right">141,915,149</td>
<td align="right">9.3%</td>
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
<td align="right">274,492,599</td>
<td align="right">18.0%</td>
<td align="right">274,632,957</td>
<td align="right">18.0%</td>
<td align="right">0.1%</td>
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
<td align="right">158,083</td>
<td align="right">5.5%</td>
<td align="right">164,221</td>
<td align="right">5.7%</td>
<td align="right">3.9%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,726,112</td>
<td align="right">94.5%</td>
<td align="right">2,728,988</td>
<td align="right">94.3%</td>
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
<td align="left">dict items</td>
<td align="right">57,585</td>
<td align="right">36.4%</td>
<td align="right">63,698</td>
<td align="right">38.8%</td>
<td align="right">10.6%</td>
</tr>
<tr>
<td align="left">itertools</td>
<td align="right">4,893</td>
<td align="right">3.1%</td>
<td align="right">4,913</td>
<td align="right">3.0%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">25,014</td>
<td align="right">15.8%</td>
<td align="right">25,028</td>
<td align="right">15.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">zip</td>
<td align="right">13,734</td>
<td align="right">8.7%</td>
<td align="right">13,728</td>
<td align="right">8.4%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">enumerate</td>
<td align="right">15,762</td>
<td align="right">10.0%</td>
<td align="right">15,759</td>
<td align="right">9.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">seq iter</td>
<td align="right">10,540</td>
<td align="right">6.7%</td>
<td align="right">10,540</td>
<td align="right">6.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">7,259</td>
<td align="right">4.6%</td>
<td align="right">7,259</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">6,839</td>
<td align="right">4.3%</td>
<td align="right">6,839</td>
<td align="right">4.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">reversed list</td>
<td align="right">6,165</td>
<td align="right">3.9%</td>
<td align="right">6,165</td>
<td align="right">3.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict values</td>
<td align="right">5,710</td>
<td align="right">3.6%</td>
<td align="right">5,710</td>
<td align="right">3.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">ascii string</td>
<td align="right">2,440</td>
<td align="right">1.5%</td>
<td align="right">2,440</td>
<td align="right">1.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">map</td>
<td align="right">1,300</td>
<td align="right">0.8%</td>
<td align="right">1,300</td>
<td align="right">0.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">520</td>
<td align="right">0.3%</td>
<td align="right">520</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">callable</td>
<td align="right">282</td>
<td align="right">0.2%</td>
<td align="right">282</td>
<td align="right">0.2%</td>
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
<td align="right">9,915,481,540</td>
<td align="right">86.0%</td>
<td align="right">9,885,557,853</td>
<td align="right">85.9%</td>
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
<td align="right">1,607,204,177</td>
<td align="right">13.9%</td>
<td align="right">1,611,295,435</td>
<td align="right">14.0%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">507,342,404</td>
<td align="right">4.4%</td>
<td align="right">507,487,722</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">1,816,189</td>
<td align="right">0.0%</td>
<td align="right">1,816,624</td>
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
<td align="right">998,944</td>
<td align="right">8.8%</td>
<td align="right">1,000,773</td>
<td align="right">8.9%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">10,291,026</td>
<td align="right">91.2%</td>
<td align="right">10,293,760</td>
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
<td align="left">non overriding descriptor</td>
<td align="right">10,992</td>
<td align="right">1.1%</td>
<td align="right">11,122</td>
<td align="right">1.1%</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">non object slot</td>
<td align="right">3,540</td>
<td align="right">0.4%</td>
<td align="right">3,580</td>
<td align="right">0.4%</td>
<td align="right">1.1%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">5,984</td>
<td align="right">0.6%</td>
<td align="right">6,040</td>
<td align="right">0.6%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">class attr descriptor</td>
<td align="right">16,540</td>
<td align="right">1.7%</td>
<td align="right">16,640</td>
<td align="right">1.7%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">122,796</td>
<td align="right">12.3%</td>
<td align="right">123,338</td>
<td align="right">12.3%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">class method obj</td>
<td align="right">18,312</td>
<td align="right">1.8%</td>
<td align="right">18,392</td>
<td align="right">1.8%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">shadowed</td>
<td align="right">90,804</td>
<td align="right">9.1%</td>
<td align="right">91,183</td>
<td align="right">9.1%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">110,707</td>
<td align="right">11.1%</td>
<td align="right">111,014</td>
<td align="right">11.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">18,490</td>
<td align="right">1.9%</td>
<td align="right">18,508</td>
<td align="right">1.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">metaclass attribute</td>
<td align="right">206,437</td>
<td align="right">20.7%</td>
<td align="right">206,537</td>
<td align="right">20.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">mutable class</td>
<td align="right">62,442</td>
<td align="right">6.3%</td>
<td align="right">62,468</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">has managed dict</td>
<td align="right">308,681</td>
<td align="right">30.9%</td>
<td align="right">308,732</td>
<td align="right">30.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">module attr not found</td>
<td align="right">10,682</td>
<td align="right">1.1%</td>
<td align="right">10,682</td>
<td align="right">1.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,260</td>
<td align="right">0.7%</td>
<td align="right">7,260</td>
<td align="right">0.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">builtin class method</td>
<td align="right">2,876</td>
<td align="right">0.3%</td>
<td align="right">2,876</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">2,341</td>
<td align="right">0.2%</td>
<td align="right">2,341</td>
<td align="right">0.2%</td>
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
<td align="right">312,750</td>
<td align="right">0.0%</td>
<td align="right">316,713</td>
<td align="right">0.0%</td>
<td align="right">1.3%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">6,865,468,479</td>
<td align="right">99.7%</td>
<td align="right">6,860,681,357</td>
<td align="right">99.7%</td>
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
<td align="right">20,321,755</td>
<td align="right">0.3%</td>
<td align="right">20,325,685</td>
<td align="right">0.3%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
deopt
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">9,342</td>
<td align="right">0.0%</td>
<td align="right">9,342</td>
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
<td align="right">546,833</td>
<td align="right">100.0%</td>
<td align="right">546,915</td>
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
<td align="right">128,079,703</td>
<td align="right">100.0%</td>
<td align="right">128,920,927</td>
<td align="right">100.0%</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">9,265</td>
<td align="right">0.0%</td>
<td align="right">9,267</td>
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
<td align="right">9,117</td>
<td align="right">100.0%</td>
<td align="right">9,117</td>
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
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">165,298,357</td>
<td align="right">17.5%</td>
<td align="right">165,297,388</td>
<td align="right">17.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
hit
<details>
<summary>ⓘ</summary>

Specialized instructions that complete.
</details>
</td>
<td align="right">780,169,229</td>
<td align="right">82.5%</td>
<td align="right">780,165,012</td>
<td align="right">82.5%</td>
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
<td align="right">6,210</td>
<td align="right">10.6%</td>
<td align="right">6,205</td>
<td align="right">10.6%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">52,584</td>
<td align="right">89.4%</td>
<td align="right">52,572</td>
<td align="right">89.4%</td>
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
<td align="right">15,904</td>
<td align="right">30.2%</td>
<td align="right">15,892</td>
<td align="right">30.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">async generator send</td>
<td align="right">33,180</td>
<td align="right">63.1%</td>
<td align="right">33,180</td>
<td align="right">63.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">list</td>
<td align="right">3,260</td>
<td align="right">6.2%</td>
<td align="right">3,260</td>
<td align="right">6.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict keys</td>
<td align="right">240</td>
<td align="right">0.5%</td>
<td align="right">240</td>
<td align="right">0.5%</td>
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
<td align="right">2,459,692,479</td>
<td align="right">91.8%</td>
<td align="right">2,460,969,044</td>
<td align="right">91.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">154,797,595</td>
<td align="right">5.8%</td>
<td align="right">154,767,382</td>
<td align="right">5.8%</td>
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
<td align="right">216,930,156</td>
<td align="right">8.1%</td>
<td align="right">216,905,933</td>
<td align="right">8.1%</td>
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
<td align="right">95,598</td>
<td align="right">3.0%</td>
<td align="right">95,760</td>
<td align="right">3.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">3,053,649</td>
<td align="right">97.0%</td>
<td align="right">3,053,080</td>
<td align="right">97.0%</td>
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
<td align="right">3,640</td>
<td align="right">3.8%</td>
<td align="right">3,740</td>
<td align="right">3.9%</td>
<td align="right">2.7%</td>
</tr>
<tr>
<td align="left">no dict</td>
<td align="right">3,100</td>
<td align="right">3.2%</td>
<td align="right">3,120</td>
<td align="right">3.3%</td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">class attr simple</td>
<td align="right">45,518</td>
<td align="right">47.6%</td>
<td align="right">45,558</td>
<td align="right">47.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">not managed dict</td>
<td align="right">2,668</td>
<td align="right">2.8%</td>
<td align="right">2,670</td>
<td align="right">2.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">not in dict</td>
<td align="right">15,545</td>
<td align="right">16.3%</td>
<td align="right">15,545</td>
<td align="right">16.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overriding descriptor</td>
<td align="right">10,440</td>
<td align="right">10.9%</td>
<td align="right">10,440</td>
<td align="right">10.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">not in keys</td>
<td align="right">7,401</td>
<td align="right">7.7%</td>
<td align="right">7,401</td>
<td align="right">7.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">overridden</td>
<td align="right">5,172</td>
<td align="right">5.4%</td>
<td align="right">5,172</td>
<td align="right">5.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">method</td>
<td align="right">1,500</td>
<td align="right">1.6%</td>
<td align="right">1,500</td>
<td align="right">1.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of versions</td>
<td align="right">594</td>
<td align="right">0.6%</td>
<td align="right">594</td>
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
<td align="right">261,028,732</td>
<td align="right">64.6%</td>
<td align="right">261,607,015</td>
<td align="right">64.7%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">
deferred
<details>
<summary>ⓘ</summary>

Lists the number of "deferred" (i.e. not specialized) instructions executed.
</details>
</td>
<td align="right">142,779,086</td>
<td align="right">35.3%</td>
<td align="right">142,781,233</td>
<td align="right">35.3%</td>
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
<td align="right">81,247</td>
<td align="right">83.4%</td>
<td align="right">81,282</td>
<td align="right">83.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">16,203</td>
<td align="right">16.6%</td>
<td align="right">16,207</td>
<td align="right">16.6%</td>
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
<td align="left">other</td>
<td align="right">780</td>
<td align="right">1.0%</td>
<td align="right">800</td>
<td align="right">1.0%</td>
<td align="right">2.6%</td>
</tr>
<tr>
<td align="left">py simple</td>
<td align="right">40,719</td>
<td align="right">50.1%</td>
<td align="right">40,737</td>
<td align="right">50.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">dict subclass no override</td>
<td align="right">28,080</td>
<td align="right">34.6%</td>
<td align="right">28,077</td>
<td align="right">34.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">array int</td>
<td align="right">7,200</td>
<td align="right">8.9%</td>
<td align="right">7,200</td>
<td align="right">8.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">out of range</td>
<td align="right">3,588</td>
<td align="right">4.4%</td>
<td align="right">3,588</td>
<td align="right">4.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytearray int</td>
<td align="right">880</td>
<td align="right">1.1%</td>
<td align="right">880</td>
<td align="right">1.1%</td>
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
<td align="right">4,007,436,305</td>
<td align="right">92.2%</td>
<td align="right">4,011,185,486</td>
<td align="right">92.2%</td>
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
<td align="right">334,651,405</td>
<td align="right">7.7%</td>
<td align="right">334,838,723</td>
<td align="right">7.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">
miss
<details>
<summary>ⓘ</summary>

Specialized instructions that deopt.
</details>
</td>
<td align="right">96,642,896</td>
<td align="right">2.2%</td>
<td align="right">96,642,772</td>
<td align="right">2.2%</td>
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
<td align="right">574,476</td>
<td align="right">21.9%</td>
<td align="right">574,674</td>
<td align="right">21.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Success</td>
<td align="right">2,049,525</td>
<td align="right">78.1%</td>
<td align="right">2,049,534</td>
<td align="right">78.1%</td>
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
<td align="left">bytearray</td>
<td align="right">1,240</td>
<td align="right">0.2%</td>
<td align="right">1,236</td>
<td align="right">0.2%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">mapping</td>
<td align="right">56,944</td>
<td align="right">9.9%</td>
<td align="right">57,024</td>
<td align="right">9.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">set</td>
<td align="right">32,671</td>
<td align="right">5.7%</td>
<td align="right">32,711</td>
<td align="right">5.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">sequence</td>
<td align="right">16,498</td>
<td align="right">2.9%</td>
<td align="right">16,516</td>
<td align="right">2.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">tuple</td>
<td align="right">95,016</td>
<td align="right">16.5%</td>
<td align="right">95,053</td>
<td align="right">16.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">float</td>
<td align="right">2,601</td>
<td align="right">0.5%</td>
<td align="right">2,600</td>
<td align="right">0.5%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">172,068</td>
<td align="right">30.0%</td>
<td align="right">172,096</td>
<td align="right">29.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">bytes</td>
<td align="right">14,878</td>
<td align="right">2.6%</td>
<td align="right">14,876</td>
<td align="right">2.6%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">dict</td>
<td align="right">27,571</td>
<td align="right">4.8%</td>
<td align="right">27,568</td>
<td align="right">4.8%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">number</td>
<td align="right">154,569</td>
<td align="right">26.9%</td>
<td align="right">154,574</td>
<td align="right">26.9%</td>
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
<td align="right">921,142,647</td>
<td align="right">99.9%</td>
<td align="right">921,766,665</td>
<td align="right">99.9%</td>
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
<td align="right">689,775</td>
<td align="right">0.1%</td>
<td align="right">689,800</td>
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
<td align="left">Success</td>
<td align="right">50,021</td>
<td align="right">95.4%</td>
<td align="right">50,033</td>
<td align="right">95.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Failure</td>
<td align="right">2,437</td>
<td align="right">4.6%</td>
<td align="right">2,437</td>
<td align="right">4.6%</td>
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
<td align="right">1,436</td>
<td align="right">58.9%</td>
<td align="right">1,436</td>
<td align="right">58.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">iterator</td>
<td align="right">621</td>
<td align="right">25.5%</td>
<td align="right">621</td>
<td align="right">25.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">other</td>
<td align="right">380</td>
<td align="right">15.6%</td>
<td align="right">380</td>
<td align="right">15.6%</td>
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
<td align="right">12,662,941,266</td>
<td align="right">9.5%</td>
<td align="right">12,632,450,984</td>
<td align="right">9.5%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Basic
<details>
<summary>ⓘ</summary>

Instructions that are not and cannot be specialized, e.g. `LOAD_FAST`.
</details>
</td>
<td align="right">73,615,063,014</td>
<td align="right">55.0%</td>
<td align="right">73,451,129,187</td>
<td align="right">55.0%</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">
Specialized hits
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that complete.
</details>
</td>
<td align="right">46,389,269,526</td>
<td align="right">34.7%</td>
<td align="right">46,321,963,905</td>
<td align="right">34.7%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">
Specialized misses
<details>
<summary>ⓘ</summary>

Specialized instructions, e.g. `LOAD_ATTR_MODULE` that deopt.
</details>
</td>
<td align="right">1,169,591,655</td>
<td align="right">0.9%</td>
<td align="right">1,169,721,766</td>
<td align="right">0.9%</td>
<td align="right">0.0%</td>
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
<td align="left">BINARY_OP</td>
<td align="right">624,965,616</td>
<td align="right">11.6%</td>
<td align="right">628,332,392</td>
<td align="right">11.7%</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR</td>
<td align="right">1,607,204,177</td>
<td align="right">29.9%</td>
<td align="right">1,611,295,435</td>
<td align="right">30.0%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">CALL</td>
<td align="right">1,423,619,900</td>
<td align="right">26.5%</td>
<td align="right">1,426,900,792</td>
<td align="right">26.5%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">COMPARE_OP</td>
<td align="right">136,746,855</td>
<td align="right">2.5%</td>
<td align="right">137,026,033</td>
<td align="right">2.5%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">TO_BOOL</td>
<td align="right">334,651,405</td>
<td align="right">6.2%</td>
<td align="right">334,838,723</td>
<td align="right">6.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER</td>
<td align="right">274,492,599</td>
<td align="right">5.1%</td>
<td align="right">274,632,957</td>
<td align="right">5.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">STORE_ATTR</td>
<td align="right">216,930,156</td>
<td align="right">4.0%</td>
<td align="right">216,905,933</td>
<td align="right">4.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR</td>
<td align="right">142,779,086</td>
<td align="right">2.7%</td>
<td align="right">142,781,233</td>
<td align="right">2.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR</td>
<td align="right">420,462,363</td>
<td align="right">7.8%</td>
<td align="right">420,467,956</td>
<td align="right">7.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">165,298,357</td>
<td align="right">3.1%</td>
<td align="right">165,297,388</td>
<td align="right">3.1%</td>
<td align="right">-0.0%</td>
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
<td align="right">132,014,572</td>
<td align="right">11.3%</td>
<td align="right">132,206,987</td>
<td align="right">11.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_LIST</td>
<td align="right">70,893,513</td>
<td align="right">6.1%</td>
<td align="right">70,975,261</td>
<td align="right">6.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">FOR_ITER_TUPLE</td>
<td align="right">70,857,910</td>
<td align="right">6.1%</td>
<td align="right">70,928,248</td>
<td align="right">6.1%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_PY_EXACT_ARGS</td>
<td align="right">119,389,763</td>
<td align="right">10.2%</td>
<td align="right">119,328,209</td>
<td align="right">10.2%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_SLOT</td>
<td align="right">95,409,570</td>
<td align="right">8.2%</td>
<td align="right">95,379,394</td>
<td align="right">8.2%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">65,879,325</td>
<td align="right">5.6%</td>
<td align="right">65,882,446</td>
<td align="right">5.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_SLOT</td>
<td align="right">106,134,724</td>
<td align="right">9.1%</td>
<td align="right">106,130,950</td>
<td align="right">9.1%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_INSTANCE_VALUE</td>
<td align="right">150,383,117</td>
<td align="right">12.9%</td>
<td align="right">150,385,525</td>
<td align="right">12.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">47,182,786</td>
<td align="right">4.0%</td>
<td align="right">47,182,524</td>
<td align="right">4.0%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">59,335,376</td>
<td align="right">5.1%</td>
<td align="right">59,335,372</td>
<td align="right">5.1%</td>
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
<td align="left">Calls via PyEval_EvalFrame (api)</td>
<td align="right">251,311,667</td>
<td align="right">3.4%</td>
<td align="right">252,011,142</td>
<td align="right">3.4%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function vectorcall)</td>
<td align="right">1,393,260,198</td>
<td align="right">19.0%</td>
<td align="right">1,395,657,394</td>
<td align="right">19.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (vector)</td>
<td align="right">1,397,694,788</td>
<td align="right">19.0%</td>
<td align="right">1,400,091,984</td>
<td align="right">19.0%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">Frames pushed</td>
<td align="right">4,833,285,978</td>
<td align="right">65.8%</td>
<td align="right">4,839,628,545</td>
<td align="right">65.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Calls to Python functions inlined</td>
<td align="right">5,089,741,029</td>
<td align="right">69.3%</td>
<td align="right">5,096,144,442</td>
<td align="right">69.3%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Calls to PyEval_EvalDefault</td>
<td align="right">2,257,045,445</td>
<td align="right">30.7%</td>
<td align="right">2,259,405,200</td>
<td align="right">30.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (total)</td>
<td align="right">2,257,045,445</td>
<td align="right">30.7%</td>
<td align="right">2,259,405,200</td>
<td align="right">30.7%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Frame objects created</td>
<td align="right">85,829,356</td>
<td align="right">1.2%</td>
<td align="right">85,837,025</td>
<td align="right">1.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (slot)</td>
<td align="right">471,877,138</td>
<td align="right">6.4%</td>
<td align="right">471,909,490</td>
<td align="right">6.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (function ex)</td>
<td align="right">27,741,588</td>
<td align="right">0.4%</td>
<td align="right">27,743,000</td>
<td align="right">0.4%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (generator)</td>
<td align="right">859,350,657</td>
<td align="right">11.7%</td>
<td align="right">859,313,216</td>
<td align="right">11.7%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (method)</td>
<td align="right">212,987,019</td>
<td align="right">2.9%</td>
<td align="right">212,980,361</td>
<td align="right">2.9%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (legacy)</td>
<td align="right">4,414,724</td>
<td align="right">0.1%</td>
<td align="right">4,414,724</td>
<td align="right">0.1%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Calls via PyEval_EvalFrame (build class)</td>
<td align="right">19,866</td>
<td align="right">0.0%</td>
<td align="right">19,866</td>
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
<td align="left">Method cache collisions</td>
<td align="right">89,490,589</td>
<td align="right"></td>
<td align="right">86,483,413</td>
<td align="right"></td>
<td align="right">-3.4%</td>
</tr>
<tr>
<td align="left">Method cache misses</td>
<td align="right">88,526,086</td>
<td align="right"></td>
<td align="right">85,703,267</td>
<td align="right"></td>
<td align="right">-3.2%</td>
</tr>
<tr>
<td align="left">Method cache dunder misses</td>
<td align="right">8,686,419</td>
<td align="right"></td>
<td align="right">8,504,346</td>
<td align="right"></td>
<td align="right">-2.1%</td>
</tr>
<tr>
<td align="left">New values</td>
<td align="right">74,563,589</td>
<td align="right"></td>
<td align="right">75,032,579</td>
<td align="right"></td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">Allocations over 4 kbytes</td>
<td align="right">20,938,311</td>
<td align="right">0.1%</td>
<td align="right">21,006,411</td>
<td align="right">0.1%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Method cache hits</td>
<td align="right">3,132,932,656</td>
<td align="right"></td>
<td align="right">3,140,855,232</td>
<td align="right"></td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">Method cache dunder hits</td>
<td align="right">3,431,106,367</td>
<td align="right"></td>
<td align="right">3,434,361,933</td>
<td align="right"></td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Allocations from freelist</td>
<td align="right">6,713,481,466</td>
<td align="right">36.5%</td>
<td align="right">6,719,594,881</td>
<td align="right">36.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Frees to freelist</td>
<td align="right">6,721,256,351</td>
<td align="right"></td>
<td align="right">6,727,366,929</td>
<td align="right"></td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Decrefs</td>
<td align="right">28,943,826,663</td>
<td align="right">21.5%</td>
<td align="right">28,969,096,719</td>
<td align="right">21.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Increfs</td>
<td align="right">25,974,959,679</td>
<td align="right">22.2%</td>
<td align="right">25,996,883,602</td>
<td align="right">22.2%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Frees</td>
<td align="right">12,027,540,835</td>
<td align="right"></td>
<td align="right">12,034,772,239</td>
<td align="right"></td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Allocations</td>
<td align="right">11,697,350,844</td>
<td align="right">63.5%</td>
<td align="right">11,703,897,026</td>
<td align="right">63.5%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Allocations to 512 bytes</td>
<td align="right">11,572,087,524</td>
<td align="right">62.9%</td>
<td align="right">11,578,540,034</td>
<td align="right">62.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">Allocations to 4 kbytes</td>
<td align="right">104,325,009</td>
<td align="right">0.6%</td>
<td align="right">104,350,581</td>
<td align="right">0.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Interpreter decrefs</td>
<td align="right">105,511,259,458</td>
<td align="right">78.5%</td>
<td align="right">105,536,109,012</td>
<td align="right">78.5%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Interpreter increfs</td>
<td align="right">91,211,220,566</td>
<td align="right">77.8%</td>
<td align="right">91,228,424,073</td>
<td align="right">77.8%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (on request)</td>
<td align="right">3,653,105</td>
<td align="right">4.9%</td>
<td align="right">3,653,105</td>
<td align="right">4.9%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">Materialize dict (new key)</td>
<td align="right">190,075</td>
<td align="right">0.3%</td>
<td align="right">190,075</td>
<td align="right">0.3%</td>
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
<tr>
<td align="left">Dematerialize dict</td>
<td align="right">2,346,160</td>
<td align="right">3.1%</td>
<td align="right">2,346,160</td>
<td align="right">3.1%</td>
<td align="right">0.0%</td>
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
<td align="right">732,749</td>
<td align="right">47,026,918</td>
<td align="right">6,078,052,924</td>
<td align="right">732,658</td>
<td align="right">47,019,348</td>
<td align="right">6,064,630,650</td>
</tr>
<tr>
<td align="right">1</td>
<td align="right">65,554</td>
<td align="right">36,502,159</td>
<td align="right">4,961,380,322</td>
<td align="right">65,550</td>
<td align="right">36,503,380</td>
<td align="right">4,960,851,814</td>
</tr>
<tr>
<td align="right">2</td>
<td align="right">20,885</td>
<td align="right">53,197,146</td>
<td align="right">18,142,960,665</td>
<td align="right">20,889</td>
<td align="right">53,196,563</td>
<td align="right">18,168,165,960</td>
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
Uops executed
<details>
<summary>ⓘ</summary>

The total number of uops (micro-operations) that were executed
</details>
</td>
<td align="right">171,662,656,891</td>
<td align="right">3,001.7%</td>
<td align="right">181,409,738,935</td>
<td align="right">3,153.7%</td>
<td align="right">5.7%</td>
</tr>
<tr>
<td align="left">
Trace too short
<details>
<summary>ⓘ</summary>

A potential trace is abandoced because it it too short.
</details>
</td>
<td align="right">47,780,830</td>
<td align="right">20,211.9%</td>
<td align="right">48,221,382</td>
<td align="right">20,360.4%</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">
Traces executed
<details>
<summary>ⓘ</summary>

The number of traces that were executed
</details>
</td>
<td align="right">5,718,771,459</td>
<td align="right"></td>
<td align="right">5,752,371,270</td>
<td align="right"></td>
<td align="right">0.6%</td>
</tr>
<tr>
<td align="left">
Low confidence
<details>
<summary>ⓘ</summary>

A trace is abandoned because the likelihood of the jump to top being taken is too low.
</details>
</td>
<td align="right">2,949</td>
<td align="right">1.2%</td>
<td align="right">2,961</td>
<td align="right">1.3%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
Inner loop found
<details>
<summary>ⓘ</summary>

A trace is truncated because it has an inner loop
</details>
</td>
<td align="right">350,982</td>
<td align="right">148.5%</td>
<td align="right">352,258</td>
<td align="right">148.7%</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">
Trace stack underflow
<details>
<summary>ⓘ</summary>

A potential trace is abandoned because it pops more frames than it pushes.
</details>
</td>
<td align="right">10,969,297</td>
<td align="right">4,640.1%</td>
<td align="right">10,937,487</td>
<td align="right">4,618.1%</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">
Optimization attempts
<details>
<summary>ⓘ</summary>

The number of times a potential trace is identified.  Specifically, this occurs in the JUMP BACKWARD instruction when the counter reaches a threshold.
</details>
</td>
<td align="right">236,400</td>
<td align="right"></td>
<td align="right">236,839</td>
<td align="right"></td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">
Trace stack overflow
<details>
<summary>ⓘ</summary>

A trace is truncated because it would require more than 5 stack frames.
</details>
</td>
<td align="right">22,626</td>
<td align="right">9.6%</td>
<td align="right">22,637</td>
<td align="right">9.6%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Traces created
<details>
<summary>ⓘ</summary>

The number of traces that were successfully created.
</details>
</td>
<td align="right">2,308,113</td>
<td align="right">976.4%</td>
<td align="right">2,308,446</td>
<td align="right">974.7%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">
Recursive call
<details>
<summary>ⓘ</summary>

A trace is truncated because it has a recursive call.
</details>
</td>
<td align="right">784,669</td>
<td align="right">331.9%</td>
<td align="right">784,663</td>
<td align="right">331.3%</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">
Trace too long
<details>
<summary>ⓘ</summary>

A trace is truncated because it is longer than the instruction buffer.
</details>
</td>
<td align="right">281</td>
<td align="right">0.1%</td>
<td align="right">281</td>
<td align="right">0.1%</td>
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
<td align="right">3,771</td>
<td align="right">0.2%</td>
<td align="right">3,781</td>
<td align="right">0.2%</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">761,733</td>
<td align="right">33.0%</td>
<td align="right">761,301</td>
<td align="right">33.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">225,361</td>
<td align="right">9.8%</td>
<td align="right">225,518</td>
<td align="right">9.8%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">798,202</td>
<td align="right">34.6%</td>
<td align="right">798,756</td>
<td align="right">34.6%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">490,012</td>
<td align="right">21.2%</td>
<td align="right">490,041</td>
<td align="right">21.2%</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">21,765</td>
<td align="right">0.9%</td>
<td align="right">21,776</td>
<td align="right">0.9%</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">7,269</td>
<td align="right">0.3%</td>
<td align="right">7,273</td>
<td align="right">0.3%</td>
<td align="right">0.1%</td>
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
<td align="right">1</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">-100.0%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">5,507</td>
<td align="right">0.2%</td>
<td align="right">2,521</td>
<td align="right">0.1%</td>
<td align="right">-54.2%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">21,545</td>
<td align="right">0.9%</td>
<td align="right">21,956</td>
<td align="right">1.0%</td>
<td align="right">1.9%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">26,999</td>
<td align="right">1.2%</td>
<td align="right">28,292</td>
<td align="right">1.2%</td>
<td align="right">4.8%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">17,790</td>
<td align="right">0.8%</td>
<td align="right">18,438</td>
<td align="right">0.8%</td>
<td align="right">3.6%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">9,368</td>
<td align="right">0.4%</td>
<td align="right">10,096</td>
<td align="right">0.4%</td>
<td align="right">7.8%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">2,817</td>
<td align="right">0.1%</td>
<td align="right">3,003</td>
<td align="right">0.1%</td>
<td align="right">6.6%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">1,164</td>
<td align="right">0.1%</td>
<td align="right">1,203</td>
<td align="right">0.1%</td>
<td align="right">3.4%</td>
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
<td align="right">142,194,919</td>
<td align="right">2.5%</td>
<td align="right">22,707,580</td>
<td align="right">0.4%</td>
<td align="right">-84.0%</td>
</tr>
<tr>
<td align="left"><= 4</td>
<td align="right">374,151,357</td>
<td align="right">6.5%</td>
<td align="right">471,391,727</td>
<td align="right">8.2%</td>
<td align="right">26.0%</td>
</tr>
<tr>
<td align="left"><= 8</td>
<td align="right">487,217,828</td>
<td align="right">8.5%</td>
<td align="right">415,825,254</td>
<td align="right">7.2%</td>
<td align="right">-14.7%</td>
</tr>
<tr>
<td align="left"><= 16</td>
<td align="right">1,112,450,370</td>
<td align="right">19.5%</td>
<td align="right">1,162,090,657</td>
<td align="right">20.2%</td>
<td align="right">4.5%</td>
</tr>
<tr>
<td align="left"><= 32</td>
<td align="right">1,020,171,817</td>
<td align="right">17.8%</td>
<td align="right">1,054,043,358</td>
<td align="right">18.3%</td>
<td align="right">3.3%</td>
</tr>
<tr>
<td align="left"><= 64</td>
<td align="right">515,474,134</td>
<td align="right">9.0%</td>
<td align="right">537,762,404</td>
<td align="right">9.3%</td>
<td align="right">4.3%</td>
</tr>
<tr>
<td align="left"><= 128</td>
<td align="right">296,436,525</td>
<td align="right">5.2%</td>
<td align="right">302,308,497</td>
<td align="right">5.3%</td>
<td align="right">2.0%</td>
</tr>
<tr>
<td align="left"><= 256</td>
<td align="right">120,568,662</td>
<td align="right">2.1%</td>
<td align="right">97,674,566</td>
<td align="right">1.7%</td>
<td align="right">-19.0%</td>
</tr>
<tr>
<td align="left"><= 512</td>
<td align="right">26,097,297</td>
<td align="right">0.5%</td>
<td align="right">51,052,899</td>
<td align="right">0.9%</td>
<td align="right">95.6%</td>
</tr>
<tr>
<td align="left"><= 1,024</td>
<td align="right">7,573,119</td>
<td align="right">0.1%</td>
<td align="right">7,280,459</td>
<td align="right">0.1%</td>
<td align="right">-3.9%</td>
</tr>
<tr>
<td align="left"><= 2,048</td>
<td align="right">18,475,167</td>
<td align="right">0.3%</td>
<td align="right">18,512,915</td>
<td align="right">0.3%</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left"><= 4,096</td>
<td align="right">1,005,885</td>
<td align="right">0.0%</td>
<td align="right">1,328,696</td>
<td align="right">0.0%</td>
<td align="right">32.1%</td>
</tr>
<tr>
<td align="left"><= 8,192</td>
<td align="right">743,400</td>
<td align="right">0.0%</td>
<td align="right">742,577</td>
<td align="right">0.0%</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left"><= 16,384</td>
<td align="right">263,620</td>
<td align="right">0.0%</td>
<td align="right">77,220</td>
<td align="right">0.0%</td>
<td align="right">-70.7%</td>
</tr>
<tr>
<td align="left"><= 32,768</td>
<td align="right">41,280</td>
<td align="right">0.0%</td>
<td align="right">233,580</td>
<td align="right">0.0%</td>
<td align="right">465.8%</td>
</tr>
<tr>
<td align="left"><= 65,536</td>
<td align="right">13,360</td>
<td align="right">0.0%</td>
<td align="right">13,040</td>
<td align="right">0.0%</td>
<td align="right">-2.4%</td>
</tr>
<tr>
<td align="left"><= 131,072</td>
<td align="right">875</td>
<td align="right">0.0%</td>
<td align="right">1,071</td>
<td align="right">0.0%</td>
<td align="right">22.4%</td>
</tr>
<tr>
<td align="left"><= 262,144</td>
<td align="right">2,180</td>
<td align="right">0.0%</td>
<td align="right">2,291</td>
<td align="right">0.0%</td>
<td align="right">5.1%</td>
</tr>
<tr>
<td align="left"><= 524,288</td>
<td align="right">460</td>
<td align="right">0.0%</td>
<td align="right">469</td>
<td align="right">0.0%</td>
<td align="right">2.0%</td>
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
<td align="right">104</td>
<td align="right">0.0%</td>
<td align="right">0</td>
<td align="right">0.0%</td>
<td align="right">-100.0%</td>
</tr>
<tr>
<td align="left"><= 4,194,304</td>
<td align="right">376</td>
<td align="right">0.0%</td>
<td align="right">480</td>
<td align="right">0.0%</td>
<td align="right">27.7%</td>
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
<td align="left">_CHECK_VALIDITY_AND_SET_IP</td>
<td align="right">1,923,543,788</td>
<td align="right">8,829,250,143</td>
<td align="right">359.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_MODULE</td>
<td align="right">112,281,804</td>
<td align="right">9,156,914</td>
<td align="right">-91.8%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_MODULE</td>
<td align="right">112,285,244</td>
<td align="right">9,160,354</td>
<td align="right">-91.8%</td>
</tr>
<tr>
<td align="left">UNARY_NEGATIVE</td>
<td align="right">21,683,537</td>
<td align="right">35,861,120</td>
<td align="right">65.4%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_MODULE</td>
<td align="right">44,955,540</td>
<td align="right">59,140,920</td>
<td align="right">31.6%</td>
</tr>
<tr>
<td align="left">_CHECK_VALIDITY</td>
<td align="right">15,534,271,077</td>
<td align="right">19,957,126,124</td>
<td align="right">28.5%</td>
</tr>
<tr>
<td align="left">_GUARD_GLOBALS_VERSION</td>
<td align="right">51,460,040</td>
<td align="right">65,653,580</td>
<td align="right">27.6%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NOT_NONE_POP</td>
<td align="right">104,633,231</td>
<td align="right">122,430,820</td>
<td align="right">17.0%</td>
</tr>
<tr>
<td align="left">_SET_IP</td>
<td align="right">20,149,888,362</td>
<td align="right">18,158,510,301</td>
<td align="right">-9.9%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST</td>
<td align="right">203,909,925</td>
<td align="right">221,531,675</td>
<td align="right">8.6%</td>
</tr>
<tr>
<td align="left">POP_TOP</td>
<td align="right">622,199,940</td>
<td align="right">660,393,391</td>
<td align="right">6.1%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_INT</td>
<td align="right">870,194,777</td>
<td align="right">902,222,642</td>
<td align="right">3.7%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE</td>
<td align="right">1,116,273,617</td>
<td align="right">1,150,911,449</td>
<td align="right">3.1%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST</td>
<td align="right">5,229,350,344</td>
<td align="right">5,348,263,346</td>
<td align="right">2.3%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_NO_DICT</td>
<td align="right">785,892,807</td>
<td align="right">803,591,787</td>
<td align="right">2.3%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_0</td>
<td align="right">1,762,413,004</td>
<td align="right">1,789,002,715</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">_CHECK_MANAGED_OBJECT_HAS_VALUES</td>
<td align="right">1,765,847,341</td>
<td align="right">1,792,437,052</td>
<td align="right">1.5%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_LIST_INT</td>
<td align="right">1,034,583,714</td>
<td align="right">1,048,990,405</td>
<td align="right">1.4%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_DICT</td>
<td align="right">223,750,386</td>
<td align="right">220,923,157</td>
<td align="right">-1.3%</td>
</tr>
<tr>
<td align="left">_STORE_FAST</td>
<td align="right">4,769,160,285</td>
<td align="right">4,826,559,652</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS</td>
<td align="right">9,538,435</td>
<td align="right">9,652,946</td>
<td align="right">1.2%</td>
</tr>
<tr>
<td align="left">_GUARD_TYPE_VERSION</td>
<td align="right">4,918,122,515</td>
<td align="right">4,961,802,048</td>
<td align="right">0.9%</td>
</tr>
<tr>
<td align="left">_COLD_EXIT</td>
<td align="right">1,595,888,084</td>
<td align="right">1,609,320,890</td>
<td align="right">0.8%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_TRUE_POP</td>
<td align="right">2,181,411,303</td>
<td align="right">2,196,589,212</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">_EXIT_TRACE</td>
<td align="right">2,086,696,277</td>
<td align="right">2,101,107,452</td>
<td align="right">0.7%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_NONE_POP</td>
<td align="right">42,232,133</td>
<td align="right">42,459,617</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">_START_EXECUTOR</td>
<td align="right">4,122,883,375</td>
<td align="right">4,143,050,380</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_CLASS</td>
<td align="right">53,050,920</td>
<td align="right">53,300,745</td>
<td align="right">0.5%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW</td>
<td align="right">8,370,844,479</td>
<td align="right">8,403,801,199</td>
<td align="right">0.4%</td>
</tr>
<tr>
<td align="left">_GUARD_IS_FALSE_POP</td>
<td align="right">5,237,869,047</td>
<td align="right">5,255,559,054</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_0</td>
<td align="right">326,809,170</td>
<td align="right">327,821,690</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_WITH_NULL</td>
<td align="right">1,368,848,717</td>
<td align="right">1,372,692,692</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_6</td>
<td align="right">1,105,842,351</td>
<td align="right">1,103,007,776</td>
<td align="right">-0.3%</td>
</tr>
<tr>
<td align="left">BUILD_MAP</td>
<td align="right">14,048,946</td>
<td align="right">14,080,616</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_2</td>
<td align="right">97,554,451</td>
<td align="right">97,346,929</td>
<td align="right">-0.2%</td>
</tr>
<tr>
<td align="left">BEFORE_WITH</td>
<td align="right">92,818</td>
<td align="right">93,010</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_POP_FRAME</td>
<td align="right">536,831,558</td>
<td align="right">537,823,862</td>
<td align="right">0.2%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_LIST</td>
<td align="right">1,391,725,376</td>
<td align="right">1,393,642,600</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LIST_APPEND</td>
<td align="right">178,148,436</td>
<td align="right">178,378,133</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_CONST_INLINE_BORROW_WITH_NULL</td>
<td align="right">285,557,358</td>
<td align="right">285,917,524</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL_BUILTINS</td>
<td align="right">6,504,500</td>
<td align="right">6,512,660</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_LIST</td>
<td align="right">1,329,742,401</td>
<td align="right">1,331,408,849</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_1</td>
<td align="right">347,103,870</td>
<td align="right">346,682,205</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_3</td>
<td align="right">573,460,395</td>
<td align="right">574,093,323</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_FOR_ITER_TIER_TWO</td>
<td align="right">387,346,512</td>
<td align="right">386,940,872</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">GET_ITER</td>
<td align="right">173,019,022</td>
<td align="right">173,194,839</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_0</td>
<td align="right">675,347,865</td>
<td align="right">674,701,552</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_2</td>
<td align="right">660,290,833</td>
<td align="right">660,903,762</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_LIST</td>
<td align="right">1,095,210,398</td>
<td align="right">1,096,174,794</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_COMPARE_OP</td>
<td align="right">103,096,964</td>
<td align="right">103,008,766</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_GLOBALS</td>
<td align="right">1,413,451,692</td>
<td align="right">1,414,392,912</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_LEN</td>
<td align="right">189,613,591</td>
<td align="right">189,736,127</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_FUNCTION_EXACT_ARGS</td>
<td align="right">1,186,801,513</td>
<td align="right">1,187,564,431</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">TO_BOOL_BOOL</td>
<td align="right">1,826,624,564</td>
<td align="right">1,827,731,528</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_DEREF</td>
<td align="right">438,523,283</td>
<td align="right">438,267,453</td>
<td align="right">-0.1%</td>
</tr>
<tr>
<td align="left">_CHECK_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">62,805,074</td>
<td align="right">62,837,394</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_BOUND_METHOD_EXACT_ARGS</td>
<td align="right">62,805,074</td>
<td align="right">62,837,394</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_TYPE_1</td>
<td align="right">165,510,324</td>
<td align="right">165,592,227</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_RANGE</td>
<td align="right">734,215,242</td>
<td align="right">734,560,196</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_RANGE</td>
<td align="right">735,573,002</td>
<td align="right">735,917,956</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_BUILTINS</td>
<td align="right">911,394,365</td>
<td align="right">911,793,701</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RESUME_CHECK</td>
<td align="right">1,136,738,472</td>
<td align="right">1,137,236,158</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_PUSH_FRAME</td>
<td align="right">1,137,430,273</td>
<td align="right">1,137,928,113</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_SAVE_RETURN_OFFSET</td>
<td align="right">1,137,430,273</td>
<td align="right">1,137,928,113</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_STACK_SPACE</td>
<td align="right">1,137,456,087</td>
<td align="right">1,137,953,928</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_CLASS_0</td>
<td align="right">18,279,675</td>
<td align="right">18,287,475</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_2</td>
<td align="right">2,505,409,032</td>
<td align="right">2,506,443,372</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_CLASS</td>
<td align="right">19,348,170</td>
<td align="right">19,355,970</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TWO_TUPLE</td>
<td align="right">578,986,011</td>
<td align="right">578,776,030</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_TUPLE</td>
<td align="right">212,482,970</td>
<td align="right">212,554,013</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_RANGE</td>
<td align="right">693,359,397</td>
<td align="right">693,589,227</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_NEXT_TUPLE</td>
<td align="right">256,625,344</td>
<td align="right">256,707,140</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">COPY_FREE_VARS</td>
<td align="right">420,457</td>
<td align="right">420,582</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_3</td>
<td align="right">2,907,062,598</td>
<td align="right">2,907,888,254</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_NOT_EXHAUSTED_TUPLE</td>
<td align="right">399,471,416</td>
<td align="right">399,581,429</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_FUNCTION</td>
<td align="right">2,006,609</td>
<td align="right">2,007,123</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_6</td>
<td align="right">644,085,094</td>
<td align="right">643,945,946</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_ISINSTANCE</td>
<td align="right">259,113,566</td>
<td align="right">259,163,738</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_0</td>
<td align="right">4,932,709,825</td>
<td align="right">4,933,658,253</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_CHECK</td>
<td align="right">334,878</td>
<td align="right">334,815</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR</td>
<td align="right">1,000,222,257</td>
<td align="right">1,000,406,004</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">PUSH_NULL</td>
<td align="right">679,475,460</td>
<td align="right">679,599,226</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST</td>
<td align="right">735,568,484</td>
<td align="right">735,683,575</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAKE_CELL</td>
<td align="right">443,223</td>
<td align="right">443,157</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_O</td>
<td align="right">18,426,864</td>
<td align="right">18,429,300</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_SUBSCR</td>
<td align="right">1,231,136,871</td>
<td align="right">1,230,976,435</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_1</td>
<td align="right">1,847,128,893</td>
<td align="right">1,847,350,397</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_INT</td>
<td align="right">193,962,186</td>
<td align="right">193,939,855</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CONTAINS_OP</td>
<td align="right">1,865,378,959</td>
<td align="right">1,865,169,572</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_4</td>
<td align="right">636,263,031</td>
<td align="right">636,330,763</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_JUMP_TO_TOP</td>
<td align="right">2,125,810,522</td>
<td align="right">2,126,035,883</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_1</td>
<td align="right">6,080,020,356</td>
<td align="right">6,079,387,635</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_7</td>
<td align="right">1,455,044,830</td>
<td align="right">1,454,901,614</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_NO_DICT</td>
<td align="right">22,436,289</td>
<td align="right">22,437,859</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_5</td>
<td align="right">833,805,978</td>
<td align="right">833,856,893</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_WITH_VALUES</td>
<td align="right">723,159,816</td>
<td align="right">723,119,842</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_KEYS_VERSION</td>
<td align="right">819,465,850</td>
<td align="right">819,425,567</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES_INST_ATTR_FROM_DICT</td>
<td align="right">819,468,296</td>
<td align="right">819,428,013</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_NOARGS</td>
<td align="right">181,149,424</td>
<td align="right">181,156,794</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_ITER_CHECK_TUPLE</td>
<td align="right">494,777,619</td>
<td align="right">494,757,652</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_4</td>
<td align="right">1,757,259,656</td>
<td align="right">1,757,206,672</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_FAST_WITH_KEYWORDS</td>
<td align="right">20,567,689</td>
<td align="right">20,568,299</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_INSTANCE_VALUE</td>
<td align="right">102,147,977</td>
<td align="right">102,149,910</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_5</td>
<td align="right">1,874,597,612</td>
<td align="right">1,874,632,853</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_DORV_VALUES</td>
<td align="right">102,843,917</td>
<td align="right">102,845,850</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_FAST_AND_CLEAR</td>
<td align="right">14,580,867</td>
<td align="right">14,581,109</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_UNPACK_SEQUENCE</td>
<td align="right">2,627,289</td>
<td align="right">2,627,262</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_GLOBAL</td>
<td align="right">188,347,439</td>
<td align="right">188,348,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_FAST_7</td>
<td align="right">3,348,249,888</td>
<td align="right">3,348,228,320</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BUILD_LIST</td>
<td align="right">242,095,799</td>
<td align="right">242,094,288</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">SWAP</td>
<td align="right">1,118,530,644</td>
<td align="right">1,118,536,656</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">MAP_ADD</td>
<td align="right">20,587,506</td>
<td align="right">20,587,597</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_LIST</td>
<td align="right">55,236,395</td>
<td align="right">55,236,177</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_TUPLE_INT</td>
<td align="right">138,440,242</td>
<td align="right">138,439,758</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP</td>
<td align="right">897,314,959</td>
<td align="right">897,318,067</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_ADD</td>
<td align="right">1,450,724</td>
<td align="right">1,450,719</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_BUILTIN_O</td>
<td align="right">486,487,037</td>
<td align="right">486,485,644</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_FAST_0</td>
<td align="right">204,501,257</td>
<td align="right">204,501,740</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_DICT</td>
<td align="right">124,407,713</td>
<td align="right">124,407,998</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">COPY</td>
<td align="right">1,299,060,465</td>
<td align="right">1,299,063,145</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_INT</td>
<td align="right">396,815,111</td>
<td align="right">396,814,406</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_INTRINSIC_1</td>
<td align="right">96,034,449</td>
<td align="right">96,034,580</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LIST_EXTEND</td>
<td align="right">96,953,489</td>
<td align="right">96,953,620</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IS_OP</td>
<td align="right">255,240,319</td>
<td align="right">255,240,609</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_SUBSCR</td>
<td align="right">301,214,970</td>
<td align="right">301,214,768</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_INT</td>
<td align="right">2,482,835,454</td>
<td align="right">2,482,836,953</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_INT</td>
<td align="right">2,360,875,017</td>
<td align="right">2,360,876,065</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SLICE</td>
<td align="right">108,461,103</td>
<td align="right">108,461,063</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR_SLOT</td>
<td align="right">127,680,715</td>
<td align="right">127,680,678</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_STR</td>
<td align="right">25,398,186</td>
<td align="right">25,398,180</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_METHOD_DESCRIPTOR_FAST_WITH_KEYWORDS</td>
<td align="right">152,742,467</td>
<td align="right">152,742,436</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_TO_BOOL</td>
<td align="right">260,362,182</td>
<td align="right">260,362,133</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">DICT_MERGE</td>
<td align="right">7,517,473</td>
<td align="right">7,517,474</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_INT</td>
<td align="right">184,996,164</td>
<td align="right">184,996,146</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_STR</td>
<td align="right">1,817,250,032</td>
<td align="right">1,817,250,151</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNARY_NOT</td>
<td align="right">62,070,471</td>
<td align="right">62,070,474</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_NONE</td>
<td align="right">168,623,237</td>
<td align="right">168,623,229</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_4</td>
<td align="right">304,728,981</td>
<td align="right">304,728,977</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_WITH_HINT</td>
<td align="right">93,452,261</td>
<td align="right">93,452,260</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_WITH_HINT</td>
<td align="right">93,452,261</td>
<td align="right">93,452,260</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_STR_INT</td>
<td align="right">1,208,342,243</td>
<td align="right">1,208,342,238</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_FLOAT</td>
<td align="right">1,570,196,446</td>
<td align="right">1,570,196,440</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_TUPLE</td>
<td align="right">470,833,065</td>
<td align="right">470,833,064</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_MULTIPLY_FLOAT</td>
<td align="right">1,195,322,480</td>
<td align="right">1,195,322,480</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_FLOAT</td>
<td align="right">579,034,920</td>
<td align="right">579,034,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SUBSCR_LIST_INT</td>
<td align="right">469,963,200</td>
<td align="right">469,963,200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_SUBTRACT_FLOAT</td>
<td align="right">393,785,140</td>
<td align="right">393,785,140</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_SLICE</td>
<td align="right">149,873,800</td>
<td align="right">149,873,800</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SLICE</td>
<td align="right">139,772,340</td>
<td align="right">139,772,340</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_ANEXT</td>
<td align="right">125,514,720</td>
<td align="right">125,514,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_NONDESCRIPTOR_WITH_VALUES</td>
<td align="right">93,198,010</td>
<td align="right">93,198,010</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNPACK_SEQUENCE_LIST</td>
<td align="right">77,460,720</td>
<td align="right">77,460,720</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">COMPARE_OP_FLOAT</td>
<td align="right">71,250,781</td>
<td align="right">71,250,781</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_STR_1</td>
<td align="right">70,977,974</td>
<td align="right">70,977,974</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_SIMPLE</td>
<td align="right">57,518,358</td>
<td align="right">57,518,358</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_CHECK_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,495,920</td>
<td align="right">57,495,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_METHOD_LAZY_DICT</td>
<td align="right">57,495,920</td>
<td align="right">57,495,920</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_STORE_ATTR</td>
<td align="right">54,160,677</td>
<td align="right">54,160,677</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_INIT_CALL_PY_EXACT_ARGS_3</td>
<td align="right">51,695,366</td>
<td align="right">51,695,366</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CONVERT_VALUE</td>
<td align="right">48,798,280</td>
<td align="right">48,798,280</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">TO_BOOL_ALWAYS_TRUE</td>
<td align="right">35,905,422</td>
<td align="right">35,905,422</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_STRING</td>
<td align="right">27,269,053</td>
<td align="right">27,269,053</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_BINARY_OP_ADD_UNICODE</td>
<td align="right">22,578,105</td>
<td align="right">22,578,105</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_GUARD_BOTH_UNICODE</td>
<td align="right">22,578,105</td>
<td align="right">22,578,105</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">UNARY_INVERT</td>
<td align="right">12,512,780</td>
<td align="right">12,512,780</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_CONST_KEY_MAP</td>
<td align="right">4,074,087</td>
<td align="right">4,074,087</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_SLOT_1</td>
<td align="right">3,993,460</td>
<td align="right">3,993,460</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">_LOAD_ATTR_INSTANCE_VALUE_1</td>
<td align="right">3,434,337</td>
<td align="right">3,434,337</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_DEREF</td>
<td align="right">2,858,065</td>
<td align="right">2,858,065</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_NAME</td>
<td align="right">1,798,000</td>
<td align="right">1,798,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">DELETE_SUBSCR</td>
<td align="right">1,373,520</td>
<td align="right">1,373,520</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_GLOBAL</td>
<td align="right">1,260,560</td>
<td align="right">1,260,560</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_NAME</td>
<td align="right">578,940</td>
<td align="right">578,940</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_TUPLE_1</td>
<td align="right">540,960</td>
<td align="right">540,960</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">GET_YIELD_FROM_ITER</td>
<td align="right">185,480</td>
<td align="right">185,480</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SET_FUNCTION_ATTRIBUTE</td>
<td align="right">63,108</td>
<td align="right">63,108</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BUILD_SET</td>
<td align="right">6,101</td>
<td align="right">6,101</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">LOAD_SUPER_ATTR_METHOD</td>
<td align="right">6,000</td>
<td align="right">6,000</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">FORMAT_WITH_SPEC</td>
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
<td align="left">CALL</td>
<td align="right">12,126,497</td>
<td align="right">12,586,399</td>
<td align="right">3.8%</td>
</tr>
<tr>
<td align="left">FOR_ITER_GEN</td>
<td align="right">68,947</td>
<td align="right">69,146</td>
<td align="right">0.3%</td>
</tr>
<tr>
<td align="left">YIELD_VALUE</td>
<td align="right">14,751,304</td>
<td align="right">14,762,310</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">LOAD_ATTR_PROPERTY</td>
<td align="right">13,410</td>
<td align="right">13,420</td>
<td align="right">0.1%</td>
</tr>
<tr>
<td align="left">CALL_LIST_APPEND</td>
<td align="right">6,778</td>
<td align="right">6,775</td>
<td align="right">-0.0%</td>
</tr>
<tr>
<td align="left">CALL_PY_WITH_DEFAULTS</td>
<td align="right">88,680</td>
<td align="right">88,718</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">RETURN_GENERATOR</td>
<td align="right">21,909</td>
<td align="right">21,911</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_ALLOC_AND_ENTER_INIT</td>
<td align="right">74,345</td>
<td align="right">74,349</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_KW</td>
<td align="right">2,077,391</td>
<td align="right">2,077,429</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">CALL_FUNCTION_EX</td>
<td align="right">3,274,658</td>
<td align="right">3,274,661</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND</td>
<td align="right">3,928,200</td>
<td align="right">3,928,200</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_SUBSCR_GETITEM</td>
<td align="right">85,900</td>
<td align="right">85,900</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">BINARY_OP_INPLACE_ADD_UNICODE</td>
<td align="right">3,495</td>
<td align="right">3,495</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">IMPORT_NAME</td>
<td align="right">550</td>
<td align="right">550</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">STORE_ATTR_WITH_HINT</td>
<td align="right">180</td>
<td align="right">180</td>
<td align="right">0.0%</td>
</tr>
<tr>
<td align="left">SEND_GEN</td>
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
<td align="right">221</td>
<td align="right">221</td>
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
<td align="right">780</td>
<td align="right">780</td>
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
<td align="right">780</td>
<td align="right">780</td>
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
<td align="right">1,920</td>
<td align="right">1,920</td>
<td align="right">0.0%</td>
</tr>
</tbody>
</table>


</details>

---
Stats gathered on: 2024-02-20
