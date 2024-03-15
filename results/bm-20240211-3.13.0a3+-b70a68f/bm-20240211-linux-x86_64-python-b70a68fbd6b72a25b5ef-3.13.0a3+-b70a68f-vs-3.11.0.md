
# Results vs. 3.11.0

- fork: python
- ref: b70a68fbd6b72a25b5ef
- machine: linux-x86_64
- commit hash: b70a68f
- commit date: 2024-02-11
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.99x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| chameleon      | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                  |
| docutils       | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| tornado_http   | 98.1 ms                                                | 94.6 ms: 1.04x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none            | 528 ms                                                 | 430 ms: 1.23x faster                                                   |
| async_tree_memoization     | 639 ms                                                 | 557 ms: 1.15x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                   |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                   |
| Geometric mean             | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 90.0 ms: 1.07x faster                                                  |
| pidigits       | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| float          | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| regex_effbot   | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                  |
| regex_dna      | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| regex_v8       | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                  |
| Geometric mean | (ref)                                                  | 1.04x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| unpickle_pure_python | 242 us                                                 | 217 us: 1.11x faster                                                   |
| tomli_loads          | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| pickle_pure_python   | 320 us                                                 | 301 us: 1.06x faster                                                   |
| json_loads           | 29.2 us                                                | 27.7 us: 1.05x faster                                                  |
| unpickle_list        | 5.21 us                                                | 4.98 us: 1.05x faster                                                  |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| pickle_dict          | 34.6 us                                                | 35.3 us: 1.02x slower                                                  |
| xml_etree_process    | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                  |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| pickle               | 11.0 us                                                | 11.8 us: 1.07x slower                                                  |
| pickle_list          | 4.59 us                                                | 5.25 us: 1.14x slower                                                  |
| unpickle             | 13.8 us                                                | 16.0 us: 1.16x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 10.1 ms: 1.19x slower                                                  |
| python_startup_no_site | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.31x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |

All benchmarks:
===============

