
# Results vs. 3.11.0

- fork: python
- ref: v3.11.7
- machine: linux-x86_64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.01x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.00x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 261 ms: 1.01x faster                                   |
| chameleon      | 6.70 ms                                                | 7.03 ms: 1.05x slower                                  |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.6 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none_tg         | 491 ms                                                 | 479 ms: 1.03x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 614 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 748 ms: 1.02x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.29 sec: 1.01x faster                                 |
| async_tree_none            | 528 ms                                                 | 533 ms: 1.01x slower                                   |
| async_tree_memoization     | 639 ms                                                 | 650 ms: 1.02x slower                                   |
| async_tree_io              | 1.29 sec                                               | 1.31 sec: 1.02x slower                                 |
| Geometric mean             | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| nbody          | 96.0 ms                                                | 93.5 ms: 1.03x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.43 ms: 1.02x faster                                  |
| regex_dna      | 205 ms                                                 | 209 ms: 1.02x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 25.8 us: 1.13x faster                                  |
| unpickle_pure_python | 242 us                                                 | 239 us: 1.01x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 163 ms: 1.01x faster                                   |
| pickle_pure_python   | 320 us                                                 | 317 us: 1.01x faster                                   |
| json_dumps           | 13.3 ms                                                | 13.2 ms: 1.01x faster                                  |
| xml_etree_process    | 56.9 ms                                                | 56.6 ms: 1.00x faster                                  |
| unpickle_list        | 5.21 us                                                | 5.23 us: 1.00x slower                                  |
| unpickle             | 13.8 us                                                | 14.1 us: 1.02x slower                                  |
| pickle_list          | 4.59 us                                                | 4.69 us: 1.02x slower                                  |
| pickle_dict          | 34.6 us                                                | 36.1 us: 1.04x slower                                  |
| Geometric mean       | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (4): xml_etree_generate, xml_etree_iterparse, pickle, tomli_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.59 ms: 1.00x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 6.04 ms: 1.00x slower                                  |
| Geometric mean         | (ref)                                                  | 1.00x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.0 ms: 1.01x slower                                  |
| genshi_text     | 22.5 ms                                                | 23.1 ms: 1.02x slower                                  |
| mako            | 10.7 ms                                                | 11.1 ms: 1.04x slower                                  |
| Geometric mean  | (ref)                                                  | 1.02x slower                                           |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads                 | 29.2 us                                                | 25.8 us: 1.13x faster                                  |
| gc_traversal               | 4.01 ms                                                | 3.74 ms: 1.07x faster                                  |
| json                       | 5.24 ms                                                | 4.94 ms: 1.06x faster                                  |
| logging_silent             | 111 ns                                                 | 106 ns: 1.05x faster                                   |
| richards                   | 49.8 ms                                                | 47.6 ms: 1.05x faster                                  |
| pycparser                  | 1.19 sec                                               | 1.14 sec: 1.04x faster                                 |
| richards_super             | 61.9 ms                                                | 59.5 ms: 1.04x faster                                  |
| go                         | 149 ms                                                 | 143 ms: 1.04x faster                                   |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.10 us: 1.04x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.79 ms: 1.04x faster                                  |
| djangocms                  | 33.5 us                                                | 32.4 us: 1.03x faster                                  |
| nqueens                    | 87.9 ms                                                | 85.2 ms: 1.03x faster                                  |
| async_generators           | 374 ms                                                 | 362 ms: 1.03x faster                                   |
| regex_compile              | 141 ms                                                 | 137 ms: 1.03x faster                                   |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| deepcopy                   | 365 us                                                 | 355 us: 1.03x faster                                   |
| pylint                     | 476 ms                                                 | 462 ms: 1.03x faster                                   |
| docutils                   | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| nbody                      | 96.0 ms                                                | 93.5 ms: 1.03x faster                                  |
| async_tree_none_tg         | 491 ms                                                 | 479 ms: 1.03x faster                                   |
| sqlalchemy_imperative      | 18.3 ms                                                | 17.9 ms: 1.02x faster                                  |
| pyflate                    | 434 ms                                                 | 424 ms: 1.02x faster                                   |
| mdp                        | 2.77 sec                                               | 2.71 sec: 1.02x faster                                 |
| pprint_pformat             | 1.55 sec                                               | 1.52 sec: 1.02x faster                                 |
| coroutines                 | 27.0 ms                                                | 26.4 ms: 1.02x faster                                  |
| comprehensions             | 23.6 us                                                | 23.1 us: 1.02x faster                                  |
| gunicorn                   | 1.20 ms                                                | 1.17 ms: 1.02x faster                                  |
| regex_effbot               | 3.51 ms                                                | 3.43 ms: 1.02x faster                                  |
| sympy_sum                  | 169 ms                                                 | 165 ms: 1.02x faster                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 614 ms: 1.02x faster                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.72 ms: 1.02x faster                                  |
| sqlalchemy_declarative     | 140 ms                                                 | 138 ms: 1.02x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 748 ms: 1.02x faster                                   |
| hexiom                     | 6.89 ms                                                | 6.77 ms: 1.02x faster                                  |
| pprint_safe_repr           | 747 ms                                                 | 735 ms: 1.02x faster                                   |
| chaos                      | 71.9 ms                                                | 70.8 ms: 1.02x faster                                  |
| flaskblogging              | 7.28 ms                                                | 7.18 ms: 1.01x faster                                  |
| tornado_http               | 98.1 ms                                                | 96.6 ms: 1.01x faster                                  |
| typing_runtime_protocols   | 520 us                                                 | 512 us: 1.01x faster                                   |
| aiohttp                    | 1.12 ms                                                | 1.10 ms: 1.01x faster                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.42 ms: 1.01x faster                                  |
| fannkuch                   | 405 ms                                                 | 400 ms: 1.01x faster                                   |
| 2to3                       | 264 ms                                                 | 261 ms: 1.01x faster                                   |
| mypy2                      | 686 ms                                                 | 679 ms: 1.01x faster                                   |
| unpickle_pure_python       | 242 us                                                 | 239 us: 1.01x faster                                   |
| telco                      | 6.86 ms                                                | 6.79 ms: 1.01x faster                                  |
| xml_etree_parse            | 164 ms                                                 | 163 ms: 1.01x faster                                   |
| deepcopy_memo              | 40.2 us                                                | 39.8 us: 1.01x faster                                  |
| sympy_str                  | 297 ms                                                 | 295 ms: 1.01x faster                                   |
| raytrace                   | 309 ms                                                 | 306 ms: 1.01x faster                                   |
| pickle_pure_python         | 320 us                                                 | 317 us: 1.01x faster                                   |
| logging_format             | 6.81 us                                                | 6.76 us: 1.01x faster                                  |
| async_tree_io_tg           | 1.29 sec                                               | 1.29 sec: 1.01x faster                                 |
| json_dumps                 | 13.3 ms                                                | 13.2 ms: 1.01x faster                                  |
| logging_simple             | 6.22 us                                                | 6.18 us: 1.01x faster                                  |
| scimark_lu                 | 116 ms                                                 | 116 ms: 1.01x faster                                   |
| sqlglot_optimize           | 55.3 ms                                                | 55.0 ms: 1.01x faster                                  |
| pathlib                    | 18.5 ms                                                | 18.4 ms: 1.01x faster                                  |
| sqlglot_normalize          | 113 ms                                                 | 112 ms: 1.01x faster                                   |
| crypto_pyaes               | 76.7 ms                                                | 76.3 ms: 1.00x faster                                  |
| xml_etree_process          | 56.9 ms                                                | 56.6 ms: 1.00x faster                                  |
| bench_thread_pool          | 834 us                                                 | 831 us: 1.00x faster                                   |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x faster                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 3.10 sec: 1.00x faster                                 |
| python_startup             | 8.56 ms                                                | 8.59 ms: 1.00x slower                                  |
| unpickle_list              | 5.21 us                                                | 5.23 us: 1.00x slower                                  |
| python_startup_no_site     | 6.01 ms                                                | 6.04 ms: 1.00x slower                                  |
| asyncio_tcp                | 875 ms                                                 | 880 ms: 1.01x slower                                   |
| generators                 | 74.9 ms                                                | 75.5 ms: 1.01x slower                                  |
| async_tree_none            | 528 ms                                                 | 533 ms: 1.01x slower                                   |
| coverage                   | 78.8 ms                                                | 79.5 ms: 1.01x slower                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.45 ms: 1.01x slower                                  |
| django_template            | 33.5 ms                                                | 34.0 ms: 1.01x slower                                  |
| thrift                     | 784 us                                                 | 797 us: 1.02x slower                                   |
| async_tree_memoization     | 639 ms                                                 | 650 ms: 1.02x slower                                   |
| scimark_sor                | 121 ms                                                 | 123 ms: 1.02x slower                                   |
| async_tree_io              | 1.29 sec                                               | 1.31 sec: 1.02x slower                                 |
| unpickle                   | 13.8 us                                                | 14.1 us: 1.02x slower                                  |
| sympy_expand               | 484 ms                                                 | 495 ms: 1.02x slower                                   |
| pickle_list                | 4.59 us                                                | 4.69 us: 1.02x slower                                  |
| regex_dna                  | 205 ms                                                 | 209 ms: 1.02x slower                                   |
| genshi_text                | 22.5 ms                                                | 23.1 ms: 1.02x slower                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 72.8 ms: 1.03x slower                                  |
| mako                       | 10.7 ms                                                | 11.1 ms: 1.04x slower                                  |
| pickle_dict                | 34.6 us                                                | 36.1 us: 1.04x slower                                  |
| chameleon                  | 6.70 ms                                                | 7.03 ms: 1.05x slower                                  |
| unpack_sequence            | 43.5 ns                                                | 47.9 ns: 1.10x slower                                  |
| Geometric mean             | (ref)                                                  | 1.01x faster                                           |

Benchmark hidden because not significant (17): dask, spectral_norm, dulwich_log, scimark_fft, html5lib, xml_etree_generate, bench_mp_pool, asyncio_websockets, regex_v8, async_tree_cpu_io_mixed, float, xml_etree_iterparse, pickle, genshi_xml, tomli_loads, sqlite_synth, scimark_sparse_mat_mult


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.00x