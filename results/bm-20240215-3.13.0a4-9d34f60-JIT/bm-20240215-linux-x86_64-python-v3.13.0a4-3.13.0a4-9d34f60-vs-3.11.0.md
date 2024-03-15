# Results vs. 3.11.0

- fork: python
- ref: v3.13.0a4
- machine: linux-x86_64
- commit hash: 9d34f60
- commit date: 2024-02-15
- overall geometric mean: 1.04x faster \*
- HPT reliability: 83.81%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 276 ms: 1.04x slower                                       |
| chameleon      | 6.70 ms                                                | 6.75 ms: 1.01x slower                                      |
| docutils       | 2.66 sec                                               | 2.64 sec: 1.01x faster                                     |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                      |
| Geometric mean | (ref)                                                  | 1.01x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                       |
| async_tree_memoization     | 639 ms                                                 | 568 ms: 1.13x faster                                       |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                     |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                       |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 716 ms: 1.05x faster                                       |
| Geometric mean             | (ref)                                                  | 1.09x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                       |
| nbody          | 96.0 ms                                                | 102 ms: 1.07x slower                                       |
| float          | 78.9 ms                                                | 86.1 ms: 1.09x slower                                      |
| Geometric mean | (ref)                                                  | 1.04x slower                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.57 ms: 1.02x slower                                      |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.10x slower                                      |
| regex_dna      | 205 ms                                                 | 225 ms: 1.10x slower                                       |
| Geometric mean | (ref)                                                  | 1.05x slower                                               |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| pickle_pure_python   | 320 us                                                 | 296 us: 1.08x faster                                       |
| json_loads           | 29.2 us                                                | 27.3 us: 1.07x faster                                      |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                       |
| tomli_loads          | 2.30 sec                                               | 2.19 sec: 1.05x faster                                     |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                       |
| pickle_dict          | 34.6 us                                                | 33.6 us: 1.03x faster                                      |
| unpickle_list        | 5.21 us                                                | 5.11 us: 1.02x faster                                      |
| xml_etree_process    | 56.9 ms                                                | 57.9 ms: 1.02x slower                                      |
| pickle               | 11.0 us                                                | 11.4 us: 1.03x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 85.7 ms: 1.06x slower                                      |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                      |
| pickle_list          | 4.59 us                                                | 5.07 us: 1.11x slower                                      |
| Geometric mean       | (ref)                                                  | 1.02x faster                                               |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.3 ms: 1.20x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 8.95 ms: 1.49x slower                                      |
| Geometric mean         | (ref)                                                  | 1.34x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.4 ms: 1.16x slower                                      |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-linux-x86_64-python-v3.13.0a4-3.13.0a4-9d34f60 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.74x faster                                       |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                      |
| asyncio_tcp                | 875 ms                                                 | 497 ms: 1.76x faster                                       |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                     |
| comprehensions             | 23.6 us                                                | 18.2 us: 1.30x faster                                      |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                      |
| richards_super             | 61.9 ms                                                | 50.8 ms: 1.22x faster                                      |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                       |
| deltablue                  | 3.92 ms                                                | 3.32 ms: 1.18x faster                                      |
| coroutines                 | 27.0 ms                                                | 23.7 ms: 1.14x faster                                      |
| async_tree_memoization     | 639 ms                                                 | 568 ms: 1.13x faster                                       |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                      |
| richards                   | 49.8 ms                                                | 44.8 ms: 1.11x faster                                      |
| raytrace                   | 309 ms                                                 | 280 ms: 1.10x faster                                       |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                       |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                     |
| sqlglot_transpile          | 1.75 ms                                                | 1.61 ms: 1.09x faster                                      |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                       |
| logging_simple             | 6.22 us                                                | 5.74 us: 1.08x faster                                      |
| pickle_pure_python         | 320 us                                                 | 296 us: 1.08x faster                                       |
| logging_format             | 6.81 us                                                | 6.30 us: 1.08x faster                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                     |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.08x faster                                       |
| json_loads                 | 29.2 us                                                | 27.3 us: 1.07x faster                                      |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                      |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                       |
| sympy_str                  | 297 ms                                                 | 281 ms: 1.06x faster                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                       |
| deepcopy                   | 365 us                                                 | 345 us: 1.06x faster                                       |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                      |
| sympy_integrate            | 21.5 ms                                                | 20.3 ms: 1.06x faster                                      |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                       |
| deepcopy_memo              | 40.2 us                                                | 38.1 us: 1.05x faster                                      |
| tomli_loads                | 2.30 sec                                               | 2.19 sec: 1.05x faster                                     |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 716 ms: 1.05x faster                                       |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                       |
| chaos                      | 71.9 ms                                                | 69.1 ms: 1.04x faster                                      |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                       |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                       |
| pickle_dict                | 34.6 us                                                | 33.6 us: 1.03x faster                                      |
| json                       | 5.24 ms                                                | 5.12 ms: 1.02x faster                                      |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                      |
| unpickle_list              | 5.21 us                                                | 5.11 us: 1.02x faster                                      |
| go                         | 149 ms                                                 | 146 ms: 1.02x faster                                       |
| tornado_http               | 98.1 ms                                                | 96.9 ms: 1.01x faster                                      |
| sympy_expand               | 484 ms                                                 | 480 ms: 1.01x faster                                       |
| docutils                   | 2.66 sec                                               | 2.64 sec: 1.01x faster                                     |
| sqlglot_optimize           | 55.3 ms                                                | 55.1 ms: 1.00x faster                                      |
| mdp                        | 2.77 sec                                               | 2.78 sec: 1.00x slower                                     |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                       |
| chameleon                  | 6.70 ms                                                | 6.75 ms: 1.01x slower                                      |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                       |
| regex_effbot               | 3.51 ms                                                | 3.57 ms: 1.02x slower                                      |
| xml_etree_process          | 56.9 ms                                                | 57.9 ms: 1.02x slower                                      |
| nqueens                    | 87.9 ms                                                | 89.8 ms: 1.02x slower                                      |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                     |
| crypto_pyaes               | 76.7 ms                                                | 79.1 ms: 1.03x slower                                      |
| unpack_sequence            | 43.5 ns                                                | 44.9 ns: 1.03x slower                                      |
| pickle                     | 11.0 us                                                | 11.4 us: 1.03x slower                                      |
| pprint_safe_repr           | 747 ms                                                 | 775 ms: 1.04x slower                                       |
| pprint_pformat             | 1.55 sec                                               | 1.61 sec: 1.04x slower                                     |
| fannkuch                   | 405 ms                                                 | 422 ms: 1.04x slower                                       |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                      |
| 2to3                       | 264 ms                                                 | 276 ms: 1.04x slower                                       |
| scimark_monte_carlo        | 70.7 ms                                                | 74.0 ms: 1.05x slower                                      |
| dulwich_log                | 64.6 ms                                                | 68.2 ms: 1.06x slower                                      |
| xml_etree_generate         | 81.1 ms                                                | 85.7 ms: 1.06x slower                                      |
| scimark_fft                | 345 ms                                                 | 366 ms: 1.06x slower                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.35 ms: 1.06x slower                                      |
| nbody                      | 96.0 ms                                                | 102 ms: 1.07x slower                                       |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                      |
| float                      | 78.9 ms                                                | 86.1 ms: 1.09x slower                                      |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                      |
| regex_v8                   | 22.9 ms                                                | 25.1 ms: 1.10x slower                                      |
| regex_dna                  | 205 ms                                                 | 225 ms: 1.10x slower                                       |
| pickle_list                | 4.59 us                                                | 5.07 us: 1.11x slower                                      |
| hexiom                     | 6.89 ms                                                | 7.72 ms: 1.12x slower                                      |
| mako                       | 10.7 ms                                                | 12.4 ms: 1.16x slower                                      |
| pyflate                    | 434 ms                                                 | 514 ms: 1.18x slower                                       |
| python_startup             | 8.56 ms                                                | 10.3 ms: 1.20x slower                                      |
| spectral_norm              | 108 ms                                                 | 132 ms: 1.22x slower                                       |
| coverage                   | 78.8 ms                                                | 95.8 ms: 1.22x slower                                      |
| telco                      | 6.86 ms                                                | 8.40 ms: 1.23x slower                                      |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                       |
| mypy2                      | 686 ms                                                 | 861 ms: 1.26x slower                                       |
| dask                       | 365 ms                                                 | 527 ms: 1.44x slower                                       |
| python_startup_no_site     | 6.01 ms                                                | 8.95 ms: 1.49x slower                                      |
| Geometric mean             | (ref)                                                  | 1.04x faster                                               |

Benchmark hidden because not significant (5): regex_compile, xml_etree_iterparse, bench_mp_pool, scimark_sor, bench_thread_pool
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 83.81% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x