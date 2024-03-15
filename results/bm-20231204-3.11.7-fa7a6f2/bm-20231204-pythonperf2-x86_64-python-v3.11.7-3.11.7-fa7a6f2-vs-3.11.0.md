
# Results vs. 3.11.0

- fork: python
- ref: v3.11.7
- machine: linux-x86_64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.01x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 280 ms: 1.02x faster                                         |
| chameleon      | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                        |
| docutils       | 2.85 sec                                                     | 2.81 sec: 1.01x faster                                       |
| html5lib       | 72.2 ms                                                      | 71.2 ms: 1.01x faster                                        |
| tornado_http   | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_memoization_tg  | 600 ms                                                       | 581 ms: 1.03x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.13 sec: 1.02x faster                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 735 ms: 1.02x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 466 ms: 1.02x faster                                         |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 743 ms: 1.01x faster                                         |
| async_tree_memoization     | 629 ms                                                       | 621 ms: 1.01x faster                                         |
| async_tree_io              | 1.17 sec                                                     | 1.16 sec: 1.01x faster                                       |
| async_tree_none            | 518 ms                                                       | 514 ms: 1.01x faster                                         |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| nbody          | 92.9 ms                                                      | 105 ms: 1.13x slower                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 23.0 ms: 1.06x faster                                        |
| regex_effbot   | 3.34 ms                                                      | 3.20 ms: 1.04x faster                                        |
| regex_compile  | 156 ms                                                       | 151 ms: 1.03x faster                                         |
| regex_dna      | 227 ms                                                       | 223 ms: 1.02x faster                                         |
| Geometric mean | (ref)                                                        | 1.04x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|--------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads         | 28.9 us                                                      | 24.9 us: 1.16x faster                                        |
| pickle_list        | 3.94 us                                                      | 3.80 us: 1.04x faster                                        |
| pickle_dict        | 32.3 us                                                      | 31.5 us: 1.03x faster                                        |
| unpickle           | 13.3 us                                                      | 13.0 us: 1.02x faster                                        |
| xml_etree_process  | 55.9 ms                                                      | 55.4 ms: 1.01x faster                                        |
| pickle_pure_python | 316 us                                                       | 314 us: 1.01x faster                                         |
| pickle             | 9.89 us                                                      | 9.84 us: 1.01x faster                                        |
| json_dumps         | 13.3 ms                                                      | 13.2 ms: 1.01x faster                                        |
| xml_etree_generate | 79.7 ms                                                      | 79.9 ms: 1.00x slower                                        |
| unpickle_list      | 4.60 us                                                      | 4.65 us: 1.01x slower                                        |
| tomli_loads        | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| xml_etree_parse    | 155 ms                                                       | 158 ms: 1.02x slower                                         |
| Geometric mean     | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (2): xml_etree_iterparse, unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                        |
| python_startup_no_site | 7.73 ms                                                      | 7.69 ms: 1.01x faster                                        |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| genshi_xml      | 57.1 ms                                                      | 58.4 ms: 1.02x slower                                        |
| genshi_text     | 25.5 ms                                                      | 26.2 ms: 1.03x slower                                        |
| django_template | 39.3 ms                                                      | 40.8 ms: 1.04x slower                                        |
| Geometric mean  | (ref)                                                        | 1.02x slower                                                 |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf2-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| json_loads                 | 28.9 us                                                      | 24.9 us: 1.16x faster                                        |
| gc_traversal               | 4.15 ms                                                      | 3.67 ms: 1.13x faster                                        |
| regex_v8                   | 24.4 ms                                                      | 23.0 ms: 1.06x faster                                        |
| json                       | 5.58 ms                                                      | 5.29 ms: 1.06x faster                                        |
| scimark_monte_carlo        | 69.8 ms                                                      | 66.3 ms: 1.05x faster                                        |
| chameleon                  | 7.92 ms                                                      | 7.53 ms: 1.05x faster                                        |
| pprint_safe_repr           | 805 ms                                                       | 767 ms: 1.05x faster                                         |
| pprint_pformat             | 1.67 sec                                                     | 1.59 sec: 1.05x faster                                       |
| nqueens                    | 103 ms                                                       | 97.8 ms: 1.05x faster                                        |
| comprehensions             | 25.1 us                                                      | 24.0 us: 1.05x faster                                        |
| regex_effbot               | 3.34 ms                                                      | 3.20 ms: 1.04x faster                                        |
| pylint                     | 514 ms                                                       | 493 ms: 1.04x faster                                         |
| richards_super             | 63.6 ms                                                      | 61.2 ms: 1.04x faster                                        |
| thrift                     | 931 us                                                       | 897 us: 1.04x faster                                         |
| sympy_integrate            | 25.8 ms                                                      | 24.9 ms: 1.04x faster                                        |
| pickle_list                | 3.94 us                                                      | 3.80 us: 1.04x faster                                        |
| sympy_sum                  | 186 ms                                                       | 180 ms: 1.03x faster                                         |
| aiohttp                    | 986 us                                                       | 954 us: 1.03x faster                                         |
| async_tree_memoization_tg  | 600 ms                                                       | 581 ms: 1.03x faster                                         |
| regex_compile              | 156 ms                                                       | 151 ms: 1.03x faster                                         |
| async_generators           | 322 ms                                                       | 312 ms: 1.03x faster                                         |
| tornado_http               | 124 ms                                                       | 121 ms: 1.03x faster                                         |
| pickle_dict                | 32.3 us                                                      | 31.5 us: 1.03x faster                                        |
| logging_simple             | 7.24 us                                                      | 7.06 us: 1.03x faster                                        |
| bench_thread_pool          | 1.00 ms                                                      | 975 us: 1.03x faster                                         |
| dask                       | 410 ms                                                       | 400 ms: 1.03x faster                                         |
| richards                   | 49.7 ms                                                      | 48.5 ms: 1.02x faster                                        |
| sympy_str                  | 337 ms                                                       | 329 ms: 1.02x faster                                         |
| 2to3                       | 287 ms                                                       | 280 ms: 1.02x faster                                         |
| async_tree_io_tg           | 1.15 sec                                                     | 1.13 sec: 1.02x faster                                       |
| telco                      | 6.81 ms                                                      | 6.67 ms: 1.02x faster                                        |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 735 ms: 1.02x faster                                         |
| sqlite_synth               | 2.52 us                                                      | 2.47 us: 1.02x faster                                        |
| pathlib                    | 18.9 ms                                                      | 18.6 ms: 1.02x faster                                        |
| regex_dna                  | 227 ms                                                       | 223 ms: 1.02x faster                                         |
| async_tree_none_tg         | 474 ms                                                       | 466 ms: 1.02x faster                                         |
| unpickle                   | 13.3 us                                                      | 13.0 us: 1.02x faster                                        |
| dulwich_log                | 67.4 ms                                                      | 66.3 ms: 1.02x faster                                        |
| pyflate                    | 449 ms                                                       | 442 ms: 1.02x faster                                         |
| sqlalchemy_imperative      | 19.8 ms                                                      | 19.5 ms: 1.02x faster                                        |
| gunicorn                   | 966 us                                                       | 951 us: 1.02x faster                                         |
| html5lib                   | 72.2 ms                                                      | 71.2 ms: 1.01x faster                                        |
| mypy2                      | 762 ms                                                       | 751 ms: 1.01x faster                                         |
| sympy_expand               | 553 ms                                                       | 545 ms: 1.01x faster                                         |
| flaskblogging              | 3.88 ms                                                      | 3.83 ms: 1.01x faster                                        |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 743 ms: 1.01x faster                                         |
| async_tree_memoization     | 629 ms                                                       | 621 ms: 1.01x faster                                         |
| docutils                   | 2.85 sec                                                     | 2.81 sec: 1.01x faster                                       |
| typing_runtime_protocols   | 532 us                                                       | 526 us: 1.01x faster                                         |
| sqlglot_transpile          | 1.91 ms                                                      | 1.89 ms: 1.01x faster                                        |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.03 ms: 1.01x faster                                        |
| xml_etree_process          | 55.9 ms                                                      | 55.4 ms: 1.01x faster                                        |
| async_tree_io              | 1.17 sec                                                     | 1.16 sec: 1.01x faster                                       |
| sqlalchemy_declarative     | 154 ms                                                       | 153 ms: 1.01x faster                                         |
| async_tree_none            | 518 ms                                                       | 514 ms: 1.01x faster                                         |
| asyncio_tcp                | 747 ms                                                       | 742 ms: 1.01x faster                                         |
| python_startup             | 10.7 ms                                                      | 10.7 ms: 1.01x faster                                        |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                         |
| crypto_pyaes               | 83.3 ms                                                      | 82.7 ms: 1.01x faster                                        |
| python_startup_no_site     | 7.73 ms                                                      | 7.69 ms: 1.01x faster                                        |
| generators                 | 54.6 ms                                                      | 54.4 ms: 1.01x faster                                        |
| pickle                     | 9.89 us                                                      | 9.84 us: 1.01x faster                                        |
| json_dumps                 | 13.3 ms                                                      | 13.2 ms: 1.01x faster                                        |
| xml_etree_generate         | 79.7 ms                                                      | 79.9 ms: 1.00x slower                                        |
| mdp                        | 2.77 sec                                                     | 2.78 sec: 1.00x slower                                       |
| sqlglot_optimize           | 59.0 ms                                                      | 59.2 ms: 1.00x slower                                        |
| deltablue                  | 3.97 ms                                                      | 3.99 ms: 1.01x slower                                        |
| go                         | 158 ms                                                       | 159 ms: 1.01x slower                                         |
| meteor_contest             | 131 ms                                                       | 132 ms: 1.01x slower                                         |
| sqlglot_parse              | 1.51 ms                                                      | 1.53 ms: 1.01x slower                                        |
| spectral_norm              | 95.1 ms                                                      | 95.9 ms: 1.01x slower                                        |
| logging_format             | 7.71 us                                                      | 7.78 us: 1.01x slower                                        |
| logging_silent             | 100 ns                                                       | 101 ns: 1.01x slower                                         |
| unpickle_list              | 4.60 us                                                      | 4.65 us: 1.01x slower                                        |
| raytrace                   | 309 ms                                                       | 313 ms: 1.01x slower                                         |
| hexiom                     | 6.98 ms                                                      | 7.07 ms: 1.01x slower                                        |
| scimark_sor                | 110 ms                                                       | 111 ms: 1.01x slower                                         |
| tomli_loads                | 2.25 sec                                                     | 2.28 sec: 1.01x slower                                       |
| sqlglot_normalize          | 122 ms                                                       | 124 ms: 1.02x slower                                         |
| deepcopy                   | 391 us                                                       | 399 us: 1.02x slower                                         |
| xml_etree_parse            | 155 ms                                                       | 158 ms: 1.02x slower                                         |
| genshi_xml                 | 57.1 ms                                                      | 58.4 ms: 1.02x slower                                        |
| deepcopy_reduce            | 3.40 us                                                      | 3.48 us: 1.03x slower                                        |
| deepcopy_memo              | 37.5 us                                                      | 38.5 us: 1.03x slower                                        |
| genshi_text                | 25.5 ms                                                      | 26.2 ms: 1.03x slower                                        |
| django_template            | 39.3 ms                                                      | 40.8 ms: 1.04x slower                                        |
| fannkuch                   | 416 ms                                                       | 435 ms: 1.05x slower                                         |
| pidigits                   | 251 ms                                                       | 268 ms: 1.07x slower                                         |
| chaos                      | 74.9 ms                                                      | 82.4 ms: 1.10x slower                                        |
| nbody                      | 92.9 ms                                                      | 105 ms: 1.13x slower                                         |
| Geometric mean             | (ref)                                                        | 1.01x faster                                                 |

Benchmark hidden because not significant (14): unpack_sequence, coverage, float, pycparser, mako, bench_mp_pool, scimark_fft, xml_etree_iterparse, asyncio_tcp_ssl, asyncio_websockets, coroutines, unpickle_pure_python, scimark_lu, create_gc_cycles


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x