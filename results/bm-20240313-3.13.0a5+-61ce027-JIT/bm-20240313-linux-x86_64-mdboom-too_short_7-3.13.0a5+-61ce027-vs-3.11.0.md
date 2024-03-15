# Results vs. 3.11.0

- fork: mdboom
- ref: too_short_7
- machine: linux-x86_64
- commit hash: 61ce027
- commit date: 2024-03-13
- overall geometric mean: 1.02x faster
- HPT reliability: 71.08%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 281 ms: 1.06x slower                                          |
| chameleon      | 6.70 ms                                                | 7.01 ms: 1.05x slower                                         |
| docutils       | 2.66 sec                                               | 2.78 sec: 1.04x slower                                        |
| html5lib       | 64.8 ms                                                | 68.1 ms: 1.05x slower                                         |
| tornado_http   | 98.1 ms                                                | 98.8 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                  | 1.04x slower                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                          |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                          |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 93.5 ms: 1.03x faster                                         |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                          |
| float          | 78.9 ms                                                | 80.6 ms: 1.02x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                          |
| regex_effbot   | 3.51 ms                                                | 3.83 ms: 1.09x slower                                         |
| regex_dna      | 205 ms                                                 | 232 ms: 1.13x slower                                          |
| regex_v8       | 22.9 ms                                                | 26.1 ms: 1.14x slower                                         |
| Geometric mean | (ref)                                                  | 1.09x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                         |
| tomli_loads          | 2.30 sec                                               | 2.07 sec: 1.11x faster                                        |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                          |
| unpickle_list        | 5.21 us                                                | 4.89 us: 1.07x faster                                         |
| json_loads           | 29.2 us                                                | 28.0 us: 1.04x faster                                         |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                          |
| pickle_dict          | 34.6 us                                                | 33.7 us: 1.03x faster                                         |
| unpickle_pure_python | 242 us                                                 | 238 us: 1.02x faster                                          |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                          |
| xml_etree_process    | 56.9 ms                                                | 59.7 ms: 1.05x slower                                         |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                         |
| unpickle             | 13.8 us                                                | 14.8 us: 1.07x slower                                         |
| xml_etree_generate   | 81.1 ms                                                | 87.4 ms: 1.08x slower                                         |
| pickle_list          | 4.59 us                                                | 4.95 us: 1.08x slower                                         |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                  |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.9 ms: 1.02x slower                                         |
| genshi_xml      | 53.4 ms                                                | 55.0 ms: 1.03x slower                                         |
| django_template | 33.5 ms                                                | 34.8 ms: 1.04x slower                                         |
| genshi_text     | 22.5 ms                                                | 24.0 ms: 1.06x slower                                         |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_7-3.13.0a5+-61ce027 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.69x faster                                          |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                         |
| asyncio_tcp                | 875 ms                                                 | 504 ms: 1.74x faster                                          |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                        |
| pylint                     | 476 ms                                                 | 324 ms: 1.47x faster                                          |
| comprehensions             | 23.6 us                                                | 17.3 us: 1.36x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                         |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.20x faster                                         |
| async_tree_none            | 528 ms                                                 | 446 ms: 1.18x faster                                          |
| richards_super             | 61.9 ms                                                | 52.5 ms: 1.18x faster                                         |
| deltablue                  | 3.92 ms                                                | 3.43 ms: 1.14x faster                                         |
| chaos                      | 71.9 ms                                                | 64.5 ms: 1.11x faster                                         |
| tomli_loads                | 2.30 sec                                               | 2.07 sec: 1.11x faster                                        |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                          |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                          |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.09x faster                                         |
| gc_traversal               | 4.01 ms                                                | 3.69 ms: 1.09x faster                                         |
| async_tree_none_tg         | 491 ms                                                 | 458 ms: 1.07x faster                                          |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                          |
| richards                   | 49.8 ms                                                | 46.5 ms: 1.07x faster                                         |
| unpickle_list              | 5.21 us                                                | 4.89 us: 1.07x faster                                         |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                        |
| raytrace                   | 309 ms                                                 | 291 ms: 1.06x faster                                          |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                         |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.06x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                          |
| logging_simple             | 6.22 us                                                | 5.92 us: 1.05x faster                                         |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                        |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                          |
| json_loads                 | 29.2 us                                                | 28.0 us: 1.04x faster                                         |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                          |
| logging_format             | 6.81 us                                                | 6.56 us: 1.04x faster                                         |
| sympy_str                  | 297 ms                                                 | 287 ms: 1.04x faster                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.11 us: 1.04x faster                                         |
| djangocms                  | 33.5 us                                                | 32.4 us: 1.03x faster                                         |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.88 ms: 1.03x faster                                         |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 727 ms: 1.03x faster                                          |
| fannkuch                   | 405 ms                                                 | 394 ms: 1.03x faster                                          |
| nbody                      | 96.0 ms                                                | 93.5 ms: 1.03x faster                                         |
| deepcopy                   | 365 us                                                 | 356 us: 1.03x faster                                          |
| pickle_dict                | 34.6 us                                                | 33.7 us: 1.03x faster                                         |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                          |
| json                       | 5.24 ms                                                | 5.12 ms: 1.02x faster                                         |
| unpickle_pure_python       | 242 us                                                 | 238 us: 1.02x faster                                          |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                         |
| deepcopy_memo              | 40.2 us                                                | 39.7 us: 1.01x faster                                         |
| crypto_pyaes               | 76.7 ms                                                | 75.8 ms: 1.01x faster                                         |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                          |
| tornado_http               | 98.1 ms                                                | 98.8 ms: 1.01x slower                                         |
| pprint_safe_repr           | 747 ms                                                 | 755 ms: 1.01x slower                                          |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                          |
| thrift                     | 784 us                                                 | 794 us: 1.01x slower                                          |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.01x slower                                         |
| sqlglot_optimize           | 55.3 ms                                                | 56.4 ms: 1.02x slower                                         |
| mako                       | 10.7 ms                                                | 10.9 ms: 1.02x slower                                         |
| float                      | 78.9 ms                                                | 80.6 ms: 1.02x slower                                         |
| hexiom                     | 6.89 ms                                                | 7.04 ms: 1.02x slower                                         |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                          |
| dask                       | 365 ms                                                 | 374 ms: 1.02x slower                                          |
| nqueens                    | 87.9 ms                                                | 90.0 ms: 1.02x slower                                         |
| genshi_xml                 | 53.4 ms                                                | 55.0 ms: 1.03x slower                                         |
| bench_thread_pool          | 834 us                                                 | 863 us: 1.03x slower                                          |
| django_template            | 33.5 ms                                                | 34.8 ms: 1.04x slower                                         |
| docutils                   | 2.66 sec                                               | 2.78 sec: 1.04x slower                                        |
| chameleon                  | 6.70 ms                                                | 7.01 ms: 1.05x slower                                         |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                         |
| xml_etree_process          | 56.9 ms                                                | 59.7 ms: 1.05x slower                                         |
| html5lib                   | 64.8 ms                                                | 68.1 ms: 1.05x slower                                         |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                         |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.06x slower                                          |
| spectral_norm              | 108 ms                                                 | 115 ms: 1.06x slower                                          |
| genshi_text                | 22.5 ms                                                | 24.0 ms: 1.06x slower                                         |
| 2to3                       | 264 ms                                                 | 281 ms: 1.06x slower                                          |
| pycparser                  | 1.19 sec                                               | 1.27 sec: 1.07x slower                                        |
| unpickle                   | 13.8 us                                                | 14.8 us: 1.07x slower                                         |
| xml_etree_generate         | 81.1 ms                                                | 87.4 ms: 1.08x slower                                         |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                         |
| dulwich_log                | 64.6 ms                                                | 69.7 ms: 1.08x slower                                         |
| pickle_list                | 4.59 us                                                | 4.95 us: 1.08x slower                                         |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.08x slower                                         |
| bench_mp_pool              | 24.0 ms                                                | 26.3 ms: 1.09x slower                                         |
| regex_effbot               | 3.51 ms                                                | 3.83 ms: 1.09x slower                                         |
| scimark_lu                 | 116 ms                                                 | 129 ms: 1.10x slower                                          |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                         |
| pyflate                    | 434 ms                                                 | 482 ms: 1.11x slower                                          |
| regex_dna                  | 205 ms                                                 | 232 ms: 1.13x slower                                          |
| regex_v8                   | 22.9 ms                                                | 26.1 ms: 1.14x slower                                         |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                          |
| coverage                   | 78.8 ms                                                | 98.0 ms: 1.24x slower                                         |
| telco                      | 6.86 ms                                                | 8.56 ms: 1.25x slower                                         |
| mypy2                      | 686 ms                                                 | 902 ms: 1.32x slower                                          |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site     | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| unpack_sequence            | 43.5 ns                                                | 87.8 ns: 2.02x slower                                         |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                  |

Benchmark hidden because not significant (6): meteor_contest, scimark_fft, pprint_pformat, sympy_expand, go, scimark_monte_carlo
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 71.08% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x