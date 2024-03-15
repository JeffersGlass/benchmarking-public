
# Results vs. 3.11.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 01a12af
- commit date: 2023-12-19
- overall geometric mean: 1.05x faster
- HPT reliability: 99.90%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| chameleon      | 6.70 ms                                                | 7.01 ms: 1.05x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.9 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 436 ms: 1.21x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 596 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 834 ms: 1.11x slower                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 866 ms: 1.14x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.2 ms: 1.08x faster                                                  |
| float          | 78.9 ms                                                | 81.5 ms: 1.03x slower                                                  |
| pidigits       | 194 ms                                                 | 289 ms: 1.49x slower                                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.5 ms: 1.07x slower                                                  |
| regex_dna      | 205 ms                                                 | 222 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 222 us: 1.09x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                 |
| pickle_dict          | 34.6 us                                                | 32.8 us: 1.06x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 306 us: 1.04x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| unpickle_list        | 5.21 us                                                | 5.16 us: 1.01x faster                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.15 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): pickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 9.00 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-01a12af |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.43x faster                                                   |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 485 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.5 us: 1.43x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| coroutines                 | 27.0 ms                                                | 21.9 ms: 1.24x faster                                                  |
| async_tree_none            | 528 ms                                                 | 436 ms: 1.21x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.30 ms: 1.19x faster                                                  |
| chaos                      | 71.9 ms                                                | 60.6 ms: 1.19x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.5 ms: 1.16x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.06 ms: 1.14x faster                                                  |
| raytrace                   | 309 ms                                                 | 272 ms: 1.13x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                  |
| sympy_str                  | 297 ms                                                 | 269 ms: 1.11x faster                                                   |
| nqueens                    | 87.9 ms                                                | 80.0 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.6 ms: 1.10x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.60 ms: 1.09x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.69 us: 1.09x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 222 us: 1.09x faster                                                   |
| logging_format             | 6.81 us                                                | 6.25 us: 1.09x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| nbody                      | 96.0 ms                                                | 89.2 ms: 1.08x faster                                                  |
| sympy_expand               | 484 ms                                                 | 455 ms: 1.06x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tomli_loads                | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                 |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 72.3 ms: 1.06x faster                                                  |
| go                         | 149 ms                                                 | 140 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| pickle_dict                | 34.6 us                                                | 32.8 us: 1.06x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 596 ms: 1.05x faster                                                   |
| richards                   | 49.8 ms                                                | 47.4 ms: 1.05x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 306 us: 1.04x faster                                                   |
| regex_compile              | 141 ms                                                 | 136 ms: 1.04x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 38.8 us: 1.04x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.9 ms: 1.03x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.51 sec: 1.03x faster                                                 |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 68.8 ms: 1.03x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.8 ms: 1.03x faster                                                  |
| deepcopy                   | 365 us                                                 | 356 us: 1.03x faster                                                   |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                 |
| json                       | 5.24 ms                                                | 5.13 ms: 1.02x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| fannkuch                   | 405 ms                                                 | 397 ms: 1.02x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 114 ms: 1.02x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.96 ms: 1.01x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.16 us: 1.01x faster                                                  |
| pprint_safe_repr           | 747 ms                                                 | 741 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 830 us: 1.01x faster                                                   |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.4 ms: 1.01x slower                                                  |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                                   |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                                   |
| float                      | 78.9 ms                                                | 81.5 ms: 1.03x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| pyflate                    | 434 ms                                                 | 452 ms: 1.04x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| scimark_fft                | 345 ms                                                 | 362 ms: 1.05x slower                                                   |
| chameleon                  | 6.70 ms                                                | 7.01 ms: 1.05x slower                                                  |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.69 ms: 1.05x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 86.2 ms: 1.06x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.5 ms: 1.07x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 46.7 ns: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.08x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 834 ms: 1.11x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.15 us: 1.12x slower                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 866 ms: 1.14x slower                                                   |
| async_generators           | 374 ms                                                 | 445 ms: 1.19x slower                                                   |
| coverage                   | 78.8 ms                                                | 94.2 ms: 1.20x slower                                                  |
| telco                      | 6.86 ms                                                | 8.30 ms: 1.21x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| mypy2                      | 686 ms                                                 | 837 ms: 1.22x slower                                                   |
| pidigits                   | 194 ms                                                 | 289 ms: 1.49x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 9.00 ms: 1.50x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (5): scimark_sparse_mat_mult, 2to3, bench_mp_pool, asyncio_websockets, pickle
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.90% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x