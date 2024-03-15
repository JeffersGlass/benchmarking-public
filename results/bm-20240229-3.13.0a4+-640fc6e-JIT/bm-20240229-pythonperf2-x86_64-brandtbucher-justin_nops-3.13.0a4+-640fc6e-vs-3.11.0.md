# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster \*
- HPT reliability: 61.53%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.25x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 287 ms                                                       | 308 ms: 1.07x slower                                                      |
| chameleon      | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                     |
| docutils       | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                    |
| html5lib       | 72.2 ms                                                      | 74.4 ms: 1.03x slower                                                     |
| Geometric mean | (ref)                                                        | 1.01x slower                                                              |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 518 ms                                                       | 441 ms: 1.17x faster                                                      |
| async_tree_memoization     | 629 ms                                                       | 554 ms: 1.14x faster                                                      |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                      |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                      |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                    |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.06x faster                                                    |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 707 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 708 ms: 1.06x faster                                                      |
| Geometric mean             | (ref)                                                        | 1.09x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 251 ms                                                       | 262 ms: 1.04x slower                                                      |
| float          | 74.9 ms                                                      | 79.0 ms: 1.05x slower                                                     |
| nbody          | 92.9 ms                                                      | 99.1 ms: 1.07x slower                                                     |
| Geometric mean | (ref)                                                        | 1.05x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 156 ms                                                       | 147 ms: 1.06x faster                                                      |
| regex_v8       | 24.4 ms                                                      | 25.0 ms: 1.02x slower                                                     |
| regex_dna      | 227 ms                                                       | 238 ms: 1.05x slower                                                      |
| regex_effbot   | 3.34 ms                                                      | 3.56 ms: 1.06x slower                                                     |
| Geometric mean | (ref)                                                        | 1.02x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark           | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|---------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps          | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                     |
| json_loads          | 28.9 us                                                      | 25.1 us: 1.15x faster                                                     |
| xml_etree_parse     | 155 ms                                                       | 143 ms: 1.08x faster                                                      |
| xml_etree_iterparse | 107 ms                                                       | 102 ms: 1.05x faster                                                      |
| tomli_loads         | 2.25 sec                                                     | 2.22 sec: 1.01x faster                                                    |
| unpickle_list       | 4.60 us                                                      | 4.63 us: 1.01x slower                                                     |
| pickle_pure_python  | 316 us                                                       | 319 us: 1.01x slower                                                      |
| pickle_dict         | 32.3 us                                                      | 32.9 us: 1.02x slower                                                     |
| xml_etree_process   | 55.9 ms                                                      | 57.7 ms: 1.03x slower                                                     |
| xml_etree_generate  | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                     |
| pickle              | 9.89 us                                                      | 10.6 us: 1.08x slower                                                     |
| pickle_list         | 3.94 us                                                      | 4.38 us: 1.11x slower                                                     |
| unpickle            | 13.3 us                                                      | 15.2 us: 1.14x slower                                                     |
| Geometric mean      | (ref)                                                        | 1.01x faster                                                              |

Benchmark hidden because not significant (1): unpickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 10.7 ms                                                      | 15.5 ms: 1.44x slower                                                     |
| python_startup_no_site | 7.73 ms                                                      | 14.0 ms: 1.81x slower                                                     |
| Geometric mean         | (ref)                                                        | 1.61x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                                     |
| django_template | 39.3 ms                                                      | 40.3 ms: 1.02x slower                                                     |
| genshi_xml      | 57.1 ms                                                      | 61.8 ms: 1.08x slower                                                     |
| genshi_text     | 25.5 ms                                                      | 28.8 ms: 1.13x slower                                                     |
| Geometric mean  | (ref)                                                        | 1.03x slower                                                              |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:------------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 532 us                                                       | 123 us: 4.32x faster                                                      |
| asyncio_tcp                | 747 ms                                                       | 372 ms: 2.01x faster                                                      |
| asyncio_tcp_ssl            | 3.07 sec                                                     | 1.58 sec: 1.94x faster                                                    |
| generators                 | 54.6 ms                                                      | 34.0 ms: 1.61x faster                                                     |
| pylint                     | 514 ms                                                       | 361 ms: 1.42x faster                                                      |
| comprehensions             | 25.1 us                                                      | 19.2 us: 1.30x faster                                                     |
| json_dumps                 | 13.3 ms                                                      | 10.6 ms: 1.25x faster                                                     |
| coroutines                 | 27.8 ms                                                      | 22.6 ms: 1.23x faster                                                     |
| async_tree_none            | 518 ms                                                       | 441 ms: 1.17x faster                                                      |
| sympy_sum                  | 186 ms                                                       | 160 ms: 1.16x faster                                                      |
| json_loads                 | 28.9 us                                                      | 25.1 us: 1.15x faster                                                     |
| async_tree_memoization     | 629 ms                                                       | 554 ms: 1.14x faster                                                      |
| richards_super             | 63.6 ms                                                      | 56.2 ms: 1.13x faster                                                     |
| gc_traversal               | 4.15 ms                                                      | 3.68 ms: 1.13x faster                                                     |
| sympy_str                  | 337 ms                                                       | 303 ms: 1.11x faster                                                      |
| chaos                      | 74.9 ms                                                      | 68.3 ms: 1.10x faster                                                     |
| mako                       | 11.0 ms                                                      | 10.1 ms: 1.09x faster                                                     |
| async_tree_none_tg         | 474 ms                                                       | 435 ms: 1.09x faster                                                      |
| async_tree_memoization_tg  | 600 ms                                                       | 554 ms: 1.08x faster                                                      |
| xml_etree_parse            | 155 ms                                                       | 143 ms: 1.08x faster                                                      |
| sympy_expand               | 553 ms                                                       | 513 ms: 1.08x faster                                                      |
| mdp                        | 2.77 sec                                                     | 2.58 sec: 1.08x faster                                                    |
| crypto_pyaes               | 83.3 ms                                                      | 77.5 ms: 1.08x faster                                                     |
| logging_simple             | 7.24 us                                                      | 6.74 us: 1.07x faster                                                     |
| async_tree_io              | 1.17 sec                                                     | 1.10 sec: 1.07x faster                                                    |
| async_tree_io_tg           | 1.15 sec                                                     | 1.08 sec: 1.06x faster                                                    |
| async_tree_cpu_io_mixed    | 753 ms                                                       | 707 ms: 1.06x faster                                                      |
| chameleon                  | 7.92 ms                                                      | 7.45 ms: 1.06x faster                                                     |
| async_tree_cpu_io_mixed_tg | 750 ms                                                       | 708 ms: 1.06x faster                                                      |
| regex_compile              | 156 ms                                                       | 147 ms: 1.06x faster                                                      |
| sqlglot_parse              | 1.51 ms                                                      | 1.43 ms: 1.06x faster                                                     |
| deltablue                  | 3.97 ms                                                      | 3.77 ms: 1.05x faster                                                     |
| sympy_integrate            | 25.8 ms                                                      | 24.5 ms: 1.05x faster                                                     |
| json                       | 5.58 ms                                                      | 5.34 ms: 1.05x faster                                                     |
| xml_etree_iterparse        | 107 ms                                                       | 102 ms: 1.05x faster                                                      |
| thrift                     | 931 us                                                       | 891 us: 1.05x faster                                                      |
| logging_format             | 7.71 us                                                      | 7.39 us: 1.04x faster                                                     |
| deepcopy                   | 391 us                                                       | 378 us: 1.04x faster                                                      |
| fannkuch                   | 416 ms                                                       | 402 ms: 1.03x faster                                                      |
| logging_silent             | 100 ns                                                       | 97.4 ns: 1.03x faster                                                     |
| sqlglot_transpile          | 1.91 ms                                                      | 1.86 ms: 1.03x faster                                                     |
| create_gc_cycles           | 1.58 ms                                                      | 1.55 ms: 1.02x faster                                                     |
| sqlglot_normalize          | 122 ms                                                       | 119 ms: 1.02x faster                                                      |
| tomli_loads                | 2.25 sec                                                     | 2.22 sec: 1.01x faster                                                    |
| deepcopy_reduce            | 3.40 us                                                      | 3.37 us: 1.01x faster                                                     |
| spectral_norm              | 95.1 ms                                                      | 94.7 ms: 1.00x faster                                                     |
| unpickle_list              | 4.60 us                                                      | 4.63 us: 1.01x slower                                                     |
| pickle_pure_python         | 316 us                                                       | 319 us: 1.01x slower                                                      |
| richards                   | 49.7 ms                                                      | 50.2 ms: 1.01x slower                                                     |
| pickle_dict                | 32.3 us                                                      | 32.9 us: 1.02x slower                                                     |
| meteor_contest             | 131 ms                                                       | 133 ms: 1.02x slower                                                      |
| docutils                   | 2.85 sec                                                     | 2.91 sec: 1.02x slower                                                    |
| regex_v8                   | 24.4 ms                                                      | 25.0 ms: 1.02x slower                                                     |
| django_template            | 39.3 ms                                                      | 40.3 ms: 1.02x slower                                                     |
| scimark_sparse_mat_mult    | 4.06 ms                                                      | 4.18 ms: 1.03x slower                                                     |
| dulwich_log                | 67.4 ms                                                      | 69.4 ms: 1.03x slower                                                     |
| html5lib                   | 72.2 ms                                                      | 74.4 ms: 1.03x slower                                                     |
| xml_etree_process          | 55.9 ms                                                      | 57.7 ms: 1.03x slower                                                     |
| scimark_lu                 | 114 ms                                                       | 118 ms: 1.03x slower                                                      |
| pathlib                    | 18.9 ms                                                      | 19.6 ms: 1.04x slower                                                     |
| pidigits                   | 251 ms                                                       | 262 ms: 1.04x slower                                                      |
| pprint_pformat             | 1.67 sec                                                     | 1.74 sec: 1.04x slower                                                    |
| regex_dna                  | 227 ms                                                       | 238 ms: 1.05x slower                                                      |
| xml_etree_generate         | 79.7 ms                                                      | 83.5 ms: 1.05x slower                                                     |
| pprint_safe_repr           | 805 ms                                                       | 846 ms: 1.05x slower                                                      |
| float                      | 74.9 ms                                                      | 79.0 ms: 1.05x slower                                                     |
| hexiom                     | 6.98 ms                                                      | 7.43 ms: 1.06x slower                                                     |
| regex_effbot               | 3.34 ms                                                      | 3.56 ms: 1.06x slower                                                     |
| nbody                      | 92.9 ms                                                      | 99.1 ms: 1.07x slower                                                     |
| sqlite_synth               | 2.52 us                                                      | 2.71 us: 1.07x slower                                                     |
| sqlglot_optimize           | 59.0 ms                                                      | 63.3 ms: 1.07x slower                                                     |
| 2to3                       | 287 ms                                                       | 308 ms: 1.07x slower                                                      |
| pickle                     | 9.89 us                                                      | 10.6 us: 1.08x slower                                                     |
| genshi_xml                 | 57.1 ms                                                      | 61.8 ms: 1.08x slower                                                     |
| go                         | 158 ms                                                       | 173 ms: 1.10x slower                                                      |
| gunicorn                   | 966 us                                                       | 1.07 ms: 1.11x slower                                                     |
| pickle_list                | 3.94 us                                                      | 4.38 us: 1.11x slower                                                     |
| scimark_monte_carlo        | 69.8 ms                                                      | 77.9 ms: 1.12x slower                                                     |
| aiohttp                    | 986 us                                                       | 1.11 ms: 1.13x slower                                                     |
| genshi_text                | 25.5 ms                                                      | 28.8 ms: 1.13x slower                                                     |
| unpickle                   | 13.3 us                                                      | 15.2 us: 1.14x slower                                                     |
| scimark_fft                | 281 ms                                                       | 327 ms: 1.17x slower                                                      |
| async_generators           | 322 ms                                                       | 377 ms: 1.17x slower                                                      |
| pyflate                    | 449 ms                                                       | 528 ms: 1.18x slower                                                      |
| mypy2                      | 762 ms                                                       | 915 ms: 1.20x slower                                                      |
| telco                      | 6.81 ms                                                      | 8.24 ms: 1.21x slower                                                     |
| coverage                   | 66.1 ms                                                      | 80.4 ms: 1.22x slower                                                     |
| unpack_sequence            | 45.7 ns                                                      | 61.0 ns: 1.34x slower                                                     |
| scimark_sor                | 110 ms                                                       | 153 ms: 1.39x slower                                                      |
| dask                       | 410 ms                                                       | 589 ms: 1.44x slower                                                      |
| python_startup             | 10.7 ms                                                      | 15.5 ms: 1.44x slower                                                     |
| bench_mp_pool              | 4.70 ms                                                      | 6.96 ms: 1.48x slower                                                     |
| python_startup_no_site     | 7.73 ms                                                      | 14.0 ms: 1.81x slower                                                     |
| Geometric mean             | (ref)                                                        | 1.02x faster                                                              |

Benchmark hidden because not significant (8): bench_thread_pool, pycparser, unpickle_pure_python, raytrace, asyncio_websockets, nqueens, deepcopy_memo, tornado_http
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf2-x86_64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 61.53% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.25x