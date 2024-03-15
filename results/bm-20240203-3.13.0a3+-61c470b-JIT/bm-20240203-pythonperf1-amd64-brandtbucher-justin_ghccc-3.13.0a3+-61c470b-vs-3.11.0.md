
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: windows-amd64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 219 ms: 1.03x slower                                                      |
| chameleon      | 5.26 ms                                                     | 4.81 ms: 1.10x faster                                                     |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                    |
| tornado_http   | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.04x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 279 ms: 1.19x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 461 ms: 1.15x faster                                                      |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                      |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 282 ms: 1.09x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 482 ms: 1.09x faster                                                      |
| async_tree_io              | 808 ms                                                      | 750 ms: 1.08x faster                                                      |
| async_tree_io_tg           | 829 ms                                                      | 773 ms: 1.07x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 55.3 ms: 1.27x faster                                                     |
| float          | 54.4 ms                                                     | 50.6 ms: 1.07x faster                                                     |
| pidigits       | 150 ms                                                      | 153 ms: 1.02x slower                                                      |
| Geometric mean | (ref)                                                       | 1.10x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                     |
| regex_dna      | 116 ms                                                      | 118 ms: 1.02x slower                                                      |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                     |
| regex_v8       | 14.2 ms                                                     | 16.4 ms: 1.16x slower                                                     |
| Geometric mean | (ref)                                                       | 1.03x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                     |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.21x faster                                                      |
| pickle_pure_python   | 208 us                                                      | 177 us: 1.18x faster                                                      |
| tomli_loads          | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                    |
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.04x faster                                                     |
| xml_etree_parse      | 97.6 ms                                                     | 94.3 ms: 1.04x faster                                                     |
| xml_etree_process    | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                     |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                     |
| pickle_list          | 2.70 us                                                     | 2.86 us: 1.06x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.84 us: 1.10x slower                                                     |
| pickle               | 6.64 us                                                     | 7.41 us: 1.12x slower                                                     |
| unpickle             | 7.57 us                                                     | 8.73 us: 1.15x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                              |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.1 ms: 1.07x slower                                                     |
| python_startup_no_site | 16.8 ms                                                     | 19.0 ms: 1.13x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.63 ms: 1.14x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-pythonperf1-amd64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.1 us: 4.65x faster                                                     |
| generators                 | 34.0 ms                                                     | 20.0 ms: 1.70x faster                                                     |
| asyncio_tcp                | 726 ms                                                      | 486 ms: 1.49x faster                                                      |
| json_dumps                 | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                     |
| comprehensions             | 15.6 us                                                     | 11.4 us: 1.37x faster                                                     |
| richards_super             | 38.7 ms                                                     | 28.6 ms: 1.35x faster                                                     |
| logging_silent             | 71.8 ns                                                     | 53.6 ns: 1.34x faster                                                     |
| deltablue                  | 2.70 ms                                                     | 2.08 ms: 1.30x faster                                                     |
| raytrace                   | 213 ms                                                      | 167 ms: 1.28x faster                                                      |
| nbody                      | 70.3 ms                                                     | 55.3 ms: 1.27x faster                                                     |
| richards                   | 31.4 ms                                                     | 25.2 ms: 1.25x faster                                                     |
| sqlglot_parse              | 953 us                                                      | 768 us: 1.24x faster                                                      |
| unpickle_pure_python       | 157 us                                                      | 130 us: 1.21x faster                                                      |
| async_tree_none            | 332 ms                                                      | 279 ms: 1.19x faster                                                      |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.71 sec: 1.19x faster                                                    |
| sqlglot_transpile          | 1.16 ms                                                     | 988 us: 1.18x faster                                                      |
| pickle_pure_python         | 208 us                                                      | 177 us: 1.18x faster                                                      |
| chaos                      | 48.4 ms                                                     | 41.3 ms: 1.17x faster                                                     |
| deepcopy_memo              | 26.0 us                                                     | 22.2 us: 1.17x faster                                                     |
| unpack_sequence            | 46.9 ns                                                     | 40.1 ns: 1.17x faster                                                     |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                                     |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 461 ms: 1.15x faster                                                      |
| logging_simple             | 6.86 us                                                     | 5.98 us: 1.15x faster                                                     |
| mako                       | 7.58 ms                                                     | 6.63 ms: 1.14x faster                                                     |
| async_tree_memoization_tg  | 405 ms                                                      | 354 ms: 1.14x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.14x faster                                                     |
| scimark_lu                 | 62.8 ms                                                     | 55.3 ms: 1.14x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 354 ms: 1.13x faster                                                      |
| deepcopy                   | 246 us                                                      | 220 us: 1.12x faster                                                      |
| crypto_pyaes               | 48.9 ms                                                     | 43.6 ms: 1.12x faster                                                     |
| nqueens                    | 68.3 ms                                                     | 61.0 ms: 1.12x faster                                                     |
| tomli_loads                | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                    |
| logging_format             | 7.16 us                                                     | 6.41 us: 1.12x faster                                                     |
| regex_compile              | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                     |
| dulwich_log                | 46.4 ms                                                     | 41.8 ms: 1.11x faster                                                     |
| chameleon                  | 5.26 ms                                                     | 4.81 ms: 1.10x faster                                                     |
| async_tree_none_tg         | 309 ms                                                      | 282 ms: 1.09x faster                                                      |
| spectral_norm              | 68.3 ms                                                     | 62.5 ms: 1.09x faster                                                     |
| sympy_sum                  | 100 ms                                                      | 91.5 ms: 1.09x faster                                                     |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 482 ms: 1.09x faster                                                      |
| sympy_str                  | 185 ms                                                      | 172 ms: 1.08x faster                                                      |
| async_tree_io              | 808 ms                                                      | 750 ms: 1.08x faster                                                      |
| pprint_safe_repr           | 529 ms                                                      | 493 ms: 1.07x faster                                                      |
| float                      | 54.4 ms                                                     | 50.6 ms: 1.07x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 773 ms: 1.07x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 1.93 us: 1.07x faster                                                     |
| fannkuch                   | 253 ms                                                      | 238 ms: 1.06x faster                                                      |
| tornado_http               | 92.8 ms                                                     | 87.4 ms: 1.06x faster                                                     |
| pprint_pformat             | 1.09 sec                                                    | 1.03 sec: 1.06x faster                                                    |
| sqlglot_normalize          | 190 ms                                                      | 180 ms: 1.06x faster                                                      |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.05x faster                                                     |
| mypy2                      | 459 ms                                                      | 436 ms: 1.05x faster                                                      |
| pickle_dict                | 18.5 us                                                     | 17.7 us: 1.04x faster                                                     |
| sympy_expand               | 299 ms                                                      | 288 ms: 1.04x faster                                                      |
| xml_etree_parse            | 97.6 ms                                                     | 94.3 ms: 1.04x faster                                                     |
| xml_etree_process          | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                     |
| dask                       | 273 ms                                                      | 264 ms: 1.03x faster                                                      |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                                    |
| go                         | 101 ms                                                      | 98.6 ms: 1.03x faster                                                     |
| scimark_sor                | 78.1 ms                                                     | 76.3 ms: 1.02x faster                                                     |
| pyflate                    | 312 ms                                                      | 310 ms: 1.01x faster                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 34.7 ms: 1.01x slower                                                     |
| xml_etree_generate         | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                     |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.02x slower                                                      |
| pidigits                   | 150 ms                                                      | 153 ms: 1.02x slower                                                      |
| gc_traversal               | 1.49 ms                                                     | 1.53 ms: 1.02x slower                                                     |
| 2to3                       | 214 ms                                                      | 219 ms: 1.03x slower                                                      |
| meteor_contest             | 75.2 ms                                                     | 78.3 ms: 1.04x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                     |
| scimark_fft                | 179 ms                                                      | 188 ms: 1.05x slower                                                      |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.05x slower                                                     |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.72 ms: 1.06x slower                                                     |
| pickle_list                | 2.70 us                                                     | 2.86 us: 1.06x slower                                                     |
| create_gc_cycles           | 713 us                                                      | 757 us: 1.06x slower                                                      |
| python_startup             | 19.8 ms                                                     | 21.1 ms: 1.07x slower                                                     |
| unpickle_list              | 2.59 us                                                     | 2.84 us: 1.10x slower                                                     |
| coverage                   | 43.4 ms                                                     | 47.8 ms: 1.10x slower                                                     |
| telco                      | 4.06 ms                                                     | 4.50 ms: 1.11x slower                                                     |
| pickle                     | 6.64 us                                                     | 7.41 us: 1.12x slower                                                     |
| bench_mp_pool              | 63.2 ms                                                     | 70.8 ms: 1.12x slower                                                     |
| python_startup_no_site     | 16.8 ms                                                     | 19.0 ms: 1.13x slower                                                     |
| pathlib                    | 70.9 ms                                                     | 80.2 ms: 1.13x slower                                                     |
| unpickle                   | 7.57 us                                                     | 8.73 us: 1.15x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 16.4 ms: 1.16x slower                                                     |
| hexiom                     | 4.55 ms                                                     | 5.29 ms: 1.16x slower                                                     |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.2 ms: 1.24x slower                                                     |
| async_generators           | 177 ms                                                      | 245 ms: 1.38x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                              |

Benchmark hidden because not significant (5): pycparser, xml_etree_iterparse, mdp, bench_thread_pool, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown