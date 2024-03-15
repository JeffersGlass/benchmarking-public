
# Results vs. 3.11.0

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.03x faster
- HPT reliability: 74.91%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 274 ms: 1.04x slower                                   |
| chameleon      | 6.70 ms                                                | 7.24 ms: 1.08x slower                                  |
| docutils       | 2.66 sec                                               | 2.71 sec: 1.02x slower                                 |
| tornado_http   | 98.1 ms                                                | 99.4 ms: 1.01x slower                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 475 ms: 1.11x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| async_tree_memoization     | 639 ms                                                 | 582 ms: 1.10x faster                                   |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 583 ms: 1.07x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                   |
| Geometric mean             | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| nbody          | 96.0 ms                                                | 93.2 ms: 1.03x faster                                  |
| float          | 78.9 ms                                                | 84.6 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 22.8 ms: 1.00x faster                                  |
| regex_dna      | 205 ms                                                 | 205 ms: 1.00x slower                                   |
| regex_effbot   | 3.51 ms                                                | 3.58 ms: 1.02x slower                                  |
| regex_compile  | 141 ms                                                 | 145 ms: 1.03x slower                                   |
| Geometric mean | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| unpickle_pure_python | 242 us                                                 | 231 us: 1.05x faster                                   |
| unpickle_list        | 5.21 us                                                | 4.99 us: 1.05x faster                                  |
| pickle_dict          | 34.6 us                                                | 33.1 us: 1.04x faster                                  |
| json_loads           | 29.2 us                                                | 28.0 us: 1.04x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.03x faster                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| tomli_loads          | 2.30 sec                                               | 2.29 sec: 1.01x faster                                 |
| pickle_pure_python   | 320 us                                                 | 322 us: 1.01x slower                                   |
| pickle               | 11.0 us                                                | 11.4 us: 1.04x slower                                  |
| pickle_list          | 4.59 us                                                | 4.93 us: 1.08x slower                                  |
| xml_etree_process    | 56.9 ms                                                | 61.2 ms: 1.08x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 88.2 ms: 1.09x slower                                  |
| unpickle             | 13.8 us                                                | 15.7 us: 1.13x slower                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.44 ms: 1.10x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 6.81 ms: 1.13x slower                                  |
| Geometric mean         | (ref)                                                  | 1.12x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 33.5 ms                                                | 34.7 ms: 1.04x slower                                  |
| mako            | 10.7 ms                                                | 11.3 ms: 1.06x slower                                  |
| Geometric mean  | (ref)                                                  | 1.05x slower                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 121 us: 4.30x faster                                   |
| generators                 | 74.9 ms                                                | 31.7 ms: 2.36x faster                                  |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                 |
| asyncio_tcp                | 875 ms                                                 | 510 ms: 1.72x faster                                   |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                  |
| richards_super             | 61.9 ms                                                | 52.0 ms: 1.19x faster                                  |
| coroutines                 | 27.0 ms                                                | 23.3 ms: 1.16x faster                                  |
| comprehensions             | 23.6 us                                                | 20.9 us: 1.13x faster                                  |
| async_tree_none            | 528 ms                                                 | 475 ms: 1.11x faster                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                 |
| async_tree_memoization     | 639 ms                                                 | 582 ms: 1.10x faster                                   |
| richards                   | 49.8 ms                                                | 45.8 ms: 1.09x faster                                  |
| async_tree_none_tg         | 491 ms                                                 | 452 ms: 1.09x faster                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                 |
| chaos                      | 71.9 ms                                                | 66.8 ms: 1.08x faster                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 583 ms: 1.07x faster                                   |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                   |
| mdp                        | 2.77 sec                                               | 2.61 sec: 1.06x faster                                 |
| go                         | 149 ms                                                 | 140 ms: 1.06x faster                                   |
| coverage                   | 78.8 ms                                                | 75.2 ms: 1.05x faster                                  |
| unpickle_pure_python       | 242 us                                                 | 231 us: 1.05x faster                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 727 ms: 1.05x faster                                   |
| unpickle_list              | 5.21 us                                                | 4.99 us: 1.05x faster                                  |
| nqueens                    | 87.9 ms                                                | 84.2 ms: 1.04x faster                                  |
| pickle_dict                | 34.6 us                                                | 33.1 us: 1.04x faster                                  |
| hexiom                     | 6.89 ms                                                | 6.60 ms: 1.04x faster                                  |
| deltablue                  | 3.92 ms                                                | 3.76 ms: 1.04x faster                                  |
| json_loads                 | 29.2 us                                                | 28.0 us: 1.04x faster                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.38 ms: 1.04x faster                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 725 ms: 1.03x faster                                   |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| nbody                      | 96.0 ms                                                | 93.2 ms: 1.03x faster                                  |
| sympy_sum                  | 169 ms                                                 | 164 ms: 1.03x faster                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.70 ms: 1.03x faster                                  |
| xml_etree_parse            | 164 ms                                                 | 160 ms: 1.03x faster                                   |
| deepcopy_memo              | 40.2 us                                                | 39.2 us: 1.02x faster                                  |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                   |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.02x faster                                   |
| gc_traversal               | 4.01 ms                                                | 3.93 ms: 1.02x faster                                  |
| sympy_expand               | 484 ms                                                 | 477 ms: 1.02x faster                                   |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.01x faster                                 |
| sqlglot_optimize           | 55.3 ms                                                | 54.7 ms: 1.01x faster                                  |
| sympy_str                  | 297 ms                                                 | 294 ms: 1.01x faster                                   |
| tomli_loads                | 2.30 sec                                               | 2.29 sec: 1.01x faster                                 |
| json                       | 5.24 ms                                                | 5.20 ms: 1.01x faster                                  |
| regex_v8                   | 22.9 ms                                                | 22.8 ms: 1.00x faster                                  |
| bench_thread_pool          | 834 us                                                 | 836 us: 1.00x slower                                   |
| regex_dna                  | 205 ms                                                 | 205 ms: 1.00x slower                                   |
| pprint_pformat             | 1.55 sec                                               | 1.56 sec: 1.00x slower                                 |
| pickle_pure_python         | 320 us                                                 | 322 us: 1.01x slower                                   |
| fannkuch                   | 405 ms                                                 | 409 ms: 1.01x slower                                   |
| scimark_lu                 | 116 ms                                                 | 118 ms: 1.01x slower                                   |
| tornado_http               | 98.1 ms                                                | 99.4 ms: 1.01x slower                                  |
| dask                       | 365 ms                                                 | 370 ms: 1.01x slower                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.01x slower                                  |
| mypy2                      | 686 ms                                                 | 696 ms: 1.02x slower                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.27 us: 1.02x slower                                  |
| docutils                   | 2.66 sec                                               | 2.71 sec: 1.02x slower                                 |
| regex_effbot               | 3.51 ms                                                | 3.58 ms: 1.02x slower                                  |
| pprint_safe_repr           | 747 ms                                                 | 764 ms: 1.02x slower                                   |
| sqlalchemy_imperative      | 18.3 ms                                                | 18.8 ms: 1.02x slower                                  |
| aiohttp                    | 1.12 ms                                                | 1.14 ms: 1.02x slower                                  |
| regex_compile              | 141 ms                                                 | 145 ms: 1.03x slower                                   |
| 2to3                       | 264 ms                                                 | 274 ms: 1.04x slower                                   |
| django_template            | 33.5 ms                                                | 34.7 ms: 1.04x slower                                  |
| gunicorn                   | 1.20 ms                                                | 1.24 ms: 1.04x slower                                  |
| pickle                     | 11.0 us                                                | 11.4 us: 1.04x slower                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.23 ms: 1.04x slower                                  |
| sqlalchemy_declarative     | 140 ms                                                 | 146 ms: 1.04x slower                                   |
| logging_simple             | 6.22 us                                                | 6.47 us: 1.04x slower                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 74.3 ms: 1.05x slower                                  |
| telco                      | 6.86 ms                                                | 7.23 ms: 1.05x slower                                  |
| logging_format             | 6.81 us                                                | 7.21 us: 1.06x slower                                  |
| dulwich_log                | 64.6 ms                                                | 68.4 ms: 1.06x slower                                  |
| mako                       | 10.7 ms                                                | 11.3 ms: 1.06x slower                                  |
| pyflate                    | 434 ms                                                 | 460 ms: 1.06x slower                                   |
| float                      | 78.9 ms                                                | 84.6 ms: 1.07x slower                                  |
| pickle_list                | 4.59 us                                                | 4.93 us: 1.08x slower                                  |
| xml_etree_process          | 56.9 ms                                                | 61.2 ms: 1.08x slower                                  |
| spectral_norm              | 108 ms                                                 | 116 ms: 1.08x slower                                   |
| chameleon                  | 6.70 ms                                                | 7.24 ms: 1.08x slower                                  |
| xml_etree_generate         | 81.1 ms                                                | 88.2 ms: 1.09x slower                                  |
| scimark_sor                | 121 ms                                                 | 132 ms: 1.09x slower                                   |
| scimark_fft                | 345 ms                                                 | 376 ms: 1.09x slower                                   |
| crypto_pyaes               | 76.7 ms                                                | 83.5 ms: 1.09x slower                                  |
| python_startup             | 8.56 ms                                                | 9.44 ms: 1.10x slower                                  |
| sqlite_synth               | 2.57 us                                                | 2.84 us: 1.11x slower                                  |
| unpickle                   | 13.8 us                                                | 15.7 us: 1.13x slower                                  |
| python_startup_no_site     | 6.01 ms                                                | 6.81 ms: 1.13x slower                                  |
| unpack_sequence            | 43.5 ns                                                | 53.0 ns: 1.22x slower                                  |
| async_generators           | 374 ms                                                 | 456 ms: 1.22x slower                                   |
| Geometric mean             | (ref)                                                  | 1.03x faster                                           |

Benchmark hidden because not significant (6): raytrace, meteor_contest, bench_mp_pool, pathlib, deepcopy, asyncio_websockets
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 74.91% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x