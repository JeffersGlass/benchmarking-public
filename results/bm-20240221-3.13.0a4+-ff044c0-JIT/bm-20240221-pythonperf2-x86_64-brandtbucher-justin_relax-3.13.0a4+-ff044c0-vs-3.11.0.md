
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.00x faster \*
- HPT reliability: 69.91%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 310 ms: 1.08x slower                                                       |
| chameleon      | 7.92 ms                                                      | 7.65 ms: 1.04x faster                                                      |
| docutils       | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                     |
| Geometric mean | (ref)                                                        | 1.02x slower                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 440 ms: 1.08x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                     |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 707 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                     |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                       |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| float          | 74.9 ms                                                      | 80.2 ms: 1.07x slower                                                      |
| nbody          | 92.9 ms                                                      | 102 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                        | 1.07x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 152 ms: 1.03x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 25.5 ms: 1.04x slower                                                      |
| regex_dna      | 227 ms                                                       | 237 ms: 1.04x slower                                                       |
| regex_effbot   | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                        | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.6 ms: 1.26x faster                                                      |
| json_loads           | 28.9 us                                                      | 24.7 us: 1.17x faster                                                      |
| xml_etree_parse      | 155 ms                                                       | 151 ms: 1.02x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 105 ms: 1.01x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 32.2 us: 1.00x faster                                                      |
| pickle_pure_python   | 316 us                                                       | 315 us: 1.00x faster                                                       |
| unpickle_pure_python | 238 us                                                       | 240 us: 1.01x slower                                                       |
| unpickle_list        | 4.60 us                                                      | 4.68 us: 1.02x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| tomli_loads          | 2.25 sec                                                     | 2.37 sec: 1.05x slower                                                     |
| xml_etree_process    | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 86.3 ms: 1.08x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.27 us: 1.09x slower                                                      |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.00x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.6 ms: 1.45x slower                                                      |
| python_startup_no_site | 7.73 ms                                                      | 14.1 ms: 1.82x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.62x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 10.7 ms: 1.03x faster                                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf2-x86_64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 118 us: 4.51x faster                                                       |
| asyncio_tcp                | 747 ms                                                       | 372 ms: 2.01x faster                                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                                     |
| generators                 | 54.6 ms                                                      | 34.8 ms: 1.57x faster                                                      |
| comprehensions             | 25.1 us                                                      | 19.1 us: 1.31x faster                                                      |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.26x faster                                                      |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                      |
| json_loads                 | 28.9 us                                                      | 24.7 us: 1.17x faster                                                      |
| async_tree_none            | 518 ms                                                       | 443 ms: 1.17x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 161 ms: 1.15x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 555 ms: 1.13x faster                                                       |
| sympy_str                  | 337 ms                                                       | 303 ms: 1.11x faster                                                       |
| chaos                      | 74.9 ms                                                      | 69.3 ms: 1.08x faster                                                      |
| async_tree_none_tg         | 474 ms                                                       | 440 ms: 1.08x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.75 us: 1.07x faster                                                      |
| sympy_expand               | 553 ms                                                       | 516 ms: 1.07x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                     |
| async_tree_memoization_tg  | 600 ms                                                       | 562 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 707 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                     |
| deltablue                  | 3.97 ms                                                      | 3.75 ms: 1.06x faster                                                      |
| mdp                        | 2.77 sec                                                     | 2.62 sec: 1.06x faster                                                     |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 711 ms: 1.05x faster                                                       |
| json                       | 5.58 ms                                                      | 5.30 ms: 1.05x faster                                                      |
| richards_super             | 63.6 ms                                                      | 60.5 ms: 1.05x faster                                                      |
| gc_traversal               | 4.15 ms                                                      | 3.95 ms: 1.05x faster                                                      |
| sqlglot_parse              | 1.51 ms                                                      | 1.44 ms: 1.05x faster                                                      |
| crypto_pyaes               | 83.3 ms                                                      | 79.7 ms: 1.04x faster                                                      |
| sympy_integrate            | 25.8 ms                                                      | 24.9 ms: 1.04x faster                                                      |
| chameleon                  | 7.92 ms                                                      | 7.65 ms: 1.04x faster                                                      |
| logging_format             | 7.71 us                                                      | 7.48 us: 1.03x faster                                                      |
| mako                       | 11.0 ms                                                      | 10.7 ms: 1.03x faster                                                      |
| regex_compile              | 156 ms                                                       | 152 ms: 1.03x faster                                                       |
| xml_etree_parse            | 155 ms                                                       | 151 ms: 1.02x faster                                                       |
| sqlglot_transpile          | 1.91 ms                                                      | 1.87 ms: 1.02x faster                                                      |
| xml_etree_iterparse        | 107 ms                                                       | 105 ms: 1.01x faster                                                       |
| deepcopy                   | 391 us                                                       | 386 us: 1.01x faster                                                       |
| sqlglot_normalize          | 122 ms                                                       | 121 ms: 1.01x faster                                                       |
| pickle_dict                | 32.3 us                                                      | 32.2 us: 1.00x faster                                                      |
| pickle_pure_python         | 316 us                                                       | 315 us: 1.00x faster                                                       |
| unpickle_pure_python       | 238 us                                                       | 240 us: 1.01x slower                                                       |
| spectral_norm              | 95.1 ms                                                      | 96.2 ms: 1.01x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.2 ms: 1.01x slower                                                      |
| nqueens                    | 103 ms                                                       | 104 ms: 1.02x slower                                                       |
| meteor_contest             | 131 ms                                                       | 133 ms: 1.02x slower                                                       |
| pycparser                  | 1.31 sec                                                     | 1.33 sec: 1.02x slower                                                     |
| unpickle_list              | 4.60 us                                                      | 4.68 us: 1.02x slower                                                      |
| deepcopy_memo              | 37.5 us                                                      | 38.4 us: 1.02x slower                                                      |
| dulwich_log                | 67.4 ms                                                      | 69.2 ms: 1.03x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                     |
| fannkuch                   | 416 ms                                                       | 431 ms: 1.04x slower                                                       |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                       |
| regex_v8                   | 24.4 ms                                                      | 25.5 ms: 1.04x slower                                                      |
| regex_dna                  | 227 ms                                                       | 237 ms: 1.04x slower                                                       |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| regex_effbot               | 3.34 ms                                                      | 3.50 ms: 1.05x slower                                                      |
| tomli_loads                | 2.25 sec                                                     | 2.37 sec: 1.05x slower                                                     |
| xml_etree_process          | 55.9 ms                                                      | 59.4 ms: 1.06x slower                                                      |
| float                      | 74.9 ms                                                      | 80.2 ms: 1.07x slower                                                      |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.36 ms: 1.07x slower                                                      |
| xml_etree_generate         | 79.7 ms                                                      | 86.3 ms: 1.08x slower                                                      |
| 2to3                       | 287 ms                                                       | 310 ms: 1.08x slower                                                       |
| pickle_list                | 3.94 us                                                      | 4.27 us: 1.09x slower                                                      |
| sqlglot_optimize           | 59.0 ms                                                      | 64.0 ms: 1.09x slower                                                      |
| sqlite_synth               | 2.52 us                                                      | 2.76 us: 1.09x slower                                                      |
| pprint_pformat             | 1.67 sec                                                     | 1.83 sec: 1.10x slower                                                     |
| richards                   | 49.7 ms                                                      | 54.4 ms: 1.10x slower                                                      |
| nbody                      | 92.9 ms                                                      | 102 ms: 1.10x slower                                                       |
| pprint_safe_repr           | 805 ms                                                       | 888 ms: 1.10x slower                                                       |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                                      |
| hexiom                     | 6.98 ms                                                      | 7.90 ms: 1.13x slower                                                      |
| scimark_lu                 | 114 ms                                                       | 131 ms: 1.14x slower                                                       |
| go                         | 158 ms                                                       | 182 ms: 1.16x slower                                                       |
| scimark_monte_carlo        | 69.8 ms                                                      | 83.6 ms: 1.20x slower                                                      |
| mypy2                      | 762 ms                                                       | 918 ms: 1.21x slower                                                       |
| telco                      | 6.81 ms                                                      | 8.23 ms: 1.21x slower                                                      |
| scimark_fft                | 281 ms                                                       | 339 ms: 1.21x slower                                                       |
| async_generators           | 322 ms                                                       | 390 ms: 1.21x slower                                                       |
| pyflate                    | 449 ms                                                       | 547 ms: 1.22x slower                                                       |
| coverage                   | 66.1 ms                                                      | 83.7 ms: 1.27x slower                                                      |
| scimark_sor                | 110 ms                                                       | 155 ms: 1.41x slower                                                       |
| python_startup             | 10.7 ms                                                      | 15.6 ms: 1.45x slower                                                      |
| bench_mp_pool              | 4.70 ms                                                      | 6.83 ms: 1.45x slower                                                      |
| unpack_sequence            | 45.7 ns                                                      | 79.7 ns: 1.75x slower                                                      |
| python_startup_no_site     | 7.73 ms                                                      | 14.1 ms: 1.82x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.00x faster                                                               |

Benchmark hidden because not significant (7): bench_thread_pool, tornado_http, raytrace, logging_silent, deepcopy_reduce, asyncio_websockets, create_gc_cycles
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 69.91% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.25x