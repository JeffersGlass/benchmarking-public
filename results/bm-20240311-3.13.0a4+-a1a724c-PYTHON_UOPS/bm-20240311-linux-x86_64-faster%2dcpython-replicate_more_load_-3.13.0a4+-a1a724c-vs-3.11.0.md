# Results vs. 3.11.0

- fork: faster-cpython
- ref: replicate_more_load_
- machine: linux-x86_64
- commit hash: a1a724c
- commit date: 2024-03-11
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 310 ms: 1.17x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.09 ms: 1.06x slower                                                            |
| docutils       | 2.66 sec                                               | 2.91 sec: 1.09x slower                                                           |
| html5lib       | 64.8 ms                                                | 70.6 ms: 1.09x slower                                                            |
| tornado_http   | 98.1 ms                                                | 105 ms: 1.07x slower                                                             |
| Geometric mean | (ref)                                                  | 1.10x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 467 ms: 1.13x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 599 ms: 1.07x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 601 ms: 1.04x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 474 ms: 1.04x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.27 sec: 1.02x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 754 ms: 1.01x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                                     |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 193 ms: 1.01x faster                                                             |
| float          | 78.9 ms                                                | 109 ms: 1.38x slower                                                             |
| nbody          | 96.0 ms                                                | 143 ms: 1.49x slower                                                             |
| Geometric mean | (ref)                                                  | 1.27x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.47 ms: 1.01x faster                                                            |
| regex_dna      | 205 ms                                                 | 215 ms: 1.05x slower                                                             |
| regex_v8       | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                            |
| regex_compile  | 141 ms                                                 | 192 ms: 1.36x slower                                                             |
| Geometric mean | (ref)                                                  | 1.11x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| unpickle_list        | 5.21 us                                                | 4.87 us: 1.07x faster                                                            |
| json_loads           | 29.2 us                                                | 28.2 us: 1.04x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 312 us: 1.02x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 161 ms: 1.02x faster                                                             |
| pickle_dict          | 34.6 us                                                | 35.2 us: 1.02x slower                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 117 ms: 1.08x slower                                                             |
| pickle               | 11.0 us                                                | 12.0 us: 1.09x slower                                                            |
| unpickle             | 13.8 us                                                | 15.3 us: 1.10x slower                                                            |
| xml_etree_process    | 56.9 ms                                                | 63.6 ms: 1.12x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 93.9 ms: 1.16x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.36 us: 1.17x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.76 sec: 1.20x slower                                                           |
| unpickle_pure_python | 242 us                                                 | 313 us: 1.29x slower                                                             |
| Geometric mean       | (ref)                                                  | 1.06x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 9.01 ms: 1.50x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 35.2 ms: 1.05x slower                                                            |
| genshi_xml      | 53.4 ms                                                | 66.8 ms: 1.25x slower                                                            |
| genshi_text     | 22.5 ms                                                | 29.6 ms: 1.31x slower                                                            |
| mako            | 10.7 ms                                                | 15.0 ms: 1.40x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.25x slower                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-faster%2dcpython-replicate_more_load_-3.13.0a4+-a1a724c |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 120 us: 4.34x faster                                                             |
| generators                 | 74.9 ms                                                | 30.3 ms: 2.47x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 508 ms: 1.72x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.86 sec: 1.67x faster                                                           |
| pylint                     | 476 ms                                                 | 336 ms: 1.42x faster                                                             |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                            |
| coroutines                 | 27.0 ms                                                | 23.0 ms: 1.17x faster                                                            |
| async_tree_none            | 528 ms                                                 | 467 ms: 1.13x faster                                                             |
| unpickle_list              | 5.21 us                                                | 4.87 us: 1.07x faster                                                            |
| async_tree_memoization     | 639 ms                                                 | 599 ms: 1.07x faster                                                             |
| djangocms                  | 33.5 us                                                | 31.7 us: 1.06x faster                                                            |
| logging_silent             | 111 ns                                                 | 105 ns: 1.06x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 601 ms: 1.04x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 474 ms: 1.04x faster                                                             |
| json_loads                 | 29.2 us                                                | 28.2 us: 1.04x faster                                                            |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                                            |
| async_tree_io              | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 312 us: 1.02x faster                                                             |
| async_tree_io_tg           | 1.29 sec                                               | 1.27 sec: 1.02x faster                                                           |
| xml_etree_parse            | 164 ms                                                 | 161 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 754 ms: 1.01x faster                                                             |
| regex_effbot               | 3.51 ms                                                | 3.47 ms: 1.01x faster                                                            |
| pidigits                   | 194 ms                                                 | 193 ms: 1.01x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 170 ms: 1.01x slower                                                             |
| deepcopy                   | 365 us                                                 | 368 us: 1.01x slower                                                             |
| logging_simple             | 6.22 us                                                | 6.32 us: 1.02x slower                                                            |
| comprehensions             | 23.6 us                                                | 24.0 us: 1.02x slower                                                            |
| pickle_dict                | 34.6 us                                                | 35.2 us: 1.02x slower                                                            |
| sqlglot_normalize          | 113 ms                                                 | 115 ms: 1.02x slower                                                             |
| gc_traversal               | 4.01 ms                                                | 4.10 ms: 1.02x slower                                                            |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                                             |
| sympy_integrate            | 21.5 ms                                                | 22.1 ms: 1.03x slower                                                            |
| logging_format             | 6.81 us                                                | 7.04 us: 1.03x slower                                                            |
| thrift                     | 784 us                                                 | 815 us: 1.04x slower                                                             |
| dask                       | 365 ms                                                 | 380 ms: 1.04x slower                                                             |
| sympy_str                  | 297 ms                                                 | 311 ms: 1.05x slower                                                             |
| django_template            | 33.5 ms                                                | 35.2 ms: 1.05x slower                                                            |
| deltablue                  | 3.92 ms                                                | 4.12 ms: 1.05x slower                                                            |
| regex_dna                  | 205 ms                                                 | 215 ms: 1.05x slower                                                             |
| pathlib                    | 18.5 ms                                                | 19.5 ms: 1.05x slower                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.51 ms: 1.05x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.09 ms: 1.06x slower                                                            |
| sqlglot_transpile          | 1.75 ms                                                | 1.85 ms: 1.06x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 888 us: 1.06x slower                                                             |
| tornado_http               | 98.1 ms                                                | 105 ms: 1.07x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.54 ms: 1.07x slower                                                            |
| sympy_expand               | 484 ms                                                 | 522 ms: 1.08x slower                                                             |
| xml_etree_iterparse        | 108 ms                                                 | 117 ms: 1.08x slower                                                             |
| regex_v8                   | 22.9 ms                                                | 24.8 ms: 1.08x slower                                                            |
| html5lib                   | 64.8 ms                                                | 70.6 ms: 1.09x slower                                                            |
| pickle                     | 11.0 us                                                | 12.0 us: 1.09x slower                                                            |
| docutils                   | 2.66 sec                                               | 2.91 sec: 1.09x slower                                                           |
| deepcopy_memo              | 40.2 us                                                | 44.0 us: 1.10x slower                                                            |
| richards_super             | 61.9 ms                                                | 67.9 ms: 1.10x slower                                                            |
| aiohttp                    | 1.12 ms                                                | 1.23 ms: 1.10x slower                                                            |
| gunicorn                   | 1.20 ms                                                | 1.32 ms: 1.10x slower                                                            |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.10x slower                                                            |
| xml_etree_process          | 56.9 ms                                                | 63.6 ms: 1.12x slower                                                            |
| pycparser                  | 1.19 sec                                               | 1.33 sec: 1.12x slower                                                           |
| dulwich_log                | 64.6 ms                                                | 74.0 ms: 1.15x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 63.4 ms: 1.15x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 93.9 ms: 1.16x slower                                                            |
| chaos                      | 71.9 ms                                                | 83.3 ms: 1.16x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.36 us: 1.17x slower                                                            |
| meteor_contest             | 109 ms                                                 | 128 ms: 1.17x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 3.01 us: 1.17x slower                                                            |
| 2to3                       | 264 ms                                                 | 310 ms: 1.17x slower                                                             |
| tomli_loads                | 2.30 sec                                               | 2.76 sec: 1.20x slower                                                           |
| raytrace                   | 309 ms                                                 | 374 ms: 1.21x slower                                                             |
| crypto_pyaes               | 76.7 ms                                                | 93.1 ms: 1.21x slower                                                            |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                            |
| richards                   | 49.8 ms                                                | 61.4 ms: 1.23x slower                                                            |
| coverage                   | 78.8 ms                                                | 97.3 ms: 1.24x slower                                                            |
| genshi_xml                 | 53.4 ms                                                | 66.8 ms: 1.25x slower                                                            |
| pprint_pformat             | 1.55 sec                                               | 1.98 sec: 1.27x slower                                                           |
| scimark_sor                | 121 ms                                                 | 155 ms: 1.27x slower                                                             |
| go                         | 149 ms                                                 | 190 ms: 1.28x slower                                                             |
| pprint_safe_repr           | 747 ms                                                 | 958 ms: 1.28x slower                                                             |
| async_generators           | 374 ms                                                 | 482 ms: 1.29x slower                                                             |
| unpickle_pure_python       | 242 us                                                 | 313 us: 1.29x slower                                                             |
| nqueens                    | 87.9 ms                                                | 114 ms: 1.30x slower                                                             |
| genshi_text                | 22.5 ms                                                | 29.6 ms: 1.31x slower                                                            |
| telco                      | 6.86 ms                                                | 9.09 ms: 1.33x slower                                                            |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 6.73 ms: 1.34x slower                                                            |
| mypy2                      | 686 ms                                                 | 929 ms: 1.36x slower                                                             |
| regex_compile              | 141 ms                                                 | 192 ms: 1.36x slower                                                             |
| float                      | 78.9 ms                                                | 109 ms: 1.38x slower                                                             |
| fannkuch                   | 405 ms                                                 | 564 ms: 1.39x slower                                                             |
| mako                       | 10.7 ms                                                | 15.0 ms: 1.40x slower                                                            |
| spectral_norm              | 108 ms                                                 | 156 ms: 1.45x slower                                                             |
| scimark_monte_carlo        | 70.7 ms                                                | 104 ms: 1.47x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 172 ms: 1.48x slower                                                             |
| scimark_fft                | 345 ms                                                 | 510 ms: 1.48x slower                                                             |
| nbody                      | 96.0 ms                                                | 143 ms: 1.49x slower                                                             |
| python_startup_no_site     | 6.01 ms                                                | 9.01 ms: 1.50x slower                                                            |
| pyflate                    | 434 ms                                                 | 663 ms: 1.53x slower                                                             |
| unpack_sequence            | 43.5 ns                                                | 67.0 ns: 1.54x slower                                                            |
| hexiom                     | 6.89 ms                                                | 10.8 ms: 1.57x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.08x slower                                                                     |

Benchmark hidden because not significant (4): async_tree_cpu_io_mixed, json, bench_mp_pool, mdp
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.05x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 1.01x