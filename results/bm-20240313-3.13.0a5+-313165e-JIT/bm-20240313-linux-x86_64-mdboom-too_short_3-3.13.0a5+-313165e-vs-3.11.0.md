# Results vs. 3.11.0

- fork: mdboom
- ref: too_short_3
- machine: linux-x86_64
- commit hash: 313165e
- commit date: 2024-03-13
- overall geometric mean: 1.02x faster
- HPT reliability: 60.59%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                          |
| chameleon      | 6.70 ms                                                | 6.86 ms: 1.02x slower                                         |
| docutils       | 2.66 sec                                               | 2.79 sec: 1.05x slower                                        |
| html5lib       | 64.8 ms                                                | 67.1 ms: 1.03x slower                                         |
| tornado_http   | 98.1 ms                                                | 101 ms: 1.03x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                  |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                          |
| async_tree_memoization     | 639 ms                                                 | 573 ms: 1.12x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                          |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 733 ms: 1.02x faster                                          |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                  |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 94.0 ms: 1.02x faster                                         |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                          |
| float          | 78.9 ms                                                | 79.9 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x faster                                                  |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.01x slower                                          |
| regex_effbot   | 3.51 ms                                                | 3.59 ms: 1.02x slower                                         |
| regex_v8       | 22.9 ms                                                | 24.1 ms: 1.05x slower                                         |
| regex_dna      | 205 ms                                                 | 220 ms: 1.07x slower                                          |
| Geometric mean | (ref)                                                  | 1.04x slower                                                  |

Benchmarks with tag 'serialize':
================================

| Benchmark          | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|--------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| json_dumps         | 13.3 ms                                                | 10.5 ms: 1.27x faster                                         |
| tomli_loads        | 2.30 sec                                               | 2.12 sec: 1.09x faster                                        |
| unpickle_list      | 5.21 us                                                | 4.91 us: 1.06x faster                                         |
| pickle_pure_python | 320 us                                                 | 302 us: 1.06x faster                                          |
| json_loads         | 29.2 us                                                | 28.0 us: 1.04x faster                                         |
| xml_etree_parse    | 164 ms                                                 | 161 ms: 1.02x faster                                          |
| pickle_dict        | 34.6 us                                                | 33.9 us: 1.02x faster                                         |
| pickle             | 11.0 us                                                | 11.6 us: 1.05x slower                                         |
| xml_etree_process  | 56.9 ms                                                | 59.8 ms: 1.05x slower                                         |
| unpickle           | 13.8 us                                                | 14.7 us: 1.06x slower                                         |
| xml_etree_generate | 81.1 ms                                                | 87.8 ms: 1.08x slower                                         |
| pickle_list        | 4.59 us                                                | 4.99 us: 1.09x slower                                         |
| Geometric mean     | (ref)                                                  | 1.01x faster                                                  |

Benchmark hidden because not significant (2): unpickle_pure_python, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                  |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 54.6 ms: 1.02x slower                                         |
| django_template | 33.5 ms                                                | 34.5 ms: 1.03x slower                                         |
| genshi_text     | 22.5 ms                                                | 24.2 ms: 1.08x slower                                         |
| Geometric mean  | (ref)                                                  | 1.03x slower                                                  |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-mdboom-too_short_3-3.13.0a5+-313165e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.63x faster                                          |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                         |
| asyncio_tcp                | 875 ms                                                 | 503 ms: 1.74x faster                                          |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                        |
| pylint                     | 476 ms                                                 | 325 ms: 1.46x faster                                          |
| comprehensions             | 23.6 us                                                | 17.4 us: 1.36x faster                                         |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                         |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                         |
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                          |
| richards_super             | 61.9 ms                                                | 53.3 ms: 1.16x faster                                         |
| deltablue                  | 3.92 ms                                                | 3.47 ms: 1.13x faster                                         |
| async_tree_memoization     | 639 ms                                                 | 573 ms: 1.12x faster                                          |
| chaos                      | 71.9 ms                                                | 65.1 ms: 1.10x faster                                         |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.09x faster                                         |
| tomli_loads                | 2.30 sec                                               | 2.12 sec: 1.09x faster                                        |
| gc_traversal               | 4.01 ms                                                | 3.69 ms: 1.09x faster                                         |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                          |
| async_tree_none_tg         | 491 ms                                                 | 456 ms: 1.08x faster                                          |
| async_tree_io              | 1.29 sec                                               | 1.20 sec: 1.07x faster                                        |
| async_tree_memoization_tg  | 626 ms                                                 | 587 ms: 1.07x faster                                          |
| raytrace                   | 309 ms                                                 | 290 ms: 1.06x faster                                          |
| logging_format             | 6.81 us                                                | 6.40 us: 1.06x faster                                         |
| unpickle_list              | 5.21 us                                                | 4.91 us: 1.06x faster                                         |
| logging_simple             | 6.22 us                                                | 5.86 us: 1.06x faster                                         |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                          |
| djangocms                  | 33.5 us                                                | 31.6 us: 1.06x faster                                         |
| mdp                        | 2.77 sec                                               | 2.62 sec: 1.06x faster                                        |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                        |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                         |
| json_loads                 | 29.2 us                                                | 28.0 us: 1.04x faster                                         |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.83 ms: 1.04x faster                                         |
| deepcopy                   | 365 us                                                 | 352 us: 1.04x faster                                          |
| richards                   | 49.8 ms                                                | 48.0 ms: 1.04x faster                                         |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                          |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 738 ms: 1.03x faster                                          |
| sympy_str                  | 297 ms                                                 | 288 ms: 1.03x faster                                          |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                         |
| deepcopy_memo              | 40.2 us                                                | 39.1 us: 1.03x faster                                         |
| fannkuch                   | 405 ms                                                 | 396 ms: 1.02x faster                                          |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.02x faster                                          |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 733 ms: 1.02x faster                                          |
| nbody                      | 96.0 ms                                                | 94.0 ms: 1.02x faster                                         |
| xml_etree_parse            | 164 ms                                                 | 161 ms: 1.02x faster                                          |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                          |
| pickle_dict                | 34.6 us                                                | 33.9 us: 1.02x faster                                         |
| crypto_pyaes               | 76.7 ms                                                | 75.7 ms: 1.01x faster                                         |
| scimark_fft                | 345 ms                                                 | 342 ms: 1.01x faster                                          |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.01x slower                                          |
| sympy_integrate            | 21.5 ms                                                | 21.6 ms: 1.01x slower                                         |
| regex_compile              | 141 ms                                                 | 142 ms: 1.01x slower                                          |
| float                      | 78.9 ms                                                | 79.9 ms: 1.01x slower                                         |
| thrift                     | 784 us                                                 | 794 us: 1.01x slower                                          |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.01x slower                                          |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.02x slower                                         |
| scimark_monte_carlo        | 70.7 ms                                                | 71.8 ms: 1.02x slower                                         |
| asyncio_websockets         | 550 ms                                                 | 562 ms: 1.02x slower                                          |
| nqueens                    | 87.9 ms                                                | 89.7 ms: 1.02x slower                                         |
| genshi_xml                 | 53.4 ms                                                | 54.6 ms: 1.02x slower                                         |
| regex_effbot               | 3.51 ms                                                | 3.59 ms: 1.02x slower                                         |
| dask                       | 365 ms                                                 | 373 ms: 1.02x slower                                          |
| chameleon                  | 6.70 ms                                                | 6.86 ms: 1.02x slower                                         |
| hexiom                     | 6.89 ms                                                | 7.06 ms: 1.03x slower                                         |
| django_template            | 33.5 ms                                                | 34.5 ms: 1.03x slower                                         |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                        |
| sqlglot_optimize           | 55.3 ms                                                | 56.9 ms: 1.03x slower                                         |
| tornado_http               | 98.1 ms                                                | 101 ms: 1.03x slower                                          |
| html5lib                   | 64.8 ms                                                | 67.1 ms: 1.03x slower                                         |
| pprint_safe_repr           | 747 ms                                                 | 774 ms: 1.04x slower                                          |
| bench_thread_pool          | 834 us                                                 | 866 us: 1.04x slower                                          |
| docutils                   | 2.66 sec                                               | 2.79 sec: 1.05x slower                                        |
| pickle                     | 11.0 us                                                | 11.6 us: 1.05x slower                                         |
| xml_etree_process          | 56.9 ms                                                | 59.8 ms: 1.05x slower                                         |
| spectral_norm              | 108 ms                                                 | 114 ms: 1.05x slower                                          |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.05x slower                                         |
| regex_v8                   | 22.9 ms                                                | 24.1 ms: 1.05x slower                                         |
| go                         | 149 ms                                                 | 157 ms: 1.06x slower                                          |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                          |
| unpickle                   | 13.8 us                                                | 14.7 us: 1.06x slower                                         |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                          |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.07x slower                                          |
| genshi_text                | 22.5 ms                                                | 24.2 ms: 1.08x slower                                         |
| xml_etree_generate         | 81.1 ms                                                | 87.8 ms: 1.08x slower                                         |
| aiohttp                    | 1.12 ms                                                | 1.21 ms: 1.09x slower                                         |
| dulwich_log                | 64.6 ms                                                | 70.2 ms: 1.09x slower                                         |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.09x slower                                         |
| pickle_list                | 4.59 us                                                | 4.99 us: 1.09x slower                                         |
| bench_mp_pool              | 24.0 ms                                                | 26.3 ms: 1.10x slower                                         |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                         |
| pyflate                    | 434 ms                                                 | 486 ms: 1.12x slower                                          |
| scimark_lu                 | 116 ms                                                 | 131 ms: 1.13x slower                                          |
| telco                      | 6.86 ms                                                | 8.41 ms: 1.23x slower                                         |
| coverage                   | 78.8 ms                                                | 97.4 ms: 1.24x slower                                         |
| async_generators           | 374 ms                                                 | 472 ms: 1.26x slower                                          |
| mypy2                      | 686 ms                                                 | 906 ms: 1.32x slower                                          |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                         |
| python_startup_no_site     | 6.01 ms                                                | 11.1 ms: 1.85x slower                                         |
| unpack_sequence            | 43.5 ns                                                | 87.5 ns: 2.01x slower                                         |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                  |

Benchmark hidden because not significant (5): json, pprint_pformat, unpickle_pure_python, xml_etree_iterparse, mako
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 60.59% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x