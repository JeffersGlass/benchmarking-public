# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.03x faster \*
- HPT reliability: 88.43%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.24x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 277 ms: 1.05x slower                                                |
| chameleon      | 6.70 ms                                                | 6.76 ms: 1.01x slower                                               |
| docutils       | 2.66 sec                                               | 2.70 sec: 1.01x slower                                              |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                               |
| Geometric mean | (ref)                                                  | 1.01x slower                                                        |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 440 ms: 1.20x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                              |
| async_tree_memoization_tg  | 626 ms                                                 | 577 ms: 1.09x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                              |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                |
| Geometric mean             | (ref)                                                  | 1.10x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                |
| nbody          | 96.0 ms                                                | 94.1 ms: 1.02x faster                                               |
| float          | 78.9 ms                                                | 80.0 ms: 1.01x slower                                               |
| Geometric mean | (ref)                                                  | 1.01x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 142 ms: 1.00x slower                                                |
| regex_effbot   | 3.51 ms                                                | 3.73 ms: 1.06x slower                                               |
| regex_v8       | 22.9 ms                                                | 24.7 ms: 1.08x slower                                               |
| regex_dna      | 205 ms                                                 | 229 ms: 1.12x slower                                                |
| Geometric mean | (ref)                                                  | 1.07x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.2 ms: 1.30x faster                                               |
| tomli_loads          | 2.30 sec                                               | 2.07 sec: 1.11x faster                                              |
| unpickle_list        | 5.21 us                                                | 4.79 us: 1.09x faster                                               |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                                |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                               |
| pickle_pure_python   | 320 us                                                 | 307 us: 1.04x faster                                                |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                |
| unpickle_pure_python | 242 us                                                 | 238 us: 1.02x faster                                                |
| pickle_dict          | 34.6 us                                                | 34.2 us: 1.01x faster                                               |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                               |
| pickle               | 11.0 us                                                | 11.3 us: 1.03x slower                                               |
| unpickle             | 13.8 us                                                | 14.5 us: 1.05x slower                                               |
| xml_etree_generate   | 81.1 ms                                                | 86.0 ms: 1.06x slower                                               |
| pickle_list          | 4.59 us                                                | 4.98 us: 1.09x slower                                               |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 12.3 ms: 1.44x slower                                               |
| python_startup_no_site | 6.01 ms                                                | 11.0 ms: 1.82x slower                                               |
| Geometric mean         | (ref)                                                  | 1.62x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 54.5 ms: 1.02x slower                                               |
| django_template | 33.5 ms                                                | 34.3 ms: 1.02x slower                                               |
| mako            | 10.7 ms                                                | 11.2 ms: 1.05x slower                                               |
| genshi_text     | 22.5 ms                                                | 24.2 ms: 1.08x slower                                               |
| Geometric mean  | (ref)                                                  | 1.04x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.74x faster                                                |
| generators                 | 74.9 ms                                                | 29.3 ms: 2.55x faster                                               |
| asyncio_tcp                | 875 ms                                                 | 485 ms: 1.80x faster                                                |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.80 sec: 1.73x faster                                              |
| pylint                     | 476 ms                                                 | 319 ms: 1.49x faster                                                |
| comprehensions             | 23.6 us                                                | 17.1 us: 1.38x faster                                               |
| json_dumps                 | 13.3 ms                                                | 10.2 ms: 1.30x faster                                               |
| async_tree_none            | 528 ms                                                 | 440 ms: 1.20x faster                                                |
| richards_super             | 61.9 ms                                                | 52.3 ms: 1.18x faster                                               |
| coroutines                 | 27.0 ms                                                | 23.0 ms: 1.18x faster                                               |
| deltablue                  | 3.92 ms                                                | 3.40 ms: 1.15x faster                                               |
| chaos                      | 71.9 ms                                                | 63.6 ms: 1.13x faster                                               |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.07 sec: 1.11x faster                                              |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                               |
| logging_silent             | 111 ns                                                 | 101 ns: 1.10x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 447 ms: 1.10x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                              |
| unpickle_list              | 5.21 us                                                | 4.79 us: 1.09x faster                                               |
| richards                   | 49.8 ms                                                | 45.8 ms: 1.09x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 577 ms: 1.09x faster                                                |
| logging_format             | 6.81 us                                                | 6.28 us: 1.08x faster                                               |
| logging_simple             | 6.22 us                                                | 5.75 us: 1.08x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.08x faster                                              |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                               |
| sympy_sum                  | 169 ms                                                 | 157 ms: 1.08x faster                                                |
| mdp                        | 2.77 sec                                               | 2.59 sec: 1.07x faster                                              |
| sympy_str                  | 297 ms                                                 | 279 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 707 ms: 1.06x faster                                                |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.75 ms: 1.06x faster                                               |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                               |
| raytrace                   | 309 ms                                                 | 292 ms: 1.06x faster                                                |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.05x faster                                                |
| xml_etree_parse            | 164 ms                                                 | 156 ms: 1.05x faster                                                |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                               |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 725 ms: 1.05x faster                                                |
| crypto_pyaes               | 76.7 ms                                                | 73.2 ms: 1.05x faster                                               |
| deepcopy                   | 365 us                                                 | 349 us: 1.05x faster                                                |
| pickle_pure_python         | 320 us                                                 | 307 us: 1.04x faster                                                |
| deepcopy_memo              | 40.2 us                                                | 38.6 us: 1.04x faster                                               |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                |
| sympy_integrate            | 21.5 ms                                                | 20.8 ms: 1.03x faster                                               |
| sympy_expand               | 484 ms                                                 | 473 ms: 1.02x faster                                                |
| gc_traversal               | 4.01 ms                                                | 3.92 ms: 1.02x faster                                               |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                |
| nbody                      | 96.0 ms                                                | 94.1 ms: 1.02x faster                                               |
| fannkuch                   | 405 ms                                                 | 398 ms: 1.02x faster                                                |
| unpickle_pure_python       | 242 us                                                 | 238 us: 1.02x faster                                                |
| djangocms                  | 33.5 us                                                | 33.0 us: 1.02x faster                                               |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                               |
| pickle_dict                | 34.6 us                                                | 34.2 us: 1.01x faster                                               |
| tornado_http               | 98.1 ms                                                | 96.9 ms: 1.01x faster                                               |
| scimark_fft                | 345 ms                                                 | 342 ms: 1.01x faster                                                |
| regex_compile              | 141 ms                                                 | 142 ms: 1.00x slower                                                |
| sqlglot_optimize           | 55.3 ms                                                | 55.8 ms: 1.01x slower                                               |
| chameleon                  | 6.70 ms                                                | 6.76 ms: 1.01x slower                                               |
| bench_thread_pool          | 834 us                                                 | 844 us: 1.01x slower                                                |
| float                      | 78.9 ms                                                | 80.0 ms: 1.01x slower                                               |
| docutils                   | 2.66 sec                                               | 2.70 sec: 1.01x slower                                              |
| pycparser                  | 1.19 sec                                               | 1.21 sec: 1.02x slower                                              |
| genshi_xml                 | 53.4 ms                                                | 54.5 ms: 1.02x slower                                               |
| thrift                     | 784 us                                                 | 800 us: 1.02x slower                                                |
| django_template            | 33.5 ms                                                | 34.3 ms: 1.02x slower                                               |
| nqueens                    | 87.9 ms                                                | 90.2 ms: 1.03x slower                                               |
| scimark_monte_carlo        | 70.7 ms                                                | 72.6 ms: 1.03x slower                                               |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                               |
| hexiom                     | 6.89 ms                                                | 7.08 ms: 1.03x slower                                               |
| pickle                     | 11.0 us                                                | 11.3 us: 1.03x slower                                               |
| pprint_safe_repr           | 747 ms                                                 | 772 ms: 1.03x slower                                                |
| go                         | 149 ms                                                 | 155 ms: 1.04x slower                                                |
| aiohttp                    | 1.12 ms                                                | 1.16 ms: 1.04x slower                                               |
| unpickle                   | 13.8 us                                                | 14.5 us: 1.05x slower                                               |
| 2to3                       | 264 ms                                                 | 277 ms: 1.05x slower                                                |
| spectral_norm              | 108 ms                                                 | 113 ms: 1.05x slower                                                |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                               |
| gunicorn                   | 1.20 ms                                                | 1.26 ms: 1.05x slower                                               |
| create_gc_cycles           | 1.43 ms                                                | 1.52 ms: 1.06x slower                                               |
| scimark_sor                | 121 ms                                                 | 129 ms: 1.06x slower                                                |
| xml_etree_generate         | 81.1 ms                                                | 86.0 ms: 1.06x slower                                               |
| dulwich_log                | 64.6 ms                                                | 68.6 ms: 1.06x slower                                               |
| regex_effbot               | 3.51 ms                                                | 3.73 ms: 1.06x slower                                               |
| genshi_text                | 22.5 ms                                                | 24.2 ms: 1.08x slower                                               |
| regex_v8                   | 22.9 ms                                                | 24.7 ms: 1.08x slower                                               |
| pickle_list                | 4.59 us                                                | 4.98 us: 1.09x slower                                               |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                               |
| regex_dna                  | 205 ms                                                 | 229 ms: 1.12x slower                                                |
| pyflate                    | 434 ms                                                 | 490 ms: 1.13x slower                                                |
| scimark_lu                 | 116 ms                                                 | 132 ms: 1.13x slower                                                |
| bench_mp_pool              | 24.0 ms                                                | 28.0 ms: 1.16x slower                                               |
| telco                      | 6.86 ms                                                | 8.29 ms: 1.21x slower                                               |
| coverage                   | 78.8 ms                                                | 95.6 ms: 1.21x slower                                               |
| async_generators           | 374 ms                                                 | 459 ms: 1.23x slower                                                |
| mypy2                      | 686 ms                                                 | 882 ms: 1.29x slower                                                |
| python_startup             | 8.56 ms                                                | 12.3 ms: 1.44x slower                                               |
| dask                       | 365 ms                                                 | 534 ms: 1.46x slower                                                |
| python_startup_no_site     | 6.01 ms                                                | 11.0 ms: 1.82x slower                                               |
| unpack_sequence            | 43.5 ns                                                | 94.6 ns: 2.18x slower                                               |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                        |

Benchmark hidden because not significant (5): pprint_pformat, meteor_contest, asyncio_websockets, html5lib, json
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 88.43% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.24x