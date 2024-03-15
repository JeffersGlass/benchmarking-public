
# Results vs. 3.11.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 522c622
- commit date: 2023-12-20
- overall geometric mean: 1.06x faster
- HPT reliability: 99.98%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.03x faster                                                 |
| tornado_http   | 98.1 ms                                                | 95.1 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 436 ms: 1.21x faster                                                   |
| async_tree_memoization    | 639 ms                                                 | 562 ms: 1.14x faster                                                   |
| async_tree_io             | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_none_tg        | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| async_tree_io_tg          | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg | 626 ms                                                 | 598 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 729 ms: 1.03x faster                                                   |
| Geometric mean            | (ref)                                                  | 1.08x faster                                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.7 ms: 1.07x faster                                                  |
| float          | 78.9 ms                                                | 82.4 ms: 1.04x slower                                                  |
| pidigits       | 194 ms                                                 | 223 ms: 1.15x slower                                                   |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 134 ms: 1.06x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                  |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 223 us: 1.08x faster                                                   |
| unpickle_list        | 5.21 us                                                | 4.88 us: 1.07x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 308 us: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| unpickle             | 13.8 us                                                | 14.3 us: 1.04x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.8 ms: 1.06x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.00 us: 1.09x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 9.04 ms: 1.50x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-522c622 |
|---------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 118 us: 4.41x faster                                                   |
| generators                | 74.9 ms                                                | 28.7 ms: 2.61x faster                                                  |
| asyncio_tcp               | 875 ms                                                 | 483 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                 |
| comprehensions            | 23.6 us                                                | 16.4 us: 1.44x faster                                                  |
| json_dumps                | 13.3 ms                                                | 10.4 ms: 1.29x faster                                                  |
| coroutines                | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                  |
| async_tree_none           | 528 ms                                                 | 436 ms: 1.21x faster                                                   |
| deltablue                 | 3.92 ms                                                | 3.31 ms: 1.18x faster                                                  |
| chaos                     | 71.9 ms                                                | 60.8 ms: 1.18x faster                                                  |
| sympy_sum                 | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| richards_super            | 61.9 ms                                                | 54.0 ms: 1.15x faster                                                  |
| async_tree_memoization    | 639 ms                                                 | 562 ms: 1.14x faster                                                   |
| raytrace                  | 309 ms                                                 | 272 ms: 1.14x faster                                                   |
| sqlglot_parse             | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                  |
| hexiom                    | 6.89 ms                                                | 6.23 ms: 1.11x faster                                                  |
| sympy_integrate           | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| sympy_str                 | 297 ms                                                 | 271 ms: 1.10x faster                                                   |
| sqlglot_transpile         | 1.75 ms                                                | 1.60 ms: 1.09x faster                                                  |
| async_tree_io             | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| nqueens                   | 87.9 ms                                                | 81.0 ms: 1.09x faster                                                  |
| unpickle_pure_python      | 242 us                                                 | 223 us: 1.08x faster                                                   |
| async_tree_none_tg        | 491 ms                                                 | 454 ms: 1.08x faster                                                   |
| logging_simple            | 6.22 us                                                | 5.77 us: 1.08x faster                                                  |
| logging_format            | 6.81 us                                                | 6.36 us: 1.07x faster                                                  |
| nbody                     | 96.0 ms                                                | 89.7 ms: 1.07x faster                                                  |
| unpickle_list             | 5.21 us                                                | 4.88 us: 1.07x faster                                                  |
| logging_silent            | 111 ns                                                 | 104 ns: 1.07x faster                                                   |
| async_tree_io_tg          | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| sympy_expand              | 484 ms                                                 | 456 ms: 1.06x faster                                                   |
| tomli_loads               | 2.30 sec                                               | 2.17 sec: 1.06x faster                                                 |
| go                        | 149 ms                                                 | 140 ms: 1.06x faster                                                   |
| sqlglot_normalize         | 113 ms                                                 | 107 ms: 1.06x faster                                                   |
| regex_compile             | 141 ms                                                 | 134 ms: 1.06x faster                                                   |
| async_tree_memoization_tg | 626 ms                                                 | 598 ms: 1.05x faster                                                   |
| crypto_pyaes              | 76.7 ms                                                | 73.3 ms: 1.05x faster                                                  |
| deepcopy                  | 365 us                                                 | 351 us: 1.04x faster                                                   |
| deepcopy_memo             | 40.2 us                                                | 38.7 us: 1.04x faster                                                  |
| pickle_pure_python        | 320 us                                                 | 308 us: 1.04x faster                                                   |
| json_loads                | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| pprint_pformat            | 1.55 sec                                               | 1.50 sec: 1.04x faster                                                 |
| richards                  | 49.8 ms                                                | 48.2 ms: 1.03x faster                                                  |
| tornado_http              | 98.1 ms                                                | 95.1 ms: 1.03x faster                                                  |
| xml_etree_parse           | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| scimark_monte_carlo       | 70.7 ms                                                | 68.8 ms: 1.03x faster                                                  |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 729 ms: 1.03x faster                                                   |
| sqlglot_optimize          | 55.3 ms                                                | 53.8 ms: 1.03x faster                                                  |
| docutils                  | 2.66 sec                                               | 2.60 sec: 1.03x faster                                                 |
| json                      | 5.24 ms                                                | 5.13 ms: 1.02x faster                                                  |
| deepcopy_reduce           | 3.22 us                                                | 3.15 us: 1.02x faster                                                  |
| pycparser                 | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                 |
| pathlib                   | 18.5 ms                                                | 18.2 ms: 1.02x faster                                                  |
| xml_etree_iterparse       | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pprint_safe_repr          | 747 ms                                                 | 735 ms: 1.02x faster                                                   |
| meteor_contest            | 109 ms                                                 | 108 ms: 1.01x faster                                                   |
| fannkuch                  | 405 ms                                                 | 402 ms: 1.01x faster                                                   |
| pickle_dict               | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| bench_thread_pool         | 834 us                                                 | 830 us: 1.00x faster                                                   |
| 2to3                      | 264 ms                                                 | 264 ms: 1.00x faster                                                   |
| dulwich_log               | 64.6 ms                                                | 65.3 ms: 1.01x slower                                                  |
| scimark_lu                | 116 ms                                                 | 118 ms: 1.01x slower                                                   |
| scimark_sor               | 121 ms                                                 | 124 ms: 1.02x slower                                                   |
| spectral_norm             | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| unpickle                  | 13.8 us                                                | 14.3 us: 1.04x slower                                                  |
| chameleon                 | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| xml_etree_process         | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| create_gc_cycles          | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| float                     | 78.9 ms                                                | 82.4 ms: 1.04x slower                                                  |
| mako                      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |
| pickle                    | 11.0 us                                                | 11.5 us: 1.05x slower                                                  |
| regex_effbot              | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                  |
| pyflate                   | 434 ms                                                 | 455 ms: 1.05x slower                                                   |
| xml_etree_generate        | 81.1 ms                                                | 85.8 ms: 1.06x slower                                                  |
| regex_v8                  | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                  |
| gc_traversal              | 4.01 ms                                                | 4.31 ms: 1.08x slower                                                  |
| scimark_fft               | 345 ms                                                 | 372 ms: 1.08x slower                                                   |
| regex_dna                 | 205 ms                                                 | 221 ms: 1.08x slower                                                   |
| unpack_sequence           | 43.5 ns                                                | 47.2 ns: 1.09x slower                                                  |
| sqlite_synth              | 2.57 us                                                | 2.80 us: 1.09x slower                                                  |
| pickle_list               | 4.59 us                                                | 5.00 us: 1.09x slower                                                  |
| pidigits                  | 194 ms                                                 | 223 ms: 1.15x slower                                                   |
| coverage                  | 78.8 ms                                                | 94.0 ms: 1.19x slower                                                  |
| async_generators          | 374 ms                                                 | 450 ms: 1.20x slower                                                   |
| python_startup            | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                  |
| telco                     | 6.86 ms                                                | 8.36 ms: 1.22x slower                                                  |
| mypy2                     | 686 ms                                                 | 838 ms: 1.22x slower                                                   |
| python_startup_no_site    | 6.01 ms                                                | 9.04 ms: 1.50x slower                                                  |
| Geometric mean            | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (5): async_tree_cpu_io_mixed_tg, scimark_sparse_mat_mult, mdp, bench_mp_pool, asyncio_websockets
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x