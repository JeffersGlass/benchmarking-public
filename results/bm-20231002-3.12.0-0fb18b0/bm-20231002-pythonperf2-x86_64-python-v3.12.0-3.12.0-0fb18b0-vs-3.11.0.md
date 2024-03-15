
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0
- machine: linux-x86_64
- commit hash: 0fb18b0
- commit date: 2023-10-02
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.13x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 285 ms: 1.01x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.23 ms: 1.10x faster                                        |
| docutils       | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                       |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                         |
| async_tree_none            | 518 ms                                                       | 452 ms: 1.15x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                       |
| async_tree_memoization_tg  | 600 ms                                                       | 540 ms: 1.11x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.05 sec: 1.10x faster                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 696 ms: 1.08x faster                                         |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 697 ms: 1.08x faster                                         |
| Geometric mean             | (ref)                                                        | 1.11x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| nbody          | 92.9 ms                                                      | 88.0 ms: 1.06x faster                                        |
| float          | 74.9 ms                                                      | 76.6 ms: 1.02x slower                                        |
| pidigits       | 251 ms                                                       | 265 ms: 1.05x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 144 ms: 1.08x faster                                         |
| regex_v8       | 24.4 ms                                                      | 23.6 ms: 1.03x faster                                        |
| regex_dna      | 227 ms                                                       | 239 ms: 1.05x slower                                         |
| regex_effbot   | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                        |
| Geometric mean | (ref)                                                        | 1.00x slower                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                        |
| json_loads           | 28.9 us                                                      | 24.4 us: 1.19x faster                                        |
| unpickle_pure_python | 238 us                                                       | 210 us: 1.14x faster                                         |
| xml_etree_parse      | 155 ms                                                       | 144 ms: 1.08x faster                                         |
| tomli_loads          | 2.25 sec                                                     | 2.16 sec: 1.04x faster                                       |
| xml_etree_iterparse  | 107 ms                                                       | 103 ms: 1.04x faster                                         |
| pickle_dict          | 32.3 us                                                      | 32.5 us: 1.01x slower                                        |
| pickle_pure_python   | 316 us                                                       | 318 us: 1.01x slower                                         |
| unpickle_list        | 4.60 us                                                      | 4.66 us: 1.01x slower                                        |
| xml_etree_process    | 55.9 ms                                                      | 58.4 ms: 1.05x slower                                        |
| pickle               | 9.89 us                                                      | 10.5 us: 1.06x slower                                        |
| xml_etree_generate   | 79.7 ms                                                      | 86.1 ms: 1.08x slower                                        |
| unpickle             | 13.3 us                                                      | 14.8 us: 1.12x slower                                        |
| pickle_list          | 3.94 us                                                      | 4.43 us: 1.12x slower                                        |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 11.6 ms: 1.08x slower                                        |
| python_startup_no_site | 7.73 ms                                                      | 8.64 ms: 1.12x slower                                        |
| Geometric mean         | (ref)                                                        | 1.10x slower                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                        |
| django_template | 39.3 ms                                                      | 38.2 ms: 1.03x faster                                        |
| Geometric mean  | (ref)                                                        | 1.06x faster                                                 |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 152 us: 3.51x faster                                         |
| asyncio_tcp                | 747 ms                                                       | 378 ms: 1.98x faster                                         |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                       |
| generators                 | 54.6 ms                                                      | 37.4 ms: 1.46x faster                                        |
| json_dumps                 | 13.3 ms                                                      | 10.2 ms: 1.30x faster                                        |
| richards_super             | 63.6 ms                                                      | 51.3 ms: 1.24x faster                                        |
| deltablue                  | 3.97 ms                                                      | 3.24 ms: 1.23x faster                                        |
| coroutines                 | 27.8 ms                                                      | 23.0 ms: 1.21x faster                                        |
| gc_traversal               | 4.15 ms                                                      | 3.48 ms: 1.19x faster                                        |
| fannkuch                   | 416 ms                                                       | 350 ms: 1.19x faster                                         |
| json_loads                 | 28.9 us                                                      | 24.4 us: 1.19x faster                                        |
| chaos                      | 74.9 ms                                                      | 64.0 ms: 1.17x faster                                        |
| hexiom                     | 6.98 ms                                                      | 5.96 ms: 1.17x faster                                        |
| async_tree_memoization     | 629 ms                                                       | 544 ms: 1.16x faster                                         |
| scimark_lu                 | 114 ms                                                       | 98.8 ms: 1.15x faster                                        |
| async_tree_none            | 518 ms                                                       | 452 ms: 1.15x faster                                         |
| sympy_sum                  | 186 ms                                                       | 162 ms: 1.15x faster                                         |
| comprehensions             | 25.1 us                                                      | 21.9 us: 1.14x faster                                        |
| sympy_expand               | 553 ms                                                       | 484 ms: 1.14x faster                                         |
| nqueens                    | 103 ms                                                       | 89.9 ms: 1.14x faster                                        |
| unpickle_pure_python       | 238 us                                                       | 210 us: 1.14x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.04 sec: 1.12x faster                                       |
| sympy_str                  | 337 ms                                                       | 302 ms: 1.11x faster                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 540 ms: 1.11x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 431 ms: 1.10x faster                                         |
| mako                       | 11.0 ms                                                      | 10.0 ms: 1.10x faster                                        |
| sqlglot_parse              | 1.51 ms                                                      | 1.38 ms: 1.10x faster                                        |
| chameleon                  | 7.92 ms                                                      | 7.23 ms: 1.10x faster                                        |
| async_tree_io_tg           | 1.15 sec                                                     | 1.05 sec: 1.10x faster                                       |
| json                       | 5.58 ms                                                      | 5.12 ms: 1.09x faster                                        |
| richards                   | 49.7 ms                                                      | 45.7 ms: 1.09x faster                                        |
| regex_compile              | 156 ms                                                       | 144 ms: 1.08x faster                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 696 ms: 1.08x faster                                         |
| logging_simple             | 7.24 us                                                      | 6.71 us: 1.08x faster                                        |
| mdp                        | 2.77 sec                                                     | 2.57 sec: 1.08x faster                                       |
| sympy_integrate            | 25.8 ms                                                      | 23.9 ms: 1.08x faster                                        |
| sqlglot_transpile          | 1.91 ms                                                      | 1.78 ms: 1.08x faster                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 697 ms: 1.08x faster                                         |
| xml_etree_parse            | 155 ms                                                       | 144 ms: 1.08x faster                                         |
| logging_silent             | 100 ns                                                       | 94.4 ns: 1.06x faster                                        |
| deepcopy                   | 391 us                                                       | 368 us: 1.06x faster                                         |
| pycparser                  | 1.31 sec                                                     | 1.23 sec: 1.06x faster                                       |
| nbody                      | 92.9 ms                                                      | 88.0 ms: 1.06x faster                                        |
| sqlalchemy_imperative      | 19.8 ms                                                      | 18.7 ms: 1.05x faster                                        |
| go                         | 158 ms                                                       | 150 ms: 1.05x faster                                         |
| bench_thread_pool          | 1.00 ms                                                      | 950 us: 1.05x faster                                         |
| sqlglot_normalize          | 122 ms                                                       | 116 ms: 1.05x faster                                         |
| dask                       | 410 ms                                                       | 392 ms: 1.05x faster                                         |
| tomli_loads                | 2.25 sec                                                     | 2.16 sec: 1.04x faster                                       |
| xml_etree_iterparse        | 107 ms                                                       | 103 ms: 1.04x faster                                         |
| raytrace                   | 309 ms                                                       | 298 ms: 1.04x faster                                         |
| spectral_norm              | 95.1 ms                                                      | 91.6 ms: 1.04x faster                                        |
| crypto_pyaes               | 83.3 ms                                                      | 80.3 ms: 1.04x faster                                        |
| regex_v8                   | 24.4 ms                                                      | 23.6 ms: 1.03x faster                                        |
| dulwich_log                | 67.4 ms                                                      | 65.4 ms: 1.03x faster                                        |
| logging_format             | 7.71 us                                                      | 7.48 us: 1.03x faster                                        |
| django_template            | 39.3 ms                                                      | 38.2 ms: 1.03x faster                                        |
| tornado_http               | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| sqlglot_optimize           | 59.0 ms                                                      | 57.5 ms: 1.03x faster                                        |
| pyflate                    | 449 ms                                                       | 439 ms: 1.02x faster                                         |
| deepcopy_memo              | 37.5 us                                                      | 36.8 us: 1.02x faster                                        |
| meteor_contest             | 131 ms                                                       | 128 ms: 1.02x faster                                         |
| scimark_monte_carlo        | 69.8 ms                                                      | 69.0 ms: 1.01x faster                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.37 us: 1.01x faster                                        |
| pprint_pformat             | 1.67 sec                                                     | 1.65 sec: 1.01x faster                                       |
| scimark_sor                | 110 ms                                                       | 109 ms: 1.01x faster                                         |
| 2to3                       | 287 ms                                                       | 285 ms: 1.01x faster                                         |
| pickle_dict                | 32.3 us                                                      | 32.5 us: 1.01x slower                                        |
| pickle_pure_python         | 316 us                                                       | 318 us: 1.01x slower                                         |
| docutils                   | 2.85 sec                                                     | 2.87 sec: 1.01x slower                                       |
| coverage                   | 66.1 ms                                                      | 66.7 ms: 1.01x slower                                        |
| unpickle_list              | 4.60 us                                                      | 4.66 us: 1.01x slower                                        |
| float                      | 74.9 ms                                                      | 76.6 ms: 1.02x slower                                        |
| telco                      | 6.81 ms                                                      | 6.96 ms: 1.02x slower                                        |
| sqlalchemy_declarative     | 154 ms                                                       | 159 ms: 1.03x slower                                         |
| aiohttp                    | 986 us                                                       | 1.02 ms: 1.03x slower                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.21 ms: 1.04x slower                                        |
| gunicorn                   | 966 us                                                       | 1.00 ms: 1.04x slower                                        |
| xml_etree_process          | 55.9 ms                                                      | 58.4 ms: 1.05x slower                                        |
| regex_dna                  | 227 ms                                                       | 239 ms: 1.05x slower                                         |
| pidigits                   | 251 ms                                                       | 265 ms: 1.05x slower                                         |
| pickle                     | 9.89 us                                                      | 10.5 us: 1.06x slower                                        |
| regex_effbot               | 3.34 ms                                                      | 3.57 ms: 1.07x slower                                        |
| scimark_fft                | 281 ms                                                       | 301 ms: 1.07x slower                                         |
| xml_etree_generate         | 79.7 ms                                                      | 86.1 ms: 1.08x slower                                        |
| python_startup             | 10.7 ms                                                      | 11.6 ms: 1.08x slower                                        |
| mypy2                      | 762 ms                                                       | 830 ms: 1.09x slower                                         |
| sqlite_synth               | 2.52 us                                                      | 2.77 us: 1.10x slower                                        |
| unpickle                   | 13.3 us                                                      | 14.8 us: 1.12x slower                                        |
| python_startup_no_site     | 7.73 ms                                                      | 8.64 ms: 1.12x slower                                        |
| pickle_list                | 3.94 us                                                      | 4.43 us: 1.12x slower                                        |
| unpack_sequence            | 45.7 ns                                                      | 53.2 ns: 1.16x slower                                        |
| async_generators           | 322 ms                                                       | 390 ms: 1.21x slower                                         |
| Geometric mean             | (ref)                                                        | 1.07x faster                                                 |

Benchmark hidden because not significant (5): asyncio_websockets, pathlib, pprint_safe_repr, create_gc_cycles, bench_mp_pool
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.13x