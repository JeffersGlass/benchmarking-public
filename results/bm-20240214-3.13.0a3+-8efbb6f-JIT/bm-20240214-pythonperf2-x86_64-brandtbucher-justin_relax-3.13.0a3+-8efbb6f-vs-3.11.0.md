
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: 8efbb6f
- commit date: 2024-02-14
- overall geometric mean: 1.05x faster \*
- HPT reliability: 99.41%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 300 ms: 1.05x slower                                                       |
| chameleon      | 7.92 ms                                                      | 7.20 ms: 1.10x faster                                                      |
| docutils       | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                     |
| Geometric mean | (ref)                                                        | 1.01x faster                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.09x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 434 ms: 1.09x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                     |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                     |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 709 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 712 ms: 1.05x faster                                                       |
| Geometric mean             | (ref)                                                        | 1.10x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 261 ms: 1.04x slower                                                       |
| float          | 74.9 ms                                                      | 78.3 ms: 1.05x slower                                                      |
| nbody          | 92.9 ms                                                      | 102 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                        | 1.06x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                      |
| regex_dna      | 227 ms                                                       | 241 ms: 1.06x slower                                                       |
| regex_effbot   | 3.34 ms                                                      | 3.69 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                        | 1.04x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                      |
| json_loads           | 28.9 us                                                      | 25.2 us: 1.15x faster                                                      |
| unpickle_pure_python | 238 us                                                       | 218 us: 1.10x faster                                                       |
| xml_etree_parse      | 155 ms                                                       | 146 ms: 1.06x faster                                                       |
| pickle_pure_python   | 316 us                                                       | 306 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.02x faster                                                       |
| tomli_loads          | 2.25 sec                                                     | 2.22 sec: 1.01x faster                                                     |
| unpickle_list        | 4.60 us                                                      | 4.67 us: 1.02x slower                                                      |
| pickle_dict          | 32.3 us                                                      | 33.0 us: 1.02x slower                                                      |
| xml_etree_process    | 55.9 ms                                                      | 58.1 ms: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.4 us: 1.05x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 85.0 ms: 1.07x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.41 us: 1.12x slower                                                      |
| unpickle             | 13.3 us                                                      | 14.9 us: 1.12x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.01x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                      |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240214-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a3+-8efbb6f |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 116 us: 4.58x faster                                                       |
| asyncio_tcp                | 747 ms                                                       | 370 ms: 2.02x faster                                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.57 sec: 1.95x faster                                                     |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                                      |
| comprehensions             | 25.1 us                                                      | 19.1 us: 1.31x faster                                                      |
| json_dumps                 | 13.3 ms                                                      | 10.5 ms: 1.27x faster                                                      |
| coroutines                 | 27.8 ms                                                      | 22.3 ms: 1.24x faster                                                      |
| chaos                      | 74.9 ms                                                      | 62.8 ms: 1.19x faster                                                      |
| async_tree_none            | 518 ms                                                       | 434 ms: 1.19x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 157 ms: 1.18x faster                                                       |
| scimark_lu                 | 114 ms                                                       | 97.6 ms: 1.17x faster                                                      |
| json_loads                 | 28.9 us                                                      | 25.2 us: 1.15x faster                                                      |
| async_tree_memoization     | 629 ms                                                       | 548 ms: 1.15x faster                                                       |
| sympy_str                  | 337 ms                                                       | 298 ms: 1.13x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.44 us: 1.13x faster                                                      |
| raytrace                   | 309 ms                                                       | 278 ms: 1.11x faster                                                       |
| chameleon                  | 7.92 ms                                                      | 7.20 ms: 1.10x faster                                                      |
| sympy_expand               | 553 ms                                                       | 503 ms: 1.10x faster                                                       |
| nqueens                    | 103 ms                                                       | 93.6 ms: 1.10x faster                                                      |
| unpickle_pure_python       | 238 us                                                       | 218 us: 1.10x faster                                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 548 ms: 1.09x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 434 ms: 1.09x faster                                                       |
| deltablue                  | 3.97 ms                                                      | 3.63 ms: 1.09x faster                                                      |
| mdp                        | 2.77 sec                                                     | 2.54 sec: 1.09x faster                                                     |
| async_tree_io              | 1.17 sec                                                     | 1.08 sec: 1.09x faster                                                     |
| sqlglot_parse              | 1.51 ms                                                      | 1.39 ms: 1.09x faster                                                      |
| crypto_pyaes               | 83.3 ms                                                      | 77.0 ms: 1.08x faster                                                      |
| mako                       | 11.0 ms                                                      | 10.2 ms: 1.08x faster                                                      |
| logging_format             | 7.71 us                                                      | 7.14 us: 1.08x faster                                                      |
| async_tree_io_tg           | 1.15 sec                                                     | 1.07 sec: 1.08x faster                                                     |
| sympy_integrate            | 25.8 ms                                                      | 24.0 ms: 1.07x faster                                                      |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| richards_super             | 63.6 ms                                                      | 59.6 ms: 1.07x faster                                                      |
| deepcopy                   | 391 us                                                       | 367 us: 1.06x faster                                                       |
| logging_silent             | 100 ns                                                       | 94.3 ns: 1.06x faster                                                      |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 709 ms: 1.06x faster                                                       |
| xml_etree_parse            | 155 ms                                                       | 146 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 712 ms: 1.05x faster                                                       |
| gc_traversal               | 4.15 ms                                                      | 3.94 ms: 1.05x faster                                                      |
| sqlglot_transpile          | 1.91 ms                                                      | 1.82 ms: 1.05x faster                                                      |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                                       |
| json                       | 5.58 ms                                                      | 5.36 ms: 1.04x faster                                                      |
| fannkuch                   | 416 ms                                                       | 401 ms: 1.04x faster                                                       |
| pickle_pure_python         | 316 us                                                       | 306 us: 1.03x faster                                                       |
| deepcopy_memo              | 37.5 us                                                      | 36.4 us: 1.03x faster                                                      |
| deepcopy_reduce            | 3.40 us                                                      | 3.30 us: 1.03x faster                                                      |
| bench_thread_pool          | 1.00 ms                                                      | 972 us: 1.03x faster                                                       |
| pprint_pformat             | 1.67 sec                                                     | 1.63 sec: 1.02x faster                                                     |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.02x faster                                                       |
| dask                       | 410 ms                                                       | 404 ms: 1.01x faster                                                       |
| tomli_loads                | 2.25 sec                                                     | 2.22 sec: 1.01x faster                                                     |
| meteor_contest             | 131 ms                                                       | 129 ms: 1.01x faster                                                       |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                       |
| hexiom                     | 6.98 ms                                                      | 6.93 ms: 1.01x faster                                                      |
| pprint_safe_repr           | 805 ms                                                       | 801 ms: 1.00x faster                                                       |
| spectral_norm              | 95.1 ms                                                      | 95.3 ms: 1.00x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.1 ms: 1.01x slower                                                      |
| sqlglot_optimize           | 59.0 ms                                                      | 59.7 ms: 1.01x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.88 sec: 1.01x slower                                                     |
| unpickle_list              | 4.60 us                                                      | 4.67 us: 1.02x slower                                                      |
| scimark_monte_carlo        | 69.8 ms                                                      | 71.1 ms: 1.02x slower                                                      |
| pickle_dict                | 32.3 us                                                      | 33.0 us: 1.02x slower                                                      |
| dulwich_log                | 67.4 ms                                                      | 69.1 ms: 1.02x slower                                                      |
| xml_etree_process          | 55.9 ms                                                      | 58.1 ms: 1.04x slower                                                      |
| pidigits                   | 251 ms                                                       | 261 ms: 1.04x slower                                                       |
| float                      | 74.9 ms                                                      | 78.3 ms: 1.05x slower                                                      |
| 2to3                       | 287 ms                                                       | 300 ms: 1.05x slower                                                       |
| pickle                     | 9.89 us                                                      | 10.4 us: 1.05x slower                                                      |
| bench_mp_pool              | 4.70 ms                                                      | 4.92 ms: 1.05x slower                                                      |
| regex_v8                   | 24.4 ms                                                      | 25.7 ms: 1.05x slower                                                      |
| go                         | 158 ms                                                       | 167 ms: 1.06x slower                                                       |
| regex_dna                  | 227 ms                                                       | 241 ms: 1.06x slower                                                       |
| xml_etree_generate         | 79.7 ms                                                      | 85.0 ms: 1.07x slower                                                      |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.34 ms: 1.07x slower                                                      |
| richards                   | 49.7 ms                                                      | 53.6 ms: 1.08x slower                                                      |
| sqlite_synth               | 2.52 us                                                      | 2.76 us: 1.09x slower                                                      |
| nbody                      | 92.9 ms                                                      | 102 ms: 1.10x slower                                                       |
| regex_effbot               | 3.34 ms                                                      | 3.69 ms: 1.10x slower                                                      |
| unpack_sequence            | 45.7 ns                                                      | 50.7 ns: 1.11x slower                                                      |
| pickle_list                | 3.94 us                                                      | 4.41 us: 1.12x slower                                                      |
| unpickle                   | 13.3 us                                                      | 14.9 us: 1.12x slower                                                      |
| pyflate                    | 449 ms                                                       | 508 ms: 1.13x slower                                                       |
| async_generators           | 322 ms                                                       | 365 ms: 1.14x slower                                                       |
| mypy2                      | 762 ms                                                       | 883 ms: 1.16x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.03 ms: 1.18x slower                                                      |
| python_startup             | 10.7 ms                                                      | 12.7 ms: 1.18x slower                                                      |
| scimark_fft                | 281 ms                                                       | 335 ms: 1.19x slower                                                       |
| coverage                   | 66.1 ms                                                      | 84.2 ms: 1.27x slower                                                      |
| scimark_sor                | 110 ms                                                       | 143 ms: 1.31x slower                                                       |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.44x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.05x faster                                                               |

Benchmark hidden because not significant (3): tornado_http, create_gc_cycles, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.41% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.03x