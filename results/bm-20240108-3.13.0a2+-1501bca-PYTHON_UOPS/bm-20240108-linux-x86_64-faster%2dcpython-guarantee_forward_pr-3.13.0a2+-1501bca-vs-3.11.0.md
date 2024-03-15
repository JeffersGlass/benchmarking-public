
# Results vs. 3.11.0

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.00x faster
- HPT reliability: 97.27%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 283 ms: 1.07x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 97.3 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| float          | 78.9 ms                                                | 92.7 ms: 1.17x slower                                                            |
| nbody          | 96.0 ms                                                | 115 ms: 1.20x slower                                                             |
| Geometric mean | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.57 ms: 1.02x slower                                                            |
| regex_compile  | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                            |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| unpickle_list        | 5.21 us                                                | 4.92 us: 1.06x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 303 us: 1.06x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| json_loads           | 29.2 us                                                | 28.5 us: 1.03x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 237 us: 1.02x faster                                                             |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.01x slower                                                             |
| tomli_loads          | 2.30 sec                                               | 2.36 sec: 1.03x slower                                                           |
| pickle_dict          | 34.6 us                                                | 35.7 us: 1.03x slower                                                            |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                                            |
| pickle_list          | 4.59 us                                                | 4.86 us: 1.06x slower                                                            |
| unpickle             | 13.8 us                                                | 14.9 us: 1.07x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 61.3 ms: 1.08x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 90.3 ms: 1.11x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.00x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.0 ms: 1.17x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.68 ms: 1.44x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.8 ms: 1.30x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 116 us: 4.47x faster                                                             |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.77x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                            |
| async_tree_none            | 528 ms                                                 | 448 ms: 1.18x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.2 us: 1.11x faster                                                            |
| richards_super             | 61.9 ms                                                | 55.6 ms: 1.11x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 39.7 ns: 1.09x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 453 ms: 1.08x faster                                                             |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.33 ms: 1.08x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 585 ms: 1.07x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                           |
| unpickle_list              | 5.21 us                                                | 4.92 us: 1.06x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 303 us: 1.06x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.05x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                             |
| mdp                        | 2.77 sec                                               | 2.69 sec: 1.03x faster                                                           |
| json_loads                 | 29.2 us                                                | 28.5 us: 1.03x faster                                                            |
| deepcopy                   | 365 us                                                 | 356 us: 1.02x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.08 us: 1.02x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 237 us: 1.02x faster                                                             |
| raytrace                   | 309 ms                                                 | 302 ms: 1.02x faster                                                             |
| sympy_str                  | 297 ms                                                 | 291 ms: 1.02x faster                                                             |
| deepcopy_reduce            | 3.22 us                                                | 3.16 us: 1.02x faster                                                            |
| richards                   | 49.8 ms                                                | 49.1 ms: 1.01x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                            |
| tornado_http               | 98.1 ms                                                | 97.3 ms: 1.01x faster                                                            |
| scimark_lu                 | 116 ms                                                 | 117 ms: 1.01x slower                                                             |
| sympy_expand               | 484 ms                                                 | 490 ms: 1.01x slower                                                             |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.01x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 40.8 us: 1.01x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 848 us: 1.02x slower                                                             |
| sqlglot_normalize          | 113 ms                                                 | 114 ms: 1.02x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                                           |
| chaos                      | 71.9 ms                                                | 73.2 ms: 1.02x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.57 ms: 1.02x slower                                                            |
| pathlib                    | 18.5 ms                                                | 18.9 ms: 1.02x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.03x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.36 sec: 1.03x slower                                                           |
| pickle_dict                | 34.6 us                                                | 35.7 us: 1.03x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 57.6 ms: 1.04x slower                                                            |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.24 sec: 1.05x slower                                                           |
| meteor_contest             | 109 ms                                                 | 115 ms: 1.05x slower                                                             |
| pickle_list                | 4.59 us                                                | 4.86 us: 1.06x slower                                                            |
| go                         | 149 ms                                                 | 158 ms: 1.06x slower                                                             |
| regex_compile              | 141 ms                                                 | 151 ms: 1.07x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.2 ms: 1.07x slower                                                            |
| gc_traversal               | 4.01 ms                                                | 4.29 ms: 1.07x slower                                                            |
| 2to3                       | 264 ms                                                 | 283 ms: 1.07x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                            |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.07x slower                                                            |
| nqueens                    | 87.9 ms                                                | 94.5 ms: 1.08x slower                                                            |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 61.3 ms: 1.08x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 83.2 ms: 1.08x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.70 sec: 1.09x slower                                                           |
| chameleon                  | 6.70 ms                                                | 7.32 ms: 1.09x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 818 ms: 1.09x slower                                                             |
| scimark_sor                | 121 ms                                                 | 133 ms: 1.10x slower                                                             |
| fannkuch                   | 405 ms                                                 | 444 ms: 1.10x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 90.3 ms: 1.11x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.90 us: 1.13x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 81.8 ms: 1.16x slower                                                            |
| pyflate                    | 434 ms                                                 | 506 ms: 1.17x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.0 ms: 1.17x slower                                                            |
| float                      | 78.9 ms                                                | 92.7 ms: 1.17x slower                                                            |
| nbody                      | 96.0 ms                                                | 115 ms: 1.20x slower                                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.03 ms: 1.20x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.71 ms: 1.20x slower                                                            |
| coverage                   | 78.8 ms                                                | 94.9 ms: 1.21x slower                                                            |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.42 ms: 1.22x slower                                                            |
| mypy2                      | 686 ms                                                 | 861 ms: 1.26x slower                                                             |
| telco                      | 6.86 ms                                                | 8.75 ms: 1.28x slower                                                            |
| mako                       | 10.7 ms                                                | 13.8 ms: 1.30x slower                                                            |
| scimark_fft                | 345 ms                                                 | 449 ms: 1.30x slower                                                             |
| spectral_norm              | 108 ms                                                 | 146 ms: 1.35x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.68 ms: 1.44x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.00x faster                                                                     |

Benchmark hidden because not significant (5): bench_mp_pool, asyncio_websockets, logging_format, json, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 97.27% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.98x