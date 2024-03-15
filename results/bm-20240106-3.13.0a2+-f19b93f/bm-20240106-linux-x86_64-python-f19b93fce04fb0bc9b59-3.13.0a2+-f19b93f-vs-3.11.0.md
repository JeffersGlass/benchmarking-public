
# Results vs. 3.11.0

- fork: python
- ref: f19b93fce04fb0bc9b59
- machine: linux-x86_64
- commit hash: f19b93f
- commit date: 2024-01-06
- overall geometric mean: 1.07x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.98x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.94 ms: 1.04x slower                                                  |
| docutils       | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.2 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 557 ms: 1.15x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 439 ms: 1.12x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 86.9 ms: 1.10x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| float          | 78.9 ms                                                | 80.0 ms: 1.01x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 130 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.62 ms: 1.03x slower                                                  |
| regex_dna      | 205 ms                                                 | 218 ms: 1.07x slower                                                   |
| regex_v8       | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 214 us: 1.13x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.12 sec: 1.08x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 299 us: 1.07x faster                                                   |
| xml_etree_parse      | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| json_loads           | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| pickle_dict          | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| pickle               | 11.0 us                                                | 11.5 us: 1.04x slower                                                  |
| unpickle_list        | 5.21 us                                                | 5.45 us: 1.04x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| unpickle             | 13.8 us                                                | 15.5 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.68 ms: 1.44x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.0 ms: 1.03x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240106-linux-x86_64-python-f19b93fce04fb0bc9b59-3.13.0a2+-f19b93f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 111 us: 4.68x faster                                                   |
| generators                 | 74.9 ms                                                | 29.4 ms: 2.55x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 475 ms: 1.84x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.5 ms: 1.27x faster                                                  |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                  |
| async_tree_none            | 528 ms                                                 | 431 ms: 1.22x faster                                                   |
| deltablue                  | 3.92 ms                                                | 3.20 ms: 1.22x faster                                                  |
| chaos                      | 71.9 ms                                                | 59.0 ms: 1.22x faster                                                  |
| raytrace                   | 309 ms                                                 | 261 ms: 1.18x faster                                                   |
| richards_super             | 61.9 ms                                                | 53.6 ms: 1.15x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.24 ms: 1.15x faster                                                  |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.15x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 557 ms: 1.15x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.53 ms: 1.14x faster                                                  |
| hexiom                     | 6.89 ms                                                | 6.07 ms: 1.13x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 214 us: 1.13x faster                                                   |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                  |
| async_tree_none_tg         | 491 ms                                                 | 439 ms: 1.12x faster                                                   |
| sympy_str                  | 297 ms                                                 | 267 ms: 1.11x faster                                                   |
| sympy_integrate            | 21.5 ms                                                | 19.3 ms: 1.11x faster                                                  |
| logging_simple             | 6.22 us                                                | 5.63 us: 1.11x faster                                                  |
| nbody                      | 96.0 ms                                                | 86.9 ms: 1.10x faster                                                  |
| logging_format             | 6.81 us                                                | 6.19 us: 1.10x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 572 ms: 1.09x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.18 sec: 1.09x faster                                                 |
| regex_compile              | 141 ms                                                 | 130 ms: 1.09x faster                                                   |
| mdp                        | 2.77 sec                                               | 2.55 sec: 1.09x faster                                                 |
| crypto_pyaes               | 76.7 ms                                                | 70.7 ms: 1.09x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.12 sec: 1.08x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.08x faster                                                 |
| pickle_pure_python         | 320 us                                                 | 299 us: 1.07x faster                                                   |
| logging_silent             | 111 ns                                                 | 104 ns: 1.07x faster                                                   |
| sympy_expand               | 484 ms                                                 | 454 ms: 1.07x faster                                                   |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 716 ms: 1.06x faster                                                   |
| richards                   | 49.8 ms                                                | 46.9 ms: 1.06x faster                                                  |
| deepcopy_memo              | 40.2 us                                                | 37.9 us: 1.06x faster                                                  |
| nqueens                    | 87.9 ms                                                | 83.1 ms: 1.06x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                                   |
| deepcopy                   | 365 us                                                 | 348 us: 1.05x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.07 us: 1.05x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.49 sec: 1.04x faster                                                 |
| xml_etree_parse            | 164 ms                                                 | 157 ms: 1.04x faster                                                   |
| scimark_monte_carlo        | 70.7 ms                                                | 67.9 ms: 1.04x faster                                                  |
| tornado_http               | 98.1 ms                                                | 94.2 ms: 1.04x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.85 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.58 sec: 1.03x faster                                                 |
| sqlglot_optimize           | 55.3 ms                                                | 53.7 ms: 1.03x faster                                                  |
| json_loads                 | 29.2 us                                                | 28.4 us: 1.03x faster                                                  |
| xml_etree_iterparse        | 108 ms                                                 | 105 ms: 1.03x faster                                                   |
| pprint_safe_repr           | 747 ms                                                 | 728 ms: 1.03x faster                                                   |
| pathlib                    | 18.5 ms                                                | 18.1 ms: 1.02x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 114 ms: 1.02x faster                                                   |
| meteor_contest             | 109 ms                                                 | 107 ms: 1.02x faster                                                   |
| dask                       | 365 ms                                                 | 360 ms: 1.01x faster                                                   |
| fannkuch                   | 405 ms                                                 | 400 ms: 1.01x faster                                                   |
| bench_thread_pool          | 834 us                                                 | 826 us: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| spectral_norm              | 108 ms                                                 | 109 ms: 1.01x slower                                                   |
| pickle_dict                | 34.6 us                                                | 34.9 us: 1.01x slower                                                  |
| pycparser                  | 1.19 sec                                               | 1.20 sec: 1.01x slower                                                 |
| float                      | 78.9 ms                                                | 80.0 ms: 1.01x slower                                                  |
| dulwich_log                | 64.6 ms                                                | 65.8 ms: 1.02x slower                                                  |
| create_gc_cycles           | 1.43 ms                                                | 1.47 ms: 1.02x slower                                                  |
| mako                       | 10.7 ms                                                | 11.0 ms: 1.03x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.62 ms: 1.03x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.94 ms: 1.04x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 59.2 ms: 1.04x slower                                                  |
| pickle                     | 11.0 us                                                | 11.5 us: 1.04x slower                                                  |
| scimark_fft                | 345 ms                                                 | 361 ms: 1.04x slower                                                   |
| unpickle_list              | 5.21 us                                                | 5.45 us: 1.04x slower                                                  |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.05x slower                                                   |
| xml_etree_generate         | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| regex_dna                  | 205 ms                                                 | 218 ms: 1.07x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 46.5 ns: 1.07x slower                                                  |
| pyflate                    | 434 ms                                                 | 468 ms: 1.08x slower                                                   |
| regex_v8                   | 22.9 ms                                                | 24.9 ms: 1.09x slower                                                  |
| sqlite_synth               | 2.57 us                                                | 2.82 us: 1.10x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.09 us: 1.11x slower                                                  |
| unpickle                   | 13.8 us                                                | 15.5 us: 1.12x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.17x slower                                                  |
| async_generators           | 374 ms                                                 | 443 ms: 1.18x slower                                                   |
| telco                      | 6.86 ms                                                | 8.26 ms: 1.20x slower                                                  |
| mypy2                      | 686 ms                                                 | 837 ms: 1.22x slower                                                   |
| coverage                   | 78.8 ms                                                | 96.4 ms: 1.22x slower                                                  |
| python_startup_no_site     | 6.01 ms                                                | 8.68 ms: 1.44x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (3): bench_mp_pool, json, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.98x