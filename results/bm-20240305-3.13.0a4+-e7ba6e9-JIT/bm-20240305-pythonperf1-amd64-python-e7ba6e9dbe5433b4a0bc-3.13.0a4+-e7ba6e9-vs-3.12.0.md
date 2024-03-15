# Results vs. 3.12.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-amd64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.65 ms: 1.07x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 85.4 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 266 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 469 ms: 1.07x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 348 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 758 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| float          | 56.8 ms                                                     | 49.4 ms: 1.15x faster                                                       |
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| regex_compile  | 87.5 ms                                                     | 83.4 ms: 1.05x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.17 sec: 1.16x faster                                                      |
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 126 us: 1.05x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 35.9 ms: 1.05x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.5 us: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                       |
| pickle               | 7.43 us                                                     | 7.16 us: 1.04x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.64 ms: 1.01x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 92.3 ms: 1.01x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.56 us: 1.05x slower                                                       |
| pickle_list          | 2.83 us                                                     | 3.13 us: 1.11x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 21.5 ms: 1.32x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 5.60 ms: 1.26x faster                                                       |
| django_template | 22.9 ms                                                     | 21.7 ms: 1.06x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.16x faster                                                                |

All benchmarks:
===============

(1.0581592000089586, 1.0508994999690913, 1.0530731999897398, 1.0565256999689154, 1.057083799969405, 1.0526052000350319, 1.0482068000128493, 1.050936300016474, 1.0625469000078738, 1.0501327000092715, 1.0541929999599233, 1.0507962999981828, 1.0469284999999218, 1.0364553999970667, 1.038367000001017, 1.0409456999623217, 1.0398322999826632, 1.03934770001797, 1.0647261000121944, 1.0584455000353046, 1.0640026000328362, 1.0273238000227138, 1.0279245999990962, 1.024962699972093, 1.0298218000098132, 1.029082200024277, 1.0314507000148296, 1.0308961999835446, 1.0296757000032812, 1.0301529999705963, 1.035241900011897, 1.035953500017058, 1.0323822999489494, 1.0266414000070654, 1.0393097000196576, 1.0428778999485075, 1.0478622999507934, 1.063087299990002, 1.0513648000196554, 1.0435614999732934, 1.0384969000006095, 1.044002900016494, 1.0615719999768771, 1.0546698000398465, 1.063662700005807, 1.0356341000297107, 1.038258099986706, 1.049909099994693, 1.0531851000268944, 1.0537685999879614, 1.054927199962549, 1.040751199994702, 1.0427462999941781, 1.0455802000360563, 1.0537894000299275, 1.0440105000161566, 1.0437913999776356, 1.0566787999705411, 1.0449613999808207, 1.041578100004699) (0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895)
| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| comprehensions             | 14.1 us                                                     | 10.3 us: 1.37x faster                                                       |
| typing_runtime_protocols   | 95.1 us                                                     | 70.3 us: 1.35x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 50.6 ms: 1.32x faster                                                       |
| mako                       | 7.09 ms                                                     | 5.60 ms: 1.26x faster                                                       |
| nbody                      | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.76 sec: 1.19x faster                                                      |
| tomli_loads                | 1.37 sec                                                    | 1.17 sec: 1.16x faster                                                      |
| mypy2                      | 509 ms                                                      | 438 ms: 1.16x faster                                                        |
| float                      | 56.8 ms                                                     | 49.4 ms: 1.15x faster                                                       |
| fannkuch                   | 247 ms                                                      | 215 ms: 1.15x faster                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.27 ms: 1.13x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.57 us: 1.12x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.12x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 43.5 ms: 1.12x faster                                                       |
| chaos                      | 43.3 ms                                                     | 39.1 ms: 1.11x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 465 ms: 1.10x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.5 ms: 1.10x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                       |
| scimark_fft                | 184 ms                                                      | 168 ms: 1.10x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.91 us: 1.10x faster                                                       |
| async_tree_none            | 291 ms                                                      | 266 ms: 1.09x faster                                                        |
| pprint_pformat             | 1.05 sec                                                    | 957 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                        |
| deepcopy                   | 238 us                                                      | 219 us: 1.09x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 21.9 us: 1.08x faster                                                       |
| raytrace                   | 192 ms                                                      | 178 ms: 1.08x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 56.1 ns: 1.08x faster                                                       |
| logging_simple             | 6.28 us                                                     | 5.82 us: 1.08x faster                                                       |
| logging_format             | 6.72 us                                                     | 6.23 us: 1.08x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 74.8 ms: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 469 ms: 1.07x faster                                                        |
| chameleon                  | 4.98 ms                                                     | 4.65 ms: 1.07x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 41.5 ms: 1.07x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.03 ms: 1.07x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 176 ms: 1.07x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                                       |
| sympy_str                  | 175 ms                                                      | 165 ms: 1.06x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 41.3 ms: 1.06x faster                                                       |
| django_template            | 22.9 ms                                                     | 21.7 ms: 1.06x faster                                                       |
| json                       | 3.05 ms                                                     | 2.88 ms: 1.06x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 348 ms: 1.05x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 126 us: 1.05x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 35.9 ms: 1.05x faster                                                       |
| pyflate                    | 295 ms                                                      | 281 ms: 1.05x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 83.4 ms: 1.05x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.5 us: 1.05x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.4 ms: 1.05x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 773 us: 1.04x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.16 us: 1.04x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| bench_thread_pool          | 857 us                                                      | 829 us: 1.03x faster                                                        |
| richards_super             | 32.1 ms                                                     | 31.1 ms: 1.03x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 991 us: 1.03x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 88.9 ms: 1.03x faster                                                       |
| nqueens                    | 62.8 ms                                                     | 61.0 ms: 1.03x faster                                                       |
| pidigits                   | 152 ms                                                      | 149 ms: 1.02x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.2 ms: 1.02x faster                                                       |
| async_tree_io_tg           | 771 ms                                                      | 758 ms: 1.02x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.9 ms: 1.02x faster                                                       |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| async_generators           | 239 ms                                                      | 237 ms: 1.01x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.64 ms: 1.01x faster                                                       |
| sympy_expand               | 284 ms                                                      | 281 ms: 1.01x faster                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 92.3 ms: 1.01x faster                                                       |
| bench_mp_pool              | 69.2 ms                                                     | 70.2 ms: 1.01x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.79 us: 1.01x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                       |
| aiohttp                    | 884 us                                                      | 903 us: 1.02x slower                                                        |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| scimark_sor                | 78.8 ms                                                     | 80.6 ms: 1.02x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.56 us: 1.05x slower                                                       |
| go                         | 91.6 ms                                                     | 96.2 ms: 1.05x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 4.40 ms: 1.07x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.13 us: 1.11x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.54 sec: 1.12x slower                                                      |
| coverage                   | 40.8 ms                                                     | 47.0 ms: 1.15x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.78 ms: 1.16x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 45.2 ns: 1.21x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 71.2 ms: 1.21x slower                                                       |
| python_startup             | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 21.5 ms: 1.32x slower                                                       |
| dask                       | 263 ms                                                      | 360 ms: 1.37x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (7): asyncio_tcp, async_tree_io, gc_traversal, create_gc_cycles, sqlglot_optimize, async_tree_memoization, pycparser
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (5) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown