
# Results vs. 3.11.0

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.07x faster
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.00x faster                                                             |
| chameleon      | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                            |
| docutils       | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                           |
| tornado_http   | 98.1 ms                                                | 93.8 ms: 1.05x faster                                                            |
| Geometric mean | (ref)                                                  | 1.01x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.12x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                           |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.8 ms: 1.08x faster                                                            |
| pidigits       | 194 ms                                                 | 195 ms: 1.00x slower                                                             |
| float          | 78.9 ms                                                | 80.1 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.10x faster                                                             |
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| regex_dna      | 205 ms                                                 | 219 ms: 1.07x slower                                                             |
| regex_v8       | 22.9 ms                                                | 26.0 ms: 1.14x slower                                                            |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.24x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 214 us: 1.13x faster                                                             |
| tomli_loads          | 2.30 sec                                               | 2.12 sec: 1.09x faster                                                           |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.11 us: 1.02x faster                                                            |
| json_loads           | 29.2 us                                                | 28.7 us: 1.02x faster                                                            |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                                            |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 86.0 ms: 1.06x slower                                                            |
| pickle_list          | 4.59 us                                                | 4.89 us: 1.07x slower                                                            |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.74x faster                                                             |
| generators                 | 74.9 ms                                                | 29.2 ms: 2.56x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 481 ms: 1.82x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.75x faster                                                           |
| comprehensions             | 23.6 us                                                | 16.1 us: 1.47x faster                                                            |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.24x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                            |
| deltablue                  | 3.92 ms                                                | 3.20 ms: 1.22x faster                                                            |
| chaos                      | 71.9 ms                                                | 58.7 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 435 ms: 1.21x faster                                                             |
| raytrace                   | 309 ms                                                 | 261 ms: 1.18x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 556 ms: 1.15x faster                                                             |
| richards_super             | 61.9 ms                                                | 54.5 ms: 1.14x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 214 us: 1.13x faster                                                             |
| hexiom                     | 6.89 ms                                                | 6.09 ms: 1.13x faster                                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                            |
| logging_simple             | 6.22 us                                                | 5.57 us: 1.12x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 440 ms: 1.12x faster                                                             |
| logging_format             | 6.81 us                                                | 6.13 us: 1.11x faster                                                            |
| sympy_str                  | 297 ms                                                 | 268 ms: 1.11x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 19.3 ms: 1.11x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                           |
| nqueens                    | 87.9 ms                                                | 80.0 ms: 1.10x faster                                                            |
| regex_compile              | 141 ms                                                 | 129 ms: 1.10x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                           |
| tomli_loads                | 2.30 sec                                               | 2.12 sec: 1.09x faster                                                           |
| crypto_pyaes               | 76.7 ms                                                | 70.6 ms: 1.09x faster                                                            |
| go                         | 149 ms                                                 | 137 ms: 1.08x faster                                                             |
| nbody                      | 96.0 ms                                                | 88.8 ms: 1.08x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                             |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                                             |
| sqlglot_normalize          | 113 ms                                                 | 106 ms: 1.07x faster                                                             |
| sympy_expand               | 484 ms                                                 | 454 ms: 1.07x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.60 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 704 ms: 1.06x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 719 ms: 1.06x faster                                                             |
| deepcopy                   | 365 us                                                 | 346 us: 1.06x faster                                                             |
| gc_traversal               | 4.01 ms                                                | 3.81 ms: 1.05x faster                                                            |
| deepcopy_memo              | 40.2 us                                                | 38.4 us: 1.05x faster                                                            |
| richards                   | 49.8 ms                                                | 47.6 ms: 1.05x faster                                                            |
| tornado_http               | 98.1 ms                                                | 93.8 ms: 1.05x faster                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 68.0 ms: 1.04x faster                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.50 sec: 1.04x faster                                                           |
| sqlglot_optimize           | 55.3 ms                                                | 53.4 ms: 1.04x faster                                                            |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| docutils                   | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                           |
| fannkuch                   | 405 ms                                                 | 394 ms: 1.03x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.13 us: 1.03x faster                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                             |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                             |
| unpickle_list              | 5.21 us                                                | 5.11 us: 1.02x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.7 us: 1.02x faster                                                            |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                             |
| dask                       | 365 ms                                                 | 361 ms: 1.01x faster                                                             |
| pprint_safe_repr           | 747 ms                                                 | 739 ms: 1.01x faster                                                             |
| bench_thread_pool          | 834 us                                                 | 826 us: 1.01x faster                                                             |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                                            |
| 2to3                       | 264 ms                                                 | 263 ms: 1.00x faster                                                             |
| pidigits                   | 194 ms                                                 | 195 ms: 1.00x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 65.5 ms: 1.01x slower                                                            |
| float                      | 78.9 ms                                                | 80.1 ms: 1.01x slower                                                            |
| chameleon                  | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                            |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                            |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.04x slower                                                             |
| unpack_sequence            | 43.5 ns                                                | 45.2 ns: 1.04x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                            |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                                            |
| pyflate                    | 434 ms                                                 | 452 ms: 1.04x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 59.4 ms: 1.04x slower                                                            |
| scimark_fft                | 345 ms                                                 | 362 ms: 1.05x slower                                                             |
| scimark_sor                | 121 ms                                                 | 127 ms: 1.05x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 86.0 ms: 1.06x slower                                                            |
| pickle_list                | 4.59 us                                                | 4.89 us: 1.07x slower                                                            |
| regex_dna                  | 205 ms                                                 | 219 ms: 1.07x slower                                                             |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.88 us: 1.12x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 26.0 ms: 1.14x slower                                                            |
| async_generators           | 374 ms                                                 | 437 ms: 1.17x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                            |
| coverage                   | 78.8 ms                                                | 94.7 ms: 1.20x slower                                                            |
| mypy2                      | 686 ms                                                 | 838 ms: 1.22x slower                                                             |
| telco                      | 6.86 ms                                                | 8.41 ms: 1.23x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.73 ms: 1.45x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                                     |

Benchmark hidden because not significant (4): scimark_sparse_mat_mult, bench_mp_pool, asyncio_websockets, json
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.98x