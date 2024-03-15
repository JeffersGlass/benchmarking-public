
# Results vs. 3.11.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 2f0a32b
- commit date: 2023-12-19
- overall geometric mean: 1.05x faster
- HPT reliability: 99.87%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 266 ms: 1.01x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.07 ms: 1.06x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 95.2 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 439 ms: 1.20x faster                                                   |
| async_tree_memoization    | 639 ms                                                 | 566 ms: 1.13x faster                                                   |
| async_tree_io             | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_none_tg        | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| async_tree_io_tg          | 1.29 sec                                               | 1.23 sec: 1.05x faster                                                 |
| async_tree_memoization_tg | 626 ms                                                 | 607 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 728 ms: 1.03x faster                                                   |
| Geometric mean            | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 90.5 ms: 1.06x faster                                                  |
| float          | 78.9 ms                                                | 82.4 ms: 1.04x slower                                                  |
| pidigits       | 194 ms                                                 | 228 ms: 1.17x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 135 ms: 1.05x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                  |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.7 ms: 1.13x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 224 us: 1.08x faster                                                   |
| unpickle_list        | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 307 us: 1.04x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.1 us: 1.01x faster                                                  |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                  |
| unpickle             | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.98 us: 1.09x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 9.04 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231219-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-2f0a32b |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 117 us: 4.46x faster                                                   |
| generators                | 74.9 ms                                                | 30.0 ms: 2.50x faster                                                  |
| asyncio_tcp               | 875 ms                                                 | 479 ms: 1.83x faster                                                   |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                 |
| comprehensions            | 23.6 us                                                | 16.6 us: 1.42x faster                                                  |
| json_dumps                | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                | 27.0 ms                                                | 21.8 ms: 1.24x faster                                                  |
| async_tree_none           | 528 ms                                                 | 439 ms: 1.20x faster                                                   |
| chaos                     | 71.9 ms                                                | 62.2 ms: 1.16x faster                                                  |
| deltablue                 | 3.92 ms                                                | 3.43 ms: 1.14x faster                                                  |
| sympy_sum                 | 169 ms                                                 | 148 ms: 1.14x faster                                                   |
| richards_super            | 61.9 ms                                                | 54.5 ms: 1.14x faster                                                  |
| async_tree_memoization    | 639 ms                                                 | 566 ms: 1.13x faster                                                   |
| raytrace                  | 309 ms                                                 | 274 ms: 1.13x faster                                                   |
| sqlglot_parse             | 1.43 ms                                                | 1.29 ms: 1.11x faster                                                  |
| sympy_integrate           | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| sympy_str                 | 297 ms                                                 | 273 ms: 1.09x faster                                                   |
| sqlglot_transpile         | 1.75 ms                                                | 1.61 ms: 1.09x faster                                                  |
| hexiom                    | 6.89 ms                                                | 6.36 ms: 1.08x faster                                                  |
| unpickle_pure_python      | 242 us                                                 | 224 us: 1.08x faster                                                   |
| async_tree_io             | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| logging_format            | 6.81 us                                                | 6.31 us: 1.08x faster                                                  |
| nqueens                   | 87.9 ms                                                | 81.7 ms: 1.08x faster                                                  |
| logging_simple            | 6.22 us                                                | 5.79 us: 1.07x faster                                                  |
| async_tree_none_tg        | 491 ms                                                 | 458 ms: 1.07x faster                                                   |
| nbody                     | 96.0 ms                                                | 90.5 ms: 1.06x faster                                                  |
| unpickle_list             | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| tomli_loads               | 2.30 sec                                               | 2.18 sec: 1.06x faster                                                 |
| sympy_expand              | 484 ms                                                 | 460 ms: 1.05x faster                                                   |
| sqlglot_normalize         | 113 ms                                                 | 107 ms: 1.05x faster                                                   |
| mdp                       | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                 |
| async_tree_io_tg          | 1.29 sec                                               | 1.23 sec: 1.05x faster                                                 |
| gc_traversal              | 4.01 ms                                                | 3.82 ms: 1.05x faster                                                  |
| regex_compile             | 141 ms                                                 | 135 ms: 1.05x faster                                                   |
| logging_silent            | 111 ns                                                 | 106 ns: 1.05x faster                                                   |
| pickle_pure_python        | 320 us                                                 | 307 us: 1.04x faster                                                   |
| richards                  | 49.8 ms                                                | 47.9 ms: 1.04x faster                                                  |
| go                        | 149 ms                                                 | 143 ms: 1.04x faster                                                   |
| xml_etree_parse           | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_memoization_tg | 626 ms                                                 | 607 ms: 1.03x faster                                                   |
| scimark_monte_carlo       | 70.7 ms                                                | 68.5 ms: 1.03x faster                                                  |
| crypto_pyaes              | 76.7 ms                                                | 74.4 ms: 1.03x faster                                                  |
| pprint_pformat            | 1.55 sec                                               | 1.51 sec: 1.03x faster                                                 |
| tornado_http              | 98.1 ms                                                | 95.2 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 728 ms: 1.03x faster                                                   |
| json_loads                | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| deepcopy                  | 365 us                                                 | 356 us: 1.03x faster                                                   |
| deepcopy_reduce           | 3.22 us                                                | 3.14 us: 1.02x faster                                                  |
| docutils                  | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| xml_etree_iterparse       | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| sqlglot_optimize          | 55.3 ms                                                | 54.3 ms: 1.02x faster                                                  |
| pathlib                   | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                  |
| pickle_dict               | 34.6 us                                                | 34.1 us: 1.01x faster                                                  |
| fannkuch                  | 405 ms                                                 | 401 ms: 1.01x faster                                                   |
| pprint_safe_repr          | 747 ms                                                 | 741 ms: 1.01x faster                                                   |
| deepcopy_memo             | 40.2 us                                                | 39.9 us: 1.01x faster                                                  |
| 2to3                      | 264 ms                                                 | 266 ms: 1.01x slower                                                   |
| meteor_contest            | 109 ms                                                 | 111 ms: 1.02x slower                                                   |
| dulwich_log               | 64.6 ms                                                | 66.0 ms: 1.02x slower                                                  |
| regex_effbot              | 3.51 ms                                                | 3.60 ms: 1.03x slower                                                  |
| pycparser                 | 1.19 sec                                               | 1.22 sec: 1.03x slower                                                 |
| scimark_sparse_mat_mult   | 5.03 ms                                                | 5.17 ms: 1.03x slower                                                  |
| scimark_sor               | 121 ms                                                 | 126 ms: 1.03x slower                                                   |
| create_gc_cycles          | 1.43 ms                                                | 1.48 ms: 1.03x slower                                                  |
| pickle                    | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| float                     | 78.9 ms                                                | 82.4 ms: 1.04x slower                                                  |
| xml_etree_process         | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                  |
| mako                      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |
| chameleon                 | 6.70 ms                                                | 7.07 ms: 1.06x slower                                                  |
| regex_dna                 | 205 ms                                                 | 216 ms: 1.06x slower                                                   |
| spectral_norm             | 108 ms                                                 | 115 ms: 1.06x slower                                                   |
| xml_etree_generate        | 81.1 ms                                                | 86.6 ms: 1.07x slower                                                  |
| scimark_fft               | 345 ms                                                 | 371 ms: 1.07x slower                                                   |
| unpack_sequence           | 43.5 ns                                                | 46.9 ns: 1.08x slower                                                  |
| pyflate                   | 434 ms                                                 | 469 ms: 1.08x slower                                                   |
| unpickle                  | 13.8 us                                                | 15.0 us: 1.09x slower                                                  |
| pickle_list               | 4.59 us                                                | 4.98 us: 1.09x slower                                                  |
| sqlite_synth              | 2.57 us                                                | 2.80 us: 1.09x slower                                                  |
| regex_v8                  | 22.9 ms                                                | 25.7 ms: 1.13x slower                                                  |
| pidigits                  | 194 ms                                                 | 228 ms: 1.17x slower                                                   |
| async_generators          | 374 ms                                                 | 446 ms: 1.19x slower                                                   |
| coverage                  | 78.8 ms                                                | 95.3 ms: 1.21x slower                                                  |
| python_startup            | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                  |
| telco                     | 6.86 ms                                                | 8.39 ms: 1.22x slower                                                  |
| mypy2                     | 686 ms                                                 | 842 ms: 1.23x slower                                                   |
| python_startup_no_site    | 6.01 ms                                                | 9.04 ms: 1.50x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.05x faster                                                           |

Benchmark hidden because not significant (6): json, scimark_lu, async_tree_cpu_io_mixed_tg, bench_thread_pool, bench_mp_pool, asyncio_websockets
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.87% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x