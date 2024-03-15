# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: f58f8ce
- commit date: 2024-02-29
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 264 ms: 1.00x faster                                   |
| chameleon      | 6.70 ms                                                | 6.91 ms: 1.03x slower                                  |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| tornado_http   | 98.1 ms                                                | 94.8 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 432 ms: 1.22x faster                                   |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.0 ms: 1.09x faster                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| float          | 78.9 ms                                                | 80.4 ms: 1.02x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 132 ms: 1.07x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.56 ms: 1.02x slower                                  |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                   |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                  |
| unpickle_pure_python | 242 us                                                 | 214 us: 1.13x faster                                   |
| pickle_pure_python   | 320 us                                                 | 295 us: 1.09x faster                                   |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                 |
| json_loads           | 29.2 us                                                | 27.6 us: 1.06x faster                                  |
| unpickle_list        | 5.21 us                                                | 4.95 us: 1.05x faster                                  |
| pickle_dict          | 34.6 us                                                | 33.1 us: 1.05x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| xml_etree_process    | 56.9 ms                                                | 58.3 ms: 1.02x slower                                  |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                  |
| unpickle             | 13.8 us                                                | 14.5 us: 1.04x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.0 ms: 1.05x slower                                  |
| pickle_list          | 4.59 us                                                | 4.91 us: 1.07x slower                                  |
| Geometric mean       | (ref)                                                  | 1.04x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 8.75 ms: 1.46x slower                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|-----------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.4 ms: 1.07x slower                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-python-main-3.13.0a4+-f58f8ce |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.71x faster                                   |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.56x faster                                  |
| asyncio_tcp                | 875 ms                                                 | 483 ms: 1.81x faster                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.74x faster                                 |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.47x faster                                  |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.16 ms: 1.24x faster                                  |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                  |
| async_tree_none            | 528 ms                                                 | 432 ms: 1.22x faster                                   |
| chaos                      | 71.9 ms                                                | 59.8 ms: 1.20x faster                                  |
| raytrace                   | 309 ms                                                 | 263 ms: 1.17x faster                                   |
| richards_super             | 61.9 ms                                                | 52.9 ms: 1.17x faster                                  |
| hexiom                     | 6.89 ms                                                | 5.97 ms: 1.15x faster                                  |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.14x faster                                  |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                   |
| unpickle_pure_python       | 242 us                                                 | 214 us: 1.13x faster                                   |
| nqueens                    | 87.9 ms                                                | 78.9 ms: 1.11x faster                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.57 ms: 1.11x faster                                  |
| sympy_str                  | 297 ms                                                 | 268 ms: 1.11x faster                                   |
| logging_simple             | 6.22 us                                                | 5.60 us: 1.11x faster                                  |
| logging_format             | 6.81 us                                                | 6.14 us: 1.11x faster                                  |
| async_tree_none_tg         | 491 ms                                                 | 445 ms: 1.10x faster                                   |
| crypto_pyaes               | 76.7 ms                                                | 69.6 ms: 1.10x faster                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 570 ms: 1.10x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| sympy_integrate            | 21.5 ms                                                | 19.6 ms: 1.10x faster                                  |
| nbody                      | 96.0 ms                                                | 88.0 ms: 1.09x faster                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                 |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                   |
| pickle_pure_python         | 320 us                                                 | 295 us: 1.09x faster                                   |
| deepcopy_memo              | 40.2 us                                                | 37.2 us: 1.08x faster                                  |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                 |
| go                         | 149 ms                                                 | 138 ms: 1.07x faster                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.69 ms: 1.07x faster                                  |
| regex_compile              | 141 ms                                                 | 132 ms: 1.07x faster                                   |
| gc_traversal               | 4.01 ms                                                | 3.75 ms: 1.07x faster                                  |
| sqlglot_normalize          | 113 ms                                                 | 105 ms: 1.07x faster                                   |
| sympy_expand               | 484 ms                                                 | 454 ms: 1.07x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                   |
| deepcopy                   | 365 us                                                 | 344 us: 1.06x faster                                   |
| json_loads                 | 29.2 us                                                | 27.6 us: 1.06x faster                                  |
| scimark_lu                 | 116 ms                                                 | 110 ms: 1.06x faster                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 66.9 ms: 1.06x faster                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                  |
| unpickle_list              | 5.21 us                                                | 4.95 us: 1.05x faster                                  |
| richards                   | 49.8 ms                                                | 47.4 ms: 1.05x faster                                  |
| pickle_dict                | 34.6 us                                                | 33.1 us: 1.05x faster                                  |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.05x faster                                 |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                   |
| fannkuch                   | 405 ms                                                 | 388 ms: 1.04x faster                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| json                       | 5.24 ms                                                | 5.05 ms: 1.04x faster                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.4 ms: 1.04x faster                                  |
| mdp                        | 2.77 sec                                               | 2.68 sec: 1.04x faster                                 |
| tornado_http               | 98.1 ms                                                | 94.8 ms: 1.03x faster                                  |
| pprint_safe_repr           | 747 ms                                                 | 724 ms: 1.03x faster                                   |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| pathlib                    | 18.5 ms                                                | 18.0 ms: 1.03x faster                                  |
| bench_thread_pool          | 834 us                                                 | 816 us: 1.02x faster                                   |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                   |
| 2to3                       | 264 ms                                                 | 264 ms: 1.00x faster                                   |
| spectral_norm              | 108 ms                                                 | 110 ms: 1.01x slower                                   |
| dulwich_log                | 64.6 ms                                                | 65.6 ms: 1.02x slower                                  |
| regex_effbot               | 3.51 ms                                                | 3.56 ms: 1.02x slower                                  |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                 |
| asyncio_websockets         | 550 ms                                                 | 560 ms: 1.02x slower                                   |
| float                      | 78.9 ms                                                | 80.4 ms: 1.02x slower                                  |
| scimark_sor                | 121 ms                                                 | 124 ms: 1.02x slower                                   |
| xml_etree_process          | 56.9 ms                                                | 58.3 ms: 1.02x slower                                  |
| chameleon                  | 6.70 ms                                                | 6.91 ms: 1.03x slower                                  |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.04x slower                                  |
| scimark_fft                | 345 ms                                                 | 360 ms: 1.04x slower                                   |
| unpickle                   | 13.8 us                                                | 14.5 us: 1.04x slower                                  |
| xml_etree_generate         | 81.1 ms                                                | 85.0 ms: 1.05x slower                                  |
| regex_dna                  | 205 ms                                                 | 216 ms: 1.06x slower                                   |
| pickle_list                | 4.59 us                                                | 4.91 us: 1.07x slower                                  |
| mako                       | 10.7 ms                                                | 11.4 ms: 1.07x slower                                  |
| pyflate                    | 434 ms                                                 | 466 ms: 1.07x slower                                   |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                  |
| unpack_sequence            | 43.5 ns                                                | 47.4 ns: 1.09x slower                                  |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                  |
| coverage                   | 78.8 ms                                                | 93.0 ms: 1.18x slower                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                  |
| telco                      | 6.86 ms                                                | 8.20 ms: 1.20x slower                                  |
| async_generators           | 374 ms                                                 | 448 ms: 1.20x slower                                   |
| mypy2                      | 686 ms                                                 | 845 ms: 1.23x slower                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.75 ms: 1.46x slower                                  |
| Geometric mean             | (ref)                                                  | 1.08x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 0.99x