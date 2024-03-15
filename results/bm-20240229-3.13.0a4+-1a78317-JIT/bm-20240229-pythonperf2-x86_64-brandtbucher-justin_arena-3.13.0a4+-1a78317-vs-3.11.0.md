# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster \*
- HPT reliability: 84.32%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 307 ms: 1.07x slower                                                       |
| chameleon      | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                                      |
| docutils       | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                     |
| html5lib       | 72.2 ms                                                      | 73.9 ms: 1.02x slower                                                      |
| Geometric mean | (ref)                                                        | 1.01x slower                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 445 ms: 1.16x faster                                                       |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 710 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                     |
| async_tree_memoization_tg  | 600 ms                                                       | 572 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                       |
| Geometric mean             | (ref)                                                        | 1.08x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 261 ms: 1.04x slower                                                       |
| float          | 74.9 ms                                                      | 78.1 ms: 1.04x slower                                                      |
| nbody          | 92.9 ms                                                      | 98.5 ms: 1.06x slower                                                      |
| Geometric mean | (ref)                                                        | 1.05x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| regex_v8       | 24.4 ms                                                      | 25.2 ms: 1.03x slower                                                      |
| regex_dna      | 227 ms                                                       | 238 ms: 1.05x slower                                                       |
| regex_effbot   | 3.34 ms                                                      | 3.56 ms: 1.06x slower                                                      |
| Geometric mean | (ref)                                                        | 1.02x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                      |
| json_loads           | 28.9 us                                                      | 24.8 us: 1.17x faster                                                      |
| xml_etree_parse      | 155 ms                                                       | 143 ms: 1.08x faster                                                       |
| xml_etree_iterparse  | 107 ms                                                       | 102 ms: 1.05x faster                                                       |
| pickle_dict          | 32.3 us                                                      | 31.0 us: 1.04x faster                                                      |
| unpickle_pure_python | 238 us                                                       | 230 us: 1.04x faster                                                       |
| tomli_loads          | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                                     |
| pickle_pure_python   | 316 us                                                       | 308 us: 1.03x faster                                                       |
| unpickle_list        | 4.60 us                                                      | 4.64 us: 1.01x slower                                                      |
| xml_etree_process    | 55.9 ms                                                      | 57.7 ms: 1.03x slower                                                      |
| xml_etree_generate   | 79.7 ms                                                      | 83.2 ms: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| pickle_list          | 3.94 us                                                      | 4.30 us: 1.09x slower                                                      |
| unpickle             | 13.3 us                                                      | 15.1 us: 1.14x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.02x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.4 ms: 1.43x slower                                                      |
| python_startup_no_site | 7.73 ms                                                      | 13.9 ms: 1.79x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.60x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 9.85 ms: 1.12x faster                                                      |
| django_template | 39.3 ms                                                      | 38.9 ms: 1.01x faster                                                      |
| genshi_xml      | 57.1 ms                                                      | 60.7 ms: 1.06x slower                                                      |
| genshi_text     | 25.5 ms                                                      | 29.6 ms: 1.16x slower                                                      |
| Geometric mean  | (ref)                                                        | 1.02x slower                                                               |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 118 us: 4.50x faster                                                       |
| asyncio_tcp                | 747 ms                                                       | 371 ms: 2.01x faster                                                       |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.95x faster                                                     |
| generators                 | 54.6 ms                                                      | 33.0 ms: 1.65x faster                                                      |
| pylint                     | 514 ms                                                       | 359 ms: 1.43x faster                                                       |
| comprehensions             | 25.1 us                                                      | 18.7 us: 1.34x faster                                                      |
| coroutines                 | 27.8 ms                                                      | 22.4 ms: 1.24x faster                                                      |
| json_dumps                 | 13.3 ms                                                      | 10.8 ms: 1.23x faster                                                      |
| gc_traversal               | 4.15 ms                                                      | 3.47 ms: 1.19x faster                                                      |
| json_loads                 | 28.9 us                                                      | 24.8 us: 1.17x faster                                                      |
| async_tree_none            | 518 ms                                                       | 445 ms: 1.16x faster                                                       |
| sympy_sum                  | 186 ms                                                       | 160 ms: 1.16x faster                                                       |
| logging_simple             | 7.24 us                                                      | 6.42 us: 1.13x faster                                                      |
| async_tree_memoization     | 629 ms                                                       | 559 ms: 1.13x faster                                                       |
| richards_super             | 63.6 ms                                                      | 56.7 ms: 1.12x faster                                                      |
| chaos                      | 74.9 ms                                                      | 66.8 ms: 1.12x faster                                                      |
| sympy_str                  | 337 ms                                                       | 301 ms: 1.12x faster                                                       |
| mako                       | 11.0 ms                                                      | 9.85 ms: 1.12x faster                                                      |
| crypto_pyaes               | 83.3 ms                                                      | 76.7 ms: 1.09x faster                                                      |
| xml_etree_parse            | 155 ms                                                       | 143 ms: 1.08x faster                                                       |
| sqlglot_parse              | 1.51 ms                                                      | 1.40 ms: 1.08x faster                                                      |
| logging_format             | 7.71 us                                                      | 7.12 us: 1.08x faster                                                      |
| sympy_expand               | 553 ms                                                       | 512 ms: 1.08x faster                                                       |
| fannkuch                   | 416 ms                                                       | 386 ms: 1.08x faster                                                       |
| mdp                        | 2.77 sec                                                     | 2.58 sec: 1.08x faster                                                     |
| thrift                     | 931 us                                                       | 868 us: 1.07x faster                                                       |
| async_tree_io              | 1.17 sec                                                     | 1.09 sec: 1.07x faster                                                     |
| regex_compile              | 156 ms                                                       | 146 ms: 1.07x faster                                                       |
| async_tree_none_tg         | 474 ms                                                       | 447 ms: 1.06x faster                                                       |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 710 ms: 1.06x faster                                                       |
| async_tree_io_tg           | 1.15 sec                                                     | 1.09 sec: 1.06x faster                                                     |
| sympy_integrate            | 25.8 ms                                                      | 24.5 ms: 1.05x faster                                                      |
| async_tree_memoization_tg  | 600 ms                                                       | 572 ms: 1.05x faster                                                       |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.05x faster                                                       |
| json                       | 5.58 ms                                                      | 5.35 ms: 1.04x faster                                                      |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 718 ms: 1.04x faster                                                       |
| sqlglot_transpile          | 1.91 ms                                                      | 1.83 ms: 1.04x faster                                                      |
| pickle_dict                | 32.3 us                                                      | 31.0 us: 1.04x faster                                                      |
| chameleon                  | 7.92 ms                                                      | 7.60 ms: 1.04x faster                                                      |
| deltablue                  | 3.97 ms                                                      | 3.81 ms: 1.04x faster                                                      |
| deepcopy                   | 391 us                                                       | 375 us: 1.04x faster                                                       |
| unpickle_pure_python       | 238 us                                                       | 230 us: 1.04x faster                                                       |
| tomli_loads                | 2.25 sec                                                     | 2.17 sec: 1.04x faster                                                     |
| logging_silent             | 100 ns                                                       | 97.0 ns: 1.03x faster                                                      |
| spectral_norm              | 95.1 ms                                                      | 92.6 ms: 1.03x faster                                                      |
| pickle_pure_python         | 316 us                                                       | 308 us: 1.03x faster                                                       |
| pycparser                  | 1.31 sec                                                     | 1.28 sec: 1.02x faster                                                     |
| deepcopy_reduce            | 3.40 us                                                      | 3.34 us: 1.02x faster                                                      |
| raytrace                   | 309 ms                                                       | 304 ms: 1.02x faster                                                       |
| sqlglot_normalize          | 122 ms                                                       | 120 ms: 1.02x faster                                                       |
| create_gc_cycles           | 1.58 ms                                                      | 1.55 ms: 1.02x faster                                                      |
| nqueens                    | 103 ms                                                       | 101 ms: 1.01x faster                                                       |
| django_template            | 39.3 ms                                                      | 38.9 ms: 1.01x faster                                                      |
| asyncio_websockets         | 390 ms                                                       | 387 ms: 1.01x faster                                                       |
| unpickle_list              | 4.60 us                                                      | 4.64 us: 1.01x slower                                                      |
| meteor_contest             | 131 ms                                                       | 132 ms: 1.01x slower                                                       |
| dulwich_log                | 67.4 ms                                                      | 68.3 ms: 1.01x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.3 ms: 1.02x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                     |
| html5lib                   | 72.2 ms                                                      | 73.9 ms: 1.02x slower                                                      |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.16 ms: 1.02x slower                                                      |
| scimark_lu                 | 114 ms                                                       | 117 ms: 1.03x slower                                                       |
| pprint_pformat             | 1.67 sec                                                     | 1.72 sec: 1.03x slower                                                     |
| regex_v8                   | 24.4 ms                                                      | 25.2 ms: 1.03x slower                                                      |
| xml_etree_process          | 55.9 ms                                                      | 57.7 ms: 1.03x slower                                                      |
| pprint_safe_repr           | 805 ms                                                       | 835 ms: 1.04x slower                                                       |
| pidigits                   | 251 ms                                                       | 261 ms: 1.04x slower                                                       |
| float                      | 74.9 ms                                                      | 78.1 ms: 1.04x slower                                                      |
| xml_etree_generate         | 79.7 ms                                                      | 83.2 ms: 1.04x slower                                                      |
| pickle                     | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| hexiom                     | 6.98 ms                                                      | 7.30 ms: 1.05x slower                                                      |
| regex_dna                  | 227 ms                                                       | 238 ms: 1.05x slower                                                       |
| nbody                      | 92.9 ms                                                      | 98.5 ms: 1.06x slower                                                      |
| genshi_xml                 | 57.1 ms                                                      | 60.7 ms: 1.06x slower                                                      |
| regex_effbot               | 3.34 ms                                                      | 3.56 ms: 1.06x slower                                                      |
| sqlite_synth               | 2.52 us                                                      | 2.69 us: 1.07x slower                                                      |
| sqlglot_optimize           | 59.0 ms                                                      | 63.0 ms: 1.07x slower                                                      |
| 2to3                       | 287 ms                                                       | 307 ms: 1.07x slower                                                       |
| go                         | 158 ms                                                       | 172 ms: 1.09x slower                                                       |
| pickle_list                | 3.94 us                                                      | 4.30 us: 1.09x slower                                                      |
| scimark_monte_carlo        | 69.8 ms                                                      | 76.6 ms: 1.10x slower                                                      |
| gunicorn                   | 966 us                                                       | 1.08 ms: 1.12x slower                                                      |
| aiohttp                    | 986 us                                                       | 1.10 ms: 1.12x slower                                                      |
| scimark_fft                | 281 ms                                                       | 318 ms: 1.13x slower                                                       |
| unpickle                   | 13.3 us                                                      | 15.1 us: 1.14x slower                                                      |
| genshi_text                | 25.5 ms                                                      | 29.6 ms: 1.16x slower                                                      |
| telco                      | 6.81 ms                                                      | 7.99 ms: 1.17x slower                                                      |
| mypy2                      | 762 ms                                                       | 910 ms: 1.19x slower                                                       |
| pyflate                    | 449 ms                                                       | 538 ms: 1.20x slower                                                       |
| async_generators           | 322 ms                                                       | 389 ms: 1.21x slower                                                       |
| coverage                   | 66.1 ms                                                      | 81.4 ms: 1.23x slower                                                      |
| unpack_sequence            | 45.7 ns                                                      | 60.5 ns: 1.32x slower                                                      |
| scimark_sor                | 110 ms                                                       | 151 ms: 1.38x slower                                                       |
| python_startup             | 10.7 ms                                                      | 15.4 ms: 1.43x slower                                                      |
| dask                       | 410 ms                                                       | 588 ms: 1.43x slower                                                       |
| bench_mp_pool              | 4.70 ms                                                      | 7.08 ms: 1.51x slower                                                      |
| python_startup_no_site     | 7.73 ms                                                      | 13.9 ms: 1.79x slower                                                      |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                               |

Benchmark hidden because not significant (4): bench_thread_pool, deepcopy_memo, richards, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 84.32% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.25x