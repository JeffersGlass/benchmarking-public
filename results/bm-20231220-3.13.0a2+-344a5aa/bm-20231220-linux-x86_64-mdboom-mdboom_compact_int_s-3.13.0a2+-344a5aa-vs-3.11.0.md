
# Results vs. 3.11.0

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 344a5aa
- commit date: 2023-12-20
- overall geometric mean: 1.06x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| chameleon      | 6.70 ms                                                | 6.94 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.03x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.8 ms: 1.03x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 435 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 715 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 746 ms: 1.02x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 91.9 ms: 1.04x faster                                                  |
| float          | 78.9 ms                                                | 81.6 ms: 1.03x slower                                                  |
| pidigits       | 194 ms                                                 | 226 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 135 ms: 1.05x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                  |
| regex_v8       | 22.9 ms                                                | 24.1 ms: 1.05x slower                                                  |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 219 us: 1.10x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.16 sec: 1.07x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 304 us: 1.05x faster                                                   |
| json_loads           | 29.2 us                                                | 27.8 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| pickle_dict          | 34.6 us                                                | 33.1 us: 1.04x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| pickle               | 11.0 us                                                | 11.1 us: 1.01x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.8 ms: 1.03x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.4 ms: 1.05x slower                                                  |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.98 us: 1.09x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.95 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.34x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.45x faster                                                   |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.6 us: 1.42x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 435 ms: 1.22x faster                                                   |
| chaos                      | 71.9 ms                                                | 60.4 ms: 1.19x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.37 ms: 1.17x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.7 ms: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 559 ms: 1.14x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.12 ms: 1.13x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                  |
| raytrace                   | 309 ms                                                 | 275 ms: 1.12x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.61 ms: 1.11x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 219 us: 1.10x faster                                                   |
| logging_format             | 6.81 us                                                | 6.20 us: 1.10x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.60 ms: 1.09x faster                                                  |
| sympy_str                  | 297 ms                                                 | 273 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.72 us: 1.09x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                   |
| nqueens                    | 87.9 ms                                                | 81.6 ms: 1.08x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.16 sec: 1.07x faster                                                 |
| sympy_expand               | 484 ms                                                 | 455 ms: 1.07x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.06x faster                                                   |
| go                         | 149 ms                                                 | 140 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                   |
| crypto_pyaes               | 76.7 ms                                                | 72.8 ms: 1.05x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 304 us: 1.05x faster                                                   |
| regex_compile              | 141 ms                                                 | 135 ms: 1.05x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.8 us: 1.05x faster                                                  |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 715 ms: 1.05x faster                                                   |
| nbody                      | 96.0 ms                                                | 91.9 ms: 1.04x faster                                                  |
| pickle_dict                | 34.6 us                                                | 33.1 us: 1.04x faster                                                  |
| deepcopy                   | 365 us                                                 | 350 us: 1.04x faster                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.04x faster                                                 |
| mdp                        | 2.77 sec                                               | 2.68 sec: 1.04x faster                                                 |
| deepcopy_memo              | 40.2 us                                                | 38.8 us: 1.04x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.8 ms: 1.03x faster                                                  |
| richards                   | 49.8 ms                                                | 48.2 ms: 1.03x faster                                                  |
| unpickle_list              | 5.21 us                                                | 5.05 us: 1.03x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 68.5 ms: 1.03x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.8 ms: 1.03x faster                                                  |
| docutils                   | 2.66 sec                                               | 2.60 sec: 1.03x faster                                                 |
| fannkuch                   | 405 ms                                                 | 396 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 746 ms: 1.02x faster                                                   |
| pprint_safe_repr           | 747 ms                                                 | 734 ms: 1.02x faster                                                   |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                 |
| json                       | 5.24 ms                                                | 5.15 ms: 1.02x faster                                                  |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                  |
| bench_thread_pool          | 834 us                                                 | 833 us: 1.00x faster                                                   |
| pickle                     | 11.0 us                                                | 11.1 us: 1.01x slower                                                  |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                   |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                                   |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                                   |
| dulwich_log                | 64.6 ms                                                | 65.7 ms: 1.02x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.8 ms: 1.03x slower                                                  |
| float                      | 78.9 ms                                                | 81.6 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.94 ms: 1.04x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                  |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                  |
| pyflate                    | 434 ms                                                 | 453 ms: 1.05x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 85.4 ms: 1.05x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 24.1 ms: 1.05x slower                                                  |
| scimark_fft                | 345 ms                                                 | 367 ms: 1.06x slower                                                   |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                                   |
| pickle_list                | 4.59 us                                                | 4.98 us: 1.09x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                                  |
| pidigits                   | 194 ms                                                 | 226 ms: 1.16x slower                                                   |
| async_generators           | 374 ms                                                 | 444 ms: 1.19x slower                                                   |
| coverage                   | 78.8 ms                                                | 93.9 ms: 1.19x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.3 ms: 1.20x slower                                                  |
| telco                      | 6.86 ms                                                | 8.27 ms: 1.21x slower                                                  |
| mypy2                      | 686 ms                                                 | 838 ms: 1.22x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.95 ms: 1.49x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.06x faster                                                           |

Benchmark hidden because not significant (6): scimark_sparse_mat_mult, unpack_sequence, 2to3, scimark_lu, bench_mp_pool, asyncio_websockets
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.97x