# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster \*
- HPT reliability: 83.39%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 307 ms: 1.07x slower                                                       |
| chameleon      | 7.92 ms                                                      | 7.48 ms: 1.06x faster                                                      |
| docutils       | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                     |
| Geometric mean | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                     |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| float          | 74.9 ms                                                      | 78.4 ms: 1.05x slower                                                      |
| nbody          | 92.9 ms                                                      | 101 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                        | 1.06x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 148 ms: 1.05x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                      |
| regex_dna      | 227 ms                                                       | 237 ms: 1.04x slower                                                       |
| regex_effbot   | 3.34 ms                                                      | 3.63 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                      |
| json_loads           | 28.9 us                                                      | 25.5 us: 1.14x faster                                                      |
| pickle_dict          | 32.3 us                                                      | 30.5 us: 1.06x faster                                                      |
| xml_etree_parse      | 155 ms                                                       | 146 ms: 1.06x faster                                                       |
| tomli_loads          | 2.25 sec                                                     | 2.14 sec: 1.05x faster                                                     |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.04x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 233 us: 1.02x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 317 us: 1.00x slower                                                       |
| unpickle_list        | 4.60 us                                                      | 4.72 us: 1.03x slower                                                      |
| xml_etree_process    | 55.9 ms                                                      | 58.0 ms: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.28 us: 1.09x slower                                                      |
| unpickle             | 13.3 us                                                      | 15.5 us: 1.17x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.5 ms: 1.45x slower                                                      |
| python_startup_no_site | 7.73 ms                                                      | 14.1 ms: 1.82x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.62x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.00 ms: 1.10x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 123 us: 4.31x faster                                                       |
| asyncio_tcp                | 747 ms                                                       | 376 ms: 1.99x faster                                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                                     |
| generators                 | 54.6 ms                                                      | 33.4 ms: 1.63x faster                                                      |
| comprehensions             | 25.1 us                                                      | 18.7 us: 1.34x faster                                                      |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.26x faster                                                      |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                                      |
| gc_traversal               | 4.15 ms                                                      | 3.47 ms: 1.20x faster                                                      |
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 159 ms: 1.17x faster                                                       |
| json_loads                 | 28.9 us                                                      | 25.5 us: 1.14x faster                                                      |
| async_tree_memoization     | 629 ms                                                       | 560 ms: 1.12x faster                                                       |
| chaos                      | 74.9 ms                                                      | 67.2 ms: 1.11x faster                                                      |
| sympy_str                  | 337 ms                                                       | 302 ms: 1.11x faster                                                       |
| mako                       | 11.0 ms                                                      | 10.00 ms: 1.10x faster                                                     |
| logging_simple             | 7.24 us                                                      | 6.60 us: 1.10x faster                                                      |
| richards_super             | 63.6 ms                                                      | 58.3 ms: 1.09x faster                                                      |
| crypto_pyaes               | 83.3 ms                                                      | 77.0 ms: 1.08x faster                                                      |
| sympy_expand               | 553 ms                                                       | 517 ms: 1.07x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 446 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 711 ms: 1.06x faster                                                       |
| pickle_dict                | 32.3 us                                                      | 30.5 us: 1.06x faster                                                      |
| chameleon                  | 7.92 ms                                                      | 7.48 ms: 1.06x faster                                                      |
| logging_format             | 7.71 us                                                      | 7.28 us: 1.06x faster                                                      |
| async_tree_memoization_tg  | 600 ms                                                       | 567 ms: 1.06x faster                                                       |
| json                       | 5.58 ms                                                      | 5.28 ms: 1.06x faster                                                      |
| xml_etree_parse            | 155 ms                                                       | 146 ms: 1.06x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.62 sec: 1.06x faster                                                     |
| sqlglot_parse              | 1.51 ms                                                      | 1.43 ms: 1.06x faster                                                      |
| fannkuch                   | 416 ms                                                       | 394 ms: 1.06x faster                                                       |
| regex_compile              | 156 ms                                                       | 148 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                       |
| sympy_integrate            | 25.8 ms                                                      | 24.5 ms: 1.05x faster                                                      |
| async_tree_io_tg           | 1.15 sec                                                     | 1.10 sec: 1.05x faster                                                     |
| tomli_loads                | 2.25 sec                                                     | 2.14 sec: 1.05x faster                                                     |
| xml_etree_iterparse        | 107 ms                                                       | 103 ms: 1.04x faster                                                       |
| nqueens                    | 103 ms                                                       | 99.1 ms: 1.04x faster                                                      |
| deltablue                  | 3.97 ms                                                      | 3.83 ms: 1.04x faster                                                      |
| sqlglot_normalize          | 122 ms                                                       | 118 ms: 1.03x faster                                                       |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                      |
| raytrace                   | 309 ms                                                       | 300 ms: 1.03x faster                                                       |
| spectral_norm              | 95.1 ms                                                      | 92.9 ms: 1.02x faster                                                      |
| unpickle_pure_python       | 238 us                                                       | 233 us: 1.02x faster                                                       |
| logging_silent             | 100 ns                                                       | 99.0 ns: 1.01x faster                                                      |
| deepcopy_reduce            | 3.40 us                                                      | 3.35 us: 1.01x faster                                                      |
| meteor_contest             | 131 ms                                                       | 131 ms: 1.00x slower                                                       |
| pickle_pure_python         | 316 us                                                       | 317 us: 1.00x slower                                                       |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                                      |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                                     |
| dulwich_log                | 67.4 ms                                                      | 69.1 ms: 1.03x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.92 sec: 1.03x slower                                                     |
| unpickle_list              | 4.60 us                                                      | 4.72 us: 1.03x slower                                                      |
| richards                   | 49.7 ms                                                      | 51.2 ms: 1.03x slower                                                      |
| regex_v8                   | 24.4 ms                                                      | 25.3 ms: 1.04x slower                                                      |
| xml_etree_process          | 55.9 ms                                                      | 58.0 ms: 1.04x slower                                                      |
| regex_dna                  | 227 ms                                                       | 237 ms: 1.04x slower                                                       |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.25 ms: 1.05x slower                                                      |
| float                      | 74.9 ms                                                      | 78.4 ms: 1.05x slower                                                      |
| pprint_safe_repr           | 805 ms                                                       | 843 ms: 1.05x slower                                                       |
| hexiom                     | 6.98 ms                                                      | 7.34 ms: 1.05x slower                                                      |
| deepcopy_memo              | 37.5 us                                                      | 39.6 us: 1.05x slower                                                      |
| pprint_pformat             | 1.67 sec                                                     | 1.76 sec: 1.05x slower                                                     |
| xml_etree_generate         | 79.7 ms                                                      | 84.4 ms: 1.06x slower                                                      |
| sqlglot_optimize           | 59.0 ms                                                      | 62.8 ms: 1.07x slower                                                      |
| sqlite_synth               | 2.52 us                                                      | 2.70 us: 1.07x slower                                                      |
| 2to3                       | 287 ms                                                       | 307 ms: 1.07x slower                                                       |
| nbody                      | 92.9 ms                                                      | 101 ms: 1.08x slower                                                       |
| scimark_lu                 | 114 ms                                                       | 124 ms: 1.08x slower                                                       |
| pickle_list                | 3.94 us                                                      | 4.28 us: 1.09x slower                                                      |
| regex_effbot               | 3.34 ms                                                      | 3.63 ms: 1.09x slower                                                      |
| scimark_monte_carlo        | 69.8 ms                                                      | 77.7 ms: 1.11x slower                                                      |
| go                         | 158 ms                                                       | 176 ms: 1.11x slower                                                       |
| scimark_fft                | 281 ms                                                       | 322 ms: 1.15x slower                                                       |
| unpickle                   | 13.3 us                                                      | 15.5 us: 1.17x slower                                                      |
| pyflate                    | 449 ms                                                       | 529 ms: 1.18x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.06 ms: 1.18x slower                                                      |
| coverage                   | 66.1 ms                                                      | 78.8 ms: 1.19x slower                                                      |
| async_generators           | 322 ms                                                       | 385 ms: 1.20x slower                                                       |
| mypy2                      | 762 ms                                                       | 915 ms: 1.20x slower                                                       |
| unpack_sequence            | 45.7 ns                                                      | 61.5 ns: 1.35x slower                                                      |
| scimark_sor                | 110 ms                                                       | 155 ms: 1.41x slower                                                       |
| python_startup             | 10.7 ms                                                      | 15.5 ms: 1.45x slower                                                      |
| bench_mp_pool              | 4.70 ms                                                      | 6.86 ms: 1.46x slower                                                      |
| python_startup_no_site     | 7.73 ms                                                      | 14.1 ms: 1.82x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                               |

Benchmark hidden because not significant (5): bench_thread_pool, create_gc_cycles, deepcopy, tornado_http, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 83.39% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.25x