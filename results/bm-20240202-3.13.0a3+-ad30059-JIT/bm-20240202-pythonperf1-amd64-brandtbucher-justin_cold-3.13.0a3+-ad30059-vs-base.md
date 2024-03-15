# Results vs. base

- fork: brandtbucher
- ref: justin_cold
- machine: windows-amd64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.00x slower
- HPT reliability: 96.95%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 219 ms                                                                      | 223 ms: 1.02x slower                                                     |
| chameleon      | 4.89 ms                                                                     | 4.82 ms: 1.02x faster                                                    |
| docutils       | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                   |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                             |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none            | 272 ms                                                                      | 264 ms: 1.03x faster                                                     |
| async_tree_none_tg         | 277 ms                                                                      | 281 ms: 1.01x slower                                                     |
| async_tree_io              | 721 ms                                                                      | 738 ms: 1.02x slower                                                     |
| async_tree_io_tg           | 755 ms                                                                      | 777 ms: 1.03x slower                                                     |
| async_tree_memoization_tg  | 347 ms                                                                      | 359 ms: 1.03x slower                                                     |
| async_tree_cpu_io_mixed_tg | 470 ms                                                                      | 488 ms: 1.04x slower                                                     |
| async_tree_cpu_io_mixed    | 450 ms                                                                      | 468 ms: 1.04x slower                                                     |
| Geometric mean             | (ref)                                                                       | 1.02x slower                                                             |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 61.0 ms                                                                     | 61.9 ms: 1.01x slower                                                    |
| Geometric mean | (ref)                                                                       | 1.01x slower                                                             |

Benchmark hidden because not significant (2): pidigits, float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_v8       | 21.8 ms                                                                     | 17.2 ms: 1.27x faster                                                    |
| regex_dna      | 122 ms                                                                      | 118 ms: 1.03x faster                                                     |
| regex_compile  | 81.0 ms                                                                     | 81.6 ms: 1.01x slower                                                    |
| Geometric mean | (ref)                                                                       | 1.07x faster                                                             |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle               | 7.48 us                                                                     | 7.30 us: 1.02x faster                                                    |
| pickle_pure_python   | 179 us                                                                      | 175 us: 1.02x faster                                                     |
| pickle_list          | 2.82 us                                                                     | 2.78 us: 1.02x faster                                                    |
| unpickle_pure_python | 127 us                                                                      | 126 us: 1.01x faster                                                     |
| pickle_dict          | 18.1 us                                                                     | 18.0 us: 1.01x faster                                                    |
| unpickle_list        | 2.73 us                                                                     | 2.76 us: 1.01x slower                                                    |
| json_dumps           | 5.48 ms                                                                     | 5.54 ms: 1.01x slower                                                    |
| xml_etree_parse      | 93.8 ms                                                                     | 95.2 ms: 1.01x slower                                                    |
| tomli_loads          | 1.30 sec                                                                    | 1.32 sec: 1.02x slower                                                   |
| json_loads           | 13.6 us                                                                     | 14.1 us: 1.03x slower                                                    |
| xml_etree_process    | 36.9 ms                                                                     | 38.2 ms: 1.04x slower                                                    |
| xml_etree_iterparse  | 63.8 ms                                                                     | 66.6 ms: 1.04x slower                                                    |
| xml_etree_generate   | 53.8 ms                                                                     | 56.3 ms: 1.05x slower                                                    |
| Geometric mean       | (ref)                                                                       | 1.01x slower                                                             |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site | 18.9 ms                                                                     | 19.2 ms: 1.01x slower                                                    |
| python_startup         | 20.9 ms                                                                     | 21.3 ms: 1.02x slower                                                    |
| Geometric mean         | (ref)                                                                       | 1.02x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako      | 6.79 ms                                                                     | 6.68 ms: 1.02x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:---------------------------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_v8                   | 21.8 ms                                                                     | 17.2 ms: 1.27x faster                                                    |
| scimark_sor                | 77.9 ms                                                                     | 74.4 ms: 1.05x faster                                                    |
| deepcopy_memo              | 22.6 us                                                                     | 21.6 us: 1.05x faster                                                    |
| regex_dna                  | 122 ms                                                                      | 118 ms: 1.03x faster                                                     |
| async_tree_none            | 272 ms                                                                      | 264 ms: 1.03x faster                                                     |
| deepcopy                   | 226 us                                                                      | 221 us: 1.02x faster                                                     |
| pickle                     | 7.48 us                                                                     | 7.30 us: 1.02x faster                                                    |
| bench_thread_pool          | 876 us                                                                      | 855 us: 1.02x faster                                                     |
| pprint_pformat             | 1.04 sec                                                                    | 1.01 sec: 1.02x faster                                                   |
| richards_super             | 29.6 ms                                                                     | 29.0 ms: 1.02x faster                                                    |
| scimark_lu                 | 57.2 ms                                                                     | 56.0 ms: 1.02x faster                                                    |
| pickle_pure_python         | 179 us                                                                      | 175 us: 1.02x faster                                                     |
| mako                       | 6.79 ms                                                                     | 6.68 ms: 1.02x faster                                                    |
| sqlglot_parse              | 764 us                                                                      | 752 us: 1.02x faster                                                     |
| chameleon                  | 4.89 ms                                                                     | 4.82 ms: 1.02x faster                                                    |
| pickle_list                | 2.82 us                                                                     | 2.78 us: 1.02x faster                                                    |
| dask                       | 268 ms                                                                      | 264 ms: 1.02x faster                                                     |
| deepcopy_reduce            | 1.96 us                                                                     | 1.93 us: 1.01x faster                                                    |
| logging_silent             | 53.9 ns                                                                     | 53.2 ns: 1.01x faster                                                    |
| sqlglot_normalize          | 183 ms                                                                      | 181 ms: 1.01x faster                                                     |
| sqlglot_optimize           | 35.2 ms                                                                     | 34.8 ms: 1.01x faster                                                    |
| unpickle_pure_python       | 127 us                                                                      | 126 us: 1.01x faster                                                     |
| richards                   | 25.9 ms                                                                     | 25.7 ms: 1.01x faster                                                    |
| pyflate                    | 315 ms                                                                      | 313 ms: 1.01x faster                                                     |
| docutils                   | 1.62 sec                                                                    | 1.61 sec: 1.01x faster                                                   |
| pickle_dict                | 18.1 us                                                                     | 18.0 us: 1.01x faster                                                    |
| scimark_monte_carlo        | 57.0 ms                                                                     | 56.6 ms: 1.01x faster                                                    |
| mypy2                      | 439 ms                                                                      | 441 ms: 1.00x slower                                                     |
| pathlib                    | 81.5 ms                                                                     | 82.0 ms: 1.01x slower                                                    |
| regex_compile              | 81.0 ms                                                                     | 81.6 ms: 1.01x slower                                                    |
| logging_simple             | 5.98 us                                                                     | 6.03 us: 1.01x slower                                                    |
| sympy_integrate            | 13.4 ms                                                                     | 13.5 ms: 1.01x slower                                                    |
| unpickle_list              | 2.73 us                                                                     | 2.76 us: 1.01x slower                                                    |
| json_dumps                 | 5.48 ms                                                                     | 5.54 ms: 1.01x slower                                                    |
| go                         | 99.3 ms                                                                     | 100 ms: 1.01x slower                                                     |
| scimark_fft                | 195 ms                                                                      | 197 ms: 1.01x slower                                                     |
| raytrace                   | 171 ms                                                                      | 173 ms: 1.01x slower                                                     |
| fannkuch                   | 244 ms                                                                      | 247 ms: 1.01x slower                                                     |
| python_startup_no_site     | 18.9 ms                                                                     | 19.2 ms: 1.01x slower                                                    |
| nbody                      | 61.0 ms                                                                     | 61.9 ms: 1.01x slower                                                    |
| sqlglot_transpile          | 977 us                                                                      | 990 us: 1.01x slower                                                     |
| async_tree_none_tg         | 277 ms                                                                      | 281 ms: 1.01x slower                                                     |
| xml_etree_parse            | 93.8 ms                                                                     | 95.2 ms: 1.01x slower                                                    |
| typing_runtime_protocols   | 70.9 us                                                                     | 72.1 us: 1.02x slower                                                    |
| tomli_loads                | 1.30 sec                                                                    | 1.32 sec: 1.02x slower                                                   |
| meteor_contest             | 76.2 ms                                                                     | 77.5 ms: 1.02x slower                                                    |
| 2to3                       | 219 ms                                                                      | 223 ms: 1.02x slower                                                     |
| python_startup             | 20.9 ms                                                                     | 21.3 ms: 1.02x slower                                                    |
| sqlite_synth               | 1.54 us                                                                     | 1.57 us: 1.02x slower                                                    |
| sympy_expand               | 284 ms                                                                      | 290 ms: 1.02x slower                                                     |
| logging_format             | 6.43 us                                                                     | 6.58 us: 1.02x slower                                                    |
| scimark_sparse_mat_mult    | 2.73 ms                                                                     | 2.79 ms: 1.02x slower                                                    |
| json                       | 2.89 ms                                                                     | 2.96 ms: 1.02x slower                                                    |
| telco                      | 4.46 ms                                                                     | 4.57 ms: 1.02x slower                                                    |
| gc_traversal               | 1.51 ms                                                                     | 1.55 ms: 1.02x slower                                                    |
| async_tree_io              | 721 ms                                                                      | 738 ms: 1.02x slower                                                     |
| async_tree_io_tg           | 755 ms                                                                      | 777 ms: 1.03x slower                                                     |
| spectral_norm              | 65.8 ms                                                                     | 67.7 ms: 1.03x slower                                                    |
| chaos                      | 42.6 ms                                                                     | 43.9 ms: 1.03x slower                                                    |
| comprehensions             | 11.5 us                                                                     | 11.9 us: 1.03x slower                                                    |
| async_generators           | 241 ms                                                                      | 248 ms: 1.03x slower                                                     |
| json_loads                 | 13.6 us                                                                     | 14.1 us: 1.03x slower                                                    |
| async_tree_memoization_tg  | 347 ms                                                                      | 359 ms: 1.03x slower                                                     |
| crypto_pyaes               | 45.3 ms                                                                     | 47.0 ms: 1.04x slower                                                    |
| xml_etree_process          | 36.9 ms                                                                     | 38.2 ms: 1.04x slower                                                    |
| async_tree_cpu_io_mixed_tg | 470 ms                                                                      | 488 ms: 1.04x slower                                                     |
| nqueens                    | 57.5 ms                                                                     | 59.7 ms: 1.04x slower                                                    |
| async_tree_cpu_io_mixed    | 450 ms                                                                      | 468 ms: 1.04x slower                                                     |
| deltablue                  | 2.06 ms                                                                     | 2.14 ms: 1.04x slower                                                    |
| xml_etree_iterparse        | 63.8 ms                                                                     | 66.6 ms: 1.04x slower                                                    |
| generators                 | 19.9 ms                                                                     | 20.8 ms: 1.05x slower                                                    |
| xml_etree_generate         | 53.8 ms                                                                     | 56.3 ms: 1.05x slower                                                    |
| hexiom                     | 5.27 ms                                                                     | 5.52 ms: 1.05x slower                                                    |
| unpack_sequence            | 38.7 ns                                                                     | 43.9 ns: 1.13x slower                                                    |
| Geometric mean             | (ref)                                                                       | 1.00x slower                                                             |

Benchmark hidden because not significant (18): asyncio_tcp_ssl, asyncio_tcp, create_gc_cycles, coverage, pprint_safe_repr, bench_mp_pool, pidigits, coroutines, sympy_sum, regex_effbot, dulwich_log, mdp, sympy_str, unpickle, tornado_http, async_tree_memoization, float, pycparser


# HPT report

- Reliability score: 96.95% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown