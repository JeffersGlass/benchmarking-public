# Results vs. 3.11.0

- fork: python
- ref: 61e54bfcee9f08a8e09a
- machine: linux-x86_64
- commit hash: 61e54bf
- commit date: 2024-03-14
- overall geometric mean: 1.02x faster
- HPT reliability: 52.33%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.78 sec: 1.04x slower                                                 |
| html5lib       | 64.8 ms                                                | 66.8 ms: 1.03x slower                                                  |
| tornado_http   | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.06x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 731 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.7 ms: 1.04x faster                                                  |
| pidigits       | 194 ms                                                 | 189 ms: 1.02x faster                                                   |
| float          | 78.9 ms                                                | 80.0 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 143 ms: 1.01x slower                                                   |
| regex_effbot   | 3.51 ms                                                | 3.79 ms: 1.08x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                  |
| regex_dna      | 205 ms                                                 | 234 ms: 1.14x slower                                                   |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 308 us: 1.04x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.02x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 239 us: 1.01x faster                                                   |
| pickle_dict          | 34.6 us                                                | 35.4 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                  |
| pickle               | 11.0 us                                                | 11.9 us: 1.09x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 88.6 ms: 1.09x slower                                                  |
| unpickle             | 13.8 us                                                | 15.4 us: 1.11x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.29 us: 1.15x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.65x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 54.6 ms: 1.02x slower                                                  |
| django_template | 33.5 ms                                                | 34.7 ms: 1.03x slower                                                  |
| mako            | 10.7 ms                                                | 11.1 ms: 1.05x slower                                                  |
| genshi_text     | 22.5 ms                                                | 24.2 ms: 1.08x slower                                                  |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240314-linux-x86_64-python-61e54bfcee9f08a8e09a-3.13.0a5+-61e54bf |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.69x faster                                                   |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.53x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 505 ms: 1.73x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                                 |
| pylint                     | 476 ms                                                 | 325 ms: 1.46x faster                                                   |
| comprehensions             | 23.6 us                                                | 17.5 us: 1.35x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.6 ms: 1.26x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.20x faster                                                  |
| async_tree_none            | 528 ms                                                 | 447 ms: 1.18x faster                                                   |
| richards_super             | 61.9 ms                                                | 53.1 ms: 1.17x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.42 ms: 1.15x faster                                                  |
| chaos                      | 71.9 ms                                                | 64.0 ms: 1.12x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.07 sec: 1.11x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 576 ms: 1.11x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.32 ms: 1.08x faster                                                  |
| logging_silent             | 111 ns                                                 | 102 ns: 1.08x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.77 us: 1.08x faster                                                  |
| richards                   | 49.8 ms                                                | 46.5 ms: 1.07x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 461 ms: 1.06x faster                                                   |
| logging_format             | 6.81 us                                                | 6.42 us: 1.06x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                  |
| deepcopy_reduce            | 3.22 us                                                | 3.06 us: 1.05x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                   |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.82 ms: 1.04x faster                                                  |
| deepcopy                   | 365 us                                                 | 351 us: 1.04x faster                                                   |
| raytrace                   | 309 ms                                                 | 297 ms: 1.04x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                  |
| djangocms                  | 33.5 us                                                | 32.3 us: 1.04x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 308 us: 1.04x faster                                                   |
| sympy_str                  | 297 ms                                                 | 287 ms: 1.04x faster                                                   |
| nbody                      | 96.0 ms                                                | 92.7 ms: 1.04x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 38.9 us: 1.03x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 731 ms: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 189 ms: 1.02x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 160 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 743 ms: 1.02x faster                                                   |
| fannkuch                   | 405 ms                                                 | 399 ms: 1.02x faster                                                   |
| unpickle_pure_python       | 242 us                                                 | 239 us: 1.01x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.3 ms: 1.01x faster                                                  |
| tornado_http               | 98.1 ms                                                | 99.0 ms: 1.01x slower                                                  |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                  |
| float                      | 78.9 ms                                                | 80.0 ms: 1.01x slower                                                  |
| regex_compile              | 141 ms                                                 | 143 ms: 1.01x slower                                                   |
| gc_traversal               | 4.01 ms                                                | 4.07 ms: 1.02x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.58 sec: 1.02x slower                                                 |
| dask                       | 365 ms                                                 | 373 ms: 1.02x slower                                                   |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.02x slower                                                   |
| genshi_xml                 | 53.4 ms                                                | 54.6 ms: 1.02x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.4 us: 1.02x slower                                                  |
| asyncio_websockets         | 550 ms                                                 | 564 ms: 1.02x slower                                                   |
| nqueens                    | 87.9 ms                                                | 90.0 ms: 1.02x slower                                                  |
| thrift                     | 784 us                                                 | 804 us: 1.02x slower                                                   |
| hexiom                     | 6.89 ms                                                | 7.06 ms: 1.02x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 56.8 ms: 1.03x slower                                                  |
| html5lib                   | 64.8 ms                                                | 66.8 ms: 1.03x slower                                                  |
| pprint_safe_repr           | 747 ms                                                 | 770 ms: 1.03x slower                                                   |
| django_template            | 33.5 ms                                                | 34.7 ms: 1.03x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 864 us: 1.04x slower                                                   |
| chameleon                  | 6.70 ms                                                | 6.96 ms: 1.04x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.78 sec: 1.04x slower                                                 |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.05x slower                                                  |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.05x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.05x slower                                                  |
| go                         | 149 ms                                                 | 157 ms: 1.06x slower                                                   |
| pycparser                  | 1.19 sec                                               | 1.26 sec: 1.06x slower                                                 |
| spectral_norm              | 108 ms                                                 | 115 ms: 1.06x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 60.6 ms: 1.06x slower                                                  |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| genshi_text                | 22.5 ms                                                | 24.2 ms: 1.08x slower                                                  |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.79 ms: 1.08x slower                                                  |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.08x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 70.0 ms: 1.08x slower                                                  |
| pickle                     | 11.0 us                                                | 11.9 us: 1.09x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 88.6 ms: 1.09x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.4 us: 1.11x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 129 ms: 1.11x slower                                                   |
| bench_mp_pool              | 24.0 ms                                                | 26.8 ms: 1.11x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.87 us: 1.12x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                  |
| pyflate                    | 434 ms                                                 | 493 ms: 1.14x slower                                                   |
| regex_dna                  | 205 ms                                                 | 234 ms: 1.14x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.29 us: 1.15x slower                                                  |
| telco                      | 6.86 ms                                                | 8.43 ms: 1.23x slower                                                  |
| coverage                   | 78.8 ms                                                | 98.5 ms: 1.25x slower                                                  |
| async_generators           | 374 ms                                                 | 469 ms: 1.25x slower                                                   |
| mypy2                      | 686 ms                                                 | 906 ms: 1.32x slower                                                   |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 87.8 ns: 2.02x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (6): json, scimark_fft, sympy_expand, scimark_monte_carlo, crypto_pyaes, xml_etree_iterparse
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 52.33% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x