
# Results vs. 3.11.0

- fork: faster-cpython
- ref: abstract_interpreter
- machine: linux-x86_64
- commit hash: 939c26f
- commit date: 2024-02-01
- overall geometric mean: 1.01x slower
- HPT reliability: 98.98%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 286 ms: 1.08x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.27 ms: 1.09x slower                                                            |
| docutils       | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                           |
| tornado_http   | 98.1 ms                                                | 99.3 ms: 1.01x slower                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                                             |
| nbody          | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| float          | 78.9 ms                                                | 100 ms: 1.27x slower                                                             |
| Geometric mean | (ref)                                                  | 1.15x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                            |
| regex_dna      | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| regex_compile  | 141 ms                                                 | 154 ms: 1.09x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 298 us: 1.07x faster                                                             |
| unpickle_list        | 5.21 us                                                | 5.01 us: 1.04x faster                                                            |
| pickle_dict          | 34.6 us                                                | 33.2 us: 1.04x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| json_loads           | 29.2 us                                                | 28.5 us: 1.02x faster                                                            |
| unpickle_pure_python | 242 us                                                 | 237 us: 1.02x faster                                                             |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 114 ms: 1.06x slower                                                             |
| pickle_list          | 4.59 us                                                | 4.93 us: 1.07x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 61.7 ms: 1.08x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 90.8 ms: 1.12x slower                                                            |
| unpickle             | 13.8 us                                                | 15.9 us: 1.15x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.70 sec: 1.17x slower                                                           |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.81 ms: 1.47x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 14.7 ms: 1.38x slower                                                            |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240201-linux-x86_64-faster%2dcpython-abstract_interpreter-3.13.0a3+-939c26f |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.50x faster                                                             |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 490 ms: 1.79x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.79 sec: 1.73x faster                                                           |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 22.4 ms: 1.21x faster                                                            |
| async_tree_none            | 528 ms                                                 | 452 ms: 1.17x faster                                                             |
| richards_super             | 61.9 ms                                                | 55.6 ms: 1.11x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 578 ms: 1.11x faster                                                             |
| unpack_sequence            | 43.5 ns                                                | 39.6 ns: 1.10x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 298 us: 1.07x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                             |
| sqlglot_parse              | 1.43 ms                                                | 1.34 ms: 1.07x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                                            |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| comprehensions             | 23.6 us                                                | 22.3 us: 1.06x faster                                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.67 ms: 1.05x faster                                                            |
| async_tree_memoization_tg  | 626 ms                                                 | 597 ms: 1.05x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                             |
| unpickle_list              | 5.21 us                                                | 5.01 us: 1.04x faster                                                            |
| pickle_dict                | 34.6 us                                                | 33.2 us: 1.04x faster                                                            |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 721 ms: 1.04x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                             |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                                             |
| pidigits                   | 194 ms                                                 | 190 ms: 1.02x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.5 us: 1.02x faster                                                            |
| unpickle_pure_python       | 242 us                                                 | 237 us: 1.02x faster                                                             |
| logging_simple             | 6.22 us                                                | 6.10 us: 1.02x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.17 us: 1.01x faster                                                            |
| logging_format             | 6.81 us                                                | 6.71 us: 1.01x faster                                                            |
| raytrace                   | 309 ms                                                 | 304 ms: 1.01x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 21.4 ms: 1.01x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.79 sec: 1.01x slower                                                           |
| pathlib                    | 18.5 ms                                                | 18.7 ms: 1.01x slower                                                            |
| tornado_http               | 98.1 ms                                                | 99.3 ms: 1.01x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.02x slower                                                             |
| sympy_expand               | 484 ms                                                 | 493 ms: 1.02x slower                                                             |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 850 us: 1.02x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.0 us: 1.02x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.73 sec: 1.02x slower                                                           |
| chaos                      | 71.9 ms                                                | 74.3 ms: 1.03x slower                                                            |
| regex_effbot               | 3.51 ms                                                | 3.65 ms: 1.04x slower                                                            |
| scimark_sor                | 121 ms                                                 | 126 ms: 1.04x slower                                                             |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.04x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 114 ms: 1.06x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.06x slower                                                           |
| sqlglot_optimize           | 55.3 ms                                                | 58.9 ms: 1.06x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.07x slower                                                            |
| pickle_list                | 4.59 us                                                | 4.93 us: 1.07x slower                                                            |
| regex_dna                  | 205 ms                                                 | 220 ms: 1.08x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 69.6 ms: 1.08x slower                                                            |
| meteor_contest             | 109 ms                                                 | 118 ms: 1.08x slower                                                             |
| 2to3                       | 264 ms                                                 | 286 ms: 1.08x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 61.7 ms: 1.08x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.27 ms: 1.09x slower                                                            |
| go                         | 149 ms                                                 | 162 ms: 1.09x slower                                                             |
| regex_compile              | 141 ms                                                 | 154 ms: 1.09x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.74 sec: 1.12x slower                                                           |
| pprint_safe_repr           | 747 ms                                                 | 837 ms: 1.12x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 90.8 ms: 1.12x slower                                                            |
| nqueens                    | 87.9 ms                                                | 98.6 ms: 1.12x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 86.2 ms: 1.12x slower                                                            |
| sqlite_synth               | 2.57 us                                                | 2.91 us: 1.13x slower                                                            |
| fannkuch                   | 405 ms                                                 | 463 ms: 1.14x slower                                                             |
| unpickle                   | 13.8 us                                                | 15.9 us: 1.15x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.70 sec: 1.17x slower                                                           |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 84.8 ms: 1.20x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.18 ms: 1.23x slower                                                            |
| coverage                   | 78.8 ms                                                | 96.9 ms: 1.23x slower                                                            |
| pyflate                    | 434 ms                                                 | 534 ms: 1.23x slower                                                             |
| nbody                      | 96.0 ms                                                | 119 ms: 1.24x slower                                                             |
| async_generators           | 374 ms                                                 | 466 ms: 1.25x slower                                                             |
| mypy2                      | 686 ms                                                 | 867 ms: 1.26x slower                                                             |
| float                      | 78.9 ms                                                | 100 ms: 1.27x slower                                                             |
| telco                      | 6.86 ms                                                | 8.73 ms: 1.27x slower                                                            |
| scimark_fft                | 345 ms                                                 | 447 ms: 1.30x slower                                                             |
| hexiom                     | 6.89 ms                                                | 9.09 ms: 1.32x slower                                                            |
| deltablue                  | 3.92 ms                                                | 5.18 ms: 1.32x slower                                                            |
| mako                       | 10.7 ms                                                | 14.7 ms: 1.38x slower                                                            |
| spectral_norm              | 108 ms                                                 | 152 ms: 1.40x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.81 ms: 1.47x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (6): json, richards, bench_mp_pool, asyncio_websockets, sympy_str, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 98.98% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x