# Results vs. 3.11.0

- fork: python
- ref: cbf3d38cbeb6e640d595
- machine: linux-x86_64
- commit hash: cbf3d38
- commit date: 2024-03-05
- overall geometric mean: 1.02x slower \*
- HPT reliability: 99.60%
- HPT 99th percentile: 1.00x slower
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 292 ms: 1.11x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.84 ms: 1.02x slower                                                  |
| docutils       | 2.66 sec                                               | 2.82 sec: 1.06x slower                                                 |
| tornado_http   | 98.1 ms                                                | 99.5 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.05x slower                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 444 ms: 1.19x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 602 ms: 1.04x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 91.4 ms: 1.16x slower                                                  |
| nbody          | 96.0 ms                                                | 117 ms: 1.21x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.57 ms: 1.02x slower                                                  |
| regex_dna      | 205 ms                                                 | 221 ms: 1.08x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| regex_compile  | 141 ms                                                 | 173 ms: 1.22x slower                                                   |
| Geometric mean | (ref)                                                  | 1.10x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| json_loads           | 29.2 us                                                | 27.2 us: 1.07x faster                                                  |
| pickle_pure_python   | 320 us                                                 | 304 us: 1.05x faster                                                   |
| unpickle_list        | 5.21 us                                                | 4.99 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| tomli_loads          | 2.30 sec                                               | 2.45 sec: 1.06x slower                                                 |
| pickle               | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 60.8 ms: 1.07x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                  |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| unpickle_pure_python | 242 us                                                 | 278 us: 1.15x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 13.0 ms: 1.22x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240305-linux-x86_64-python-cbf3d38cbeb6e640d595-3.13.0a4+-cbf3d38 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 115 us: 4.51x faster                                                   |
| generators                 | 74.9 ms                                                | 29.6 ms: 2.53x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 482 ms: 1.82x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.72x faster                                                 |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.1 ms: 1.22x faster                                                  |
| async_tree_none            | 528 ms                                                 | 444 ms: 1.19x faster                                                   |
| comprehensions             | 23.6 us                                                | 20.8 us: 1.13x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 572 ms: 1.12x faster                                                   |
| logging_silent             | 111 ns                                                 | 100 ns: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 455 ms: 1.08x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.2 us: 1.07x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.68 ms: 1.07x faster                                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| deepcopy_reduce            | 3.22 us                                                | 3.05 us: 1.06x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 304 us: 1.05x faster                                                   |
| unpickle_list              | 5.21 us                                                | 4.99 us: 1.05x faster                                                  |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 717 ms: 1.04x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 158 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 732 ms: 1.04x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 602 ms: 1.04x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.67 sec: 1.04x faster                                                 |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                   |
| logging_simple             | 6.22 us                                                | 6.04 us: 1.03x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                                   |
| json                       | 5.24 ms                                                | 5.10 ms: 1.03x faster                                                  |
| deepcopy                   | 365 us                                                 | 358 us: 1.02x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 111 ms: 1.01x faster                                                   |
| richards_super             | 61.9 ms                                                | 61.2 ms: 1.01x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.42 ms: 1.01x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 4.03 ms: 1.00x slower                                                  |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                                   |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| tornado_http               | 98.1 ms                                                | 99.5 ms: 1.01x slower                                                  |
| deepcopy_memo              | 40.2 us                                                | 40.8 us: 1.02x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.57 ms: 1.02x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.84 ms: 1.02x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 853 us: 1.02x slower                                                   |
| chaos                      | 71.9 ms                                                | 73.6 ms: 1.02x slower                                                  |
| pathlib                    | 18.5 ms                                                | 19.0 ms: 1.03x slower                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 111 ms: 1.03x slower                                                   |
| sympy_expand               | 484 ms                                                 | 502 ms: 1.04x slower                                                   |
| meteor_contest             | 109 ms                                                 | 115 ms: 1.05x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.51 ms: 1.05x slower                                                  |
| docutils                   | 2.66 sec                                               | 2.82 sec: 1.06x slower                                                 |
| tomli_loads                | 2.30 sec                                               | 2.45 sec: 1.06x slower                                                 |
| pickle                     | 11.0 us                                                | 11.7 us: 1.07x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 60.8 ms: 1.07x slower                                                  |
| regex_dna                  | 205 ms                                                 | 221 ms: 1.08x slower                                                   |
| sqlglot_optimize           | 55.3 ms                                                | 60.2 ms: 1.09x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 88.8 ms: 1.10x slower                                                  |
| crypto_pyaes               | 76.7 ms                                                | 84.2 ms: 1.10x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 71.1 ms: 1.10x slower                                                  |
| raytrace                   | 309 ms                                                 | 340 ms: 1.10x slower                                                   |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.11x slower                                                  |
| 2to3                       | 264 ms                                                 | 292 ms: 1.11x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.11x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.31 sec: 1.11x slower                                                 |
| richards                   | 49.8 ms                                                | 55.1 ms: 1.11x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| nqueens                    | 87.9 ms                                                | 97.8 ms: 1.11x slower                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.75 sec: 1.12x slower                                                 |
| pprint_safe_repr           | 747 ms                                                 | 843 ms: 1.13x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.91 us: 1.13x slower                                                  |
| unpickle_pure_python       | 242 us                                                 | 278 us: 1.15x slower                                                   |
| float                      | 78.9 ms                                                | 91.4 ms: 1.16x slower                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.85 ms: 1.16x slower                                                  |
| fannkuch                   | 405 ms                                                 | 473 ms: 1.17x slower                                                   |
| scimark_sor                | 121 ms                                                 | 142 ms: 1.17x slower                                                   |
| go                         | 149 ms                                                 | 175 ms: 1.18x slower                                                   |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 85.5 ms: 1.21x slower                                                  |
| nbody                      | 96.0 ms                                                | 117 ms: 1.21x slower                                                   |
| mako                       | 10.7 ms                                                | 13.0 ms: 1.22x slower                                                  |
| regex_compile              | 141 ms                                                 | 173 ms: 1.22x slower                                                   |
| coverage                   | 78.8 ms                                                | 96.9 ms: 1.23x slower                                                  |
| async_generators           | 374 ms                                                 | 463 ms: 1.24x slower                                                   |
| scimark_fft                | 345 ms                                                 | 433 ms: 1.25x slower                                                   |
| spectral_norm              | 108 ms                                                 | 136 ms: 1.25x slower                                                   |
| telco                      | 6.86 ms                                                | 8.62 ms: 1.26x slower                                                  |
| mypy2                      | 686 ms                                                 | 892 ms: 1.30x slower                                                   |
| hexiom                     | 6.89 ms                                                | 9.02 ms: 1.31x slower                                                  |
| pyflate                    | 434 ms                                                 | 586 ms: 1.35x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 157 ms: 1.35x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 58.9 ns: 1.36x slower                                                  |
| dask                       | 365 ms                                                 | 536 ms: 1.47x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.83 ms: 1.47x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x slower                                                           |

Benchmark hidden because not significant (4): logging_format, sqlglot_transpile, bench_mp_pool, sympy_str
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.60% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: 1.00x