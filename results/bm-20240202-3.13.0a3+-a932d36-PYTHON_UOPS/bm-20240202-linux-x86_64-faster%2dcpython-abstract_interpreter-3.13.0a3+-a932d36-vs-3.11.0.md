
# Results vs. 3.11.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: a932d36
- commit date: 2024-02-02
- overall geometric mean: 1.00x faster
- HPT reliability: 93.71%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 93.1 ms: 1.18x slower                                                            |
| nbody          | 96.0 ms                                                | 117 ms: 1.22x slower                                                             |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                            |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                            |
| regex_dna      | 205 ms                                                 | 226 ms: 1.11x slower                                                             |
| Geometric mean | (ref)                                                  | 1.08x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                             |
| unpickle_list        | 5.21 us                                                | 4.96 us: 1.05x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 235 us: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.6 us: 1.02x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| pickle_dict          | 34.6 us                                                | 36.6 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 60.7 ms: 1.07x slower                                                            |
| pickle               | 11.0 us                                                | 11.8 us: 1.08x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.59 sec: 1.13x slower                                                           |
| pickle_list          | 4.59 us                                                | 5.37 us: 1.17x slower                                                            |
| unpickle             | 13.8 us                                                | 17.0 us: 1.23x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.0 ms: 1.31x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.66x faster                                                             |
| generators                 | 74.9 ms                                                | 29.8 ms: 2.51x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 492 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.2 ms: 1.21x faster                                                            |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.49 ms: 1.15x faster                                                            |
| richards_super             | 61.9 ms                                                | 54.2 ms: 1.14x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.3 us: 1.11x faster                                                            |
| unpack_sequence            | 43.5 ns                                                | 39.4 ns: 1.10x faster                                                            |
| deltablue                  | 3.92 ms                                                | 3.57 ms: 1.10x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                                             |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.34 ms: 1.07x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                             |
| logging_simple             | 6.22 us                                                | 5.88 us: 1.06x faster                                                            |
| unpickle_list              | 5.21 us                                                | 4.96 us: 1.05x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 599 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 734 ms: 1.04x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                           |
| unpickle_pure_python       | 242 us                                                 | 235 us: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| raytrace                   | 309 ms                                                 | 301 ms: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                            |
| richards                   | 49.8 ms                                                | 48.6 ms: 1.02x faster                                                            |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.6 us: 1.02x faster                                                            |
| logging_format             | 6.81 us                                                | 6.68 us: 1.02x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                            |
| deepcopy                   | 365 us                                                 | 362 us: 1.01x faster                                                             |
| sympy_expand               | 484 ms                                                 | 488 ms: 1.01x slower                                                             |
| chaos                      | 71.9 ms                                                | 72.4 ms: 1.01x slower                                                            |
| tornado_http               | 98.1 ms                                                | 99.2 ms: 1.01x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.72 sec: 1.02x slower                                                           |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                            |
| scimark_sor                | 121 ms                                                 | 126 ms: 1.03x slower                                                             |
| sqlglot_optimize           | 55.3 ms                                                | 57.4 ms: 1.04x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.24 sec: 1.05x slower                                                           |
| pickle_dict                | 34.6 us                                                | 36.6 us: 1.06x slower                                                            |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.06x slower                                                             |
| regex_effbot               | 3.51 ms                                                | 3.74 ms: 1.07x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.7 ms: 1.07x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 69.0 ms: 1.07x slower                                                            |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| 2to3                       | 264 ms                                                 | 284 ms: 1.07x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.67 sec: 1.07x slower                                                           |
| nqueens                    | 87.9 ms                                                | 94.5 ms: 1.08x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 804 ms: 1.08x slower                                                             |
| pickle                     | 11.0 us                                                | 11.8 us: 1.08x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 83.9 ms: 1.09x slower                                                            |
| fannkuch                   | 405 ms                                                 | 445 ms: 1.10x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 89.1 ms: 1.10x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                                            |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.11x slower                                                             |
| tomli_loads                | 2.30 sec                                               | 2.59 sec: 1.13x slower                                                           |
| scimark_monte_carlo        | 70.7 ms                                                | 81.0 ms: 1.15x slower                                                            |
| go                         | 149 ms                                                 | 173 ms: 1.16x slower                                                             |
| pickle_list                | 4.59 us                                                | 5.37 us: 1.17x slower                                                            |
| float                      | 78.9 ms                                                | 93.1 ms: 1.18x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| pyflate                    | 434 ms                                                 | 519 ms: 1.20x slower                                                             |
| async_generators           | 374 ms                                                 | 450 ms: 1.20x slower                                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.06 ms: 1.21x slower                                                            |
| hexiom                     | 6.89 ms                                                | 8.38 ms: 1.22x slower                                                            |
| coverage                   | 78.8 ms                                                | 96.1 ms: 1.22x slower                                                            |
| nbody                      | 96.0 ms                                                | 117 ms: 1.22x slower                                                             |
| unpickle                   | 13.8 us                                                | 17.0 us: 1.23x slower                                                            |
| scimark_fft                | 345 ms                                                 | 436 ms: 1.26x slower                                                             |
| mypy2                      | 686 ms                                                 | 871 ms: 1.27x slower                                                             |
| telco                      | 6.86 ms                                                | 8.97 ms: 1.31x slower                                                            |
| mako                       | 10.7 ms                                                | 14.0 ms: 1.31x slower                                                            |
| spectral_norm              | 108 ms                                                 | 147 ms: 1.36x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.84 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (8): pathlib, scimark_lu, bench_mp_pool, sqlglot_normalize, asyncio_websockets, deepcopy_memo, json, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 93.71% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x