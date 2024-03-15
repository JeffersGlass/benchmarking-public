# Results vs. 3.11.0

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: b6ae6da
- commit date: 2024-03-11
- overall geometric mean: 1.03x slower
- HPT reliability: 99.99%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.01x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 297 ms: 1.13x slower                                   |
| chameleon      | 6.70 ms                                                | 7.13 ms: 1.06x slower                                  |
| docutils       | 2.66 sec                                               | 2.86 sec: 1.07x slower                                 |
| html5lib       | 64.8 ms                                                | 69.5 ms: 1.07x slower                                  |
| tornado_http   | 98.1 ms                                                | 103 ms: 1.05x slower                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none           | 528 ms                                                 | 459 ms: 1.15x faster                                   |
| async_tree_memoization    | 639 ms                                                 | 593 ms: 1.08x faster                                   |
| async_tree_io             | 1.29 sec                                               | 1.23 sec: 1.04x faster                                 |
| async_tree_none_tg        | 491 ms                                                 | 472 ms: 1.04x faster                                   |
| async_tree_io_tg          | 1.29 sec                                               | 1.26 sec: 1.03x faster                                 |
| async_tree_memoization_tg | 626 ms                                                 | 608 ms: 1.03x faster                                   |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 743 ms: 1.01x faster                                   |
| Geometric mean            | (ref)                                                  | 1.05x faster                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 191 ms: 1.02x faster                                   |
| float          | 78.9 ms                                                | 93.0 ms: 1.18x slower                                  |
| nbody          | 96.0 ms                                                | 120 ms: 1.25x slower                                   |
| Geometric mean | (ref)                                                  | 1.13x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.59 ms: 1.02x slower                                  |
| regex_dna      | 205 ms                                                 | 216 ms: 1.06x slower                                   |
| regex_v8       | 22.9 ms                                                | 25.1 ms: 1.09x slower                                  |
| regex_compile  | 141 ms                                                 | 174 ms: 1.23x slower                                   |
| Geometric mean | (ref)                                                  | 1.10x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.6 ms: 1.26x faster                                  |
| unpickle_list        | 5.21 us                                                | 4.88 us: 1.07x faster                                  |
| pickle_dict          | 34.6 us                                                | 32.9 us: 1.05x faster                                  |
| json_loads           | 29.2 us                                                | 28.2 us: 1.03x faster                                  |
| pickle_pure_python   | 320 us                                                 | 310 us: 1.03x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| xml_etree_iterparse  | 108 ms                                                 | 112 ms: 1.03x slower                                   |
| tomli_loads          | 2.30 sec                                               | 2.43 sec: 1.05x slower                                 |
| pickle_list          | 4.59 us                                                | 4.90 us: 1.07x slower                                  |
| xml_etree_process    | 56.9 ms                                                | 62.3 ms: 1.09x slower                                  |
| pickle               | 11.0 us                                                | 12.0 us: 1.10x slower                                  |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                  |
| unpickle_pure_python | 242 us                                                 | 269 us: 1.11x slower                                   |
| xml_etree_generate   | 81.1 ms                                                | 90.8 ms: 1.12x slower                                  |
| Geometric mean       | (ref)                                                  | 1.02x slower                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.4 ms: 1.22x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 9.01 ms: 1.50x slower                                  |
| Geometric mean         | (ref)                                                  | 1.35x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 33.5 ms                                                | 35.3 ms: 1.05x slower                                  |
| genshi_xml      | 53.4 ms                                                | 61.5 ms: 1.15x slower                                  |
| mako            | 10.7 ms                                                | 12.7 ms: 1.19x slower                                  |
| genshi_text     | 22.5 ms                                                | 27.1 ms: 1.20x slower                                  |
| Geometric mean  | (ref)                                                  | 1.15x slower                                           |

All benchmarks:
===============

| Benchmark                 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|---------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols  | 520 us                                                 | 119 us: 4.37x faster                                   |
| generators                | 74.9 ms                                                | 30.0 ms: 2.49x faster                                  |
| asyncio_tcp               | 875 ms                                                 | 507 ms: 1.73x faster                                   |
| asyncio_tcp_ssl           | 3.11 sec                                               | 1.86 sec: 1.67x faster                                 |
| pylint                    | 476 ms                                                 | 331 ms: 1.44x faster                                   |
| json_dumps                | 13.3 ms                                                | 10.6 ms: 1.26x faster                                  |
| coroutines                | 27.0 ms                                                | 22.5 ms: 1.20x faster                                  |
| async_tree_none           | 528 ms                                                 | 459 ms: 1.15x faster                                   |
| comprehensions            | 23.6 us                                                | 20.7 us: 1.14x faster                                  |
| async_tree_memoization    | 639 ms                                                 | 593 ms: 1.08x faster                                   |
| unpickle_list             | 5.21 us                                                | 4.88 us: 1.07x faster                                  |
| logging_silent            | 111 ns                                                 | 105 ns: 1.06x faster                                   |
| pickle_dict               | 34.6 us                                                | 32.9 us: 1.05x faster                                  |
| async_tree_io             | 1.29 sec                                               | 1.23 sec: 1.04x faster                                 |
| async_tree_none_tg        | 491 ms                                                 | 472 ms: 1.04x faster                                   |
| json_loads                | 29.2 us                                                | 28.2 us: 1.03x faster                                  |
| pickle_pure_python        | 320 us                                                 | 310 us: 1.03x faster                                   |
| async_tree_io_tg          | 1.29 sec                                               | 1.26 sec: 1.03x faster                                 |
| async_tree_memoization_tg | 626 ms                                                 | 608 ms: 1.03x faster                                   |
| xml_etree_parse           | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| djangocms                 | 33.5 us                                                | 32.6 us: 1.03x faster                                  |
| deltablue                 | 3.92 ms                                                | 3.82 ms: 1.03x faster                                  |
| mdp                       | 2.77 sec                                               | 2.72 sec: 1.02x faster                                 |
| gc_traversal              | 4.01 ms                                                | 3.94 ms: 1.02x faster                                  |
| pidigits                  | 194 ms                                                 | 191 ms: 1.02x faster                                   |
| deepcopy_reduce           | 3.22 us                                                | 3.18 us: 1.01x faster                                  |
| sympy_sum                 | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed   | 749 ms                                                 | 743 ms: 1.01x faster                                   |
| deepcopy                  | 365 us                                                 | 367 us: 1.00x slower                                   |
| logging_simple            | 6.22 us                                                | 6.33 us: 1.02x slower                                  |
| sqlglot_transpile         | 1.75 ms                                                | 1.78 ms: 1.02x slower                                  |
| sympy_str                 | 297 ms                                                 | 303 ms: 1.02x slower                                   |
| asyncio_websockets        | 550 ms                                                 | 564 ms: 1.02x slower                                   |
| regex_effbot              | 3.51 ms                                                | 3.59 ms: 1.02x slower                                  |
| xml_etree_iterparse       | 108 ms                                                 | 112 ms: 1.03x slower                                   |
| dask                      | 365 ms                                                 | 378 ms: 1.03x slower                                   |
| logging_format            | 6.81 us                                                | 7.08 us: 1.04x slower                                  |
| thrift                    | 784 us                                                 | 817 us: 1.04x slower                                   |
| chaos                     | 71.9 ms                                                | 74.9 ms: 1.04x slower                                  |
| bench_thread_pool         | 834 us                                                 | 872 us: 1.04x slower                                   |
| pathlib                   | 18.5 ms                                                | 19.5 ms: 1.05x slower                                  |
| django_template           | 33.5 ms                                                | 35.3 ms: 1.05x slower                                  |
| tornado_http              | 98.1 ms                                                | 103 ms: 1.05x slower                                   |
| tomli_loads               | 2.30 sec                                               | 2.43 sec: 1.05x slower                                 |
| deepcopy_memo             | 40.2 us                                                | 42.3 us: 1.05x slower                                  |
| sympy_expand              | 484 ms                                                 | 512 ms: 1.06x slower                                   |
| regex_dna                 | 205 ms                                                 | 216 ms: 1.06x slower                                   |
| chameleon                 | 6.70 ms                                                | 7.13 ms: 1.06x slower                                  |
| pickle_list               | 4.59 us                                                | 4.90 us: 1.07x slower                                  |
| html5lib                  | 64.8 ms                                                | 69.5 ms: 1.07x slower                                  |
| docutils                  | 2.66 sec                                               | 2.86 sec: 1.07x slower                                 |
| meteor_contest            | 109 ms                                                 | 117 ms: 1.07x slower                                   |
| create_gc_cycles          | 1.43 ms                                                | 1.54 ms: 1.08x slower                                  |
| aiohttp                   | 1.12 ms                                                | 1.21 ms: 1.09x slower                                  |
| pycparser                 | 1.19 sec                                               | 1.29 sec: 1.09x slower                                 |
| xml_etree_process         | 56.9 ms                                                | 62.3 ms: 1.09x slower                                  |
| regex_v8                  | 22.9 ms                                                | 25.1 ms: 1.09x slower                                  |
| pickle                    | 11.0 us                                                | 12.0 us: 1.10x slower                                  |
| gunicorn                  | 1.20 ms                                                | 1.31 ms: 1.10x slower                                  |
| sqlglot_optimize          | 55.3 ms                                                | 61.0 ms: 1.10x slower                                  |
| unpickle                  | 13.8 us                                                | 15.3 us: 1.11x slower                                  |
| raytrace                  | 309 ms                                                 | 342 ms: 1.11x slower                                   |
| unpickle_pure_python      | 242 us                                                 | 269 us: 1.11x slower                                   |
| richards                  | 49.8 ms                                                | 55.6 ms: 1.12x slower                                  |
| xml_etree_generate        | 81.1 ms                                                | 90.8 ms: 1.12x slower                                  |
| 2to3                      | 264 ms                                                 | 297 ms: 1.13x slower                                   |
| nqueens                   | 87.9 ms                                                | 99.1 ms: 1.13x slower                                  |
| crypto_pyaes              | 76.7 ms                                                | 86.5 ms: 1.13x slower                                  |
| dulwich_log               | 64.6 ms                                                | 73.1 ms: 1.13x slower                                  |
| scimark_sparse_mat_mult   | 5.03 ms                                                | 5.69 ms: 1.13x slower                                  |
| genshi_xml                | 53.4 ms                                                | 61.5 ms: 1.15x slower                                  |
| pprint_safe_repr          | 747 ms                                                 | 860 ms: 1.15x slower                                   |
| pprint_pformat            | 1.55 sec                                               | 1.79 sec: 1.15x slower                                 |
| sqlite_synth              | 2.57 us                                                | 2.96 us: 1.15x slower                                  |
| fannkuch                  | 405 ms                                                 | 472 ms: 1.16x slower                                   |
| scimark_monte_carlo       | 70.7 ms                                                | 82.6 ms: 1.17x slower                                  |
| float                     | 78.9 ms                                                | 93.0 ms: 1.18x slower                                  |
| go                        | 149 ms                                                 | 176 ms: 1.18x slower                                   |
| mako                      | 10.7 ms                                                | 12.7 ms: 1.19x slower                                  |
| genshi_text               | 22.5 ms                                                | 27.1 ms: 1.20x slower                                  |
| python_startup            | 8.56 ms                                                | 10.4 ms: 1.22x slower                                  |
| regex_compile             | 141 ms                                                 | 174 ms: 1.23x slower                                   |
| scimark_sor               | 121 ms                                                 | 150 ms: 1.24x slower                                   |
| coverage                  | 78.8 ms                                                | 97.4 ms: 1.24x slower                                  |
| nbody                     | 96.0 ms                                                | 120 ms: 1.25x slower                                   |
| async_generators          | 374 ms                                                 | 469 ms: 1.25x slower                                   |
| scimark_fft               | 345 ms                                                 | 436 ms: 1.26x slower                                   |
| telco                     | 6.86 ms                                                | 8.66 ms: 1.26x slower                                  |
| hexiom                    | 6.89 ms                                                | 8.79 ms: 1.28x slower                                  |
| pyflate                   | 434 ms                                                 | 564 ms: 1.30x slower                                   |
| spectral_norm             | 108 ms                                                 | 141 ms: 1.30x slower                                   |
| unpack_sequence           | 43.5 ns                                                | 57.0 ns: 1.31x slower                                  |
| mypy2                     | 686 ms                                                 | 918 ms: 1.34x slower                                   |
| scimark_lu                | 116 ms                                                 | 158 ms: 1.35x slower                                   |
| python_startup_no_site    | 6.01 ms                                                | 9.01 ms: 1.50x slower                                  |
| Geometric mean            | (ref)                                                  | 1.03x slower                                           |

Benchmark hidden because not significant (7): async_tree_cpu_io_mixed_tg, json, richards_super, bench_mp_pool, sqlglot_normalize, sympy_integrate, sqlglot_parse
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.01x