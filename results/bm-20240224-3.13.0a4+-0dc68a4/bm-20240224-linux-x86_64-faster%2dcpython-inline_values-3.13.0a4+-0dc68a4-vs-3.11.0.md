# Results vs. 3.11.0

- fork: faster-cpython
- ref: inline_values
- machine: linux-x86_64
- commit hash: 0dc68a4
- commit date: 2024-02-24
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 262 ms: 1.01x faster                                                      |
| docutils       | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                    |
| tornado_http   | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                     |
| Geometric mean | (ref)                                                  | 1.02x faster                                                              |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 575 ms: 1.11x faster                                                      |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                    |
| async_tree_none            | 528 ms                                                 | 477 ms: 1.11x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                      |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 90.6 ms: 1.06x faster                                                     |
| float          | 78.9 ms                                                | 79.5 ms: 1.01x slower                                                     |
| pidigits       | 194 ms                                                 | 203 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                  | 1.00x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.08x faster                                                      |
| regex_effbot   | 3.51 ms                                                | 3.55 ms: 1.01x slower                                                     |
| regex_dna      | 205 ms                                                 | 215 ms: 1.05x slower                                                      |
| regex_v8       | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                     |
| Geometric mean | (ref)                                                  | 1.02x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                     |
| unpickle_pure_python | 242 us                                                 | 212 us: 1.14x faster                                                      |
| unpickle_list        | 5.21 us                                                | 4.74 us: 1.10x faster                                                     |
| pickle_pure_python   | 320 us                                                 | 294 us: 1.09x faster                                                      |
| tomli_loads          | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                    |
| json_loads           | 29.2 us                                                | 27.6 us: 1.06x faster                                                     |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                      |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                      |
| pickle_dict          | 34.6 us                                                | 35.3 us: 1.02x slower                                                     |
| xml_etree_process    | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                     |
| xml_etree_generate   | 81.1 ms                                                | 85.3 ms: 1.05x slower                                                     |
| pickle               | 11.0 us                                                | 11.9 us: 1.08x slower                                                     |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                     |
| pickle_list          | 4.59 us                                                | 5.30 us: 1.16x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.20x slower                                                     |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240224-linux-x86_64-faster%2dcpython-inline_values-3.13.0a4+-0dc68a4 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.73x faster                                                      |
| generators                 | 74.9 ms                                                | 28.6 ms: 2.61x faster                                                     |
| asyncio_tcp                | 875 ms                                                 | 489 ms: 1.79x faster                                                      |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                    |
| comprehensions             | 23.6 us                                                | 16.0 us: 1.48x faster                                                     |
| json_dumps                 | 13.3 ms                                                | 10.3 ms: 1.29x faster                                                     |
| coroutines                 | 27.0 ms                                                | 21.5 ms: 1.26x faster                                                     |
| deltablue                  | 3.92 ms                                                | 3.17 ms: 1.24x faster                                                     |
| chaos                      | 71.9 ms                                                | 59.2 ms: 1.21x faster                                                     |
| raytrace                   | 309 ms                                                 | 256 ms: 1.21x faster                                                      |
| richards_super             | 61.9 ms                                                | 52.6 ms: 1.18x faster                                                     |
| sqlglot_parse              | 1.43 ms                                                | 1.23 ms: 1.17x faster                                                     |
| unpickle_pure_python       | 242 us                                                 | 212 us: 1.14x faster                                                      |
| sympy_sum                  | 169 ms                                                 | 148 ms: 1.14x faster                                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.55 ms: 1.13x faster                                                     |
| hexiom                     | 6.89 ms                                                | 6.16 ms: 1.12x faster                                                     |
| logging_silent             | 111 ns                                                 | 99.7 ns: 1.11x faster                                                     |
| sympy_str                  | 297 ms                                                 | 267 ms: 1.11x faster                                                      |
| logging_format             | 6.81 us                                                | 6.12 us: 1.11x faster                                                     |
| async_tree_none_tg         | 491 ms                                                 | 441 ms: 1.11x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 575 ms: 1.11x faster                                                      |
| mdp                        | 2.77 sec                                               | 2.50 sec: 1.11x faster                                                    |
| async_tree_io              | 1.29 sec                                               | 1.16 sec: 1.11x faster                                                    |
| async_tree_none            | 528 ms                                                 | 477 ms: 1.11x faster                                                      |
| logging_simple             | 6.22 us                                                | 5.63 us: 1.10x faster                                                     |
| unpickle_list              | 5.21 us                                                | 4.74 us: 1.10x faster                                                     |
| async_tree_memoization_tg  | 626 ms                                                 | 574 ms: 1.09x faster                                                      |
| nqueens                    | 87.9 ms                                                | 80.5 ms: 1.09x faster                                                     |
| sympy_integrate            | 21.5 ms                                                | 19.7 ms: 1.09x faster                                                     |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                    |
| pickle_pure_python         | 320 us                                                 | 294 us: 1.09x faster                                                      |
| regex_compile              | 141 ms                                                 | 130 ms: 1.08x faster                                                      |
| go                         | 149 ms                                                 | 137 ms: 1.08x faster                                                      |
| crypto_pyaes               | 76.7 ms                                                | 71.2 ms: 1.08x faster                                                     |
| gc_traversal               | 4.01 ms                                                | 3.73 ms: 1.08x faster                                                     |
| sympy_expand               | 484 ms                                                 | 452 ms: 1.07x faster                                                      |
| tomli_loads                | 2.30 sec                                               | 2.15 sec: 1.07x faster                                                    |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.71 ms: 1.07x faster                                                     |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.07x faster                                                      |
| deepcopy                   | 365 us                                                 | 343 us: 1.06x faster                                                      |
| scimark_monte_carlo        | 70.7 ms                                                | 66.7 ms: 1.06x faster                                                     |
| nbody                      | 96.0 ms                                                | 90.6 ms: 1.06x faster                                                     |
| json_loads                 | 29.2 us                                                | 27.6 us: 1.06x faster                                                     |
| fannkuch                   | 405 ms                                                 | 384 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 721 ms: 1.06x faster                                                      |
| deepcopy_memo              | 40.2 us                                                | 38.1 us: 1.05x faster                                                     |
| richards                   | 49.8 ms                                                | 47.3 ms: 1.05x faster                                                     |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.05x faster                                                     |
| pprint_pformat             | 1.55 sec                                               | 1.48 sec: 1.05x faster                                                    |
| sqlglot_optimize           | 55.3 ms                                                | 52.9 ms: 1.05x faster                                                     |
| meteor_contest             | 109 ms                                                 | 104 ms: 1.04x faster                                                      |
| tornado_http               | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                     |
| scimark_lu                 | 116 ms                                                 | 112 ms: 1.04x faster                                                      |
| pprint_safe_repr           | 747 ms                                                 | 723 ms: 1.03x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                      |
| json                       | 5.24 ms                                                | 5.08 ms: 1.03x faster                                                     |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                      |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                      |
| docutils                   | 2.66 sec                                               | 2.60 sec: 1.02x faster                                                    |
| scimark_sor                | 121 ms                                                 | 119 ms: 1.02x faster                                                      |
| bench_thread_pool          | 834 us                                                 | 820 us: 1.02x faster                                                      |
| spectral_norm              | 108 ms                                                 | 107 ms: 1.01x faster                                                      |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                     |
| 2to3                       | 264 ms                                                 | 262 ms: 1.01x faster                                                      |
| float                      | 78.9 ms                                                | 79.5 ms: 1.01x slower                                                     |
| regex_effbot               | 3.51 ms                                                | 3.55 ms: 1.01x slower                                                     |
| pickle_dict                | 34.6 us                                                | 35.3 us: 1.02x slower                                                     |
| xml_etree_process          | 56.9 ms                                                | 58.2 ms: 1.02x slower                                                     |
| dulwich_log                | 64.6 ms                                                | 66.5 ms: 1.03x slower                                                     |
| pyflate                    | 434 ms                                                 | 449 ms: 1.04x slower                                                      |
| scimark_fft                | 345 ms                                                 | 361 ms: 1.04x slower                                                      |
| pidigits                   | 194 ms                                                 | 203 ms: 1.05x slower                                                      |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                     |
| regex_dna                  | 205 ms                                                 | 215 ms: 1.05x slower                                                      |
| xml_etree_generate         | 81.1 ms                                                | 85.3 ms: 1.05x slower                                                     |
| pickle                     | 11.0 us                                                | 11.9 us: 1.08x slower                                                     |
| create_gc_cycles           | 1.43 ms                                                | 1.56 ms: 1.09x slower                                                     |
| regex_v8                   | 22.9 ms                                                | 25.0 ms: 1.09x slower                                                     |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                                     |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                     |
| pickle_list                | 4.59 us                                                | 5.30 us: 1.16x slower                                                     |
| unpack_sequence            | 43.5 ns                                                | 50.5 ns: 1.16x slower                                                     |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.20x slower                                                     |
| async_generators           | 374 ms                                                 | 448 ms: 1.20x slower                                                      |
| telco                      | 6.86 ms                                                | 8.42 ms: 1.23x slower                                                     |
| mypy2                      | 686 ms                                                 | 844 ms: 1.23x slower                                                      |
| coverage                   | 78.8 ms                                                | 97.1 ms: 1.23x slower                                                     |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                     |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                              |

Benchmark hidden because not significant (4): pycparser, bench_mp_pool, asyncio_websockets, chameleon
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: 1.00x