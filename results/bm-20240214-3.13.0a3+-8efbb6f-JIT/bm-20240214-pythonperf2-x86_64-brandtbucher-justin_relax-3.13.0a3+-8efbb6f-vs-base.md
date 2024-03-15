# Results vs. base

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: 8efbb6f
- commit date: 2024-02-14
- overall geometric mean: 1.01x faster
- HPT reliability: 99.30%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 298 ms                                                                       | 300 ms: 1.00x slower                                                       |
| chameleon      | 7.54 ms                                                                      | 7.20 ms: 1.05x faster                                                      |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none_tg         | 435 ms                                                                       | 434 ms: 1.00x faster                                                       |
| async_tree_io_tg           | 1.07 sec                                                                     | 1.07 sec: 1.00x faster                                                     |
| async_tree_io              | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                     |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 709 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 701 ms                                                                       | 712 ms: 1.02x slower                                                       |
| Geometric mean             | (ref)                                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (3): async_tree_memoization, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 107 ms                                                                       | 102 ms: 1.05x faster                                                       |
| float          | 81.7 ms                                                                      | 78.3 ms: 1.04x faster                                                      |
| pidigits       | 263 ms                                                                       | 261 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.03x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_v8       | 26.3 ms                                                                      | 25.7 ms: 1.02x faster                                                      |
| regex_compile  | 146 ms                                                                       | 146 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (2): regex_effbot, regex_dna

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpickle_pure_python | 228 us                                                                       | 218 us: 1.05x faster                                                       |
| tomli_loads          | 2.31 sec                                                                     | 2.22 sec: 1.04x faster                                                     |
| xml_etree_iterparse  | 107 ms                                                                       | 105 ms: 1.02x faster                                                       |
| xml_etree_parse      | 148 ms                                                                       | 146 ms: 1.01x faster                                                       |
| pickle               | 10.5 us                                                                      | 10.4 us: 1.01x faster                                                      |
| pickle_list          | 4.44 us                                                                      | 4.41 us: 1.01x faster                                                      |
| unpickle             | 14.8 us                                                                      | 14.9 us: 1.01x slower                                                      |
| xml_etree_generate   | 84.5 ms                                                                      | 85.0 ms: 1.01x slower                                                      |
| pickle_dict          | 32.7 us                                                                      | 33.0 us: 1.01x slower                                                      |
| pickle_pure_python   | 301 us                                                                       | 306 us: 1.01x slower                                                       |
| Geometric mean       | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (4): json_loads, xml_etree_process, json_dumps, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                      |
| python_startup         | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                      |
| Geometric mean         | (ref)                                                                        | 1.00x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|-----------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.8 ms                                                                      | 10.2 ms: 1.16x faster                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20240212-pythonperf2-x86_64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:----------------------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| spectral_norm              | 118 ms                                                                       | 95.3 ms: 1.24x faster                                                      |
| mako                       | 11.8 ms                                                                      | 10.2 ms: 1.16x faster                                                      |
| scimark_sparse_mat_mult    | 5.01 ms                                                                      | 4.34 ms: 1.16x faster                                                      |
| chaos                      | 70.3 ms                                                                      | 62.8 ms: 1.12x faster                                                      |
| hexiom                     | 7.70 ms                                                                      | 6.93 ms: 1.11x faster                                                      |
| scimark_monte_carlo        | 78.5 ms                                                                      | 71.1 ms: 1.10x faster                                                      |
| comprehensions             | 20.7 us                                                                      | 19.1 us: 1.09x faster                                                      |
| scimark_fft                | 360 ms                                                                       | 335 ms: 1.08x faster                                                       |
| crypto_pyaes               | 81.5 ms                                                                      | 77.0 ms: 1.06x faster                                                      |
| pprint_safe_repr           | 847 ms                                                                       | 801 ms: 1.06x faster                                                       |
| pprint_pformat             | 1.72 sec                                                                     | 1.63 sec: 1.05x faster                                                     |
| unpickle_pure_python       | 228 us                                                                       | 218 us: 1.05x faster                                                       |
| chameleon                  | 7.54 ms                                                                      | 7.20 ms: 1.05x faster                                                      |
| nbody                      | 107 ms                                                                       | 102 ms: 1.05x faster                                                       |
| float                      | 81.7 ms                                                                      | 78.3 ms: 1.04x faster                                                      |
| tomli_loads                | 2.31 sec                                                                     | 2.22 sec: 1.04x faster                                                     |
| nqueens                    | 97.4 ms                                                                      | 93.6 ms: 1.04x faster                                                      |
| typing_runtime_protocols   | 119 us                                                                       | 116 us: 1.03x faster                                                       |
| logging_format             | 7.33 us                                                                      | 7.14 us: 1.03x faster                                                      |
| logging_simple             | 6.60 us                                                                      | 6.44 us: 1.03x faster                                                      |
| pyflate                    | 521 ms                                                                       | 508 ms: 1.03x faster                                                       |
| sqlglot_optimize           | 61.1 ms                                                                      | 59.7 ms: 1.02x faster                                                      |
| sqlglot_normalize          | 119 ms                                                                       | 116 ms: 1.02x faster                                                       |
| regex_v8                   | 26.3 ms                                                                      | 25.7 ms: 1.02x faster                                                      |
| xml_etree_iterparse        | 107 ms                                                                       | 105 ms: 1.02x faster                                                       |
| deepcopy_memo              | 37.0 us                                                                      | 36.4 us: 1.02x faster                                                      |
| telco                      | 8.15 ms                                                                      | 8.03 ms: 1.02x faster                                                      |
| xml_etree_parse            | 148 ms                                                                       | 146 ms: 1.01x faster                                                       |
| deltablue                  | 3.68 ms                                                                      | 3.63 ms: 1.01x faster                                                      |
| sympy_sum                  | 159 ms                                                                       | 157 ms: 1.01x faster                                                       |
| go                         | 169 ms                                                                       | 167 ms: 1.01x faster                                                       |
| deepcopy_reduce            | 3.34 us                                                                      | 3.30 us: 1.01x faster                                                      |
| async_generators           | 370 ms                                                                       | 365 ms: 1.01x faster                                                       |
| fannkuch                   | 406 ms                                                                       | 401 ms: 1.01x faster                                                       |
| pickle                     | 10.5 us                                                                      | 10.4 us: 1.01x faster                                                      |
| sympy_integrate            | 24.3 ms                                                                      | 24.0 ms: 1.01x faster                                                      |
| logging_silent             | 95.1 ns                                                                      | 94.3 ns: 1.01x faster                                                      |
| pickle_list                | 4.44 us                                                                      | 4.41 us: 1.01x faster                                                      |
| mdp                        | 2.56 sec                                                                     | 2.54 sec: 1.01x faster                                                     |
| meteor_contest             | 130 ms                                                                       | 129 ms: 1.01x faster                                                       |
| pidigits                   | 263 ms                                                                       | 261 ms: 1.01x faster                                                       |
| coroutines                 | 22.4 ms                                                                      | 22.3 ms: 1.00x faster                                                      |
| regex_compile              | 146 ms                                                                       | 146 ms: 1.00x faster                                                       |
| sympy_str                  | 299 ms                                                                       | 298 ms: 1.00x faster                                                       |
| dulwich_log                | 69.3 ms                                                                      | 69.1 ms: 1.00x faster                                                      |
| async_tree_none_tg         | 435 ms                                                                       | 434 ms: 1.00x faster                                                       |
| async_tree_io_tg           | 1.07 sec                                                                     | 1.07 sec: 1.00x faster                                                     |
| asyncio_tcp_ssl            | 1.57 sec                                                                     | 1.57 sec: 1.00x faster                                                     |
| asyncio_tcp                | 369 ms                                                                       | 370 ms: 1.00x slower                                                       |
| 2to3                       | 298 ms                                                                       | 300 ms: 1.00x slower                                                       |
| python_startup_no_site     | 11.1 ms                                                                      | 11.1 ms: 1.00x slower                                                      |
| python_startup             | 12.6 ms                                                                      | 12.7 ms: 1.00x slower                                                      |
| json                       | 5.33 ms                                                                      | 5.36 ms: 1.01x slower                                                      |
| pathlib                    | 19.0 ms                                                                      | 19.1 ms: 1.01x slower                                                      |
| unpickle                   | 14.8 us                                                                      | 14.9 us: 1.01x slower                                                      |
| xml_etree_generate         | 84.5 ms                                                                      | 85.0 ms: 1.01x slower                                                      |
| async_tree_io              | 1.07 sec                                                                     | 1.08 sec: 1.01x slower                                                     |
| sqlite_synth               | 2.74 us                                                                      | 2.76 us: 1.01x slower                                                      |
| pickle_dict                | 32.7 us                                                                      | 33.0 us: 1.01x slower                                                      |
| scimark_sor                | 142 ms                                                                       | 143 ms: 1.01x slower                                                       |
| generators                 | 33.6 ms                                                                      | 34.0 ms: 1.01x slower                                                      |
| sqlglot_transpile          | 1.80 ms                                                                      | 1.82 ms: 1.01x slower                                                      |
| raytrace                   | 275 ms                                                                       | 278 ms: 1.01x slower                                                       |
| pickle_pure_python         | 301 us                                                                       | 306 us: 1.01x slower                                                       |
| async_tree_cpu_io_mixed    | 699 ms                                                                       | 709 ms: 1.02x slower                                                       |
| async_tree_cpu_io_mixed_tg | 701 ms                                                                       | 712 ms: 1.02x slower                                                       |
| sqlglot_parse              | 1.37 ms                                                                      | 1.39 ms: 1.02x slower                                                      |
| create_gc_cycles           | 1.53 ms                                                                      | 1.57 ms: 1.02x slower                                                      |
| coverage                   | 81.8 ms                                                                      | 84.2 ms: 1.03x slower                                                      |
| bench_mp_pool              | 4.77 ms                                                                      | 4.92 ms: 1.03x slower                                                      |
| richards_super             | 56.9 ms                                                                      | 59.6 ms: 1.05x slower                                                      |
| richards                   | 51.0 ms                                                                      | 53.6 ms: 1.05x slower                                                      |
| gc_traversal               | 3.64 ms                                                                      | 3.94 ms: 1.08x slower                                                      |
| unpack_sequence            | 45.1 ns                                                                      | 50.7 ns: 1.12x slower                                                      |
| Geometric mean             | (ref)                                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (19): tornado_http, mypy2, asyncio_websockets, deepcopy, json_loads, xml_etree_process, regex_effbot, json_dumps, pycparser, scimark_lu, async_tree_memoization, docutils, unpickle_list, dask, regex_dna, sympy_expand, async_tree_memoization_tg, bench_thread_pool, async_tree_none


# HPT report

- Reliability score: 99.30% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.01x