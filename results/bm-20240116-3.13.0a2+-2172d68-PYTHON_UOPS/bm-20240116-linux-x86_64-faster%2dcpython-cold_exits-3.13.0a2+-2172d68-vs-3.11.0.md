
# Results vs. 3.11.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 2172d68
- commit date: 2024-01-16
- overall geometric mean: 1.02x slower
- HPT reliability: 99.87%
- HPT 99th percentile: 1.00x slower
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| chameleon      | 6.70 ms                                                | 7.27 ms: 1.08x slower                                                  |
| docutils       | 2.66 sec                                               | 2.75 sec: 1.03x slower                                                 |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 578 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 197 ms: 1.01x slower                                                   |
| float          | 78.9 ms                                                | 92.1 ms: 1.17x slower                                                  |
| nbody          | 96.0 ms                                                | 115 ms: 1.20x slower                                                   |
| Geometric mean | (ref)                                                  | 1.12x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| regex_dna      | 205 ms                                                 | 226 ms: 1.11x slower                                                   |
| regex_compile  | 141 ms                                                 | 170 ms: 1.21x slower                                                   |
| Geometric mean | (ref)                                                  | 1.12x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 233 us: 1.04x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| unpickle_list        | 5.21 us                                                | 5.36 us: 1.03x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| pickle_list          | 4.59 us                                                | 4.88 us: 1.06x slower                                                  |
| unpickle             | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 89.9 ms: 1.11x slower                                                  |
| tomli_loads          | 2.30 sec                                               | 2.71 sec: 1.17x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.6 ms: 1.27x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 119 us: 4.36x faster                                                   |
| generators                 | 74.9 ms                                                | 29.1 ms: 2.57x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.78x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                  |
| async_tree_none            | 528 ms                                                 | 451 ms: 1.17x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                   |
| comprehensions             | 23.6 us                                                | 21.2 us: 1.11x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 446 ms: 1.10x faster                                                   |
| richards_super             | 61.9 ms                                                | 56.5 ms: 1.09x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 578 ms: 1.08x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                                  |
| async_tree_io              | 1.29 sec                                               | 1.21 sec: 1.06x faster                                                 |
| unpickle_pure_python       | 242 us                                                 | 233 us: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                   |
| logging_silent             | 111 ns                                                 | 107 ns: 1.04x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.38 ms: 1.04x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.03x faster                                                   |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.71 ms: 1.02x faster                                                  |
| raytrace                   | 309 ms                                                 | 302 ms: 1.02x faster                                                   |
| deepcopy                   | 365 us                                                 | 361 us: 1.01x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.19 us: 1.01x faster                                                  |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.01x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.78 sec: 1.00x slower                                                 |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                   |
| richards                   | 49.8 ms                                                | 50.0 ms: 1.01x slower                                                  |
| sympy_integrate            | 21.5 ms                                                | 21.7 ms: 1.01x slower                                                  |
| pidigits                   | 194 ms                                                 | 197 ms: 1.01x slower                                                   |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 855 us: 1.02x slower                                                   |
| logging_simple             | 6.22 us                                                | 6.39 us: 1.03x slower                                                  |
| unpickle_list              | 5.21 us                                                | 5.36 us: 1.03x slower                                                  |
| sqlglot_normalize          | 113 ms                                                 | 116 ms: 1.03x slower                                                   |
| pathlib                    | 18.5 ms                                                | 19.1 ms: 1.03x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.75 sec: 1.03x slower                                                 |
| sympy_expand               | 484 ms                                                 | 500 ms: 1.03x slower                                                   |
| chaos                      | 71.9 ms                                                | 74.4 ms: 1.03x slower                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                                  |
| deepcopy_memo              | 40.2 us                                                | 41.7 us: 1.04x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.05x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.72 ms: 1.06x slower                                                  |
| pickle_list                | 4.59 us                                                | 4.88 us: 1.06x slower                                                  |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.06x slower                                                   |
| logging_format             | 6.81 us                                                | 7.24 us: 1.06x slower                                                  |
| unpickle                   | 13.8 us                                                | 14.9 us: 1.08x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 59.9 ms: 1.08x slower                                                  |
| chameleon                  | 6.70 ms                                                | 7.27 ms: 1.08x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 61.8 ms: 1.09x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 83.5 ms: 1.09x slower                                                  |
| 2to3                       | 264 ms                                                 | 288 ms: 1.09x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 25.2 ms: 1.10x slower                                                  |
| regex_dna                  | 205 ms                                                 | 226 ms: 1.11x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.85 us: 1.11x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 89.9 ms: 1.11x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 71.8 ms: 1.11x slower                                                  |
| nqueens                    | 87.9 ms                                                | 98.8 ms: 1.12x slower                                                  |
| scimark_sor                | 121 ms                                                 | 139 ms: 1.14x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.78 sec: 1.14x slower                                                 |
| pprint_safe_repr           | 747 ms                                                 | 856 ms: 1.15x slower                                                   |
| float                      | 78.9 ms                                                | 92.1 ms: 1.17x slower                                                  |
| tomli_loads                | 2.30 sec                                               | 2.71 sec: 1.17x slower                                                 |
| go                         | 149 ms                                                 | 175 ms: 1.18x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.98 ms: 1.19x slower                                                  |
| fannkuch                   | 405 ms                                                 | 487 ms: 1.20x slower                                                   |
| nbody                      | 96.0 ms                                                | 115 ms: 1.20x slower                                                   |
| regex_compile              | 141 ms                                                 | 170 ms: 1.21x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.8 ms: 1.22x slower                                                  |
| async_generators           | 374 ms                                                 | 459 ms: 1.23x slower                                                   |
| deltablue                  | 3.92 ms                                                | 4.82 ms: 1.23x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 89.5 ms: 1.27x slower                                                  |
| telco                      | 6.86 ms                                                | 8.69 ms: 1.27x slower                                                  |
| mako                       | 10.7 ms                                                | 13.6 ms: 1.27x slower                                                  |
| scimark_lu                 | 116 ms                                                 | 149 ms: 1.28x slower                                                   |
| mypy2                      | 686 ms                                                 | 881 ms: 1.29x slower                                                   |
| scimark_fft                | 345 ms                                                 | 449 ms: 1.30x slower                                                   |
| hexiom                     | 6.89 ms                                                | 9.05 ms: 1.31x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 57.5 ns: 1.32x slower                                                  |
| spectral_norm              | 108 ms                                                 | 145 ms: 1.34x slower                                                   |
| pyflate                    | 434 ms                                                 | 582 ms: 1.34x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.78 ms: 1.46x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (5): tornado_http, bench_mp_pool, json, sympy_str, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.87% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 0.99x