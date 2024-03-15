# Results vs. base

- fork: brandtbucher
- ref: justin_nops
- machine: windows-amd64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.01x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 223 ms                                                                      | 226 ms: 1.01x slower                                                     |
| chameleon      | 4.65 ms                                                                     | 4.76 ms: 1.02x slower                                                    |
| docutils       | 1.60 sec                                                                    | 1.59 sec: 1.01x faster                                                   |
| tornado_http   | 85.4 ms                                                                     | 84.8 ms: 1.01x faster                                                    |
| Geometric mean | (ref)                                                                       | 1.01x slower                                                             |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|---------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_memoization    | 343 ms                                                                      | 349 ms: 1.02x slower                                                     |
| async_tree_memoization_tg | 348 ms                                                                      | 355 ms: 1.02x slower                                                     |
| async_tree_cpu_io_mixed   | 450 ms                                                                      | 460 ms: 1.02x slower                                                     |
| async_tree_none_tg        | 272 ms                                                                      | 279 ms: 1.03x slower                                                     |
| async_tree_none           | 266 ms                                                                      | 276 ms: 1.04x slower                                                     |
| Geometric mean            | (ref)                                                                       | 1.02x slower                                                             |

Benchmark hidden because not significant (3): async_tree_io_tg, async_tree_io, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| pidigits       | 149 ms                                                                      | 150 ms: 1.01x slower                                                     |
| Geometric mean | (ref)                                                                       | 1.00x slower                                                             |

Benchmark hidden because not significant (2): nbody, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 83.4 ms                                                                     | 82.2 ms: 1.01x faster                                                    |
| regex_v8       | 14.5 ms                                                                     | 14.5 ms: 1.00x slower                                                    |
| regex_effbot   | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                    |
| regex_dna      | 119 ms                                                                      | 121 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                                       | 1.00x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle_list          | 3.13 us                                                                     | 2.84 us: 1.10x faster                                                    |
| unpickle             | 8.56 us                                                                     | 8.47 us: 1.01x faster                                                    |
| json_dumps           | 5.64 ms                                                                     | 5.59 ms: 1.01x faster                                                    |
| pickle_pure_python   | 175 us                                                                      | 176 us: 1.01x slower                                                     |
| xml_etree_process    | 35.9 ms                                                                     | 36.3 ms: 1.01x slower                                                    |
| pickle_dict          | 17.5 us                                                                     | 17.7 us: 1.01x slower                                                    |
| json_loads           | 13.7 us                                                                     | 13.9 us: 1.01x slower                                                    |
| xml_etree_parse      | 92.3 ms                                                                     | 93.6 ms: 1.01x slower                                                    |
| xml_etree_generate   | 52.5 ms                                                                     | 53.3 ms: 1.01x slower                                                    |
| xml_etree_iterparse  | 62.7 ms                                                                     | 64.1 ms: 1.02x slower                                                    |
| tomli_loads          | 1.17 sec                                                                    | 1.20 sec: 1.02x slower                                                   |
| unpickle_pure_python | 126 us                                                                      | 130 us: 1.03x slower                                                     |
| pickle               | 7.16 us                                                                     | 7.42 us: 1.04x slower                                                    |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                             |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 23.8 ms                                                                     | 24.1 ms: 1.01x slower                                                    |
| python_startup_no_site | 21.5 ms                                                                     | 21.9 ms: 1.02x slower                                                    |
| Geometric mean         | (ref)                                                                       | 1.01x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| genshi_xml     | 34.0 ms                                                                     | 34.7 ms: 1.02x slower                                                    |
| genshi_text    | 15.1 ms                                                                     | 15.5 ms: 1.03x slower                                                    |
| mako           | 5.60 ms                                                                     | 5.78 ms: 1.03x slower                                                    |
| Geometric mean | (ref)                                                                       | 1.02x slower                                                             |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

