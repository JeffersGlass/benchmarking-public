
# Results vs. 3.11.0

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: linux-x86_64
- commit hash: 7de4b37
- commit date: 2024-01-26
- overall geometric mean: 1.00x slower
- HPT reliability: 96.02%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 285 ms: 1.08x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                            |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| tornado_http   | 98.1 ms                                                | 98.8 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 579 ms: 1.10x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 460 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 739 ms: 1.03x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 92.9 ms: 1.18x slower                                                            |
| nbody          | 96.0 ms                                                | 125 ms: 1.30x slower                                                             |
| Geometric mean | (ref)                                                  | 1.14x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| regex_compile  | 141 ms                                                 | 152 ms: 1.08x slower                                                             |
| regex_dna      | 205 ms                                                 | 228 ms: 1.12x slower                                                             |
| regex_v8       | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                            |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.06x faster                                                             |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| unpickle_pure_python | 242 us                                                 | 236 us: 1.02x faster                                                             |
| pickle_dict          | 34.6 us                                                | 35.2 us: 1.02x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.04x slower                                                             |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| unpickle_list        | 5.21 us                                                | 5.52 us: 1.06x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 61.4 ms: 1.08x slower                                                            |
| unpickle             | 13.8 us                                                | 15.2 us: 1.10x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 89.7 ms: 1.11x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.56 sec: 1.11x slower                                                           |
| pickle_list          | 4.59 us                                                | 5.19 us: 1.13x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.9 ms: 1.31x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240126-linux-x86_64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-7de4b37 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 117 us: 4.43x faster                                                             |
| generators                 | 74.9 ms                                                | 30.0 ms: 2.49x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                             |
| richards_super             | 61.9 ms                                                | 54.7 ms: 1.13x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 579 ms: 1.10x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.5 us: 1.10x faster                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| unpack_sequence            | 43.5 ns                                                | 40.6 ns: 1.07x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 460 ms: 1.07x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.06x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 594 ms: 1.05x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.63 sec: 1.05x faster                                                           |
| gc_traversal               | 4.01 ms                                                | 3.82 ms: 1.05x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.10 us: 1.04x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| logging_silent             | 111 ns                                                 | 107 ns: 1.03x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                                             |
| raytrace                   | 309 ms                                                 | 299 ms: 1.03x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 739 ms: 1.03x faster                                                             |
| richards                   | 49.8 ms                                                | 48.4 ms: 1.03x faster                                                            |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.08 us: 1.02x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 236 us: 1.02x faster                                                             |
| sympy_str                  | 297 ms                                                 | 292 ms: 1.02x faster                                                             |
| deepcopy                   | 365 us                                                 | 359 us: 1.02x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                            |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                                             |
| sqlglot_normalize          | 113 ms                                                 | 113 ms: 1.01x slower                                                             |
| asyncio_websockets         | 550 ms                                                 | 554 ms: 1.01x slower                                                             |
| tornado_http               | 98.1 ms                                                | 98.8 ms: 1.01x slower                                                            |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                            |
| chaos                      | 71.9 ms                                                | 72.7 ms: 1.01x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 847 us: 1.01x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.2 us: 1.02x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 40.9 us: 1.02x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.04x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.66 ms: 1.04x slower                                                            |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.9 ms: 1.05x slower                                                            |
| go                         | 149 ms                                                 | 156 ms: 1.05x slower                                                             |
| unpickle_list              | 5.21 us                                                | 5.52 us: 1.06x slower                                                            |
| meteor_contest             | 109 ms                                                 | 115 ms: 1.06x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.1 ms: 1.07x slower                                                            |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                                             |
| nqueens                    | 87.9 ms                                                | 94.1 ms: 1.07x slower                                                            |
| regex_compile              | 141 ms                                                 | 152 ms: 1.08x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 61.4 ms: 1.08x slower                                                            |
| 2to3                       | 264 ms                                                 | 285 ms: 1.08x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 814 ms: 1.09x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.70 sec: 1.09x slower                                                           |
| unpickle                   | 13.8 us                                                | 15.2 us: 1.10x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.39 ms: 1.10x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 89.7 ms: 1.11x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 84.9 ms: 1.11x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.56 sec: 1.11x slower                                                           |
| fannkuch                   | 405 ms                                                 | 451 ms: 1.11x slower                                                             |
| scimark_monte_carlo        | 70.7 ms                                                | 79.0 ms: 1.12x slower                                                            |
| regex_dna                  | 205 ms                                                 | 228 ms: 1.12x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 25.9 ms: 1.13x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.19 us: 1.13x slower                                                            |
| float                      | 78.9 ms                                                | 92.9 ms: 1.18x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.65 ms: 1.18x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.98 ms: 1.19x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| coverage                   | 78.8 ms                                                | 95.0 ms: 1.21x slower                                                            |
| async_generators           | 374 ms                                                 | 460 ms: 1.23x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.49 ms: 1.23x slower                                                            |
| telco                      | 6.86 ms                                                | 8.56 ms: 1.25x slower                                                            |
| scimark_fft                | 345 ms                                                 | 432 ms: 1.25x slower                                                             |
| pyflate                    | 434 ms                                                 | 546 ms: 1.26x slower                                                             |
| mypy2                      | 686 ms                                                 | 868 ms: 1.27x slower                                                             |
| nbody                      | 96.0 ms                                                | 125 ms: 1.30x slower                                                             |
| mako                       | 10.7 ms                                                | 13.9 ms: 1.31x slower                                                            |
| spectral_norm              | 108 ms                                                 | 143 ms: 1.33x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.82 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.00x slower                                                                     |

Benchmark hidden because not significant (5): json, bench_mp_pool, logging_format, sympy_expand, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 96.02% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x