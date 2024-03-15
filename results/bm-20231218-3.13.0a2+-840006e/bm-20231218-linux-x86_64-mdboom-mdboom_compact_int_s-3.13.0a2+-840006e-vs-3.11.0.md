
# Results vs. 3.11.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 840006e
- commit date: 2023-12-18
- overall geometric mean: 1.05x faster
- HPT reliability: 99.39%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 266 ms: 1.01x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.08 ms: 1.06x slower                                                  |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 95.2 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 438 ms: 1.20x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 831 ms: 1.11x slower                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 861 ms: 1.13x slower                                                   |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.2 ms: 1.08x faster                                                  |
| float          | 78.9 ms                                                | 81.9 ms: 1.04x slower                                                  |
| pidigits       | 194 ms                                                 | 288 ms: 1.48x slower                                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 135 ms: 1.04x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                  |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                                   |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 222 us: 1.09x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.87 us: 1.07x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 305 us: 1.05x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle               | 11.0 us                                                | 11.2 us: 1.02x slower                                                  |
| pickle_dict          | 34.6 us                                                | 35.3 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.5 ms: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.33 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.99 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231218-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-840006e |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.49x faster                                                   |
| generators                 | 74.9 ms                                                | 29.0 ms: 2.58x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 486 ms: 1.80x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.4 us: 1.44x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 21.3 ms: 1.27x faster                                                  |
| async_tree_none            | 528 ms                                                 | 438 ms: 1.20x faster                                                   |
| chaos                      | 71.9 ms                                                | 60.3 ms: 1.19x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.34 ms: 1.17x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| richards_super             | 61.9 ms                                                | 54.7 ms: 1.13x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.59 ms: 1.12x faster                                                  |
| nqueens                    | 87.9 ms                                                | 79.1 ms: 1.11x faster                                                  |
| raytrace                   | 309 ms                                                 | 279 ms: 1.11x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.51 sec: 1.10x faster                                                 |
| hexiom                     | 6.89 ms                                                | 6.25 ms: 1.10x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.60 ms: 1.09x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 222 us: 1.09x faster                                                   |
| sympy_str                  | 297 ms                                                 | 273 ms: 1.09x faster                                                   |
| logging_format             | 6.81 us                                                | 6.28 us: 1.08x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                   |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.76 us: 1.08x faster                                                  |
| nbody                      | 96.0 ms                                                | 89.2 ms: 1.08x faster                                                  |
| unpickle_list              | 5.21 us                                                | 4.87 us: 1.07x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| sympy_expand               | 484 ms                                                 | 456 ms: 1.06x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 72.7 ms: 1.05x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                                   |
| go                         | 149 ms                                                 | 141 ms: 1.05x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 305 us: 1.05x faster                                                   |
| regex_compile              | 141 ms                                                 | 135 ms: 1.04x faster                                                   |
| logging_silent             | 111 ns                                                 | 107 ns: 1.04x faster                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 68.1 ms: 1.04x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.03x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.0 ms: 1.03x faster                                                  |
| richards                   | 49.8 ms                                                | 48.3 ms: 1.03x faster                                                  |
| deepcopy                   | 365 us                                                 | 355 us: 1.03x faster                                                   |
| tornado_http               | 98.1 ms                                                | 95.2 ms: 1.03x faster                                                  |
| fannkuch                   | 405 ms                                                 | 394 ms: 1.03x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                 |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.91 ms: 1.02x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 54.1 ms: 1.02x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 39.3 us: 1.02x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.53 sec: 1.02x faster                                                 |
| json                       | 5.24 ms                                                | 5.15 ms: 1.02x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.01x faster                                                 |
| bench_thread_pool          | 834 us                                                 | 832 us: 1.00x faster                                                   |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| regex_effbot               | 3.51 ms                                                | 3.52 ms: 1.00x slower                                                  |
| 2to3                       | 264 ms                                                 | 266 ms: 1.01x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.5 ms: 1.01x slower                                                  |
| pickle                     | 11.0 us                                                | 11.2 us: 1.02x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.3 us: 1.02x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                  |
| pyflate                    | 434 ms                                                 | 448 ms: 1.03x slower                                                   |
| scimark_fft                | 345 ms                                                 | 357 ms: 1.03x slower                                                   |
| float                      | 78.9 ms                                                | 81.9 ms: 1.04x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                  |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.05x slower                                                   |
| chameleon                  | 6.70 ms                                                | 7.08 ms: 1.06x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 86.5 ms: 1.07x slower                                                  |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.77 us: 1.08x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 831 ms: 1.11x slower                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 861 ms: 1.13x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.33 us: 1.16x slower                                                  |
| coverage                   | 78.8 ms                                                | 93.7 ms: 1.19x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.21x slower                                                  |
| telco                      | 6.86 ms                                                | 8.30 ms: 1.21x slower                                                  |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                                   |
| mypy2                      | 686 ms                                                 | 837 ms: 1.22x slower                                                   |
| pidigits                   | 194 ms                                                 | 288 ms: 1.48x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.99 ms: 1.50x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (6): unpack_sequence, meteor_contest, spectral_norm, bench_mp_pool, scimark_lu, pprint_safe_repr
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.39% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x