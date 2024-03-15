
# Results vs. 3.11.0

- fork: faster-cpython
- ref: split_end_for
- machine: linux-x86_64
- commit hash: ed98265
- commit date: 2024-01-17
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                    |
| tornado_http   | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                     |
| Geometric mean | (ref)                                                  | 1.01x faster                                                              |

Benchmark hidden because not significant (2): 2to3, chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.14x faster                                                      |
| async_tree_none_tg         | 491 ms                                                 | 439 ms: 1.12x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                      |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                    |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                    |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                      |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 86.6 ms: 1.11x faster                                                     |
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                      |
| Geometric mean | (ref)                                                  | 1.05x faster                                                              |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.09x faster                                                      |
| regex_effbot   | 3.51 ms                                                | 3.71 ms: 1.06x slower                                                     |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                      |
| regex_v8       | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                     |
| Geometric mean | (ref)                                                  | 1.04x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                     |
| unpickle_pure_python | 242 us                                                 | 211 us: 1.14x faster                                                      |
| tomli_loads          | 2.30 sec                                               | 2.11 sec: 1.09x faster                                                    |
| pickle_pure_python   | 320 us                                                 | 297 us: 1.08x faster                                                      |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                      |
| json_loads           | 29.2 us                                                | 28.1 us: 1.04x faster                                                     |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                      |
| unpickle_list        | 5.21 us                                                | 5.16 us: 1.01x faster                                                     |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                     |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                     |
| xml_etree_generate   | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                     |
| pickle               | 11.0 us                                                | 11.8 us: 1.08x slower                                                     |
| pickle_list          | 4.59 us                                                | 5.25 us: 1.15x slower                                                     |
| unpickle             | 13.8 us                                                | 15.9 us: 1.15x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                     |
| python_startup_no_site | 6.01 ms                                                | 8.69 ms: 1.45x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240117-linux-x86_64-faster%2dcpython-split_end_for-3.13.0a3+-ed98265 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.72x faster                                                      |
| generators                 | 74.9 ms                                                | 29.5 ms: 2.54x faster                                                     |
| asyncio_tcp                | 875 ms                                                 | 482 ms: 1.82x faster                                                      |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                    |
| comprehensions             | 23.6 us                                                | 16.2 us: 1.45x faster                                                     |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.28x faster                                                     |
| chaos                      | 71.9 ms                                                | 58.8 ms: 1.22x faster                                                     |
| deltablue                  | 3.92 ms                                                | 3.22 ms: 1.22x faster                                                     |
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                      |
| raytrace                   | 309 ms                                                 | 258 ms: 1.20x faster                                                      |
| coroutines                 | 27.0 ms                                                | 22.6 ms: 1.20x faster                                                     |
| gc_traversal               | 4.01 ms                                                | 3.47 ms: 1.15x faster                                                     |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                     |
| hexiom                     | 6.89 ms                                                | 5.97 ms: 1.15x faster                                                     |
| richards_super             | 61.9 ms                                                | 53.8 ms: 1.15x faster                                                     |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                      |
| unpickle_pure_python       | 242 us                                                 | 211 us: 1.14x faster                                                      |
| async_tree_memoization     | 639 ms                                                 | 563 ms: 1.14x faster                                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                     |
| async_tree_none_tg         | 491 ms                                                 | 439 ms: 1.12x faster                                                      |
| nbody                      | 96.0 ms                                                | 86.6 ms: 1.11x faster                                                     |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                                      |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                     |
| logging_simple             | 6.22 us                                                | 5.65 us: 1.10x faster                                                     |
| logging_format             | 6.81 us                                                | 6.20 us: 1.10x faster                                                     |
| mdp                        | 2.77 sec                                               | 2.53 sec: 1.10x faster                                                    |
| regex_compile              | 141 ms                                                 | 129 ms: 1.09x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                      |
| tomli_loads                | 2.30 sec                                               | 2.11 sec: 1.09x faster                                                    |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                    |
| nqueens                    | 87.9 ms                                                | 80.8 ms: 1.09x faster                                                     |
| go                         | 149 ms                                                 | 137 ms: 1.09x faster                                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                    |
| sympy_str                  | 297 ms                                                 | 275 ms: 1.08x faster                                                      |
| pickle_pure_python         | 320 us                                                 | 297 us: 1.08x faster                                                      |
| crypto_pyaes               | 76.7 ms                                                | 71.7 ms: 1.07x faster                                                     |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.71 ms: 1.07x faster                                                     |
| scimark_monte_carlo        | 70.7 ms                                                | 66.2 ms: 1.07x faster                                                     |
| deepcopy_memo              | 40.2 us                                                | 37.9 us: 1.06x faster                                                     |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                      |
| deepcopy                   | 365 us                                                 | 345 us: 1.06x faster                                                      |
| pprint_pformat             | 1.55 sec                                               | 1.47 sec: 1.06x faster                                                    |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 708 ms: 1.06x faster                                                      |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                                      |
| deepcopy_reduce            | 3.22 us                                                | 3.06 us: 1.05x faster                                                     |
| scimark_lu                 | 116 ms                                                 | 111 ms: 1.05x faster                                                      |
| pprint_safe_repr           | 747 ms                                                 | 717 ms: 1.04x faster                                                      |
| tornado_http               | 98.1 ms                                                | 94.1 ms: 1.04x faster                                                     |
| sympy_expand               | 484 ms                                                 | 465 ms: 1.04x faster                                                      |
| richards                   | 49.8 ms                                                | 47.8 ms: 1.04x faster                                                     |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                      |
| json_loads                 | 29.2 us                                                | 28.1 us: 1.04x faster                                                     |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                      |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                      |
| sqlglot_optimize           | 55.3 ms                                                | 53.8 ms: 1.03x faster                                                     |
| meteor_contest             | 109 ms                                                 | 106 ms: 1.03x faster                                                      |
| json                       | 5.24 ms                                                | 5.12 ms: 1.02x faster                                                     |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                                     |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                    |
| bench_thread_pool          | 834 us                                                 | 823 us: 1.01x faster                                                      |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                                      |
| unpickle_list              | 5.21 us                                                | 5.16 us: 1.01x faster                                                     |
| fannkuch                   | 405 ms                                                 | 403 ms: 1.01x faster                                                      |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                     |
| unpack_sequence            | 43.5 ns                                                | 44.3 ns: 1.02x slower                                                     |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                     |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                                     |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.03x slower                                                      |
| pyflate                    | 434 ms                                                 | 448 ms: 1.03x slower                                                      |
| scimark_fft                | 345 ms                                                 | 362 ms: 1.05x slower                                                      |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                     |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.06x slower                                                      |
| regex_effbot               | 3.51 ms                                                | 3.71 ms: 1.06x slower                                                     |
| xml_etree_generate         | 81.1 ms                                                | 85.7 ms: 1.06x slower                                                     |
| pickle                     | 11.0 us                                                | 11.8 us: 1.08x slower                                                     |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                      |
| sqlite_synth               | 2.57 us                                                | 2.80 us: 1.09x slower                                                     |
| regex_v8                   | 22.9 ms                                                | 25.5 ms: 1.11x slower                                                     |
| pickle_list                | 4.59 us                                                | 5.25 us: 1.15x slower                                                     |
| unpickle                   | 13.8 us                                                | 15.9 us: 1.15x slower                                                     |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                     |
| async_generators           | 374 ms                                                 | 443 ms: 1.19x slower                                                      |
| coverage                   | 78.8 ms                                                | 95.5 ms: 1.21x slower                                                     |
| mypy2                      | 686 ms                                                 | 840 ms: 1.23x slower                                                      |
| telco                      | 6.86 ms                                                | 8.43 ms: 1.23x slower                                                     |
| python_startup_no_site     | 6.01 ms                                                | 8.69 ms: 1.45x slower                                                     |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                              |

Benchmark hidden because not significant (7): 2to3, bench_mp_pool, asyncio_websockets, dulwich_log, float, chameleon, pycparser
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x