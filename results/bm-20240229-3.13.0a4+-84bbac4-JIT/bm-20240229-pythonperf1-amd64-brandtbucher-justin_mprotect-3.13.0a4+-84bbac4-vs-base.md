# Results vs. base

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-amd64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.00x slower \*
- HPT reliability: 62.97%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| chameleon      | 4.65 ms                                                                     | 4.78 ms: 1.03x slower                                                        |
| docutils       | 1.60 sec                                                                    | 1.60 sec: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                       | 1.00x slower                                                                 |

Benchmark hidden because not significant (2): 2to3, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_memoization, async_tree_io, async_tree_cpu_io_mixed, async_tree_none_tg, async_tree_none, async_tree_io_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 59.9 ms                                                                     | 57.7 ms: 1.04x faster                                                        |
| pidigits       | 149 ms                                                                      | 150 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 83.4 ms                                                                     | 82.2 ms: 1.01x faster                                                        |
| regex_effbot   | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                        |
| regex_dna      | 119 ms                                                                      | 122 ms: 1.02x slower                                                         |
| regex_v8       | 14.5 ms                                                                     | 15.2 ms: 1.05x slower                                                        |
| Geometric mean | (ref)                                                                       | 1.02x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_list          | 3.13 us                                                                     | 2.90 us: 1.08x faster                                                        |
| json_dumps           | 5.64 ms                                                                     | 5.52 ms: 1.02x faster                                                        |
| pickle_dict          | 17.5 us                                                                     | 17.3 us: 1.01x faster                                                        |
| unpickle_pure_python | 126 us                                                                      | 127 us: 1.01x slower                                                         |
| tomli_loads          | 1.17 sec                                                                    | 1.19 sec: 1.01x slower                                                       |
| unpickle             | 8.56 us                                                                     | 8.68 us: 1.01x slower                                                        |
| json_loads           | 13.7 us                                                                     | 14.0 us: 1.02x slower                                                        |
| Geometric mean       | (ref)                                                                       | 1.00x faster                                                                 |

Benchmark hidden because not significant (7): xml_etree_iterparse, xml_etree_process, unpickle_list, pickle, xml_etree_generate, pickle_pure_python, xml_etree_parse

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup_no_site, python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 5.60 ms                                                                     | 5.66 ms: 1.01x slower                                                        |

All benchmarks:
===============

(0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895) (0.9636358999996446, 0.9632778000086546, 0.9665349000133574, 0.9785352000035346, 0.9740889000240713, 0.976940700027626, 0.9554213000228629, 0.9567683999775909, 0.9556110000121407, 0.9551827000104822, 0.95862670004135, 0.962217700027395, 0.961788600019645, 0.9580743000260554, 0.959195900009945, 0.9563548999722116, 0.9537574999849312, 0.9602033999981359, 0.952844199957326, 0.9557405000086874, 0.9565271000028588, 0.9492216000217013, 0.9487981999991462, 0.9470336000085808, 0.9570288999821059, 0.9560706000193022, 0.9579875000054017, 0.9605241999961436, 0.9546692000003532, 0.9516164000378922, 0.9556227999855764, 0.9574985000072047, 0.956743499962613, 0.9871384000289254, 0.9881266999873333, 0.9867071999469772, 0.9815744999796152, 0.9827854000031948, 0.9802835999871604, 0.9568969999672845, 0.9615148999728262, 0.9573435000493191, 0.9453412999864668, 0.9452975000021979, 0.9492357000126503, 0.9667770999949425, 0.969097800028976, 0.9700271000037901, 0.9645702000125311, 0.9619393000029959, 0.9626558999880217, 0.9634958999813534, 0.964584700006526, 0.964076699980069, 0.9643200000282377, 0.9662327999831177, 0.965881799987983, 0.9648692999617197, 0.9656454999931157, 0.9647056999965571)
| Benchmark            | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:---------------------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mdp                  | 1.54 sec                                                                    | 1.38 sec: 1.11x faster                                                       |
| pickle_list          | 3.13 us                                                                     | 2.90 us: 1.08x faster                                                        |
| nbody                | 59.9 ms                                                                     | 57.7 ms: 1.04x faster                                                        |
| sympy_sum            | 88.9 ms                                                                     | 86.0 ms: 1.03x faster                                                        |
| telco                | 4.78 ms                                                                     | 4.66 ms: 1.03x faster                                                        |
| sympy_expand         | 281 ms                                                                      | 275 ms: 1.02x faster                                                         |
| json_dumps           | 5.64 ms                                                                     | 5.52 ms: 1.02x faster                                                        |
| crypto_pyaes         | 43.5 ms                                                                     | 42.7 ms: 1.02x faster                                                        |
| sympy_str            | 165 ms                                                                      | 162 ms: 1.02x faster                                                         |
| regex_compile        | 83.4 ms                                                                     | 82.2 ms: 1.01x faster                                                        |
| pickle_dict          | 17.5 us                                                                     | 17.3 us: 1.01x faster                                                        |
| coverage             | 47.0 ms                                                                     | 46.4 ms: 1.01x faster                                                        |
| sqlglot_optimize     | 34.6 ms                                                                     | 34.2 ms: 1.01x faster                                                        |
| scimark_lu           | 71.2 ms                                                                     | 70.4 ms: 1.01x faster                                                        |
| sympy_integrate      | 13.2 ms                                                                     | 13.1 ms: 1.01x faster                                                        |
| sqlglot_normalize    | 176 ms                                                                      | 174 ms: 1.01x faster                                                         |
| dulwich_log          | 41.5 ms                                                                     | 41.1 ms: 1.01x faster                                                        |
| deepcopy             | 219 us                                                                      | 217 us: 1.01x faster                                                         |
| bench_thread_pool    | 829 us                                                                      | 821 us: 1.01x faster                                                         |
| hexiom               | 4.40 ms                                                                     | 4.37 ms: 1.01x faster                                                        |
| bench_mp_pool        | 70.2 ms                                                                     | 69.8 ms: 1.01x faster                                                        |
| richards             | 27.9 ms                                                                     | 27.8 ms: 1.00x faster                                                        |
| generators           | 20.5 ms                                                                     | 20.4 ms: 1.00x faster                                                        |
| docutils             | 1.60 sec                                                                    | 1.60 sec: 1.00x faster                                                       |
| meteor_contest       | 73.2 ms                                                                     | 73.4 ms: 1.00x slower                                                        |
| pidigits             | 149 ms                                                                      | 150 ms: 1.00x slower                                                         |
| unpickle_pure_python | 126 us                                                                      | 127 us: 1.01x slower                                                         |
| pprint_pformat       | 957 ms                                                                      | 962 ms: 1.01x slower                                                         |
| sqlite_synth         | 1.57 us                                                                     | 1.58 us: 1.01x slower                                                        |
| nqueens              | 61.0 ms                                                                     | 61.4 ms: 1.01x slower                                                        |
| pprint_safe_repr     | 465 ms                                                                      | 468 ms: 1.01x slower                                                         |
| logging_format       | 6.23 us                                                                     | 6.28 us: 1.01x slower                                                        |
| pyflate              | 281 ms                                                                      | 283 ms: 1.01x slower                                                         |
| spectral_norm        | 50.6 ms                                                                     | 51.0 ms: 1.01x slower                                                        |
| scimark_monte_carlo  | 41.3 ms                                                                     | 41.7 ms: 1.01x slower                                                        |
| deepcopy_reduce      | 1.91 us                                                                     | 1.93 us: 1.01x slower                                                        |
| logging_simple       | 5.82 us                                                                     | 5.88 us: 1.01x slower                                                        |
| tomli_loads          | 1.17 sec                                                                    | 1.19 sec: 1.01x slower                                                       |
| mako                 | 5.60 ms                                                                     | 5.66 ms: 1.01x slower                                                        |
| chaos                | 39.1 ms                                                                     | 39.6 ms: 1.01x slower                                                        |
| async_generators     | 237 ms                                                                      | 240 ms: 1.01x slower                                                         |
| raytrace             | 178 ms                                                                      | 180 ms: 1.01x slower                                                         |
| regex_effbot         | 1.56 ms                                                                     | 1.58 ms: 1.01x slower                                                        |
| unpickle             | 8.56 us                                                                     | 8.68 us: 1.01x slower                                                        |
| json_loads           | 13.7 us                                                                     | 14.0 us: 1.02x slower                                                        |
| regex_dna            | 119 ms                                                                      | 122 ms: 1.02x slower                                                         |
| go                   | 96.2 ms                                                                     | 98.4 ms: 1.02x slower                                                        |
| fannkuch             | 215 ms                                                                      | 220 ms: 1.02x slower                                                         |
| comprehensions       | 10.3 us                                                                     | 10.6 us: 1.03x slower                                                        |
| chameleon            | 4.65 ms                                                                     | 4.78 ms: 1.03x slower                                                        |
| unpack_sequence      | 45.2 ns                                                                     | 46.6 ns: 1.03x slower                                                        |
| coroutines           | 13.0 ms                                                                     | 13.4 ms: 1.03x slower                                                        |
| regex_v8             | 14.5 ms                                                                     | 15.2 ms: 1.05x slower                                                        |
| deltablue            | 2.03 ms                                                                     | 2.13 ms: 1.05x slower                                                        |
| json                 | 2.88 ms                                                                     | 3.22 ms: 1.12x slower                                                        |
| Geometric mean       | (ref)                                                                       | 1.00x slower                                                                 |

Benchmark hidden because not significant (37): asyncio_tcp, async_tree_cpu_io_mixed_tg, xml_etree_iterparse, float, async_tree_memoization, async_tree_io, logging_silent, tornado_http, create_gc_cycles, xml_etree_process, 2to3, unpickle_list, dask, python_startup_no_site, async_tree_cpu_io_mixed, mypy2, pickle, async_tree_none_tg, xml_etree_generate, scimark_sor, deepcopy_memo, python_startup, sqlglot_parse, typing_runtime_protocols, async_tree_none, scimark_sparse_mat_mult, async_tree_io_tg, pickle_pure_python, pathlib, richards_super, sqlglot_transpile, xml_etree_parse, gc_traversal, scimark_fft, async_tree_memoization_tg, asyncio_tcp_ssl, pycparser
Ignored benchmarks (7) of results/bm-20240305-3.13.0a4+-e7ba6e9-JIT/bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9.json: aiohttp, django_template, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 62.97% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown