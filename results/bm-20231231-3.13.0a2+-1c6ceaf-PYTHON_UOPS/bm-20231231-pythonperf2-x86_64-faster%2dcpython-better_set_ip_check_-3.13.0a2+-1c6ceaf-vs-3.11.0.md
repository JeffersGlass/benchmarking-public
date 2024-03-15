
# Results vs. 3.11.0

- fork: faster-cpython
- ref: better_set_ip_check_
- machine: linux-x86_64
- commit hash: 1c6ceaf
- commit date: 2023-12-31
- overall geometric mean: 1.02x slower
- HPT reliability: 94.64%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 309 ms: 1.08x slower                                                                   |
| chameleon      | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                                  |
| docutils       | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                                 |
| tornado_http   | 124 ms                                                       | 122 ms: 1.02x faster                                                                   |
| Geometric mean | (ref)                                                        | 1.03x slower                                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 448 ms: 1.16x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                                   |
| async_tree_memoization_tg  | 600 ms                                                       | 556 ms: 1.08x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                                 |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                                                   |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.05x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                                   |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                                   |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 263 ms: 1.05x slower                                                                   |
| float          | 74.9 ms                                                      | 103 ms: 1.37x slower                                                                   |
| nbody          | 92.9 ms                                                      | 129 ms: 1.39x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.26x slower                                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| regex_v8       | 24.4 ms                                                      | 25.5 ms: 1.04x slower                                                                  |
| regex_dna      | 227 ms                                                       | 245 ms: 1.08x slower                                                                   |
| regex_effbot   | 3.34 ms                                                      | 3.62 ms: 1.08x slower                                                                  |
| regex_compile  | 156 ms                                                       | 170 ms: 1.09x slower                                                                   |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                                  |
| json_loads           | 28.9 us                                                      | 25.0 us: 1.16x faster                                                                  |
| pickle_dict          | 32.3 us                                                      | 30.7 us: 1.05x faster                                                                  |
| xml_etree_parse      | 155 ms                                                       | 147 ms: 1.05x faster                                                                   |
| pickle_pure_python   | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| pickle               | 9.89 us                                                      | 10.0 us: 1.01x slower                                                                  |
| unpickle_pure_python | 238 us                                                       | 242 us: 1.02x slower                                                                   |
| unpickle_list        | 4.60 us                                                      | 4.69 us: 1.02x slower                                                                  |
| xml_etree_iterparse  | 107 ms                                                       | 112 ms: 1.05x slower                                                                   |
| pickle_list          | 3.94 us                                                      | 4.23 us: 1.07x slower                                                                  |
| xml_etree_process    | 55.9 ms                                                      | 61.5 ms: 1.10x slower                                                                  |
| xml_etree_generate   | 79.7 ms                                                      | 90.5 ms: 1.14x slower                                                                  |
| unpickle             | 13.3 us                                                      | 15.2 us: 1.14x slower                                                                  |
| tomli_loads          | 2.25 sec                                                     | 2.75 sec: 1.22x slower                                                                 |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                                  |
| python_startup_no_site | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                                  |
| Geometric mean         | (ref)                                                        | 1.30x slower                                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| mako      | 11.0 ms                                                      | 14.1 ms: 1.29x slower                                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231231-pythonperf2-x86_64-faster%2dcpython-better_set_ip_check_-3.13.0a2+-1c6ceaf |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 124 us: 4.27x faster                                                                   |
| asyncio_tcp                | 747 ms                                                       | 373 ms: 2.00x faster                                                                   |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.59 sec: 1.93x faster                                                                 |
| generators                 | 54.6 ms                                                      | 33.9 ms: 1.61x faster                                                                  |
| coroutines                 | 27.8 ms                                                      | 22.0 ms: 1.26x faster                                                                  |
| json_dumps                 | 13.3 ms                                                      | 10.9 ms: 1.22x faster                                                                  |
| gc_traversal               | 4.15 ms                                                      | 3.51 ms: 1.18x faster                                                                  |
| json_loads                 | 28.9 us                                                      | 25.0 us: 1.16x faster                                                                  |
| async_tree_none            | 518 ms                                                       | 448 ms: 1.16x faster                                                                   |
| async_tree_memoization     | 629 ms                                                       | 562 ms: 1.12x faster                                                                   |
| sympy_sum                  | 186 ms                                                       | 167 ms: 1.11x faster                                                                   |
| scimark_lu                 | 114 ms                                                       | 105 ms: 1.09x faster                                                                   |
| async_tree_memoization_tg  | 600 ms                                                       | 556 ms: 1.08x faster                                                                   |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                                 |
| json                       | 5.58 ms                                                      | 5.24 ms: 1.07x faster                                                                  |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                                                   |
| logging_simple             | 7.24 us                                                      | 6.84 us: 1.06x faster                                                                  |
| mdp                        | 2.77 sec                                                     | 2.62 sec: 1.06x faster                                                                 |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.05x faster                                                                 |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 714 ms: 1.05x faster                                                                   |
| pickle_dict                | 32.3 us                                                      | 30.7 us: 1.05x faster                                                                  |
| xml_etree_parse            | 155 ms                                                       | 147 ms: 1.05x faster                                                                   |
| sqlglot_parse              | 1.51 ms                                                      | 1.44 ms: 1.05x faster                                                                  |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                                   |
| sympy_str                  | 337 ms                                                       | 323 ms: 1.04x faster                                                                   |
| richards_super             | 63.6 ms                                                      | 61.3 ms: 1.04x faster                                                                  |
| logging_format             | 7.71 us                                                      | 7.45 us: 1.04x faster                                                                  |
| sympy_integrate            | 25.8 ms                                                      | 25.0 ms: 1.03x faster                                                                  |
| raytrace                   | 309 ms                                                       | 300 ms: 1.03x faster                                                                   |
| bench_thread_pool          | 1.00 ms                                                      | 972 us: 1.03x faster                                                                   |
| sympy_expand               | 553 ms                                                       | 538 ms: 1.03x faster                                                                   |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                                  |
| comprehensions             | 25.1 us                                                      | 24.5 us: 1.02x faster                                                                  |
| tornado_http               | 124 ms                                                       | 122 ms: 1.02x faster                                                                   |
| asyncio_websockets         | 390 ms                                                       | 386 ms: 1.01x faster                                                                   |
| deepcopy                   | 391 us                                                       | 388 us: 1.01x faster                                                                   |
| pickle_pure_python         | 316 us                                                       | 314 us: 1.01x faster                                                                   |
| sqlglot_normalize          | 122 ms                                                       | 122 ms: 1.00x slower                                                                   |
| pickle                     | 9.89 us                                                      | 10.0 us: 1.01x slower                                                                  |
| unpickle_pure_python       | 238 us                                                       | 242 us: 1.02x slower                                                                   |
| deepcopy_reduce            | 3.40 us                                                      | 3.45 us: 1.02x slower                                                                  |
| create_gc_cycles           | 1.58 ms                                                      | 1.61 ms: 1.02x slower                                                                  |
| unpickle_list              | 4.60 us                                                      | 4.69 us: 1.02x slower                                                                  |
| chameleon                  | 7.92 ms                                                      | 8.09 ms: 1.02x slower                                                                  |
| unpack_sequence            | 45.7 ns                                                      | 46.7 ns: 1.02x slower                                                                  |
| crypto_pyaes               | 83.3 ms                                                      | 85.4 ms: 1.03x slower                                                                  |
| pycparser                  | 1.31 sec                                                     | 1.34 sec: 1.03x slower                                                                 |
| docutils                   | 2.85 sec                                                     | 2.94 sec: 1.03x slower                                                                 |
| chaos                      | 74.9 ms                                                      | 77.4 ms: 1.03x slower                                                                  |
| pathlib                    | 18.9 ms                                                      | 19.7 ms: 1.04x slower                                                                  |
| regex_v8                   | 24.4 ms                                                      | 25.5 ms: 1.04x slower                                                                  |
| nqueens                    | 103 ms                                                       | 107 ms: 1.04x slower                                                                   |
| pidigits                   | 251 ms                                                       | 263 ms: 1.05x slower                                                                   |
| xml_etree_iterparse        | 107 ms                                                       | 112 ms: 1.05x slower                                                                   |
| meteor_contest             | 131 ms                                                       | 138 ms: 1.06x slower                                                                   |
| dulwich_log                | 67.4 ms                                                      | 71.7 ms: 1.06x slower                                                                  |
| pickle_list                | 3.94 us                                                      | 4.23 us: 1.07x slower                                                                  |
| deepcopy_memo              | 37.5 us                                                      | 40.3 us: 1.07x slower                                                                  |
| sqlglot_optimize           | 59.0 ms                                                      | 63.4 ms: 1.08x slower                                                                  |
| regex_dna                  | 227 ms                                                       | 245 ms: 1.08x slower                                                                   |
| 2to3                       | 287 ms                                                       | 309 ms: 1.08x slower                                                                   |
| regex_effbot               | 3.34 ms                                                      | 3.62 ms: 1.08x slower                                                                  |
| regex_compile              | 156 ms                                                       | 170 ms: 1.09x slower                                                                   |
| xml_etree_process          | 55.9 ms                                                      | 61.5 ms: 1.10x slower                                                                  |
| richards                   | 49.7 ms                                                      | 54.7 ms: 1.10x slower                                                                  |
| sqlite_synth               | 2.52 us                                                      | 2.79 us: 1.11x slower                                                                  |
| async_generators           | 322 ms                                                       | 361 ms: 1.12x slower                                                                   |
| xml_etree_generate         | 79.7 ms                                                      | 90.5 ms: 1.14x slower                                                                  |
| pprint_pformat             | 1.67 sec                                                     | 1.90 sec: 1.14x slower                                                                 |
| pprint_safe_repr           | 805 ms                                                       | 920 ms: 1.14x slower                                                                   |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.14x slower                                                                  |
| fannkuch                   | 416 ms                                                       | 478 ms: 1.15x slower                                                                   |
| go                         | 158 ms                                                       | 182 ms: 1.16x slower                                                                   |
| python_startup             | 10.7 ms                                                      | 12.6 ms: 1.18x slower                                                                  |
| mypy2                      | 762 ms                                                       | 897 ms: 1.18x slower                                                                   |
| tomli_loads                | 2.25 sec                                                     | 2.75 sec: 1.22x slower                                                                 |
| scimark_monte_carlo        | 69.8 ms                                                      | 86.1 ms: 1.23x slower                                                                  |
| telco                      | 6.81 ms                                                      | 8.45 ms: 1.24x slower                                                                  |
| coverage                   | 66.1 ms                                                      | 83.2 ms: 1.26x slower                                                                  |
| pyflate                    | 449 ms                                                       | 567 ms: 1.26x slower                                                                   |
| mako                       | 11.0 ms                                                      | 14.1 ms: 1.29x slower                                                                  |
| scimark_sor                | 110 ms                                                       | 144 ms: 1.32x slower                                                                   |
| deltablue                  | 3.97 ms                                                      | 5.42 ms: 1.37x slower                                                                  |
| float                      | 74.9 ms                                                      | 103 ms: 1.37x slower                                                                   |
| hexiom                     | 6.98 ms                                                      | 9.70 ms: 1.39x slower                                                                  |
| nbody                      | 92.9 ms                                                      | 129 ms: 1.39x slower                                                                   |
| python_startup_no_site     | 7.73 ms                                                      | 11.1 ms: 1.43x slower                                                                  |
| scimark_fft                | 281 ms                                                       | 423 ms: 1.51x slower                                                                   |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 6.30 ms: 1.55x slower                                                                  |
| spectral_norm              | 95.1 ms                                                      | 162 ms: 1.70x slower                                                                   |
| Geometric mean             | (ref)                                                        | 1.02x slower                                                                           |

Benchmark hidden because not significant (3): logging_silent, bench_mp_pool, dask
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.64% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x