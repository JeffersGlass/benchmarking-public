# Results vs. 3.11.0

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-amd64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.65 ms: 1.13x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                      |
| html5lib       | 38.9 ms                                                     | 35.9 ms: 1.08x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 85.4 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 343 ms: 1.16x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 348 ms: 1.16x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 758 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| float          | 54.4 ms                                                     | 49.4 ms: 1.10x faster                                                       |
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 83.4 ms: 1.09x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.64 ms: 1.44x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.24x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.17 sec: 1.24x faster                                                      |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.3 ms: 1.06x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.5 us: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 35.9 ms: 1.04x faster                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.16 us: 1.08x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.79 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.56 us: 1.13x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.13 us: 1.16x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 21.5 ms: 1.28x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 5.60 ms: 1.35x faster                                                       |
| genshi_text     | 18.4 ms                                                     | 15.1 ms: 1.22x faster                                                       |
| genshi_xml      | 39.9 ms                                                     | 34.0 ms: 1.18x faster                                                       |
| django_template | 24.4 ms                                                     | 21.7 ms: 1.13x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.22x faster                                                                |

All benchmarks:
===============

(1.069666800001869, 1.070101799996337, 1.0674801999994088, 1.0642418999923393, 1.0656395000114571, 1.0802792999893427, 1.081038600008469, 1.0816271000076085, 1.0906404000124894, 1.0890951000037603, 1.0878060999966692, 1.0899319000018295, 1.0925985999929253, 1.0938545000099111, 1.0958068999752868, 1.096803299995372, 1.0952175999991596, 1.098600199999055, 1.0900612999976147, 1.0916431000223383, 1.0743766999803483, 1.0910071000107564, 1.0936696999997366, 1.0878396999905817, 1.092336100002285, 1.0832517000089865, 1.0854626999935135, 1.0951543000119273, 1.0830008999910206, 1.0815367999894079, 1.0806350999919232, 1.0803374999959487, 1.0779242999851704, 1.1151329999847803, 1.1177138999919407, 1.1167247999983374, 1.0823095999949146, 1.0807415999879595, 1.080060100008268, 1.0768554000242148, 1.0720981000049505, 1.0720887000206858, 1.0773757999995723, 1.0790796000219416, 1.0945622000144795, 1.089039699989371, 1.089327499998035, 1.092257399985101, 1.1006929999857675, 1.1013289999973495, 1.1003696999978274, 1.081657999980962, 1.0909678000025451, 1.0791036000009626, 1.0824866000039037, 1.0808675000153016, 1.0863290000124834, 1.0934808000165503, 1.103394899982959, 1.0943593999836594) (0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895)
| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.3 us: 4.64x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.5 ms: 1.66x faster                                                       |
| pylint                     | 323 ms                                                      | 211 ms: 1.53x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.3 us: 1.52x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 479 ms: 1.51x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.64 ms: 1.44x faster                                                       |
| mako                       | 7.58 ms                                                     | 5.60 ms: 1.35x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 50.6 ms: 1.35x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.03 ms: 1.33x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.1 ns: 1.28x faster                                                       |
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.1 ms: 1.24x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.24x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.17 sec: 1.24x faster                                                      |
| chaos                      | 48.4 ms                                                     | 39.1 ms: 1.24x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 773 us: 1.23x faster                                                        |
| genshi_text                | 18.4 ms                                                     | 15.1 ms: 1.22x faster                                                       |
| raytrace                   | 213 ms                                                      | 178 ms: 1.20x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.9 us: 1.19x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.82 us: 1.18x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                        |
| fannkuch                   | 253 ms                                                      | 215 ms: 1.18x faster                                                        |
| genshi_xml                 | 39.9 ms                                                     | 34.0 ms: 1.18x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 991 us: 1.18x faster                                                        |
| nbody                      | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 343 ms: 1.16x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 348 ms: 1.16x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.76 sec: 1.15x faster                                                      |
| logging_format             | 7.16 us                                                     | 6.23 us: 1.15x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 465 ms: 1.14x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.27 ms: 1.14x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 957 ms: 1.14x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.65 ms: 1.13x faster                                                       |
| django_template            | 24.4 ms                                                     | 21.7 ms: 1.13x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 88.9 ms: 1.13x faster                                                       |
| deepcopy                   | 246 us                                                      | 219 us: 1.13x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.13x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.9 ms: 1.12x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 43.5 ms: 1.12x faster                                                       |
| sympy_str                  | 185 ms                                                      | 165 ms: 1.12x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 61.0 ms: 1.12x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 41.5 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 469 ms: 1.12x faster                                                        |
| pyflate                    | 312 ms                                                      | 281 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| float                      | 54.4 ms                                                     | 49.4 ms: 1.10x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.3 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 758 ms: 1.09x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 83.4 ms: 1.09x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 85.4 ms: 1.09x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 176 ms: 1.08x faster                                                        |
| html5lib                   | 38.9 ms                                                     | 35.9 ms: 1.08x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.91 us: 1.08x faster                                                       |
| scimark_fft                | 179 ms                                                      | 168 ms: 1.07x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.06x faster                                                       |
| sympy_expand               | 299 ms                                                      | 281 ms: 1.06x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.3 ms: 1.06x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.5 us: 1.05x faster                                                       |
| bench_thread_pool          | 872 us                                                      | 829 us: 1.05x faster                                                        |
| go                         | 101 ms                                                      | 96.2 ms: 1.05x faster                                                       |
| mypy2                      | 459 ms                                                      | 438 ms: 1.05x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 45.2 ns: 1.04x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 35.9 ms: 1.04x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.54 sec: 1.04x faster                                                      |
| hexiom                     | 4.55 ms                                                     | 4.40 ms: 1.03x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 73.2 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                      |
| pidigits                   | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| gc_traversal               | 1.49 ms                                                     | 1.52 ms: 1.02x slower                                                       |
| aiohttp                    | 883 us                                                      | 903 us: 1.02x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.03x slower                                                        |
| scimark_sor                | 78.1 ms                                                     | 80.6 ms: 1.03x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| 2to3                       | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 751 us: 1.05x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 74.8 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.16 us: 1.08x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.79 us: 1.08x slower                                                       |
| coverage                   | 43.4 ms                                                     | 47.0 ms: 1.08x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 70.2 ms: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.56 us: 1.13x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 71.2 ms: 1.13x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.13 us: 1.16x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.78 ms: 1.18x slower                                                       |
| python_startup             | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 21.5 ms: 1.28x slower                                                       |
| dask                       | 273 ms                                                      | 360 ms: 1.32x slower                                                        |
| async_generators           | 177 ms                                                      | 237 ms: 1.34x slower                                                        |
| thrift                     | 494 us                                                      | 8.87 ms: 17.96x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                                |

Benchmark hidden because not significant (4): json, xml_etree_generate, pycparser, sqlglot_optimize
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown