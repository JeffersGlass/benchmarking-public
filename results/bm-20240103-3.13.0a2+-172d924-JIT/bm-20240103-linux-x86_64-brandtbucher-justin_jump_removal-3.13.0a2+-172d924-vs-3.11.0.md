
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jump_removal
- machine: linux-x86_64
- commit hash: 172d924
- commit date: 2024-01-03
- overall geometric mean: 1.03x faster
- HPT reliability: 90.72%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 274 ms: 1.04x slower                                                        |
| chameleon      | 6.70 ms                                                | 7.00 ms: 1.04x slower                                                       |
| docutils       | 2.66 sec                                               | 2.65 sec: 1.00x faster                                                      |
| tornado_http   | 98.1 ms                                                | 96.6 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                  | 1.02x slower                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 441 ms: 1.20x faster                                                        |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                        |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                      |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                      |
| async_tree_memoization_tg  | 626 ms                                                 | 582 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                        |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                        |
| float          | 78.9 ms                                                | 84.3 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                  | 1.01x slower                                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 139 ms: 1.01x faster                                                        |
| regex_effbot   | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                       |
| regex_dna      | 205 ms                                                 | 222 ms: 1.09x slower                                                        |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                  | 1.06x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                       |
| unpickle_pure_python | 242 us                                                 | 226 us: 1.07x faster                                                        |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                        |
| tomli_loads          | 2.30 sec                                               | 2.16 sec: 1.06x faster                                                      |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                        |
| json_loads           | 29.2 us                                                | 28.6 us: 1.02x faster                                                       |
| pickle_dict          | 34.6 us                                                | 34.4 us: 1.01x faster                                                       |
| unpickle_list        | 5.21 us                                                | 5.37 us: 1.03x slower                                                       |
| xml_etree_process    | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                       |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                       |
| xml_etree_generate   | 81.1 ms                                                | 86.9 ms: 1.07x slower                                                       |
| pickle_list          | 4.59 us                                                | 5.03 us: 1.10x slower                                                       |
| unpickle             | 13.8 us                                                | 15.3 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                       |
| python_startup_no_site | 6.01 ms                                                | 8.86 ms: 1.47x slower                                                       |
| Geometric mean         | (ref)                                                  | 1.33x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.67x faster                                                        |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                       |
| asyncio_tcp                | 875 ms                                                 | 487 ms: 1.80x faster                                                        |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                                      |
| comprehensions             | 23.6 us                                                | 18.3 us: 1.29x faster                                                       |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                       |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                       |
| async_tree_none            | 528 ms                                                 | 441 ms: 1.20x faster                                                        |
| richards_super             | 61.9 ms                                                | 52.0 ms: 1.19x faster                                                       |
| async_tree_memoization     | 639 ms                                                 | 570 ms: 1.12x faster                                                        |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                       |
| raytrace                   | 309 ms                                                 | 280 ms: 1.10x faster                                                        |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                        |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                      |
| richards                   | 49.8 ms                                                | 45.6 ms: 1.09x faster                                                       |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                      |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                       |
| chaos                      | 71.9 ms                                                | 66.8 ms: 1.08x faster                                                       |
| async_tree_memoization_tg  | 626 ms                                                 | 582 ms: 1.08x faster                                                        |
| mdp                        | 2.77 sec                                               | 2.59 sec: 1.07x faster                                                      |
| unpickle_pure_python       | 242 us                                                 | 226 us: 1.07x faster                                                        |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                        |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                                       |
| sympy_sum                  | 169 ms                                                 | 158 ms: 1.07x faster                                                        |
| tomli_loads                | 2.30 sec                                               | 2.16 sec: 1.06x faster                                                      |
| logging_format             | 6.81 us                                                | 6.42 us: 1.06x faster                                                       |
| logging_simple             | 6.22 us                                                | 5.92 us: 1.05x faster                                                       |
| sympy_str                  | 297 ms                                                 | 283 ms: 1.05x faster                                                        |
| logging_silent             | 111 ns                                                 | 106 ns: 1.04x faster                                                        |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 720 ms: 1.04x faster                                                        |
| deepcopy                   | 365 us                                                 | 351 us: 1.04x faster                                                        |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                        |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 733 ms: 1.04x faster                                                        |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                        |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                        |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                                       |
| deepcopy_reduce            | 3.22 us                                                | 3.12 us: 1.03x faster                                                       |
| deepcopy_memo              | 40.2 us                                                | 39.2 us: 1.02x faster                                                       |
| json_loads                 | 29.2 us                                                | 28.6 us: 1.02x faster                                                       |
| sympy_expand               | 484 ms                                                 | 474 ms: 1.02x faster                                                        |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.02x faster                                                      |
| tornado_http               | 98.1 ms                                                | 96.6 ms: 1.01x faster                                                       |
| regex_compile              | 141 ms                                                 | 139 ms: 1.01x faster                                                        |
| scimark_lu                 | 116 ms                                                 | 115 ms: 1.01x faster                                                        |
| pickle_dict                | 34.6 us                                                | 34.4 us: 1.01x faster                                                       |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.00x faster                                                       |
| docutils                   | 2.66 sec                                               | 2.65 sec: 1.00x faster                                                      |
| asyncio_websockets         | 550 ms                                                 | 553 ms: 1.00x slower                                                        |
| go                         | 149 ms                                                 | 149 ms: 1.01x slower                                                        |
| bench_thread_pool          | 834 us                                                 | 843 us: 1.01x slower                                                        |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.02x slower                                                        |
| nqueens                    | 87.9 ms                                                | 89.4 ms: 1.02x slower                                                       |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.14 ms: 1.02x slower                                                       |
| meteor_contest             | 109 ms                                                 | 112 ms: 1.03x slower                                                        |
| unpickle_list              | 5.21 us                                                | 5.37 us: 1.03x slower                                                       |
| dulwich_log                | 64.6 ms                                                | 66.9 ms: 1.04x slower                                                       |
| 2to3                       | 264 ms                                                 | 274 ms: 1.04x slower                                                        |
| xml_etree_process          | 56.9 ms                                                | 59.1 ms: 1.04x slower                                                       |
| create_gc_cycles           | 1.43 ms                                                | 1.50 ms: 1.04x slower                                                       |
| chameleon                  | 6.70 ms                                                | 7.00 ms: 1.04x slower                                                       |
| regex_effbot               | 3.51 ms                                                | 3.68 ms: 1.05x slower                                                       |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                       |
| fannkuch                   | 405 ms                                                 | 426 ms: 1.05x slower                                                        |
| scimark_monte_carlo        | 70.7 ms                                                | 74.4 ms: 1.05x slower                                                       |
| pprint_safe_repr           | 747 ms                                                 | 788 ms: 1.05x slower                                                        |
| pprint_pformat             | 1.55 sec                                               | 1.65 sec: 1.06x slower                                                      |
| scimark_fft                | 345 ms                                                 | 367 ms: 1.06x slower                                                        |
| float                      | 78.9 ms                                                | 84.3 ms: 1.07x slower                                                       |
| xml_etree_generate         | 81.1 ms                                                | 86.9 ms: 1.07x slower                                                       |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.09x slower                                                        |
| pickle_list                | 4.59 us                                                | 5.03 us: 1.10x slower                                                       |
| hexiom                     | 6.89 ms                                                | 7.58 ms: 1.10x slower                                                       |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.10x slower                                                       |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.10x slower                                                       |
| regex_v8                   | 22.9 ms                                                | 25.3 ms: 1.10x slower                                                       |
| mako                       | 10.7 ms                                                | 12.1 ms: 1.13x slower                                                       |
| unpack_sequence            | 43.5 ns                                                | 49.7 ns: 1.14x slower                                                       |
| pyflate                    | 434 ms                                                 | 502 ms: 1.16x slower                                                        |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                                       |
| coverage                   | 78.8 ms                                                | 94.6 ms: 1.20x slower                                                       |
| spectral_norm              | 108 ms                                                 | 131 ms: 1.21x slower                                                        |
| async_generators           | 374 ms                                                 | 452 ms: 1.21x slower                                                        |
| telco                      | 6.86 ms                                                | 8.60 ms: 1.25x slower                                                       |
| mypy2                      | 686 ms                                                 | 863 ms: 1.26x slower                                                        |
| python_startup_no_site     | 6.01 ms                                                | 8.86 ms: 1.47x slower                                                       |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                                |

Benchmark hidden because not significant (8): deltablue, nbody, json, bench_mp_pool, dask, sqlglot_optimize, xml_etree_iterparse, crypto_pyaes
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 90.72% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x