# Results vs. 3.10.4

- fork: python
- ref: e7ba6e9dbe5433b4a0bc
- machine: windows-amd64
- commit hash: e7ba6e9
- commit date: 2024-03-05
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.65 ms: 1.24x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| html5lib       | 51.0 ms                                                     | 35.9 ms: 1.42x faster                                                       |
| tornado_http   | 108 ms                                                      | 85.4 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.24x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 266 ms: 1.63x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 343 ms: 1.53x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.4 ms: 1.25x faster                                                       |
| nbody          | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 83.4 ms: 1.27x faster                                                       |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.07x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.64 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 126 us: 1.45x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.17 sec: 1.42x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 35.9 ms: 1.24x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.56 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.3 ms: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.5 us: 1.02x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.16 us: 1.05x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.13 us: 1.14x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.8 ms: 1.15x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 21.5 ms: 1.39x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 5.60 ms: 1.61x faster                                                       |
| django_template | 28.9 ms                                                     | 21.7 ms: 1.33x faster                                                       |
| genshi_text     | 19.8 ms                                                     | 15.1 ms: 1.31x faster                                                       |
| genshi_xml      | 41.0 ms                                                     | 34.0 ms: 1.21x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.36x faster                                                                |

All benchmarks:
===============

(1.2228629000019282, 1.221847600012552, 1.229935299983481, 1.2293889000138734, 1.2387021000031382, 1.2114858999848366, 1.220408299996052, 1.2296389999974053, 1.2264187000109814, 1.21996489999583, 1.220440300006885, 1.2168154999963008, 1.2132056999835186, 1.2237406999920495, 1.2149781000043731, 1.2292622000095434, 1.2187314999755472, 1.2097657000122126, 1.2068776999949478, 1.2039292999834288, 1.1992265000008047, 1.2085009000147693, 1.2081141000089701, 1.2093100000056438, 1.2204678999842145, 1.2192479000077583, 1.2191150000144262, 1.2127564999973401, 1.2184550000238232, 1.209821100026602, 1.2113817000063136, 1.214227699994808, 1.2141529000073206, 1.2385967999871355, 1.247022299998207, 1.2656406000023708, 1.2178605999797583, 1.2233886999893002, 1.2133217999944463, 1.2450236000004224, 1.2472425999876577, 1.2472157999873161, 1.2308516000048257, 1.235978000011528, 1.236487699992722, 1.2397190000046976, 1.2303900999831967, 1.2260595000116155, 1.2148622999957297, 1.2189961000112817, 1.2147572000103537, 1.239117699995404, 1.2182410000241362, 1.1907736000139266, 1.1933201999927405, 1.2016497000004165, 1.1979826999886427, 1.1815624000155367, 1.193626399995992, 1.1803671999950893) (0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895)
| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.3 us: 4.78x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.03 ms: 2.07x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.1 ns: 1.69x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.1 ms: 1.68x faster                                                       |
| pylint                   | 350 ms                                                      | 211 ms: 1.66x faster                                                        |
| async_tree_none          | 435 ms                                                      | 266 ms: 1.63x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.64 ms: 1.62x faster                                                       |
| mako                     | 9.03 ms                                                     | 5.60 ms: 1.61x faster                                                       |
| comprehensions           | 16.5 us                                                     | 10.3 us: 1.60x faster                                                       |
| generators               | 32.4 ms                                                     | 20.5 ms: 1.58x faster                                                       |
| chaos                    | 61.7 ms                                                     | 39.1 ms: 1.58x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 773 us: 1.57x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                                        |
| raytrace                 | 273 ms                                                      | 178 ms: 1.54x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 343 ms: 1.53x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 479 ms: 1.53x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 50.6 ms: 1.53x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.9 ms: 1.52x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 991 us: 1.49x faster                                                        |
| pyflate                  | 409 ms                                                      | 281 ms: 1.46x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 126 us: 1.45x faster                                                        |
| go                       | 139 ms                                                      | 96.2 ms: 1.44x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 43.5 ms: 1.44x faster                                                       |
| html5lib                 | 51.0 ms                                                     | 35.9 ms: 1.42x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.17 sec: 1.42x faster                                                      |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.3 ms: 1.39x faster                                                       |
| django_template          | 28.9 ms                                                     | 21.7 ms: 1.33x faster                                                       |
| scimark_sor              | 106 ms                                                      | 80.6 ms: 1.32x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 21.9 us: 1.31x faster                                                       |
| genshi_text              | 19.8 ms                                                     | 15.1 ms: 1.31x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 4.40 ms: 1.30x faster                                                       |
| pycparser                | 930 ms                                                      | 719 ms: 1.29x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 957 ms: 1.27x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 465 ms: 1.27x faster                                                        |
| regex_compile            | 106 ms                                                      | 83.4 ms: 1.27x faster                                                       |
| tornado_http             | 108 ms                                                      | 85.4 ms: 1.27x faster                                                       |
| mypy2                    | 555 ms                                                      | 438 ms: 1.27x faster                                                        |
| float                    | 61.7 ms                                                     | 49.4 ms: 1.25x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.65 ms: 1.24x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 35.9 ms: 1.24x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.22x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 41.5 ms: 1.22x faster                                                       |
| genshi_xml               | 41.0 ms                                                     | 34.0 ms: 1.21x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 71.2 ms: 1.20x faster                                                       |
| sympy_sum                | 107 ms                                                      | 88.9 ms: 1.20x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.27 ms: 1.20x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.76 sec: 1.20x faster                                                      |
| nbody                    | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| fannkuch                 | 256 ms                                                      | 215 ms: 1.19x faster                                                        |
| sympy_str                | 194 ms                                                      | 165 ms: 1.18x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 176 ms: 1.17x faster                                                        |
| deepcopy                 | 255 us                                                      | 219 us: 1.17x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.54 sec: 1.16x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 829 us: 1.16x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.91 us: 1.15x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.6 ms: 1.15x faster                                                       |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| sympy_expand             | 314 ms                                                      | 281 ms: 1.12x faster                                                        |
| scimark_fft              | 187 ms                                                      | 168 ms: 1.12x faster                                                        |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| aiohttp                  | 995 us                                                      | 903 us: 1.10x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 61.0 ms: 1.09x faster                                                       |
| json                     | 3.14 ms                                                     | 2.88 ms: 1.09x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.23 us: 1.08x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.82 us: 1.07x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.07x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 751 us: 1.07x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.56 us: 1.06x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.3 ms: 1.05x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.2 ms: 1.04x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 74.8 ms: 1.01x faster                                                       |
| pickle_dict              | 17.2 us                                                     | 17.5 us: 1.02x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.79 us: 1.03x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.16 us: 1.05x slower                                                       |
| async_generators         | 222 ms                                                      | 237 ms: 1.07x slower                                                        |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 70.2 ms: 1.13x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.13 us: 1.14x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 45.2 ns: 1.14x slower                                                       |
| dask                     | 313 ms                                                      | 360 ms: 1.15x slower                                                        |
| python_startup           | 20.6 ms                                                     | 23.8 ms: 1.15x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.0 ms: 1.20x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.78 ms: 1.21x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 21.5 ms: 1.39x slower                                                       |
| thrift                   | 617 us                                                      | 8.87 ms: 14.37x slower                                                      |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                                |

Benchmark hidden because not significant (1): pidigits
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown