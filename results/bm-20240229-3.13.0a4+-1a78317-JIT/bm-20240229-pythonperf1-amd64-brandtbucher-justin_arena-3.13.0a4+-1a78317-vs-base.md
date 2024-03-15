# Results vs. base

- fork: brandtbucher
- ref: justin_arena
- machine: windows-amd64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.01x faster
- HPT reliability: 65.21%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| chameleon      | 4.65 ms                                                                     | 4.85 ms: 1.04x slower                                                     |
| docutils       | 1.60 sec                                                                    | 1.57 sec: 1.02x faster                                                    |
| Geometric mean | (ref)                                                                       | 1.01x slower                                                              |

Benchmark hidden because not significant (3): 2to3, html5lib, tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_io, async_tree_memoization, async_tree_none_tg, async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 59.9 ms                                                                     | 57.6 ms: 1.04x faster                                                     |
| pidigits       | 149 ms                                                                      | 150 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                              |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 83.4 ms                                                                     | 77.7 ms: 1.07x faster                                                     |
| regex_effbot   | 1.56 ms                                                                     | 1.59 ms: 1.02x slower                                                     |
| regex_dna      | 119 ms                                                                      | 125 ms: 1.05x slower                                                      |
| regex_v8       | 14.5 ms                                                                     | 15.3 ms: 1.06x slower                                                     |
| Geometric mean | (ref)                                                                       | 1.01x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 2.79 us                                                                     | 2.72 us: 1.03x faster                                                     |
| json_dumps           | 5.64 ms                                                                     | 5.52 ms: 1.02x faster                                                     |
| unpickle             | 8.56 us                                                                     | 8.39 us: 1.02x faster                                                     |
| pickle_dict          | 17.5 us                                                                     | 17.4 us: 1.01x faster                                                     |
| pickle_pure_python   | 175 us                                                                      | 175 us: 1.00x slower                                                      |
| xml_etree_generate   | 52.5 ms                                                                     | 52.9 ms: 1.01x slower                                                     |
| tomli_loads          | 1.17 sec                                                                    | 1.18 sec: 1.01x slower                                                    |
| xml_etree_parse      | 92.3 ms                                                                     | 93.4 ms: 1.01x slower                                                     |
| xml_etree_process    | 35.9 ms                                                                     | 36.4 ms: 1.01x slower                                                     |
| unpickle_pure_python | 126 us                                                                      | 129 us: 1.02x slower                                                      |
| Geometric mean       | (ref)                                                                       | 1.00x faster                                                              |

Benchmark hidden because not significant (4): pickle_list, pickle, json_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 21.5 ms                                                                     | 21.1 ms: 1.02x faster                                                     |
| python_startup         | 23.8 ms                                                                     | 23.4 ms: 1.02x faster                                                     |
| Geometric mean         | (ref)                                                                       | 1.02x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| genshi_xml      | 34.0 ms                                                                     | 34.6 ms: 1.02x slower                                                     |
| mako            | 5.60 ms                                                                     | 5.75 ms: 1.03x slower                                                     |
| django_template | 21.7 ms                                                                     | 22.7 ms: 1.05x slower                                                     |
| Geometric mean  | (ref)                                                                       | 1.02x slower                                                              |

Benchmark hidden because not significant (1): genshi_text

All benchmarks:
===============

(0.9802414000150748, 0.9817258000257425, 0.983259700005874, 0.9464508999953978, 0.943858899991028, 0.9435233999975026, 0.9522970999823883, 0.9537883999873884, 0.9502483999822289, 0.9537391000194475, 0.9532421000185423, 0.9551256000413559, 0.9615367000224069, 0.9557708000065759, 0.9577341999975033, 0.9559007000061683, 0.9556479000020772, 0.9581971000297926, 0.948384499992244, 0.949968499946408, 0.9497418999671936, 0.983502299990505, 0.9819843000150286, 0.9786233999766409, 0.9497646999661811, 0.9532970999716781, 0.9517057000193745, 0.9479628000408411, 0.9499812999856658, 0.950471899996046, 0.9446143000386655, 0.9481056000222452, 0.9430782999843359, 0.9576117999968119, 0.9517827000236139, 0.9558519000420347, 0.9579373000306077, 0.9541297000250779, 0.9582457999931648, 0.9488390000187792, 0.9476644000387751, 0.9486552000162192, 0.9629601000342518, 0.9652758999727666, 0.9637638999847695, 0.9912697999970987, 0.9892013000207953, 0.9870476000360213, 0.960979099967517, 0.9612147999578156, 0.9586885999888182, 0.9550085000228137, 0.9582801000215113, 0.9554780999897048, 0.9457708999980241, 0.9407628999906592, 0.9427646000403911, 0.9527994000236504, 0.9506565000046976, 0.9515495999949053, 0.947808199969586, 0.945997700036969, 0.9474746999912895) (0.9720709000248462, 0.9732116999803111, 0.9729988000472076, 0.9703076999867335, 0.9703336999518797, 0.9704669999773614, 1.0045878000091761, 1.009446799987927, 1.0071647999575362, 0.9714827000279911, 0.9709494999842718, 0.970517799956724, 0.9629267000127584, 0.9614479999872856, 0.9622531000059098, 0.9698039999930188, 0.9701629999908619, 0.9710780000314116, 0.9773939999868162, 0.9703908999799751, 0.9697880999883637, 1.001585200021509, 1.0080348000046797, 1.0015007999609224, 0.9679173000040464, 0.9692407000111416, 0.9694847000064328, 0.9630739000276662, 0.9634944000281394, 0.9638779000379145, 0.9639500000048429, 0.9597838000045158, 0.9618731999653392, 0.9719934000167996, 0.9726792000001296, 0.9700204000109807, 0.9696568000363186, 0.9665068999747746, 0.9704479000065476, 0.9662335999892093, 0.9677032000035979, 0.966772600018885, 1.014807200001087, 1.0171958000282757, 1.0217493000091054, 0.9634522999986075, 0.9657048999797553, 0.9661713000386953, 0.9767930000089109, 0.9928792000282556, 0.9956172999809496, 0.9711593999527395, 0.9757439999957569, 0.9740453000413254, 0.9789985999814235, 0.975258499966003, 0.9786095999879763, 0.9700021999888122, 0.9683350000414066, 0.972192500019446)
| Benchmark                | bm-20240305-pythonperf1-amd64-python-e7ba6e9dbe5433b4a0bc-3.13.0a4+-e7ba6e9 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpack_sequence          | 45.2 ns                                                                     | 37.7 ns: 1.20x faster                                                     |
| mdp                      | 1.54 sec                                                                    | 1.38 sec: 1.11x faster                                                    |
| richards                 | 27.9 ms                                                                     | 25.5 ms: 1.09x faster                                                     |
| hexiom                   | 4.40 ms                                                                     | 4.04 ms: 1.09x faster                                                     |
| regex_compile            | 83.4 ms                                                                     | 77.7 ms: 1.07x faster                                                     |
| pycparser                | 719 ms                                                                      | 673 ms: 1.07x faster                                                      |
| richards_super           | 31.1 ms                                                                     | 29.3 ms: 1.06x faster                                                     |
| nbody                    | 59.9 ms                                                                     | 57.6 ms: 1.04x faster                                                     |
| fannkuch                 | 215 ms                                                                      | 209 ms: 1.03x faster                                                      |
| unpickle_list            | 2.79 us                                                                     | 2.72 us: 1.03x faster                                                     |
| crypto_pyaes             | 43.5 ms                                                                     | 42.4 ms: 1.03x faster                                                     |
| go                       | 96.2 ms                                                                     | 93.9 ms: 1.02x faster                                                     |
| json_dumps               | 5.64 ms                                                                     | 5.52 ms: 1.02x faster                                                     |
| scimark_sparse_mat_mult  | 2.27 ms                                                                     | 2.22 ms: 1.02x faster                                                     |
| coverage                 | 47.0 ms                                                                     | 46.0 ms: 1.02x faster                                                     |
| python_startup_no_site   | 21.5 ms                                                                     | 21.1 ms: 1.02x faster                                                     |
| unpickle                 | 8.56 us                                                                     | 8.39 us: 1.02x faster                                                     |
| docutils                 | 1.60 sec                                                                    | 1.57 sec: 1.02x faster                                                    |
| telco                    | 4.78 ms                                                                     | 4.70 ms: 1.02x faster                                                     |
| python_startup           | 23.8 ms                                                                     | 23.4 ms: 1.02x faster                                                     |
| gc_traversal             | 1.52 ms                                                                     | 1.50 ms: 1.01x faster                                                     |
| sympy_expand             | 281 ms                                                                      | 278 ms: 1.01x faster                                                      |
| bench_mp_pool            | 70.2 ms                                                                     | 69.2 ms: 1.01x faster                                                     |
| sympy_str                | 165 ms                                                                      | 163 ms: 1.01x faster                                                      |
| spectral_norm            | 50.6 ms                                                                     | 50.0 ms: 1.01x faster                                                     |
| typing_runtime_protocols | 70.3 us                                                                     | 69.5 us: 1.01x faster                                                     |
| sqlglot_parse            | 773 us                                                                      | 766 us: 1.01x faster                                                      |
| aiohttp                  | 903 us                                                                      | 894 us: 1.01x faster                                                      |
| scimark_fft              | 168 ms                                                                      | 166 ms: 1.01x faster                                                      |
| sympy_sum                | 88.9 ms                                                                     | 88.1 ms: 1.01x faster                                                     |
| mypy2                    | 438 ms                                                                      | 436 ms: 1.01x faster                                                      |
| pickle_dict              | 17.5 us                                                                     | 17.4 us: 1.01x faster                                                     |
| pickle_pure_python       | 175 us                                                                      | 175 us: 1.00x slower                                                      |
| meteor_contest           | 73.2 ms                                                                     | 73.6 ms: 1.01x slower                                                     |
| pidigits                 | 149 ms                                                                      | 150 ms: 1.01x slower                                                      |
| generators               | 20.5 ms                                                                     | 20.6 ms: 1.01x slower                                                     |
| chaos                    | 39.1 ms                                                                     | 39.4 ms: 1.01x slower                                                     |
| deepcopy                 | 219 us                                                                      | 221 us: 1.01x slower                                                      |
| xml_etree_generate       | 52.5 ms                                                                     | 52.9 ms: 1.01x slower                                                     |
| tomli_loads              | 1.17 sec                                                                    | 1.18 sec: 1.01x slower                                                    |
| logging_format           | 6.23 us                                                                     | 6.29 us: 1.01x slower                                                     |
| sqlglot_normalize        | 176 ms                                                                      | 177 ms: 1.01x slower                                                      |
| xml_etree_parse          | 92.3 ms                                                                     | 93.4 ms: 1.01x slower                                                     |
| xml_etree_process        | 35.9 ms                                                                     | 36.4 ms: 1.01x slower                                                     |
| nqueens                  | 61.0 ms                                                                     | 61.9 ms: 1.01x slower                                                     |
| pprint_safe_repr         | 465 ms                                                                      | 473 ms: 1.02x slower                                                      |
| coroutines               | 13.0 ms                                                                     | 13.2 ms: 1.02x slower                                                     |
| genshi_xml               | 34.0 ms                                                                     | 34.6 ms: 1.02x slower                                                     |
| unpickle_pure_python     | 126 us                                                                      | 129 us: 1.02x slower                                                      |
| pprint_pformat           | 957 ms                                                                      | 976 ms: 1.02x slower                                                      |
| scimark_lu               | 71.2 ms                                                                     | 72.7 ms: 1.02x slower                                                     |
| comprehensions           | 10.3 us                                                                     | 10.5 us: 1.02x slower                                                     |
| deepcopy_reduce          | 1.91 us                                                                     | 1.95 us: 1.02x slower                                                     |
| regex_effbot             | 1.56 ms                                                                     | 1.59 ms: 1.02x slower                                                     |
| deepcopy_memo            | 21.9 us                                                                     | 22.4 us: 1.02x slower                                                     |
| mako                     | 5.60 ms                                                                     | 5.75 ms: 1.03x slower                                                     |
| deltablue                | 2.03 ms                                                                     | 2.09 ms: 1.03x slower                                                     |
| scimark_sor              | 80.6 ms                                                                     | 83.1 ms: 1.03x slower                                                     |
| chameleon                | 4.65 ms                                                                     | 4.85 ms: 1.04x slower                                                     |
| django_template          | 21.7 ms                                                                     | 22.7 ms: 1.05x slower                                                     |
| regex_dna                | 119 ms                                                                      | 125 ms: 1.05x slower                                                      |
| regex_v8                 | 14.5 ms                                                                     | 15.3 ms: 1.06x slower                                                     |
| Geometric mean           | (ref)                                                                       | 1.01x faster                                                              |

Benchmark hidden because not significant (37): pickle_list, asyncio_tcp, async_tree_cpu_io_mixed_tg, bench_thread_pool, logging_silent, raytrace, thrift, create_gc_cycles, pylint, sqlglot_transpile, dulwich_log, tornado_http, logging_simple, pathlib, pickle, json, sympy_integrate, float, json_loads, pyflate, async_generators, sqlglot_optimize, asyncio_tcp_ssl, 2to3, scimark_monte_carlo, sqlite_synth, async_tree_io_tg, async_tree_io, genshi_text, async_tree_memoization, xml_etree_iterparse, async_tree_none_tg, async_tree_cpu_io_mixed, dask, async_tree_memoization_tg, async_tree_none, html5lib


# HPT report

- Reliability score: 65.21% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown