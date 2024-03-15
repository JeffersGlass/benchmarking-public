# Results vs. 3.11.0

- fork: faster-cpython
- ref: optimize_inline_valu
- machine: linux-x86_64
- commit hash: b93e9d3
- commit date: 2024-03-07
- overall geometric mean: 1.01x slower \*
- HPT reliability: 97.35%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 290 ms: 1.10x slower                                                             |
| chameleon      | 6.70 ms                                                | 6.93 ms: 1.04x slower                                                            |
| docutils       | 2.66 sec                                               | 2.83 sec: 1.06x slower                                                           |
| html5lib       | 64.8 ms                                                | 68.8 ms: 1.06x slower                                                            |
| tornado_http   | 98.1 ms                                                | 97.5 ms: 1.01x faster                                                            |
| Geometric mean | (ref)                                                  | 1.05x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 444 ms: 1.19x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                             |
| float          | 78.9 ms                                                | 93.3 ms: 1.18x slower                                                            |
| nbody          | 96.0 ms                                                | 122 ms: 1.28x slower                                                             |
| Geometric mean | (ref)                                                  | 1.13x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                            |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                            |
| regex_compile  | 141 ms                                                 | 160 ms: 1.13x slower                                                             |
| Geometric mean | (ref)                                                  | 1.07x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| unpickle_list        | 5.21 us                                                | 4.86 us: 1.07x faster                                                            |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                             |
| json_loads           | 29.2 us                                                | 27.8 us: 1.05x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 306 us: 1.05x faster                                                             |
| pickle_dict          | 34.6 us                                                | 34.3 us: 1.01x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| xml_etree_process    | 56.9 ms                                                | 60.2 ms: 1.06x slower                                                            |
| pickle               | 11.0 us                                                | 11.7 us: 1.06x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.48 sec: 1.08x slower                                                           |
| unpickle_pure_python | 242 us                                                 | 262 us: 1.09x slower                                                             |
| xml_etree_generate   | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                            |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.07 us: 1.11x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.01x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.79 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.0 ms: 1.01x slower                                                            |
| genshi_xml      | 53.4 ms                                                | 57.4 ms: 1.07x slower                                                            |
| genshi_text     | 22.5 ms                                                | 25.1 ms: 1.11x slower                                                            |
| mako            | 10.7 ms                                                | 11.9 ms: 1.12x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.08x slower                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 114 us: 4.56x faster                                                             |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 491 ms: 1.78x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                           |
| pylint                     | 476 ms                                                 | 321 ms: 1.48x faster                                                             |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                            |
| coroutines                 | 27.0 ms                                                | 21.8 ms: 1.24x faster                                                            |
| async_tree_none            | 528 ms                                                 | 444 ms: 1.19x faster                                                             |
| richards_super             | 61.9 ms                                                | 53.8 ms: 1.15x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.2 us: 1.11x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 451 ms: 1.09x faster                                                             |
| logging_format             | 6.81 us                                                | 6.26 us: 1.09x faster                                                            |
| logging_simple             | 6.22 us                                                | 5.73 us: 1.09x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.71 ms: 1.08x faster                                                            |
| logging_silent             | 111 ns                                                 | 103 ns: 1.08x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                           |
| unpickle_list              | 5.21 us                                                | 4.86 us: 1.07x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.21 sec: 1.07x faster                                                           |
| sqlglot_parse              | 1.43 ms                                                | 1.35 ms: 1.06x faster                                                            |
| sympy_sum                  | 169 ms                                                 | 159 ms: 1.06x faster                                                             |
| richards                   | 49.8 ms                                                | 47.3 ms: 1.05x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                             |
| json_loads                 | 29.2 us                                                | 27.8 us: 1.05x faster                                                            |
| pickle_pure_python         | 320 us                                                 | 306 us: 1.05x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 718 ms: 1.04x faster                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.68 ms: 1.04x faster                                                            |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                             |
| deltablue                  | 3.92 ms                                                | 3.78 ms: 1.04x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.10 us: 1.04x faster                                                            |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                             |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                            |
| djangocms                  | 33.5 us                                                | 32.9 us: 1.02x faster                                                            |
| sympy_str                  | 297 ms                                                 | 292 ms: 1.02x faster                                                             |
| deepcopy                   | 365 us                                                 | 362 us: 1.01x faster                                                             |
| pickle_dict                | 34.6 us                                                | 34.3 us: 1.01x faster                                                            |
| tornado_http               | 98.1 ms                                                | 97.5 ms: 1.01x faster                                                            |
| regex_effbot               | 3.51 ms                                                | 3.49 ms: 1.00x faster                                                            |
| asyncio_websockets         | 550 ms                                                 | 552 ms: 1.00x slower                                                             |
| chaos                      | 71.9 ms                                                | 72.3 ms: 1.01x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 55.9 ms: 1.01x slower                                                            |
| sympy_expand               | 484 ms                                                 | 490 ms: 1.01x slower                                                             |
| thrift                     | 784 us                                                 | 793 us: 1.01x slower                                                             |
| django_template            | 33.5 ms                                                | 34.0 ms: 1.01x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 110 ms: 1.02x slower                                                             |
| bench_thread_pool          | 834 us                                                 | 857 us: 1.03x slower                                                             |
| chameleon                  | 6.70 ms                                                | 6.93 ms: 1.04x slower                                                            |
| deepcopy_memo              | 40.2 us                                                | 41.8 us: 1.04x slower                                                            |
| pathlib                    | 18.5 ms                                                | 19.3 ms: 1.04x slower                                                            |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.05x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 60.2 ms: 1.06x slower                                                            |
| spectral_norm              | 108 ms                                                 | 114 ms: 1.06x slower                                                             |
| aiohttp                    | 1.12 ms                                                | 1.18 ms: 1.06x slower                                                            |
| html5lib                   | 64.8 ms                                                | 68.8 ms: 1.06x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.83 sec: 1.06x slower                                                           |
| pickle                     | 11.0 us                                                | 11.7 us: 1.06x slower                                                            |
| meteor_contest             | 109 ms                                                 | 116 ms: 1.07x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.66 sec: 1.07x slower                                                           |
| gunicorn                   | 1.20 ms                                                | 1.28 ms: 1.07x slower                                                            |
| dulwich_log                | 64.6 ms                                                | 69.1 ms: 1.07x slower                                                            |
| raytrace                   | 309 ms                                                 | 330 ms: 1.07x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 801 ms: 1.07x slower                                                             |
| genshi_xml                 | 53.4 ms                                                | 57.4 ms: 1.07x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.48 sec: 1.08x slower                                                           |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 83.1 ms: 1.08x slower                                                            |
| unpickle_pure_python       | 242 us                                                 | 262 us: 1.09x slower                                                             |
| xml_etree_generate         | 81.1 ms                                                | 88.3 ms: 1.09x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                            |
| 2to3                       | 264 ms                                                 | 290 ms: 1.10x slower                                                             |
| pickle_list                | 4.59 us                                                | 5.07 us: 1.11x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.32 sec: 1.11x slower                                                           |
| genshi_text                | 22.5 ms                                                | 25.1 ms: 1.11x slower                                                            |
| nqueens                    | 87.9 ms                                                | 98.1 ms: 1.12x slower                                                            |
| mako                       | 10.7 ms                                                | 11.9 ms: 1.12x slower                                                            |
| regex_compile              | 141 ms                                                 | 160 ms: 1.13x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.93 us: 1.14x slower                                                            |
| go                         | 149 ms                                                 | 175 ms: 1.17x slower                                                             |
| float                      | 78.9 ms                                                | 93.3 ms: 1.18x slower                                                            |
| fannkuch                   | 405 ms                                                 | 481 ms: 1.19x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.02 ms: 1.20x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 85.7 ms: 1.21x slower                                                            |
| coverage                   | 78.8 ms                                                | 96.5 ms: 1.23x slower                                                            |
| scimark_fft                | 345 ms                                                 | 426 ms: 1.23x slower                                                             |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                                             |
| telco                      | 6.86 ms                                                | 8.51 ms: 1.24x slower                                                            |
| scimark_sor                | 121 ms                                                 | 151 ms: 1.24x slower                                                             |
| hexiom                     | 6.89 ms                                                | 8.78 ms: 1.27x slower                                                            |
| mypy2                      | 686 ms                                                 | 874 ms: 1.27x slower                                                             |
| nbody                      | 96.0 ms                                                | 122 ms: 1.28x slower                                                             |
| pyflate                    | 434 ms                                                 | 571 ms: 1.32x slower                                                             |
| unpack_sequence            | 43.5 ns                                                | 57.7 ns: 1.33x slower                                                            |
| scimark_lu                 | 116 ms                                                 | 160 ms: 1.37x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 8.79 ms: 1.46x slower                                                            |
| dask                       | 365 ms                                                 | 536 ms: 1.47x slower                                                             |
| Geometric mean             | (ref)                                                  | 1.01x slower                                                                     |

Benchmark hidden because not significant (2): json, bench_mp_pool
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 97.35% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.01x