(0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895) (0.9764001999865286, 0.9774779999861494, 0.9788565000053495, 0.9762938999920152, 0.988859000033699, 0.979882900021039, 0.9904326999676414, 0.9868033000384457, 0.9847668000147678, 0.9704423999646679, 0.9730444000451826, 0.9758911000099033, 0.9732155000092462, 0.970263299997896, 0.9703320999979042, 0.9756191999767907, 0.9787188000045717, 0.9768069999990985, 0.9840637000161223, 0.9885248999926262, 0.9944943000446074, 0.9847567999968305, 0.9814009999972768, 0.9767556000151671, 0.9866828999947757, 0.9819498999859206, 0.9867800999782048, 0.9786330999922939, 0.9811491000000387, 0.9790855000028387, 0.9700897000147961, 0.9687190999975428, 0.9720036999788135, 0.9736299999640323, 0.9765694999950938, 0.977438899979461, 0.9811544999829493, 0.9835996000329033, 0.9838219999801368, 0.980018200003542, 0.9821254000416957, 0.9833258999860846, 0.9855413000332192, 0.9858886000001803, 0.9872898999601603, 0.9872823999612592, 0.9853110000258312, 0.9851304000476375, 1.0655423999996856, 1.0645429999567568, 1.0631619999767281, 0.9833418999915011, 0.9841200000373647, 0.9832981000072323, 1.0471948999911547, 1.047182200010866, 1.048487699998077, 0.9852730000275187, 0.9855715999729, 0.9864275999716483)
| Benchmark                 | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|---------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle_list               | 3.13 us                                                                     | 2.84 us: 1.10x faster                                                    |
| unpack_sequence           | 45.2 ns                                                                     | 43.8 ns: 1.03x faster                                                    |
| asyncio_tcp               | 479 ms                                                                      | 465 ms: 1.03x faster                                                     |
| sympy_sum                 | 88.9 ms                                                                     | 86.2 ms: 1.03x faster                                                    |
| logging_silent            | 56.1 ns                                                                     | 55.2 ns: 1.02x faster                                                    |
| typing_runtime_protocols  | 70.3 us                                                                     | 69.2 us: 1.02x faster                                                    |
| crypto_pyaes              | 43.5 ms                                                                     | 42.8 ms: 1.02x faster                                                    |
| gc_traversal              | 1.52 ms                                                                     | 1.50 ms: 1.01x faster                                                    |
| regex_compile             | 83.4 ms                                                                     | 82.2 ms: 1.01x faster                                                    |
| sympy_expand              | 281 ms                                                                      | 278 ms: 1.01x faster                                                     |
| sympy_str                 | 165 ms                                                                      | 163 ms: 1.01x faster                                                     |
| unpickle                  | 8.56 us                                                                     | 8.47 us: 1.01x faster                                                    |
| docutils                  | 1.60 sec                                                                    | 1.59 sec: 1.01x faster                                                   |
| json_dumps                | 5.64 ms                                                                     | 5.59 ms: 1.01x faster                                                    |
| sqlglot_parse             | 773 us                                                                      | 767 us: 1.01x faster                                                     |
| go                        | 96.2 ms                                                                     | 95.4 ms: 1.01x faster                                                    |
| telco                     | 4.78 ms                                                                     | 4.74 ms: 1.01x faster                                                    |
| tornado_http              | 85.4 ms                                                                     | 84.8 ms: 1.01x faster                                                    |
| mypy2                     | 438 ms                                                                      | 435 ms: 1.01x faster                                                     |
| sympy_integrate           | 13.2 ms                                                                     | 13.1 ms: 1.01x faster                                                    |
| dulwich_log               | 41.5 ms                                                                     | 41.2 ms: 1.01x faster                                                    |
| sqlglot_optimize          | 34.6 ms                                                                     | 34.4 ms: 1.01x faster                                                    |
| meteor_contest            | 73.2 ms                                                                     | 72.9 ms: 1.00x faster                                                    |
| sqlite_synth              | 1.57 us                                                                     | 1.56 us: 1.00x faster                                                    |
| regex_v8                  | 14.5 ms                                                                     | 14.5 ms: 1.00x slower                                                    |
| pathlib                   | 74.8 ms                                                                     | 75.3 ms: 1.01x slower                                                    |
| logging_simple            | 5.82 us                                                                     | 5.86 us: 1.01x slower                                                    |
| hexiom                    | 4.40 ms                                                                     | 4.43 ms: 1.01x slower                                                    |
| richards_super            | 31.1 ms                                                                     | 31.3 ms: 1.01x slower                                                    |
| pidigits                  | 149 ms                                                                      | 150 ms: 1.01x slower                                                     |
| deltablue                 | 2.03 ms                                                                     | 2.04 ms: 1.01x slower                                                    |
| logging_format            | 6.23 us                                                                     | 6.29 us: 1.01x slower                                                    |
| pickle_pure_python        | 175 us                                                                      | 176 us: 1.01x slower                                                     |
| deepcopy_reduce           | 1.91 us                                                                     | 1.93 us: 1.01x slower                                                    |
| xml_etree_process         | 35.9 ms                                                                     | 36.3 ms: 1.01x slower                                                    |
| pickle_dict               | 17.5 us                                                                     | 17.7 us: 1.01x slower                                                    |
| bench_thread_pool         | 829 us                                                                      | 838 us: 1.01x slower                                                     |
| 2to3                      | 223 ms                                                                      | 226 ms: 1.01x slower                                                     |
| async_generators          | 237 ms                                                                      | 240 ms: 1.01x slower                                                     |
| regex_effbot              | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                    |
| comprehensions            | 10.3 us                                                                     | 10.4 us: 1.01x slower                                                    |
| pyflate                   | 281 ms                                                                      | 284 ms: 1.01x slower                                                     |
| json_loads                | 13.7 us                                                                     | 13.9 us: 1.01x slower                                                    |
| coverage                  | 47.0 ms                                                                     | 47.6 ms: 1.01x slower                                                    |
| python_startup            | 23.8 ms                                                                     | 24.1 ms: 1.01x slower                                                    |
| xml_etree_parse           | 92.3 ms                                                                     | 93.6 ms: 1.01x slower                                                    |
| scimark_sor               | 80.6 ms                                                                     | 81.7 ms: 1.01x slower                                                    |
| xml_etree_generate        | 52.5 ms                                                                     | 53.3 ms: 1.01x slower                                                    |
| python_startup_no_site    | 21.5 ms                                                                     | 21.9 ms: 1.02x slower                                                    |
| deepcopy                  | 219 us                                                                      | 222 us: 1.02x slower                                                     |
| regex_dna                 | 119 ms                                                                      | 121 ms: 1.02x slower                                                     |
| async_tree_memoization    | 343 ms                                                                      | 349 ms: 1.02x slower                                                     |
| scimark_sparse_mat_mult   | 2.27 ms                                                                     | 2.31 ms: 1.02x slower                                                    |
| generators                | 20.5 ms                                                                     | 20.8 ms: 1.02x slower                                                    |
| deepcopy_memo             | 21.9 us                                                                     | 22.3 us: 1.02x slower                                                    |
| chaos                     | 39.1 ms                                                                     | 39.9 ms: 1.02x slower                                                    |
| async_tree_memoization_tg | 348 ms                                                                      | 355 ms: 1.02x slower                                                     |
| xml_etree_iterparse       | 62.7 ms                                                                     | 64.1 ms: 1.02x slower                                                    |
| genshi_xml                | 34.0 ms                                                                     | 34.7 ms: 1.02x slower                                                    |
| scimark_lu                | 71.2 ms                                                                     | 72.8 ms: 1.02x slower                                                    |
| async_tree_cpu_io_mixed   | 450 ms                                                                      | 460 ms: 1.02x slower                                                     |
| tomli_loads               | 1.17 sec                                                                    | 1.20 sec: 1.02x slower                                                   |
| chameleon                 | 4.65 ms                                                                     | 4.76 ms: 1.02x slower                                                    |
| genshi_text               | 15.1 ms                                                                     | 15.5 ms: 1.03x slower                                                    |
| spectral_norm             | 50.6 ms                                                                     | 51.9 ms: 1.03x slower                                                    |
| unpickle_pure_python      | 126 us                                                                      | 130 us: 1.03x slower                                                     |
| fannkuch                  | 215 ms                                                                      | 221 ms: 1.03x slower                                                     |
| async_tree_none_tg        | 272 ms                                                                      | 279 ms: 1.03x slower                                                     |
| nqueens                   | 61.0 ms                                                                     | 62.7 ms: 1.03x slower                                                    |
| coroutines                | 13.0 ms                                                                     | 13.3 ms: 1.03x slower                                                    |
| mako                      | 5.60 ms                                                                     | 5.78 ms: 1.03x slower                                                    |
| pprint_pformat            | 957 ms                                                                      | 988 ms: 1.03x slower                                                     |
| scimark_fft               | 168 ms                                                                      | 173 ms: 1.03x slower                                                     |
| async_tree_none           | 266 ms                                                                      | 276 ms: 1.04x slower                                                     |
| pickle                    | 7.16 us                                                                     | 7.42 us: 1.04x slower                                                    |
| scimark_monte_carlo       | 41.3 ms                                                                     | 43.0 ms: 1.04x slower                                                    |
| pprint_safe_repr          | 465 ms                                                                      | 491 ms: 1.06x slower                                                     |
| json                      | 2.88 ms                                                                     | 3.18 ms: 1.10x slower                                                    |
| Geometric mean            | (ref)                                                                       | 1.01x slower                                                             |

Benchmark hidden because not significant (21): pycparser, nbody, unpickle_list, pylint, django_template, sqlglot_transpile, create_gc_cycles, sqlglot_normalize, mdp, thrift, float, richards, raytrace, aiohttp, bench_mp_pool, dask, html5lib, async_tree_io_tg, async_tree_io, async_tree_cpu_io_mixed_tg, asyncio_tcp_ssl


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown