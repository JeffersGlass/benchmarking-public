# Results vs. base

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-amd64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.01x faster
- HPT reliability: 76.55%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                                      | 219 ms: 1.01x slower                                                      |
| chameleon      | 4.91 ms                                                                     | 4.81 ms: 1.02x faster                                                     |
| docutils       | 1.61 sec                                                                    | 1.60 sec: 1.01x faster                                                    |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_none_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 61.2 ms                                                                     | 55.3 ms: 1.11x faster                                                     |
| float          | 52.2 ms                                                                     | 50.6 ms: 1.03x faster                                                     |
| pidigits       | 154 ms                                                                      | 153 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                                       | 1.05x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8       | 18.9 ms                                                                     | 16.4 ms: 1.15x faster                                                     |
| regex_dna      | 128 ms                                                                      | 118 ms: 1.08x faster                                                      |
| regex_effbot   | 1.62 ms                                                                     | 1.57 ms: 1.03x faster                                                     |
| Geometric mean | (ref)                                                                       | 1.06x faster                                                              |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|---------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| xml_etree_generate  | 53.9 ms                                                                     | 53.1 ms: 1.01x faster                                                     |
| xml_etree_process   | 36.4 ms                                                                     | 36.0 ms: 1.01x faster                                                     |
| pickle              | 7.47 us                                                                     | 7.41 us: 1.01x faster                                                     |
| pickle_dict         | 17.8 us                                                                     | 17.7 us: 1.00x faster                                                     |
| pickle_pure_python  | 176 us                                                                      | 177 us: 1.01x slower                                                      |
| json_dumps          | 5.50 ms                                                                     | 5.54 ms: 1.01x slower                                                     |
| xml_etree_iterparse | 64.5 ms                                                                     | 65.2 ms: 1.01x slower                                                     |
| unpickle            | 8.51 us                                                                     | 8.73 us: 1.03x slower                                                     |
| Geometric mean      | (ref)                                                                       | 1.00x slower                                                              |

Benchmark hidden because not significant (6): json_loads, unpickle_pure_python, tomli_loads, xml_etree_parse, pickle_list, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 21.0 ms                                                                     | 21.1 ms: 1.01x slower                                                     |
| python_startup_no_site | 18.7 ms                                                                     | 19.0 ms: 1.01x slower                                                     |
| Geometric mean         | (ref)                                                                       | 1.01x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 6.86 ms                                                                     | 6.63 ms: 1.03x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20240130-pythonperf1-amd64-python-0990d55725cb649e7473-3.13.0a3+-0990d55 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8                 | 18.9 ms                                                                     | 16.4 ms: 1.15x faster                                                     |
| nbody                    | 61.2 ms                                                                     | 55.3 ms: 1.11x faster                                                     |
| regex_dna                | 128 ms                                                                      | 118 ms: 1.08x faster                                                      |
| crypto_pyaes             | 46.1 ms                                                                     | 43.6 ms: 1.06x faster                                                     |
| generators               | 21.0 ms                                                                     | 20.0 ms: 1.05x faster                                                     |
| chaos                    | 43.2 ms                                                                     | 41.3 ms: 1.05x faster                                                     |
| scimark_fft              | 195 ms                                                                      | 188 ms: 1.03x faster                                                      |
| mako                     | 6.86 ms                                                                     | 6.63 ms: 1.03x faster                                                     |
| spectral_norm            | 64.6 ms                                                                     | 62.5 ms: 1.03x faster                                                     |
| scimark_monte_carlo      | 58.1 ms                                                                     | 56.2 ms: 1.03x faster                                                     |
| float                    | 52.2 ms                                                                     | 50.6 ms: 1.03x faster                                                     |
| regex_effbot             | 1.62 ms                                                                     | 1.57 ms: 1.03x faster                                                     |
| scimark_lu               | 56.6 ms                                                                     | 55.3 ms: 1.02x faster                                                     |
| chameleon                | 4.91 ms                                                                     | 4.81 ms: 1.02x faster                                                     |
| pprint_safe_repr         | 503 ms                                                                      | 493 ms: 1.02x faster                                                      |
| comprehensions           | 11.6 us                                                                     | 11.4 us: 1.02x faster                                                     |
| deepcopy_reduce          | 1.96 us                                                                     | 1.93 us: 1.02x faster                                                     |
| telco                    | 4.57 ms                                                                     | 4.50 ms: 1.02x faster                                                     |
| pyflate                  | 315 ms                                                                      | 310 ms: 1.02x faster                                                      |
| coroutines               | 13.1 ms                                                                     | 12.9 ms: 1.02x faster                                                     |
| meteor_contest           | 79.4 ms                                                                     | 78.3 ms: 1.01x faster                                                     |
| xml_etree_generate       | 53.9 ms                                                                     | 53.1 ms: 1.01x faster                                                     |
| xml_etree_process        | 36.4 ms                                                                     | 36.0 ms: 1.01x faster                                                     |
| sqlite_synth             | 1.57 us                                                                     | 1.56 us: 1.01x faster                                                     |
| scimark_sor              | 77.2 ms                                                                     | 76.3 ms: 1.01x faster                                                     |
| dulwich_log              | 42.2 ms                                                                     | 41.8 ms: 1.01x faster                                                     |
| logging_simple           | 6.05 us                                                                     | 5.98 us: 1.01x faster                                                     |
| pickle                   | 7.47 us                                                                     | 7.41 us: 1.01x faster                                                     |
| deepcopy                 | 222 us                                                                      | 220 us: 1.01x faster                                                      |
| fannkuch                 | 240 ms                                                                      | 238 ms: 1.01x faster                                                      |
| logging_format           | 6.47 us                                                                     | 6.41 us: 1.01x faster                                                     |
| docutils                 | 1.61 sec                                                                    | 1.60 sec: 1.01x faster                                                    |
| pidigits                 | 154 ms                                                                      | 153 ms: 1.01x faster                                                      |
| pickle_dict              | 17.8 us                                                                     | 17.7 us: 1.00x faster                                                     |
| pathlib                  | 79.9 ms                                                                     | 80.2 ms: 1.00x slower                                                     |
| deepcopy_memo            | 22.1 us                                                                     | 22.2 us: 1.00x slower                                                     |
| pickle_pure_python       | 176 us                                                                      | 177 us: 1.01x slower                                                      |
| go                       | 98.1 ms                                                                     | 98.6 ms: 1.01x slower                                                     |
| logging_silent           | 53.3 ns                                                                     | 53.6 ns: 1.01x slower                                                     |
| 2to3                     | 218 ms                                                                      | 219 ms: 1.01x slower                                                      |
| bench_mp_pool            | 70.4 ms                                                                     | 70.8 ms: 1.01x slower                                                     |
| typing_runtime_protocols | 69.6 us                                                                     | 70.1 us: 1.01x slower                                                     |
| python_startup           | 21.0 ms                                                                     | 21.1 ms: 1.01x slower                                                     |
| json_dumps               | 5.50 ms                                                                     | 5.54 ms: 1.01x slower                                                     |
| richards_super           | 28.4 ms                                                                     | 28.6 ms: 1.01x slower                                                     |
| sqlglot_transpile        | 980 us                                                                      | 988 us: 1.01x slower                                                      |
| sqlglot_normalize        | 178 ms                                                                      | 180 ms: 1.01x slower                                                      |
| xml_etree_iterparse      | 64.5 ms                                                                     | 65.2 ms: 1.01x slower                                                     |
| sympy_sum                | 90.5 ms                                                                     | 91.5 ms: 1.01x slower                                                     |
| richards                 | 24.9 ms                                                                     | 25.2 ms: 1.01x slower                                                     |
| python_startup_no_site   | 18.7 ms                                                                     | 19.0 ms: 1.01x slower                                                     |
| gc_traversal             | 1.50 ms                                                                     | 1.53 ms: 1.02x slower                                                     |
| create_gc_cycles         | 742 us                                                                      | 757 us: 1.02x slower                                                      |
| coverage                 | 46.9 ms                                                                     | 47.8 ms: 1.02x slower                                                     |
| sqlglot_parse            | 753 us                                                                      | 768 us: 1.02x slower                                                      |
| sympy_str                | 168 ms                                                                      | 172 ms: 1.02x slower                                                      |
| nqueens                  | 59.5 ms                                                                     | 61.0 ms: 1.03x slower                                                     |
| unpickle                 | 8.51 us                                                                     | 8.73 us: 1.03x slower                                                     |
| sympy_expand             | 280 ms                                                                      | 288 ms: 1.03x slower                                                      |
| mdp                      | 1.52 sec                                                                    | 1.60 sec: 1.05x slower                                                    |
| Geometric mean           | (ref)                                                                       | 1.01x faster                                                              |

Benchmark hidden because not significant (32): asyncio_tcp_ssl, asyncio_tcp, bench_thread_pool, pprint_pformat, raytrace, json_loads, scimark_sparse_mat_mult, hexiom, deltablue, async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, unpack_sequence, mypy2, regex_compile, async_tree_io_tg, unpickle_pure_python, async_generators, sympy_integrate, sqlglot_optimize, tomli_loads, xml_etree_parse, dask, tornado_http, pickle_list, unpickle_list, json, async_tree_none_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none, pycparser


# HPT report

- Reliability score: 76.55% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown