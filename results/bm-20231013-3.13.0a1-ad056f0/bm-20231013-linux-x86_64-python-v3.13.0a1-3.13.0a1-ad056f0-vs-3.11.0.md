
# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a1
- machine: linux-x86_64
- commit hash: ad056f0
- commit date: 2023-10-13
- overall geometric mean: 1.05x faster \*
- HPT reliability: 99.89%
- HPT 99th percentile: 1.00x faster
- Memory change: 0.97x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 269 ms: 1.02x slower                                       |
| chameleon      | 6.70 ms                                                | 7.07 ms: 1.06x slower                                      |
| docutils       | 2.66 sec                                               | 2.64 sec: 1.01x faster                                     |
| tornado_http   | 98.1 ms                                                | 96.0 ms: 1.02x faster                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                       |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                       |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                     |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.05x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 741 ms: 1.03x faster                                       |
| Geometric mean             | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.6 ms: 1.08x faster                                      |
| pidigits       | 194 ms                                                 | 195 ms: 1.00x slower                                       |
| float          | 78.9 ms                                                | 81.6 ms: 1.03x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 138 ms: 1.02x faster                                       |
| regex_dna      | 205 ms                                                 | 212 ms: 1.04x slower                                       |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                      |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                      |
| Geometric mean | (ref)                                                  | 1.04x slower                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| unpickle_pure_python | 242 us                                                 | 222 us: 1.09x faster                                       |
| tomli_loads          | 2.30 sec                                               | 2.15 sec: 1.07x faster                                     |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                       |
| json_loads           | 29.2 us                                                | 27.8 us: 1.05x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                       |
| unpickle_list        | 5.21 us                                                | 5.05 us: 1.03x faster                                      |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                       |
| xml_etree_process    | 56.9 ms                                                | 59.9 ms: 1.05x slower                                      |
| pickle               | 11.0 us                                                | 11.6 us: 1.06x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 86.9 ms: 1.07x slower                                      |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                      |
| pickle_list          | 4.59 us                                                | 5.10 us: 1.11x slower                                      |
| Geometric mean       | (ref)                                                  | 1.02x faster                                               |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 6.87 ms: 1.14x slower                                      |
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                      |
| Geometric mean         | (ref)                                                  | 1.16x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.06x slower                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231013-linux-x86_64-python-v3.13.0a1-3.13.0a1-ad056f0 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 156 us: 3.34x faster                                       |
| generators                 | 74.9 ms                                                | 29.9 ms: 2.50x faster                                      |
| asyncio_tcp                | 875 ms                                                 | 484 ms: 1.81x faster                                       |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                     |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| async_tree_none            | 528 ms                                                 | 437 ms: 1.21x faster                                       |
| deltablue                  | 3.92 ms                                                | 3.34 ms: 1.17x faster                                      |
| chaos                      | 71.9 ms                                                | 61.7 ms: 1.16x faster                                      |
| coroutines                 | 27.0 ms                                                | 23.4 ms: 1.16x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 564 ms: 1.13x faster                                       |
| comprehensions             | 23.6 us                                                | 20.8 us: 1.13x faster                                      |
| raytrace                   | 309 ms                                                 | 274 ms: 1.13x faster                                       |
| richards_super             | 61.9 ms                                                | 55.0 ms: 1.13x faster                                      |
| hexiom                     | 6.89 ms                                                | 6.16 ms: 1.12x faster                                      |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.60 ms: 1.09x faster                                      |
| unpickle_pure_python       | 242 us                                                 | 222 us: 1.09x faster                                       |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                     |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                       |
| sympy_sum                  | 169 ms                                                 | 156 ms: 1.08x faster                                       |
| nbody                      | 96.0 ms                                                | 88.6 ms: 1.08x faster                                      |
| nqueens                    | 87.9 ms                                                | 81.9 ms: 1.07x faster                                      |
| tomli_loads                | 2.30 sec                                               | 2.15 sec: 1.07x faster                                     |
| sympy_expand               | 484 ms                                                 | 452 ms: 1.07x faster                                       |
| crypto_pyaes               | 76.7 ms                                                | 71.8 ms: 1.07x faster                                      |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                       |
| sympy_integrate            | 21.5 ms                                                | 20.2 ms: 1.06x faster                                      |
| sympy_str                  | 297 ms                                                 | 281 ms: 1.06x faster                                       |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.23 sec: 1.05x faster                                     |
| logging_simple             | 6.22 us                                                | 5.90 us: 1.05x faster                                      |
| logging_format             | 6.81 us                                                | 6.47 us: 1.05x faster                                      |
| go                         | 149 ms                                                 | 141 ms: 1.05x faster                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 595 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 712 ms: 1.05x faster                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.79 ms: 1.05x faster                                      |
| json_loads                 | 29.2 us                                                | 27.8 us: 1.05x faster                                      |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                       |
| deepcopy_memo              | 40.2 us                                                | 38.7 us: 1.04x faster                                      |
| logging_silent             | 111 ns                                                 | 107 ns: 1.04x faster                                       |
| gc_traversal               | 4.01 ms                                                | 3.87 ms: 1.04x faster                                      |
| deepcopy                   | 365 us                                                 | 353 us: 1.04x faster                                       |
| unpickle_list              | 5.21 us                                                | 5.05 us: 1.03x faster                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 741 ms: 1.03x faster                                       |
| sqlglot_optimize           | 55.3 ms                                                | 53.9 ms: 1.03x faster                                      |
| richards                   | 49.8 ms                                                | 48.6 ms: 1.03x faster                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.14 us: 1.02x faster                                      |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                       |
| bench_thread_pool          | 834 us                                                 | 815 us: 1.02x faster                                       |
| tornado_http               | 98.1 ms                                                | 96.0 ms: 1.02x faster                                      |
| regex_compile              | 141 ms                                                 | 138 ms: 1.02x faster                                       |
| pprint_pformat             | 1.55 sec                                               | 1.53 sec: 1.02x faster                                     |
| scimark_monte_carlo        | 70.7 ms                                                | 69.5 ms: 1.02x faster                                      |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                      |
| mdp                        | 2.77 sec                                               | 2.74 sec: 1.01x faster                                     |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                       |
| docutils                   | 2.66 sec                                               | 2.64 sec: 1.01x faster                                     |
| fannkuch                   | 405 ms                                                 | 402 ms: 1.01x faster                                       |
| pidigits                   | 194 ms                                                 | 195 ms: 1.00x slower                                       |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x slower                                       |
| pprint_safe_repr           | 747 ms                                                 | 752 ms: 1.01x slower                                       |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.01x slower                                       |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.02x slower                                     |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.02x slower                                       |
| 2to3                       | 264 ms                                                 | 269 ms: 1.02x slower                                       |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                      |
| float                      | 78.9 ms                                                | 81.6 ms: 1.03x slower                                      |
| regex_dna                  | 205 ms                                                 | 212 ms: 1.04x slower                                       |
| dulwich_log                | 64.6 ms                                                | 67.1 ms: 1.04x slower                                      |
| pathlib                    | 18.5 ms                                                | 19.4 ms: 1.05x slower                                      |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                      |
| xml_etree_process          | 56.9 ms                                                | 59.9 ms: 1.05x slower                                      |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.06x slower                                      |
| chameleon                  | 6.70 ms                                                | 7.07 ms: 1.06x slower                                      |
| pickle                     | 11.0 us                                                | 11.6 us: 1.06x slower                                      |
| scimark_fft                | 345 ms                                                 | 369 ms: 1.07x slower                                       |
| xml_etree_generate         | 81.1 ms                                                | 86.9 ms: 1.07x slower                                      |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                      |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                      |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                      |
| pyflate                    | 434 ms                                                 | 473 ms: 1.09x slower                                       |
| pickle_list                | 4.59 us                                                | 5.10 us: 1.11x slower                                      |
| python_startup_no_site     | 6.01 ms                                                | 6.87 ms: 1.14x slower                                      |
| unpack_sequence            | 43.5 ns                                                | 51.0 ns: 1.17x slower                                      |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                      |
| telco                      | 6.86 ms                                                | 8.17 ms: 1.19x slower                                      |
| coverage                   | 78.8 ms                                                | 94.4 ms: 1.20x slower                                      |
| async_generators           | 374 ms                                                 | 453 ms: 1.21x slower                                       |
| Geometric mean             | (ref)                                                  | 1.05x faster                                               |

Benchmark hidden because not significant (3): bench_mp_pool, pickle_dict, asyncio_websockets
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.89% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 0.97x