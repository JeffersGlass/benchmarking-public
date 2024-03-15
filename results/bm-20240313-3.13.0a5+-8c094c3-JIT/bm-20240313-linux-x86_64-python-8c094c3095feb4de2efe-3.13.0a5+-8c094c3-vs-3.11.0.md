# Results vs. 3.11.0

- fork: python
- ref: 8c094c3095feb4de2efe
- machine: linux-x86_64
- commit hash: 8c094c3
- commit date: 2024-03-13
- overall geometric mean: 1.02x faster
- HPT reliability: 54.85%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| chameleon      | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| docutils       | 2.66 sec                                               | 2.77 sec: 1.04x slower                                                 |
| tornado_http   | 98.1 ms                                                | 98.7 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.03x slower                                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 92.4 ms: 1.04x faster                                                  |
| pidigits       | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| float          | 78.9 ms                                                | 79.8 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                                   |
| regex_effbot   | 3.51 ms                                                | 3.82 ms: 1.09x slower                                                  |
| regex_v8       | 22.9 ms                                                | 25.4 ms: 1.11x slower                                                  |
| regex_dna      | 205 ms                                                 | 238 ms: 1.16x slower                                                   |
| Geometric mean | (ref)                                                  | 1.09x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| tomli_loads          | 2.30 sec                                               | 2.08 sec: 1.11x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                                   |
| unpickle_list        | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| json_loads           | 29.2 us                                                | 27.9 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| unpickle_pure_python | 242 us                                                 | 239 us: 1.01x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| pickle_dict          | 34.6 us                                                | 35.4 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 86.8 ms: 1.07x slower                                                  |
| pickle               | 11.0 us                                                | 12.0 us: 1.09x slower                                                  |
| unpickle             | 13.8 us                                                | 15.1 us: 1.09x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.31 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.66x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 10.7 ms                                                | 10.7 ms: 1.00x slower                                                  |
| django_template | 33.5 ms                                                | 34.4 ms: 1.03x slower                                                  |
| genshi_xml      | 53.4 ms                                                | 54.9 ms: 1.03x slower                                                  |
| genshi_text     | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                  |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                           |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.70x faster                                                   |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 503 ms: 1.74x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.85 sec: 1.68x faster                                                 |
| pylint                     | 476 ms                                                 | 324 ms: 1.47x faster                                                   |
| comprehensions             | 23.6 us                                                | 17.3 us: 1.36x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.7 ms: 1.19x faster                                                  |
| richards_super             | 61.9 ms                                                | 52.2 ms: 1.19x faster                                                  |
| async_tree_none            | 528 ms                                                 | 449 ms: 1.18x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.44 ms: 1.14x faster                                                  |
| chaos                      | 71.9 ms                                                | 64.1 ms: 1.12x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.08 sec: 1.11x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 577 ms: 1.11x faster                                                   |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                   |
| sqlglot_parse              | 1.43 ms                                                | 1.31 ms: 1.09x faster                                                  |
| richards                   | 49.8 ms                                                | 46.5 ms: 1.07x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 459 ms: 1.07x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.86 us: 1.06x faster                                                  |
| pickle_pure_python         | 320 us                                                 | 302 us: 1.06x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.22 sec: 1.06x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.93 us: 1.06x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 592 ms: 1.06x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.66 ms: 1.06x faster                                                  |
| logging_format             | 6.81 us                                                | 6.46 us: 1.05x faster                                                  |
| raytrace                   | 309 ms                                                 | 294 ms: 1.05x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.24 sec: 1.05x faster                                                 |
| json_loads                 | 29.2 us                                                | 27.9 us: 1.05x faster                                                  |
| djangocms                  | 33.5 us                                                | 32.2 us: 1.04x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 108 ms: 1.04x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                                  |
| nbody                      | 96.0 ms                                                | 92.4 ms: 1.04x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 163 ms: 1.04x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 724 ms: 1.04x faster                                                   |
| deepcopy                   | 365 us                                                 | 354 us: 1.03x faster                                                   |
| sympy_str                  | 297 ms                                                 | 288 ms: 1.03x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 740 ms: 1.03x faster                                                   |
| fannkuch                   | 405 ms                                                 | 395 ms: 1.03x faster                                                   |
| pidigits                   | 194 ms                                                 | 189 ms: 1.03x faster                                                   |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.91 ms: 1.02x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 39.5 us: 1.02x faster                                                  |
| json                       | 5.24 ms                                                | 5.16 ms: 1.02x faster                                                  |
| crypto_pyaes               | 76.7 ms                                                | 75.6 ms: 1.02x faster                                                  |
| gc_traversal               | 4.01 ms                                                | 3.95 ms: 1.01x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 239 us: 1.01x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 21.2 ms: 1.01x faster                                                  |
| scimark_monte_carlo        | 70.7 ms                                                | 70.1 ms: 1.01x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                 |
| xml_etree_iterparse        | 108 ms                                                 | 107 ms: 1.01x faster                                                   |
| scimark_fft                | 345 ms                                                 | 343 ms: 1.01x faster                                                   |
| mako                       | 10.7 ms                                                | 10.7 ms: 1.00x slower                                                  |
| sympy_expand               | 484 ms                                                 | 487 ms: 1.01x slower                                                   |
| tornado_http               | 98.1 ms                                                | 98.7 ms: 1.01x slower                                                  |
| meteor_contest             | 109 ms                                                 | 110 ms: 1.01x slower                                                   |
| float                      | 78.9 ms                                                | 79.8 ms: 1.01x slower                                                  |
| pathlib                    | 18.5 ms                                                | 18.8 ms: 1.01x slower                                                  |
| regex_compile              | 141 ms                                                 | 144 ms: 1.02x slower                                                   |
| pprint_pformat             | 1.55 sec                                               | 1.58 sec: 1.02x slower                                                 |
| asyncio_websockets         | 550 ms                                                 | 563 ms: 1.02x slower                                                   |
| pickle_dict                | 34.6 us                                                | 35.4 us: 1.02x slower                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 56.6 ms: 1.02x slower                                                  |
| dask                       | 365 ms                                                 | 374 ms: 1.02x slower                                                   |
| django_template            | 33.5 ms                                                | 34.4 ms: 1.03x slower                                                  |
| genshi_xml                 | 53.4 ms                                                | 54.9 ms: 1.03x slower                                                  |
| hexiom                     | 6.89 ms                                                | 7.09 ms: 1.03x slower                                                  |
| nqueens                    | 87.9 ms                                                | 90.5 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.90 ms: 1.03x slower                                                  |
| bench_thread_pool          | 834 us                                                 | 862 us: 1.03x slower                                                   |
| thrift                     | 784 us                                                 | 811 us: 1.03x slower                                                   |
| docutils                   | 2.66 sec                                               | 2.77 sec: 1.04x slower                                                 |
| pprint_safe_repr           | 747 ms                                                 | 779 ms: 1.04x slower                                                   |
| xml_etree_process          | 56.9 ms                                                | 59.9 ms: 1.05x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.52 ms: 1.06x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.25 sec: 1.06x slower                                                 |
| go                         | 149 ms                                                 | 158 ms: 1.06x slower                                                   |
| scimark_sor                | 121 ms                                                 | 130 ms: 1.07x slower                                                   |
| 2to3                       | 264 ms                                                 | 282 ms: 1.07x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 86.8 ms: 1.07x slower                                                  |
| aiohttp                    | 1.12 ms                                                | 1.20 ms: 1.08x slower                                                  |
| gunicorn                   | 1.20 ms                                                | 1.30 ms: 1.08x slower                                                  |
| spectral_norm              | 108 ms                                                 | 118 ms: 1.09x slower                                                   |
| pickle                     | 11.0 us                                                | 12.0 us: 1.09x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.82 ms: 1.09x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 70.5 ms: 1.09x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.1 us: 1.09x slower                                                  |
| genshi_text                | 22.5 ms                                                | 24.7 ms: 1.10x slower                                                  |
| bench_mp_pool              | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.83 us: 1.10x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.4 ms: 1.11x slower                                                  |
| pyflate                    | 434 ms                                                 | 490 ms: 1.13x slower                                                   |
| scimark_lu                 | 116 ms                                                 | 132 ms: 1.14x slower                                                   |
| pickle_list                | 4.59 us                                                | 5.31 us: 1.16x slower                                                  |
| regex_dna                  | 205 ms                                                 | 238 ms: 1.16x slower                                                   |
| telco                      | 6.86 ms                                                | 8.42 ms: 1.23x slower                                                  |
| coverage                   | 78.8 ms                                                | 97.6 ms: 1.24x slower                                                  |
| async_generators           | 374 ms                                                 | 469 ms: 1.26x slower                                                   |
| mypy2                      | 686 ms                                                 | 904 ms: 1.32x slower                                                   |
| python_startup             | 8.56 ms                                                | 12.6 ms: 1.47x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 11.2 ms: 1.86x slower                                                  |
| unpack_sequence            | 43.5 ns                                                | 90.6 ns: 2.08x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.02x faster                                                           |

Benchmark hidden because not significant (1): html5lib
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 54.85% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x