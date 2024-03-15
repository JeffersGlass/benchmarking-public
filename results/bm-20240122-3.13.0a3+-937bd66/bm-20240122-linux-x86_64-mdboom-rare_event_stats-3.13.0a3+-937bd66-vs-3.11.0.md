
# Results vs. 3.11.0

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: 937bd66
- commit date: 2024-01-22
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                               |
| chameleon      | 6.70 ms                                                | 7.06 ms: 1.05x slower                                              |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.02x faster                                             |
| tornado_http   | 98.1 ms                                                | 94.2 ms: 1.04x faster                                              |
| Geometric mean | (ref)                                                  | 1.00x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 431 ms: 1.23x faster                                               |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                               |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 569 ms: 1.10x faster                                               |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                               |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                               |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 86.1 ms: 1.11x faster                                              |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                               |
| float          | 78.9 ms                                                | 80.1 ms: 1.02x slower                                              |
| Geometric mean | (ref)                                                  | 1.04x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.09x faster                                               |
| regex_effbot   | 3.51 ms                                                | 3.54 ms: 1.01x slower                                              |
| regex_dna      | 205 ms                                                 | 222 ms: 1.09x slower                                               |
| regex_v8       | 22.9 ms                                                | 25.5 ms: 1.11x slower                                              |
| Geometric mean | (ref)                                                  | 1.03x slower                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                              |
| unpickle_pure_python | 242 us                                                 | 212 us: 1.14x faster                                               |
| tomli_loads          | 2.30 sec                                               | 2.12 sec: 1.09x faster                                             |
| pickle_pure_python   | 320 us                                                 | 297 us: 1.08x faster                                               |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                              |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                               |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                               |
| pickle_dict          | 34.6 us                                                | 34.8 us: 1.01x slower                                              |
| xml_etree_process    | 56.9 ms                                                | 58.6 ms: 1.03x slower                                              |
| unpickle_list        | 5.21 us                                                | 5.41 us: 1.04x slower                                              |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                              |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                              |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                              |
| pickle_list          | 4.59 us                                                | 5.27 us: 1.15x slower                                              |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                              |
| python_startup_no_site | 6.01 ms                                                | 8.68 ms: 1.44x slower                                              |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240122-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-937bd66 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.70x faster                                               |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                              |
| asyncio_tcp                | 875 ms                                                 | 480 ms: 1.82x faster                                               |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                             |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.47x faster                                              |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                              |
| deltablue                  | 3.92 ms                                                | 3.15 ms: 1.25x faster                                              |
| async_tree_none            | 528 ms                                                 | 431 ms: 1.23x faster                                               |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                              |
| chaos                      | 71.9 ms                                                | 59.5 ms: 1.21x faster                                              |
| raytrace                   | 309 ms                                                 | 257 ms: 1.20x faster                                               |
| hexiom                     | 6.89 ms                                                | 5.89 ms: 1.17x faster                                              |
| richards_super             | 61.9 ms                                                | 53.3 ms: 1.16x faster                                              |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.14x faster                                              |
| async_tree_memoization     | 639 ms                                                 | 560 ms: 1.14x faster                                               |
| unpickle_pure_python       | 242 us                                                 | 212 us: 1.14x faster                                               |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                               |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                               |
| nbody                      | 96.0 ms                                                | 86.1 ms: 1.11x faster                                              |
| sqlglot_transpile          | 1.75 ms                                                | 1.58 ms: 1.11x faster                                              |
| async_tree_memoization_tg  | 626 ms                                                 | 569 ms: 1.10x faster                                               |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                              |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                             |
| nqueens                    | 87.9 ms                                                | 80.1 ms: 1.10x faster                                              |
| regex_compile              | 141 ms                                                 | 130 ms: 1.09x faster                                               |
| go                         | 149 ms                                                 | 137 ms: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                             |
| logging_format             | 6.81 us                                                | 6.26 us: 1.09x faster                                              |
| tomli_loads                | 2.30 sec                                               | 2.12 sec: 1.09x faster                                             |
| crypto_pyaes               | 76.7 ms                                                | 70.9 ms: 1.08x faster                                              |
| logging_simple             | 6.22 us                                                | 5.76 us: 1.08x faster                                              |
| pickle_pure_python         | 320 us                                                 | 297 us: 1.08x faster                                               |
| sympy_str                  | 297 ms                                                 | 279 ms: 1.07x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 702 ms: 1.07x faster                                               |
| scimark_monte_carlo        | 70.7 ms                                                | 66.4 ms: 1.07x faster                                              |
| deepcopy_memo              | 40.2 us                                                | 37.7 us: 1.06x faster                                              |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                               |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                               |
| deepcopy                   | 365 us                                                 | 348 us: 1.05x faster                                               |
| richards                   | 49.8 ms                                                | 47.4 ms: 1.05x faster                                              |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                               |
| deepcopy_reduce            | 3.22 us                                                | 3.07 us: 1.05x faster                                              |
| sympy_expand               | 484 ms                                                 | 464 ms: 1.04x faster                                               |
| tornado_http               | 98.1 ms                                                | 94.2 ms: 1.04x faster                                              |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                              |
| xml_etree_iterparse        | 108 ms                                                 | 104 ms: 1.04x faster                                               |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                               |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                               |
| pprint_pformat             | 1.55 sec                                               | 1.51 sec: 1.03x faster                                             |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                               |
| pycparser                  | 1.19 sec                                               | 1.15 sec: 1.03x faster                                             |
| json                       | 5.24 ms                                                | 5.11 ms: 1.02x faster                                              |
| docutils                   | 2.66 sec                                               | 2.60 sec: 1.02x faster                                             |
| sqlglot_optimize           | 55.3 ms                                                | 54.2 ms: 1.02x faster                                              |
| gc_traversal               | 4.01 ms                                                | 3.94 ms: 1.02x faster                                              |
| mdp                        | 2.77 sec                                               | 2.73 sec: 1.02x faster                                             |
| pprint_safe_repr           | 747 ms                                                 | 736 ms: 1.02x faster                                               |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                              |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                               |
| bench_thread_pool          | 834 us                                                 | 825 us: 1.01x faster                                               |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                               |
| fannkuch                   | 405 ms                                                 | 403 ms: 1.00x faster                                               |
| 2to3                       | 264 ms                                                 | 264 ms: 1.00x faster                                               |
| pickle_dict                | 34.6 us                                                | 34.8 us: 1.01x slower                                              |
| regex_effbot               | 3.51 ms                                                | 3.54 ms: 1.01x slower                                              |
| dulwich_log                | 64.6 ms                                                | 65.3 ms: 1.01x slower                                              |
| asyncio_websockets         | 550 ms                                                 | 557 ms: 1.01x slower                                               |
| scimark_fft                | 345 ms                                                 | 350 ms: 1.01x slower                                               |
| float                      | 78.9 ms                                                | 80.1 ms: 1.02x slower                                              |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                              |
| xml_etree_process          | 56.9 ms                                                | 58.6 ms: 1.03x slower                                              |
| unpickle_list              | 5.21 us                                                | 5.41 us: 1.04x slower                                              |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                              |
| unpack_sequence            | 43.5 ns                                                | 45.2 ns: 1.04x slower                                              |
| chameleon                  | 6.70 ms                                                | 7.06 ms: 1.05x slower                                              |
| xml_etree_generate         | 81.1 ms                                                | 85.6 ms: 1.06x slower                                              |
| pyflate                    | 434 ms                                                 | 460 ms: 1.06x slower                                               |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                              |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.09x slower                                               |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                              |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                              |
| regex_v8                   | 22.9 ms                                                | 25.5 ms: 1.11x slower                                              |
| pickle_list                | 4.59 us                                                | 5.27 us: 1.15x slower                                              |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                              |
| async_generators           | 374 ms                                                 | 442 ms: 1.18x slower                                               |
| coverage                   | 78.8 ms                                                | 94.4 ms: 1.20x slower                                              |
| telco                      | 6.86 ms                                                | 8.24 ms: 1.20x slower                                              |
| mypy2                      | 686 ms                                                 | 839 ms: 1.22x slower                                               |
| python_startup_no_site     | 6.01 ms                                                | 8.68 ms: 1.44x slower                                              |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                       |

Benchmark hidden because not significant (4): spectral_norm, scimark_sor, bench_mp_pool, scimark_sparse_mat_mult
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x