
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.03x faster \*
- HPT reliability: 69.95%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 277 ms: 1.05x slower                                                |
| chameleon      | 6.70 ms                                                | 6.98 ms: 1.04x slower                                               |
| Geometric mean | (ref)                                                  | 1.02x slower                                                        |

Benchmark hidden because not significant (2): docutils, tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 441 ms: 1.20x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                              |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                              |
| async_tree_memoization_tg  | 626 ms                                                 | 593 ms: 1.06x faster                                                |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 713 ms: 1.05x faster                                                |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                |
| Geometric mean             | (ref)                                                  | 1.09x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                                |
| float          | 78.9 ms                                                | 86.5 ms: 1.10x slower                                               |
| nbody          | 96.0 ms                                                | 106 ms: 1.10x slower                                                |
| Geometric mean | (ref)                                                  | 1.05x slower                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 144 ms: 1.02x slower                                                |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                               |
| regex_dna      | 205 ms                                                 | 222 ms: 1.09x slower                                                |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                               |
| Geometric mean | (ref)                                                  | 1.06x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                               |
| pickle_pure_python   | 320 us                                                 | 295 us: 1.08x faster                                                |
| unpickle_pure_python | 242 us                                                 | 228 us: 1.06x faster                                                |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                |
| tomli_loads          | 2.30 sec                                               | 2.22 sec: 1.04x faster                                              |
| unpickle_list        | 5.21 us                                                | 5.04 us: 1.03x faster                                               |
| json_loads           | 29.2 us                                                | 28.3 us: 1.03x faster                                               |
| xml_etree_iterparse  | 108 ms                                                 | 109 ms: 1.01x slower                                                |
| pickle_dict          | 34.6 us                                                | 35.1 us: 1.01x slower                                               |
| xml_etree_process    | 56.9 ms                                                | 58.5 ms: 1.03x slower                                               |
| xml_etree_generate   | 81.1 ms                                                | 86.6 ms: 1.07x slower                                               |
| pickle               | 11.0 us                                                | 11.9 us: 1.08x slower                                               |
| unpickle             | 13.8 us                                                | 15.3 us: 1.11x slower                                               |
| pickle_list          | 4.59 us                                                | 5.20 us: 1.13x slower                                               |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.2 ms: 1.19x slower                                               |
| python_startup_no_site | 6.01 ms                                                | 8.83 ms: 1.47x slower                                               |
| Geometric mean         | (ref)                                                  | 1.32x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 12.7 ms: 1.19x slower                                               |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.68x faster                                                |
| generators                 | 74.9 ms                                                | 30.0 ms: 2.50x faster                                               |
| asyncio_tcp                | 875 ms                                                 | 496 ms: 1.77x faster                                                |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.81 sec: 1.72x faster                                              |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                               |
| coroutines                 | 27.0 ms                                                | 22.3 ms: 1.21x faster                                               |
| richards_super             | 61.9 ms                                                | 51.3 ms: 1.21x faster                                               |
| comprehensions             | 23.6 us                                                | 19.7 us: 1.20x faster                                               |
| async_tree_none            | 528 ms                                                 | 441 ms: 1.20x faster                                                |
| async_tree_memoization     | 639 ms                                                 | 566 ms: 1.13x faster                                                |
| logging_silent             | 111 ns                                                 | 99.3 ns: 1.12x faster                                               |
| sqlglot_parse              | 1.43 ms                                                | 1.29 ms: 1.11x faster                                               |
| richards                   | 49.8 ms                                                | 45.6 ms: 1.09x faster                                               |
| raytrace                   | 309 ms                                                 | 283 ms: 1.09x faster                                                |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                              |
| pickle_pure_python         | 320 us                                                 | 295 us: 1.08x faster                                                |
| async_tree_none_tg         | 491 ms                                                 | 454 ms: 1.08x faster                                                |
| sqlglot_transpile          | 1.75 ms                                                | 1.62 ms: 1.08x faster                                               |
| logging_simple             | 6.22 us                                                | 5.77 us: 1.08x faster                                               |
| async_tree_io_tg           | 1.29 sec                                               | 1.20 sec: 1.07x faster                                              |
| deepcopy_memo              | 40.2 us                                                | 37.4 us: 1.07x faster                                               |
| logging_format             | 6.81 us                                                | 6.36 us: 1.07x faster                                               |
| unpickle_pure_python       | 242 us                                                 | 228 us: 1.06x faster                                                |
| deepcopy_reduce            | 3.22 us                                                | 3.03 us: 1.06x faster                                               |
| async_tree_memoization_tg  | 626 ms                                                 | 593 ms: 1.06x faster                                                |
| deepcopy                   | 365 us                                                 | 346 us: 1.05x faster                                                |
| mdp                        | 2.77 sec                                               | 2.64 sec: 1.05x faster                                              |
| gc_traversal               | 4.01 ms                                                | 3.81 ms: 1.05x faster                                               |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 713 ms: 1.05x faster                                                |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 729 ms: 1.04x faster                                                |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                |
| tomli_loads                | 2.30 sec                                               | 2.22 sec: 1.04x faster                                              |
| sympy_sum                  | 169 ms                                                 | 162 ms: 1.04x faster                                                |
| unpickle_list              | 5.21 us                                                | 5.04 us: 1.03x faster                                               |
| sympy_str                  | 297 ms                                                 | 288 ms: 1.03x faster                                                |
| json_loads                 | 29.2 us                                                | 28.3 us: 1.03x faster                                               |
| pidigits                   | 194 ms                                                 | 188 ms: 1.03x faster                                                |
| sqlglot_normalize          | 113 ms                                                 | 110 ms: 1.03x faster                                                |
| chaos                      | 71.9 ms                                                | 70.4 ms: 1.02x faster                                               |
| pycparser                  | 1.19 sec                                               | 1.17 sec: 1.02x faster                                              |
| pathlib                    | 18.5 ms                                                | 18.2 ms: 1.02x faster                                               |
| sympy_integrate            | 21.5 ms                                                | 21.1 ms: 1.02x faster                                               |
| scimark_sor                | 121 ms                                                 | 120 ms: 1.01x faster                                                |
| scimark_lu                 | 116 ms                                                 | 116 ms: 1.01x faster                                                |
| sympy_expand               | 484 ms                                                 | 482 ms: 1.00x faster                                                |
| sqlglot_optimize           | 55.3 ms                                                | 55.9 ms: 1.01x slower                                               |
| xml_etree_iterparse        | 108 ms                                                 | 109 ms: 1.01x slower                                                |
| bench_thread_pool          | 834 us                                                 | 845 us: 1.01x slower                                                |
| pickle_dict                | 34.6 us                                                | 35.1 us: 1.01x slower                                               |
| regex_compile              | 141 ms                                                 | 144 ms: 1.02x slower                                                |
| meteor_contest             | 109 ms                                                 | 111 ms: 1.02x slower                                                |
| xml_etree_process          | 56.9 ms                                                | 58.5 ms: 1.03x slower                                               |
| create_gc_cycles           | 1.43 ms                                                | 1.48 ms: 1.03x slower                                               |
| go                         | 149 ms                                                 | 154 ms: 1.03x slower                                                |
| deltablue                  | 3.92 ms                                                | 4.06 ms: 1.04x slower                                               |
| chameleon                  | 6.70 ms                                                | 6.98 ms: 1.04x slower                                               |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                               |
| nqueens                    | 87.9 ms                                                | 92.0 ms: 1.05x slower                                               |
| 2to3                       | 264 ms                                                 | 277 ms: 1.05x slower                                                |
| crypto_pyaes               | 76.7 ms                                                | 80.5 ms: 1.05x slower                                               |
| dulwich_log                | 64.6 ms                                                | 68.0 ms: 1.05x slower                                               |
| fannkuch                   | 405 ms                                                 | 428 ms: 1.06x slower                                                |
| xml_etree_generate         | 81.1 ms                                                | 86.6 ms: 1.07x slower                                               |
| pickle                     | 11.0 us                                                | 11.9 us: 1.08x slower                                               |
| regex_dna                  | 205 ms                                                 | 222 ms: 1.09x slower                                                |
| scimark_monte_carlo        | 70.7 ms                                                | 76.9 ms: 1.09x slower                                               |
| pprint_safe_repr           | 747 ms                                                 | 814 ms: 1.09x slower                                                |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                               |
| sqlite_synth               | 2.57 us                                                | 2.81 us: 1.09x slower                                               |
| float                      | 78.9 ms                                                | 86.5 ms: 1.10x slower                                               |
| pprint_pformat             | 1.55 sec                                               | 1.71 sec: 1.10x slower                                              |
| nbody                      | 96.0 ms                                                | 106 ms: 1.10x slower                                                |
| unpack_sequence            | 43.5 ns                                                | 48.0 ns: 1.10x slower                                               |
| unpickle                   | 13.8 us                                                | 15.3 us: 1.11x slower                                               |
| scimark_fft                | 345 ms                                                 | 383 ms: 1.11x slower                                                |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 5.62 ms: 1.12x slower                                               |
| pickle_list                | 4.59 us                                                | 5.20 us: 1.13x slower                                               |
| pyflate                    | 434 ms                                                 | 506 ms: 1.17x slower                                                |
| mako                       | 10.7 ms                                                | 12.7 ms: 1.19x slower                                               |
| python_startup             | 8.56 ms                                                | 10.2 ms: 1.19x slower                                               |
| coverage                   | 78.8 ms                                                | 93.8 ms: 1.19x slower                                               |
| hexiom                     | 6.89 ms                                                | 8.28 ms: 1.20x slower                                               |
| telco                      | 6.86 ms                                                | 8.49 ms: 1.24x slower                                               |
| async_generators           | 374 ms                                                 | 473 ms: 1.27x slower                                                |
| mypy2                      | 686 ms                                                 | 876 ms: 1.28x slower                                                |
| spectral_norm              | 108 ms                                                 | 139 ms: 1.29x slower                                                |
| python_startup_no_site     | 6.01 ms                                                | 8.83 ms: 1.47x slower                                               |
| Geometric mean             | (ref)                                                  | 1.03x faster                                                        |

Benchmark hidden because not significant (6): json, tornado_http, bench_mp_pool, docutils, asyncio_websockets, dask
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 69.95% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.05x