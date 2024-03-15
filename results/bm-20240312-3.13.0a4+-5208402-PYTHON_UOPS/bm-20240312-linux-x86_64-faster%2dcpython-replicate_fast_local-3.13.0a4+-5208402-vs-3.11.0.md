# Results vs. 3.11.0

- fork: faster-cpython
- ref: replicate_fast_local
- machine: linux-x86_64
- commit hash: 5208402
- commit date: 2024-03-12
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 301 ms: 1.14x slower                                                             |
| chameleon      | 6.70 ms                                                | 7.08 ms: 1.06x slower                                                            |
| docutils       | 2.66 sec                                               | 2.89 sec: 1.08x slower                                                           |
| html5lib       | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                            |
| tornado_http   | 98.1 ms                                                | 104 ms: 1.06x slower                                                             |
| Geometric mean | (ref)                                                  | 1.09x slower                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 461 ms: 1.15x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 592 ms: 1.08x faster                                                             |
| async_tree_none_tg         | 491 ms                                                 | 470 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 602 ms: 1.04x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                           |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                           |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 750 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 742 ms: 1.01x faster                                                             |
| Geometric mean             | (ref)                                                  | 1.05x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 192 ms: 1.01x faster                                                             |
| float          | 78.9 ms                                                | 94.6 ms: 1.20x slower                                                            |
| nbody          | 96.0 ms                                                | 124 ms: 1.29x slower                                                             |
| Geometric mean | (ref)                                                  | 1.15x slower                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.71 ms: 1.06x slower                                                            |
| regex_v8       | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                            |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| regex_compile  | 141 ms                                                 | 179 ms: 1.27x slower                                                             |
| Geometric mean | (ref)                                                  | 1.12x slower                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| unpickle_list        | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| pickle_pure_python   | 320 us                                                 | 311 us: 1.03x faster                                                             |
| xml_etree_parse      | 164 ms                                                 | 161 ms: 1.02x faster                                                             |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.00x faster                                                            |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.04x slower                                                             |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| pickle_list          | 4.59 us                                                | 5.06 us: 1.10x slower                                                            |
| tomli_loads          | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| xml_etree_process    | 56.9 ms                                                | 63.5 ms: 1.12x slower                                                            |
| xml_etree_generate   | 81.1 ms                                                | 92.7 ms: 1.14x slower                                                            |
| unpickle_pure_python | 242 us                                                 | 277 us: 1.15x slower                                                             |
| unpickle             | 13.8 us                                                | 16.0 us: 1.15x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.03x slower                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                            |
| python_startup_no_site | 6.01 ms                                                | 8.99 ms: 1.50x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.35x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 33.5 ms                                                | 35.0 ms: 1.04x slower                                                            |
| genshi_xml      | 53.4 ms                                                | 63.2 ms: 1.18x slower                                                            |
| genshi_text     | 22.5 ms                                                | 26.9 ms: 1.19x slower                                                            |
| mako            | 10.7 ms                                                | 12.8 ms: 1.20x slower                                                            |
| Geometric mean  | (ref)                                                  | 1.15x slower                                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.52x faster                                                             |
| generators                 | 74.9 ms                                                | 30.3 ms: 2.47x faster                                                            |
| asyncio_tcp                | 875 ms                                                 | 507 ms: 1.73x faster                                                             |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.86 sec: 1.67x faster                                                           |
| pylint                     | 476 ms                                                 | 333 ms: 1.43x faster                                                             |
| json_dumps                 | 13.3 ms                                                | 10.7 ms: 1.25x faster                                                            |
| async_tree_none            | 528 ms                                                 | 461 ms: 1.15x faster                                                             |
| comprehensions             | 23.6 us                                                | 21.3 us: 1.11x faster                                                            |
| coroutines                 | 27.0 ms                                                | 24.7 ms: 1.10x faster                                                            |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                             |
| async_tree_memoization     | 639 ms                                                 | 592 ms: 1.08x faster                                                             |
| djangocms                  | 33.5 us                                                | 31.4 us: 1.07x faster                                                            |
| gc_traversal               | 4.01 ms                                                | 3.79 ms: 1.06x faster                                                            |
| async_tree_none_tg         | 491 ms                                                 | 470 ms: 1.04x faster                                                             |
| async_tree_memoization_tg  | 626 ms                                                 | 602 ms: 1.04x faster                                                             |
| async_tree_io              | 1.29 sec                                               | 1.24 sec: 1.04x faster                                                           |
| deepcopy_reduce            | 3.22 us                                                | 3.11 us: 1.03x faster                                                            |
| async_tree_io_tg           | 1.29 sec                                               | 1.25 sec: 1.03x faster                                                           |
| unpickle_list              | 5.21 us                                                | 5.06 us: 1.03x faster                                                            |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                                            |
| mdp                        | 2.77 sec                                               | 2.70 sec: 1.03x faster                                                           |
| pickle_pure_python         | 320 us                                                 | 311 us: 1.03x faster                                                             |
| xml_etree_parse            | 164 ms                                                 | 161 ms: 1.02x faster                                                             |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 750 ms: 1.02x faster                                                             |
| pidigits                   | 194 ms                                                 | 192 ms: 1.01x faster                                                             |
| sympy_sum                  | 169 ms                                                 | 167 ms: 1.01x faster                                                             |
| deepcopy                   | 365 us                                                 | 362 us: 1.01x faster                                                             |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 742 ms: 1.01x faster                                                             |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.00x faster                                                            |
| sympy_integrate            | 21.5 ms                                                | 21.6 ms: 1.01x slower                                                            |
| sqlglot_parse              | 1.43 ms                                                | 1.45 ms: 1.01x slower                                                            |
| richards_super             | 61.9 ms                                                | 62.7 ms: 1.01x slower                                                            |
| logging_simple             | 6.22 us                                                | 6.34 us: 1.02x slower                                                            |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                                             |
| sqlglot_transpile          | 1.75 ms                                                | 1.79 ms: 1.02x slower                                                            |
| sympy_str                  | 297 ms                                                 | 304 ms: 1.02x slower                                                             |
| deepcopy_memo              | 40.2 us                                                | 41.5 us: 1.03x slower                                                            |
| dask                       | 365 ms                                                 | 377 ms: 1.03x slower                                                             |
| thrift                     | 784 us                                                 | 813 us: 1.04x slower                                                             |
| logging_format             | 6.81 us                                                | 7.07 us: 1.04x slower                                                            |
| xml_etree_iterparse        | 108 ms                                                 | 112 ms: 1.04x slower                                                             |
| django_template            | 33.5 ms                                                | 35.0 ms: 1.04x slower                                                            |
| bench_thread_pool          | 834 us                                                 | 874 us: 1.05x slower                                                             |
| pathlib                    | 18.5 ms                                                | 19.4 ms: 1.05x slower                                                            |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                            |
| tornado_http               | 98.1 ms                                                | 104 ms: 1.06x slower                                                             |
| regex_effbot               | 3.51 ms                                                | 3.71 ms: 1.06x slower                                                            |
| chameleon                  | 6.70 ms                                                | 7.08 ms: 1.06x slower                                                            |
| chaos                      | 71.9 ms                                                | 76.6 ms: 1.07x slower                                                            |
| sympy_expand               | 484 ms                                                 | 517 ms: 1.07x slower                                                             |
| create_gc_cycles           | 1.43 ms                                                | 1.54 ms: 1.07x slower                                                            |
| regex_v8                   | 22.9 ms                                                | 24.6 ms: 1.08x slower                                                            |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                                             |
| docutils                   | 2.66 sec                                               | 2.89 sec: 1.08x slower                                                           |
| meteor_contest             | 109 ms                                                 | 119 ms: 1.09x slower                                                             |
| pycparser                  | 1.19 sec                                               | 1.30 sec: 1.10x slower                                                           |
| aiohttp                    | 1.12 ms                                                | 1.22 ms: 1.10x slower                                                            |
| gunicorn                   | 1.20 ms                                                | 1.32 ms: 1.10x slower                                                            |
| pickle_list                | 4.59 us                                                | 5.06 us: 1.10x slower                                                            |
| tomli_loads                | 2.30 sec                                               | 2.55 sec: 1.11x slower                                                           |
| html5lib                   | 64.8 ms                                                | 71.7 ms: 1.11x slower                                                            |
| sqlglot_optimize           | 55.3 ms                                                | 61.2 ms: 1.11x slower                                                            |
| raytrace                   | 309 ms                                                 | 343 ms: 1.11x slower                                                             |
| xml_etree_process          | 56.9 ms                                                | 63.5 ms: 1.12x slower                                                            |
| crypto_pyaes               | 76.7 ms                                                | 85.8 ms: 1.12x slower                                                            |
| richards                   | 49.8 ms                                                | 56.1 ms: 1.13x slower                                                            |
| 2to3                       | 264 ms                                                 | 301 ms: 1.14x slower                                                             |
| dulwich_log                | 64.6 ms                                                | 73.7 ms: 1.14x slower                                                            |
| xml_etree_generate         | 81.1 ms                                                | 92.7 ms: 1.14x slower                                                            |
| unpickle_pure_python       | 242 us                                                 | 277 us: 1.15x slower                                                             |
| sqlite_synth               | 2.57 us                                                | 2.96 us: 1.15x slower                                                            |
| unpickle                   | 13.8 us                                                | 16.0 us: 1.15x slower                                                            |
| nqueens                    | 87.9 ms                                                | 101 ms: 1.15x slower                                                             |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.91 ms: 1.18x slower                                                            |
| genshi_xml                 | 53.4 ms                                                | 63.2 ms: 1.18x slower                                                            |
| pprint_safe_repr           | 747 ms                                                 | 885 ms: 1.18x slower                                                             |
| pprint_pformat             | 1.55 sec                                               | 1.85 sec: 1.19x slower                                                           |
| genshi_text                | 22.5 ms                                                | 26.9 ms: 1.19x slower                                                            |
| float                      | 78.9 ms                                                | 94.6 ms: 1.20x slower                                                            |
| go                         | 149 ms                                                 | 178 ms: 1.20x slower                                                             |
| mako                       | 10.7 ms                                                | 12.8 ms: 1.20x slower                                                            |
| fannkuch                   | 405 ms                                                 | 490 ms: 1.21x slower                                                             |
| python_startup             | 8.56 ms                                                | 10.4 ms: 1.22x slower                                                            |
| scimark_monte_carlo        | 70.7 ms                                                | 88.3 ms: 1.25x slower                                                            |
| coverage                   | 78.8 ms                                                | 99.2 ms: 1.26x slower                                                            |
| regex_compile              | 141 ms                                                 | 179 ms: 1.27x slower                                                             |
| scimark_sor                | 121 ms                                                 | 154 ms: 1.27x slower                                                             |
| telco                      | 6.86 ms                                                | 8.79 ms: 1.28x slower                                                            |
| nbody                      | 96.0 ms                                                | 124 ms: 1.29x slower                                                             |
| async_generators           | 374 ms                                                 | 484 ms: 1.30x slower                                                             |
| spectral_norm              | 108 ms                                                 | 142 ms: 1.31x slower                                                             |
| scimark_fft                | 345 ms                                                 | 459 ms: 1.33x slower                                                             |
| hexiom                     | 6.89 ms                                                | 9.23 ms: 1.34x slower                                                            |
| mypy2                      | 686 ms                                                 | 922 ms: 1.34x slower                                                             |
| pyflate                    | 434 ms                                                 | 594 ms: 1.37x slower                                                             |
| scimark_lu                 | 116 ms                                                 | 160 ms: 1.37x slower                                                             |
| unpack_sequence            | 43.5 ns                                                | 62.0 ns: 1.43x slower                                                            |
| python_startup_no_site     | 6.01 ms                                                | 8.99 ms: 1.50x slower                                                            |
| Geometric mean             | (ref)                                                  | 1.04x slower                                                                     |

Benchmark hidden because not significant (4): deltablue, bench_mp_pool, json, sqlglot_normalize
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.01x