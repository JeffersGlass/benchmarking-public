
# Results vs. 3.12.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: a932d36
- commit date: 2024-02-02
- overall geometric mean: 1.02x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 284 ms: 1.03x slower                                                             |
| chameleon      | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                            |
| docutils       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                           |
| tornado_http   | 103 ms                                                 | 99.2 ms: 1.03x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| async_tree_memoization     | 578 ms                                                 | 570 ms: 1.01x faster                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                           |
| async_tree_none_tg         | 450 ms                                                 | 456 ms: 1.01x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| float          | 84.7 ms                                                | 93.1 ms: 1.10x slower                                                            |
| nbody          | 97.0 ms                                                | 117 ms: 1.21x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| regex_effbot   | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                            |
| regex_dna      | 212 ms                                                 | 226 ms: 1.07x slower                                                             |
| regex_v8       | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                             |
| unpickle_list        | 5.29 us                                                | 4.96 us: 1.07x faster                                                            |
| xml_etree_process    | 61.7 ms                                                | 60.7 ms: 1.02x faster                                                            |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| json_loads           | 28.5 us                                                | 28.6 us: 1.00x slower                                                            |
| pickle               | 11.6 us                                                | 11.8 us: 1.02x slower                                                            |
| json_dumps           | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| unpickle_pure_python | 230 us                                                 | 235 us: 1.02x slower                                                             |
| xml_etree_iterparse  | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| pickle_dict          | 35.5 us                                                | 36.6 us: 1.03x slower                                                            |
| pickle_list          | 5.08 us                                                | 5.37 us: 1.06x slower                                                            |
| unpickle             | 15.9 us                                                | 17.0 us: 1.07x slower                                                            |
| tomli_loads          | 2.33 sec                                               | 2.59 sec: 1.11x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| python_startup_no_site | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.17x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240202-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-a932d36 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 158 us                                                 | 112 us: 1.41x faster                                                             |
| unpack_sequence            | 54.0 ns                                                | 39.4 ns: 1.37x faster                                                            |
| logging_simple             | 6.46 us                                                | 5.88 us: 1.10x faster                                                            |
| gc_traversal               | 3.79 ms                                                | 3.49 ms: 1.09x faster                                                            |
| logging_format             | 7.23 us                                                | 6.68 us: 1.08x faster                                                            |
| pickle_pure_python         | 324 us                                                 | 300 us: 1.08x faster                                                             |
| deepcopy_reduce            | 3.35 us                                                | 3.14 us: 1.07x faster                                                            |
| unpickle_list              | 5.29 us                                                | 4.96 us: 1.07x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 161 ms: 1.05x faster                                                             |
| async_tree_none            | 472 ms                                                 | 449 ms: 1.05x faster                                                             |
| pathlib                    | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                            |
| generators                 | 31.2 ms                                                | 29.8 ms: 1.05x faster                                                            |
| deltablue                  | 3.72 ms                                                | 3.57 ms: 1.04x faster                                                            |
| coroutines                 | 23.2 ms                                                | 22.2 ms: 1.04x faster                                                            |
| raytrace                   | 312 ms                                                 | 301 ms: 1.04x faster                                                             |
| tornado_http               | 103 ms                                                 | 99.2 ms: 1.03x faster                                                            |
| sympy_str                  | 300 ms                                                 | 291 ms: 1.03x faster                                                             |
| async_generators           | 463 ms                                                 | 450 ms: 1.03x faster                                                             |
| scimark_sor                | 129 ms                                                 | 126 ms: 1.03x faster                                                             |
| deepcopy                   | 371 us                                                 | 362 us: 1.02x faster                                                             |
| comprehensions             | 21.8 us                                                | 21.3 us: 1.02x faster                                                            |
| docutils                   | 2.77 sec                                               | 2.72 sec: 1.02x faster                                                           |
| sqlglot_parse              | 1.36 ms                                                | 1.34 ms: 1.02x faster                                                            |
| scimark_lu                 | 118 ms                                                 | 116 ms: 1.02x faster                                                             |
| sympy_integrate            | 21.4 ms                                                | 21.1 ms: 1.02x faster                                                            |
| xml_etree_process          | 61.7 ms                                                | 60.7 ms: 1.02x faster                                                            |
| async_tree_memoization     | 578 ms                                                 | 570 ms: 1.01x faster                                                             |
| chameleon                  | 7.41 ms                                                | 7.32 ms: 1.01x faster                                                            |
| deepcopy_memo              | 40.7 us                                                | 40.3 us: 1.01x faster                                                            |
| logging_silent             | 104 ns                                                 | 103 ns: 1.01x faster                                                             |
| xml_etree_parse            | 159 ms                                                 | 158 ms: 1.01x faster                                                             |
| sqlglot_transpile          | 1.68 ms                                                | 1.67 ms: 1.01x faster                                                            |
| asyncio_tcp                | 491 ms                                                 | 492 ms: 1.00x slower                                                             |
| json_loads                 | 28.5 us                                                | 28.6 us: 1.00x slower                                                            |
| asyncio_tcp_ssl            | 1.79 sec                                               | 1.79 sec: 1.01x slower                                                           |
| bench_thread_pool          | 842 us                                                 | 848 us: 1.01x slower                                                             |
| dulwich_log                | 68.5 ms                                                | 69.0 ms: 1.01x slower                                                            |
| pidigits                   | 187 ms                                                 | 189 ms: 1.01x slower                                                             |
| async_tree_cpu_io_mixed_tg | 726 ms                                                 | 734 ms: 1.01x slower                                                             |
| async_tree_io_tg           | 1.18 sec                                               | 1.20 sec: 1.01x slower                                                           |
| async_tree_none_tg         | 450 ms                                                 | 456 ms: 1.01x slower                                                             |
| regex_compile              | 148 ms                                                 | 151 ms: 1.02x slower                                                             |
| sympy_expand               | 478 ms                                                 | 488 ms: 1.02x slower                                                             |
| pickle                     | 11.6 us                                                | 11.8 us: 1.02x slower                                                            |
| mdp                        | 2.63 sec                                               | 2.69 sec: 1.02x slower                                                           |
| json_dumps                 | 10.4 ms                                                | 10.6 ms: 1.02x slower                                                            |
| unpickle_pure_python       | 230 us                                                 | 235 us: 1.02x slower                                                             |
| sqlglot_normalize          | 110 ms                                                 | 113 ms: 1.02x slower                                                             |
| xml_etree_iterparse        | 107 ms                                                 | 109 ms: 1.02x slower                                                             |
| crypto_pyaes               | 81.9 ms                                                | 83.9 ms: 1.03x slower                                                            |
| meteor_contest             | 112 ms                                                 | 116 ms: 1.03x slower                                                             |
| async_tree_io              | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                           |
| pickle_dict                | 35.5 us                                                | 36.6 us: 1.03x slower                                                            |
| 2to3                       | 274 ms                                                 | 284 ms: 1.03x slower                                                             |
| regex_effbot               | 3.61 ms                                                | 3.74 ms: 1.04x slower                                                            |
| pprint_safe_repr           | 776 ms                                                 | 804 ms: 1.04x slower                                                             |
| async_tree_memoization_tg  | 575 ms                                                 | 599 ms: 1.04x slower                                                             |
| sqlglot_optimize           | 54.8 ms                                                | 57.4 ms: 1.05x slower                                                            |
| richards_super             | 51.5 ms                                                | 54.2 ms: 1.05x slower                                                            |
| pycparser                  | 1.18 sec                                               | 1.24 sec: 1.06x slower                                                           |
| pickle_list                | 5.08 us                                                | 5.37 us: 1.06x slower                                                            |
| richards                   | 45.8 ms                                                | 48.6 ms: 1.06x slower                                                            |
| pprint_pformat             | 1.57 sec                                               | 1.67 sec: 1.06x slower                                                           |
| fannkuch                   | 417 ms                                                 | 445 ms: 1.07x slower                                                             |
| regex_dna                  | 212 ms                                                 | 226 ms: 1.07x slower                                                             |
| python_startup             | 9.55 ms                                                | 10.2 ms: 1.07x slower                                                            |
| regex_v8                   | 23.1 ms                                                | 24.8 ms: 1.07x slower                                                            |
| unpickle                   | 15.9 us                                                | 17.0 us: 1.07x slower                                                            |
| pyflate                    | 482 ms                                                 | 519 ms: 1.08x slower                                                             |
| scimark_monte_carlo        | 75.1 ms                                                | 81.0 ms: 1.08x slower                                                            |
| chaos                      | 67.0 ms                                                | 72.4 ms: 1.08x slower                                                            |
| float                      | 84.7 ms                                                | 93.1 ms: 1.10x slower                                                            |
| tomli_loads                | 2.33 sec                                               | 2.59 sec: 1.11x slower                                                           |
| nqueens                    | 83.3 ms                                                | 94.5 ms: 1.13x slower                                                            |
| scimark_fft                | 382 ms                                                 | 436 ms: 1.14x slower                                                             |
| mako                       | 11.9 ms                                                | 14.0 ms: 1.18x slower                                                            |
| scimark_sparse_mat_mult    | 5.06 ms                                                | 6.06 ms: 1.20x slower                                                            |
| nbody                      | 97.0 ms                                                | 117 ms: 1.21x slower                                                             |
| go                         | 139 ms                                                 | 173 ms: 1.24x slower                                                             |
| telco                      | 7.10 ms                                                | 8.97 ms: 1.26x slower                                                            |
| python_startup_no_site     | 6.94 ms                                                | 8.84 ms: 1.27x slower                                                            |
| spectral_norm              | 115 ms                                                 | 147 ms: 1.28x slower                                                             |
| hexiom                     | 6.41 ms                                                | 8.38 ms: 1.31x slower                                                            |
| coverage                   | 72.7 ms                                                | 96.1 ms: 1.32x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                                     |

Benchmark hidden because not significant (9): dask, async_tree_cpu_io_mixed, bench_mp_pool, xml_etree_generate, asyncio_websockets, json, create_gc_cycles, sqlite_synth, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.93x