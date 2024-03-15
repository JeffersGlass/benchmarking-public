
# Results vs. 3.11.0

- fork: mdboom
- ref: rare_event_stats
- machine: linux-x86_64
- commit hash: f5a8425
- commit date: 2024-01-23
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.01x faster                                               |
| chameleon      | 6.70 ms                                                | 6.87 ms: 1.03x slower                                              |
| docutils       | 2.66 sec                                               | 2.64 sec: 1.01x faster                                             |
| tornado_http   | 98.1 ms                                                | 94.8 ms: 1.03x faster                                              |
| Geometric mean | (ref)                                                  | 1.01x faster                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                               |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                               |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.10x faster                                               |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 705 ms: 1.06x faster                                               |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                       |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.6 ms: 1.08x faster                                              |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                               |
| float          | 78.9 ms                                                | 80.5 ms: 1.02x slower                                              |
| Geometric mean | (ref)                                                  | 1.03x faster                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.10x faster                                               |
| regex_effbot   | 3.51 ms                                                | 3.55 ms: 1.01x slower                                              |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                               |
| regex_v8       | 22.9 ms                                                | 25.4 ms: 1.11x slower                                              |
| Geometric mean | (ref)                                                  | 1.03x slower                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                              |
| unpickle_pure_python | 242 us                                                 | 215 us: 1.12x faster                                               |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                             |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                               |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                              |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                               |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                               |
| pickle_dict          | 34.6 us                                                | 34.0 us: 1.02x faster                                              |
| unpickle_list        | 5.21 us                                                | 5.32 us: 1.02x slower                                              |
| xml_etree_process    | 56.9 ms                                                | 58.8 ms: 1.03x slower                                              |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                              |
| xml_etree_generate   | 81.1 ms                                                | 86.3 ms: 1.06x slower                                              |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                              |
| pickle_list          | 4.59 us                                                | 5.11 us: 1.11x slower                                              |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                       |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                              |
| python_startup_no_site | 6.01 ms                                                | 8.73 ms: 1.45x slower                                              |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|-----------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.0 ms: 1.03x slower                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240123-linux-x86_64-mdboom-rare_event_stats-3.13.0a3+-f5a8425 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 109 us: 4.76x faster                                               |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.54x faster                                              |
| asyncio_tcp                | 875 ms                                                 | 482 ms: 1.82x faster                                               |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                             |
| comprehensions             | 23.6 us                                                | 16.2 us: 1.46x faster                                              |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                              |
| coroutines                 | 27.0 ms                                                | 21.9 ms: 1.23x faster                                              |
| chaos                      | 71.9 ms                                                | 58.7 ms: 1.22x faster                                              |
| deltablue                  | 3.92 ms                                                | 3.22 ms: 1.22x faster                                              |
| async_tree_none            | 528 ms                                                 | 433 ms: 1.22x faster                                               |
| raytrace                   | 309 ms                                                 | 260 ms: 1.19x faster                                               |
| richards_super             | 61.9 ms                                                | 53.2 ms: 1.16x faster                                              |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.15x faster                                              |
| async_tree_memoization     | 639 ms                                                 | 561 ms: 1.14x faster                                               |
| sympy_sum                  | 169 ms                                                 | 149 ms: 1.14x faster                                               |
| unpickle_pure_python       | 242 us                                                 | 215 us: 1.12x faster                                               |
| hexiom                     | 6.89 ms                                                | 6.13 ms: 1.12x faster                                              |
| async_tree_none_tg         | 491 ms                                                 | 438 ms: 1.12x faster                                               |
| sqlglot_transpile          | 1.75 ms                                                | 1.58 ms: 1.11x faster                                              |
| nqueens                    | 87.9 ms                                                | 79.4 ms: 1.11x faster                                              |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                              |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                             |
| regex_compile              | 141 ms                                                 | 129 ms: 1.10x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.10x faster                                               |
| logging_simple             | 6.22 us                                                | 5.69 us: 1.09x faster                                              |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                             |
| sympy_str                  | 297 ms                                                 | 273 ms: 1.09x faster                                               |
| go                         | 149 ms                                                 | 137 ms: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                             |
| nbody                      | 96.0 ms                                                | 88.6 ms: 1.08x faster                                              |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                               |
| deepcopy                   | 365 us                                                 | 339 us: 1.08x faster                                               |
| logging_format             | 6.81 us                                                | 6.33 us: 1.08x faster                                              |
| deepcopy_memo              | 40.2 us                                                | 37.3 us: 1.08x faster                                              |
| deepcopy_reduce            | 3.22 us                                                | 2.99 us: 1.08x faster                                              |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.69 ms: 1.07x faster                                              |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                               |
| gc_traversal               | 4.01 ms                                                | 3.74 ms: 1.07x faster                                              |
| crypto_pyaes               | 76.7 ms                                                | 71.7 ms: 1.07x faster                                              |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 705 ms: 1.06x faster                                               |
| scimark_monte_carlo        | 70.7 ms                                                | 66.6 ms: 1.06x faster                                              |
| sympy_expand               | 484 ms                                                 | 460 ms: 1.05x faster                                               |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                               |
| richards                   | 49.8 ms                                                | 47.4 ms: 1.05x faster                                              |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                             |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                              |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                               |
| tornado_http               | 98.1 ms                                                | 94.8 ms: 1.03x faster                                              |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                               |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                               |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                               |
| sqlglot_optimize           | 55.3 ms                                                | 53.9 ms: 1.03x faster                                              |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                             |
| json                       | 5.24 ms                                                | 5.14 ms: 1.02x faster                                              |
| pprint_safe_repr           | 747 ms                                                 | 733 ms: 1.02x faster                                               |
| pickle_dict                | 34.6 us                                                | 34.0 us: 1.02x faster                                              |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                              |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                               |
| docutils                   | 2.66 sec                                               | 2.64 sec: 1.01x faster                                             |
| fannkuch                   | 405 ms                                                 | 402 ms: 1.01x faster                                               |
| scimark_sor                | 121 ms                                                 | 121 ms: 1.01x faster                                               |
| 2to3                       | 264 ms                                                 | 263 ms: 1.01x faster                                               |
| asyncio_websockets         | 550 ms                                                 | 556 ms: 1.01x slower                                               |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.01x slower                                               |
| regex_effbot               | 3.51 ms                                                | 3.55 ms: 1.01x slower                                              |
| dulwich_log                | 64.6 ms                                                | 65.9 ms: 1.02x slower                                              |
| float                      | 78.9 ms                                                | 80.5 ms: 1.02x slower                                              |
| unpickle_list              | 5.21 us                                                | 5.32 us: 1.02x slower                                              |
| chameleon                  | 6.70 ms                                                | 6.87 ms: 1.03x slower                                              |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                              |
| mako                       | 10.7 ms                                                | 11.0 ms: 1.03x slower                                              |
| xml_etree_process          | 56.9 ms                                                | 58.8 ms: 1.03x slower                                              |
| scimark_fft                | 345 ms                                                 | 360 ms: 1.04x slower                                               |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                              |
| pyflate                    | 434 ms                                                 | 458 ms: 1.06x slower                                               |
| xml_etree_generate         | 81.1 ms                                                | 86.3 ms: 1.06x slower                                              |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                              |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                               |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                              |
| regex_v8                   | 22.9 ms                                                | 25.4 ms: 1.11x slower                                              |
| pickle_list                | 4.59 us                                                | 5.11 us: 1.11x slower                                              |
| async_generators           | 374 ms                                                 | 441 ms: 1.18x slower                                               |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                              |
| coverage                   | 78.8 ms                                                | 93.9 ms: 1.19x slower                                              |
| telco                      | 6.86 ms                                                | 8.33 ms: 1.22x slower                                              |
| mypy2                      | 686 ms                                                 | 840 ms: 1.22x slower                                               |
| unpack_sequence            | 43.5 ns                                                | 55.0 ns: 1.26x slower                                              |
| python_startup_no_site     | 6.01 ms                                                | 8.73 ms: 1.45x slower                                              |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                       |

Benchmark hidden because not significant (3): meteor_contest, bench_mp_pool, bench_thread_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x