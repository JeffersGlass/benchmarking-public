
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.04x faster \*
- HPT reliability: 94.03%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 275 ms: 1.04x slower                                                 |
| chameleon      | 6.70 ms                                                | 7.04 ms: 1.05x slower                                                |
| docutils       | 2.66 sec                                               | 2.65 sec: 1.01x faster                                               |
| Geometric mean | (ref)                                                  | 1.02x slower                                                         |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                 |
| async_tree_memoization     | 639 ms                                                 | 565 ms: 1.13x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 723 ms: 1.05x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 711 ms: 1.05x faster                                                 |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 88.2 ms: 1.09x faster                                                |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| float          | 78.9 ms                                                | 81.7 ms: 1.04x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 140 ms: 1.01x faster                                                 |
| regex_effbot   | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                |
| regex_dna      | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| regex_v8       | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                |
| Geometric mean | (ref)                                                  | 1.05x slower                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.14 sec: 1.08x faster                                               |
| unpickle_pure_python | 242 us                                                 | 226 us: 1.07x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 300 us: 1.07x faster                                                 |
| xml_etree_parse      | 164 ms                                                 | 155 ms: 1.06x faster                                                 |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                                |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                                |
| xml_etree_process    | 56.9 ms                                                | 58.4 ms: 1.03x slower                                                |
| pickle               | 11.0 us                                                | 11.5 us: 1.05x slower                                                |
| xml_etree_generate   | 81.1 ms                                                | 86.4 ms: 1.07x slower                                                |
| pickle_list          | 4.59 us                                                | 4.99 us: 1.09x slower                                                |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                |
| Geometric mean       | (ref)                                                  | 1.02x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                |
| python_startup_no_site | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.9 ms: 1.12x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 112 us: 4.64x faster                                                 |
| generators                 | 74.9 ms                                                | 29.7 ms: 2.52x faster                                                |
| asyncio_tcp                | 875 ms                                                 | 493 ms: 1.78x faster                                                 |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                               |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                |
| comprehensions             | 23.6 us                                                | 18.6 us: 1.27x faster                                                |
| async_tree_none            | 528 ms                                                 | 439 ms: 1.20x faster                                                 |
| coroutines                 | 27.0 ms                                                | 22.5 ms: 1.20x faster                                                |
| richards_super             | 61.9 ms                                                | 52.0 ms: 1.19x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 565 ms: 1.13x faster                                                 |
| gc_traversal               | 4.01 ms                                                | 3.59 ms: 1.12x faster                                                |
| sqlglot_parse              | 1.43 ms                                                | 1.28 ms: 1.12x faster                                                |
| raytrace                   | 309 ms                                                 | 281 ms: 1.10x faster                                                 |
| async_tree_none_tg         | 491 ms                                                 | 448 ms: 1.10x faster                                                 |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                               |
| logging_silent             | 111 ns                                                 | 102 ns: 1.09x faster                                                 |
| nbody                      | 96.0 ms                                                | 88.2 ms: 1.09x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                               |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                                |
| richards                   | 49.8 ms                                                | 46.2 ms: 1.08x faster                                                |
| async_tree_memoization_tg  | 626 ms                                                 | 581 ms: 1.08x faster                                                 |
| tomli_loads                | 2.30 sec                                               | 2.14 sec: 1.08x faster                                               |
| unpickle_pure_python       | 242 us                                                 | 226 us: 1.07x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 300 us: 1.07x faster                                                 |
| crypto_pyaes               | 76.7 ms                                                | 72.5 ms: 1.06x faster                                                |
| xml_etree_parse            | 164 ms                                                 | 155 ms: 1.06x faster                                                 |
| logging_simple             | 6.22 us                                                | 5.88 us: 1.06x faster                                                |
| sympy_sum                  | 169 ms                                                 | 160 ms: 1.05x faster                                                 |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 723 ms: 1.05x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 711 ms: 1.05x faster                                                 |
| chaos                      | 71.9 ms                                                | 68.4 ms: 1.05x faster                                                |
| logging_format             | 6.81 us                                                | 6.49 us: 1.05x faster                                                |
| sympy_str                  | 297 ms                                                 | 284 ms: 1.05x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.98 us: 1.05x faster                                                |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                 |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.81 ms: 1.04x faster                                                |
| deepcopy_reduce            | 3.22 us                                                | 3.09 us: 1.04x faster                                                |
| deltablue                  | 3.92 ms                                                | 3.78 ms: 1.04x faster                                                |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                 |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                 |
| sqlglot_normalize          | 113 ms                                                 | 109 ms: 1.03x faster                                                 |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 21.0 ms: 1.02x faster                                                |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                 |
| deepcopy_memo              | 40.2 us                                                | 39.5 us: 1.02x faster                                                |
| regex_compile              | 141 ms                                                 | 140 ms: 1.01x faster                                                 |
| nqueens                    | 87.9 ms                                                | 87.0 ms: 1.01x faster                                                |
| docutils                   | 2.66 sec                                               | 2.65 sec: 1.01x faster                                               |
| mdp                        | 2.77 sec                                               | 2.77 sec: 1.00x faster                                               |
| meteor_contest             | 109 ms                                                 | 109 ms: 1.00x slower                                                 |
| bench_thread_pool          | 834 us                                                 | 840 us: 1.01x slower                                                 |
| scimark_fft                | 345 ms                                                 | 349 ms: 1.01x slower                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 55.9 ms: 1.01x slower                                                |
| go                         | 149 ms                                                 | 150 ms: 1.01x slower                                                 |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                                |
| create_gc_cycles           | 1.43 ms                                                | 1.46 ms: 1.02x slower                                                |
| regex_effbot               | 3.51 ms                                                | 3.58 ms: 1.02x slower                                                |
| fannkuch                   | 405 ms                                                 | 414 ms: 1.02x slower                                                 |
| xml_etree_process          | 56.9 ms                                                | 58.4 ms: 1.03x slower                                                |
| pycparser                  | 1.19 sec                                               | 1.22 sec: 1.03x slower                                               |
| scimark_monte_carlo        | 70.7 ms                                                | 73.2 ms: 1.03x slower                                                |
| float                      | 78.9 ms                                                | 81.7 ms: 1.04x slower                                                |
| 2to3                       | 264 ms                                                 | 275 ms: 1.04x slower                                                 |
| pickle                     | 11.0 us                                                | 11.5 us: 1.05x slower                                                |
| chameleon                  | 6.70 ms                                                | 7.04 ms: 1.05x slower                                                |
| dulwich_log                | 64.6 ms                                                | 68.4 ms: 1.06x slower                                                |
| xml_etree_generate         | 81.1 ms                                                | 86.4 ms: 1.07x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 47.2 ns: 1.09x slower                                                |
| pprint_pformat             | 1.55 sec                                               | 1.69 sec: 1.09x slower                                               |
| pprint_safe_repr           | 747 ms                                                 | 812 ms: 1.09x slower                                                 |
| pickle_list                | 4.59 us                                                | 4.99 us: 1.09x slower                                                |
| scimark_sor                | 121 ms                                                 | 133 ms: 1.09x slower                                                 |
| regex_dna                  | 205 ms                                                 | 224 ms: 1.09x slower                                                 |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.09x slower                                                |
| pyflate                    | 434 ms                                                 | 484 ms: 1.12x slower                                                 |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                                |
| regex_v8                   | 22.9 ms                                                | 25.6 ms: 1.12x slower                                                |
| mako                       | 10.7 ms                                                | 11.9 ms: 1.12x slower                                                |
| hexiom                     | 6.89 ms                                                | 7.81 ms: 1.13x slower                                                |
| spectral_norm              | 108 ms                                                 | 126 ms: 1.16x slower                                                 |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.18x slower                                                |
| coverage                   | 78.8 ms                                                | 94.5 ms: 1.20x slower                                                |
| telco                      | 6.86 ms                                                | 8.44 ms: 1.23x slower                                                |
| async_generators           | 374 ms                                                 | 470 ms: 1.26x slower                                                 |
| mypy2                      | 686 ms                                                 | 868 ms: 1.27x slower                                                 |
| python_startup_no_site     | 6.01 ms                                                | 8.77 ms: 1.46x slower                                                |
| Geometric mean             | (ref)                                                  | 1.04x faster                                                         |

Benchmark hidden because not significant (6): tornado_http, sympy_expand, json, bench_mp_pool, asyncio_websockets, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 94.03% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.02x