| Benchmark                  | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols   | 520 us                                                 | 110 us: 4.71x faster                                                   |
| generators                 | 74.9 ms                                                | 29.2 ms: 2.56x faster                                                  |
| asyncio_tcp                | 875 ms                                                 | 487 ms: 1.80x faster                                                   |
| asyncio_tcp_ssl            | 3.11 sec                                               | 1.78 sec: 1.74x faster                                                 |
| comprehensions             | 23.6 us                                                | 16.3 us: 1.45x faster                                                  |
| json_dumps                 | 13.3 ms                                                | 10.4 ms: 1.28x faster                                                  |
| deltablue                  | 3.92 ms                                                | 3.16 ms: 1.24x faster                                                  |
| async_tree_none            | 528 ms                                                 | 430 ms: 1.23x faster                                                   |
| coroutines                 | 27.0 ms                                                | 22.0 ms: 1.23x faster                                                  |
| chaos                      | 71.9 ms                                                | 58.8 ms: 1.22x faster                                                  |
| raytrace                   | 309 ms                                                 | 256 ms: 1.20x faster                                                   |
| logging_silent             | 111 ns                                                 | 94.2 ns: 1.18x faster                                                  |
| richards_super             | 61.9 ms                                                | 53.3 ms: 1.16x faster                                                  |
| sqlglot_parse              | 1.43 ms                                                | 1.25 ms: 1.15x faster                                                  |
| async_tree_memoization     | 639 ms                                                 | 557 ms: 1.15x faster                                                   |
| sympy_sum                  | 169 ms                                                 | 147 ms: 1.14x faster                                                   |
| hexiom                     | 6.89 ms                                                | 6.05 ms: 1.14x faster                                                  |
| sqlglot_transpile          | 1.75 ms                                                | 1.56 ms: 1.12x faster                                                  |
| unpickle_pure_python       | 242 us                                                 | 217 us: 1.11x faster                                                   |
| async_tree_none_tg         | 491 ms                                                 | 442 ms: 1.11x faster                                                   |
| sympy_str                  | 297 ms                                                 | 268 ms: 1.11x faster                                                   |
| logging_simple             | 6.22 us                                                | 5.62 us: 1.11x faster                                                  |
| logging_format             | 6.81 us                                                | 6.19 us: 1.10x faster                                                  |
| sympy_integrate            | 21.5 ms                                                | 19.5 ms: 1.10x faster                                                  |
| async_tree_memoization_tg  | 626 ms                                                 | 571 ms: 1.10x faster                                                   |
| async_tree_io              | 1.29 sec                                               | 1.17 sec: 1.10x faster                                                 |
| regex_compile              | 141 ms                                                 | 129 ms: 1.09x faster                                                   |
| async_tree_io_tg           | 1.29 sec                                               | 1.19 sec: 1.09x faster                                                 |
| crypto_pyaes               | 76.7 ms                                                | 70.7 ms: 1.09x faster                                                  |
| tomli_loads                | 2.30 sec                                               | 2.13 sec: 1.08x faster                                                 |
| nqueens                    | 87.9 ms                                                | 81.4 ms: 1.08x faster                                                  |
| mdp                        | 2.77 sec                                               | 2.58 sec: 1.08x faster                                                 |
| scimark_monte_carlo        | 70.7 ms                                                | 65.7 ms: 1.08x faster                                                  |
| go                         | 149 ms                                                 | 139 ms: 1.07x faster                                                   |
| gc_traversal               | 4.01 ms                                                | 3.76 ms: 1.07x faster                                                  |
| nbody                      | 96.0 ms                                                | 90.0 ms: 1.07x faster                                                  |
| sympy_expand               | 484 ms                                                 | 454 ms: 1.07x faster                                                   |
| async_tree_cpu_io_mixed    | 749 ms                                                 | 703 ms: 1.07x faster                                                   |
| pickle_pure_python         | 320 us                                                 | 301 us: 1.06x faster                                                   |
| richards                   | 49.8 ms                                                | 46.9 ms: 1.06x faster                                                  |
| deepcopy                   | 365 us                                                 | 344 us: 1.06x faster                                                   |
| deepcopy_memo              | 40.2 us                                                | 37.9 us: 1.06x faster                                                  |
| async_tree_cpu_io_mixed_tg | 761 ms                                                 | 718 ms: 1.06x faster                                                   |
| deepcopy_reduce            | 3.22 us                                                | 3.04 us: 1.06x faster                                                  |
| sqlglot_normalize          | 113 ms                                                 | 107 ms: 1.06x faster                                                   |
| json_loads                 | 29.2 us                                                | 27.7 us: 1.05x faster                                                  |
| pprint_pformat             | 1.55 sec                                               | 1.48 sec: 1.05x faster                                                 |
| unpickle_list              | 5.21 us                                                | 4.98 us: 1.05x faster                                                  |
| scimark_sparse_mat_mult    | 5.03 ms                                                | 4.83 ms: 1.04x faster                                                  |
| pidigits                   | 194 ms                                                 | 187 ms: 1.04x faster                                                   |
| pprint_safe_repr           | 747 ms                                                 | 721 ms: 1.04x faster                                                   |
| tornado_http               | 98.1 ms                                                | 94.6 ms: 1.04x faster                                                  |
| scimark_lu                 | 116 ms                                                 | 113 ms: 1.03x faster                                                   |
| xml_etree_parse            | 164 ms                                                 | 159 ms: 1.03x faster                                                   |
| json                       | 5.24 ms                                                | 5.07 ms: 1.03x faster                                                  |
| sqlglot_optimize           | 55.3 ms                                                | 53.8 ms: 1.03x faster                                                  |
| fannkuch                   | 405 ms                                                 | 395 ms: 1.02x faster                                                   |
| xml_etree_iterparse        | 108 ms                                                 | 106 ms: 1.02x faster                                                   |
| docutils                   | 2.66 sec                                               | 2.61 sec: 1.02x faster                                                 |
| bench_thread_pool          | 834 us                                                 | 818 us: 1.02x faster                                                   |
| pycparser                  | 1.19 sec                                               | 1.16 sec: 1.02x faster                                                 |
| pathlib                    | 18.5 ms                                                | 18.3 ms: 1.01x faster                                                  |
| meteor_contest             | 109 ms                                                 | 108 ms: 1.01x faster                                                   |
| 2to3                       | 264 ms                                                 | 263 ms: 1.01x faster                                                   |
| dulwich_log                | 64.6 ms                                                | 65.0 ms: 1.01x slower                                                  |
| pickle_dict                | 34.6 us                                                | 35.3 us: 1.02x slower                                                  |
| xml_etree_process          | 56.9 ms                                                | 58.3 ms: 1.02x slower                                                  |
| chameleon                  | 6.70 ms                                                | 6.89 ms: 1.03x slower                                                  |
| float                      | 78.9 ms                                                | 81.3 ms: 1.03x slower                                                  |
| spectral_norm              | 108 ms                                                 | 112 ms: 1.04x slower                                                   |
| create_gc_cycles           | 1.43 ms                                                | 1.49 ms: 1.04x slower                                                  |
| regex_effbot               | 3.51 ms                                                | 3.67 ms: 1.05x slower                                                  |
| scimark_fft                | 345 ms                                                 | 363 ms: 1.05x slower                                                   |
| mako                       | 10.7 ms                                                | 11.2 ms: 1.05x slower                                                  |
| xml_etree_generate         | 81.1 ms                                                | 85.6 ms: 1.06x slower                                                  |
| scimark_sor                | 121 ms                                                 | 128 ms: 1.06x slower                                                   |
| pickle                     | 11.0 us                                                | 11.8 us: 1.07x slower                                                  |
| pyflate                    | 434 ms                                                 | 470 ms: 1.08x slower                                                   |
| sqlite_synth               | 2.57 us                                                | 2.79 us: 1.09x slower                                                  |
| regex_dna                  | 205 ms                                                 | 223 ms: 1.09x slower                                                   |
| unpack_sequence            | 43.5 ns                                                | 48.8 ns: 1.12x slower                                                  |
| regex_v8                   | 22.9 ms                                                | 25.7 ms: 1.12x slower                                                  |
| pickle_list                | 4.59 us                                                | 5.25 us: 1.14x slower                                                  |
| unpickle                   | 13.8 us                                                | 16.0 us: 1.16x slower                                                  |
| python_startup             | 8.56 ms                                                | 10.1 ms: 1.19x slower                                                  |
| async_generators           | 374 ms                                                 | 449 ms: 1.20x slower                                                   |
| coverage                   | 78.8 ms                                                | 95.3 ms: 1.21x slower                                                  |
| telco                      | 6.86 ms                                                | 8.35 ms: 1.22x slower                                                  |
| mypy2                      | 686 ms                                                 | 844 ms: 1.23x slower                                                   |
| python_startup_no_site     | 6.01 ms                                                | 8.76 ms: 1.46x slower                                                  |
| Geometric mean             | (ref)                                                  | 1.07x faster                                                           |

Benchmark hidden because not significant (3): dask, bench_mp_pool, asyncio_websockets
Ignored benchmarks (12) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.99x