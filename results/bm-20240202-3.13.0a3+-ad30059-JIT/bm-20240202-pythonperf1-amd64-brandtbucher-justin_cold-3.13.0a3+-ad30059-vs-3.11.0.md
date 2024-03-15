
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_cold
- machine: windows-amd64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.05x slower                                                     |
| chameleon      | 5.26 ms                                                     | 4.82 ms: 1.09x faster                                                    |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                   |
| tornado_http   | 92.8 ms                                                     | 87.3 ms: 1.06x faster                                                    |
| Geometric mean | (ref)                                                       | 1.03x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                     |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 468 ms: 1.13x faster                                                     |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                                     |
| async_tree_none_tg         | 309 ms                                                      | 281 ms: 1.10x faster                                                     |
| async_tree_io              | 808 ms                                                      | 738 ms: 1.09x faster                                                     |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 777 ms: 1.07x faster                                                     |
| Geometric mean             | (ref)                                                       | 1.12x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                                    |
| float          | 54.4 ms                                                     | 50.8 ms: 1.07x faster                                                    |
| pidigits       | 150 ms                                                      | 152 ms: 1.02x slower                                                     |
| Geometric mean | (ref)                                                       | 1.06x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                    |
| regex_dna      | 116 ms                                                      | 118 ms: 1.02x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                    |
| regex_v8       | 14.2 ms                                                     | 17.2 ms: 1.22x slower                                                    |
| Geometric mean | (ref)                                                       | 1.04x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                    |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.25x faster                                                     |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                     |
| tomli_loads          | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                                   |
| pickle_dict          | 18.5 us                                                     | 18.0 us: 1.03x faster                                                    |
| xml_etree_parse      | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                    |
| xml_etree_iterparse  | 65.6 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                    |
| pickle_list          | 2.70 us                                                     | 2.78 us: 1.03x slower                                                    |
| unpickle_list        | 2.59 us                                                     | 2.76 us: 1.07x slower                                                    |
| xml_etree_generate   | 52.5 ms                                                     | 56.3 ms: 1.07x slower                                                    |
| json_loads           | 13.0 us                                                     | 14.1 us: 1.08x slower                                                    |
| pickle               | 6.64 us                                                     | 7.30 us: 1.10x slower                                                    |
| unpickle             | 7.57 us                                                     | 8.82 us: 1.16x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 21.3 ms: 1.08x slower                                                    |
| python_startup_no_site | 16.8 ms                                                     | 19.2 ms: 1.14x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.68 ms: 1.14x faster                                                    |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240202-pythonperf1-amd64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.1 us: 4.52x faster                                                    |
| generators                 | 34.0 ms                                                     | 20.8 ms: 1.63x faster                                                    |
| asyncio_tcp                | 726 ms                                                      | 494 ms: 1.47x faster                                                     |
| json_dumps                 | 8.09 ms                                                     | 5.54 ms: 1.46x faster                                                    |
| logging_silent             | 71.8 ns                                                     | 53.2 ns: 1.35x faster                                                    |
| richards_super             | 38.7 ms                                                     | 29.0 ms: 1.34x faster                                                    |
| comprehensions             | 15.6 us                                                     | 11.9 us: 1.31x faster                                                    |
| sqlglot_parse              | 953 us                                                      | 752 us: 1.27x faster                                                     |
| deltablue                  | 2.70 ms                                                     | 2.14 ms: 1.26x faster                                                    |
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                     |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.25x faster                                                     |
| raytrace                   | 213 ms                                                      | 173 ms: 1.23x faster                                                     |
| richards                   | 31.4 ms                                                     | 25.7 ms: 1.22x faster                                                    |
| deepcopy_memo              | 26.0 us                                                     | 21.6 us: 1.20x faster                                                    |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                     |
| sqlglot_transpile          | 1.16 ms                                                     | 990 us: 1.18x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 344 ms: 1.16x faster                                                     |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                    |
| nqueens                    | 68.3 ms                                                     | 59.7 ms: 1.14x faster                                                    |
| logging_simple             | 6.86 us                                                     | 6.03 us: 1.14x faster                                                    |
| nbody                      | 70.3 ms                                                     | 61.9 ms: 1.14x faster                                                    |
| mako                       | 7.58 ms                                                     | 6.68 ms: 1.14x faster                                                    |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 468 ms: 1.13x faster                                                     |
| async_tree_memoization_tg  | 405 ms                                                      | 359 ms: 1.13x faster                                                     |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.12x faster                                                    |
| scimark_lu                 | 62.8 ms                                                     | 56.0 ms: 1.12x faster                                                    |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.81 sec: 1.12x faster                                                   |
| deepcopy                   | 246 us                                                      | 221 us: 1.12x faster                                                     |
| regex_compile              | 91.0 ms                                                     | 81.6 ms: 1.12x faster                                                    |
| chaos                      | 48.4 ms                                                     | 43.9 ms: 1.10x faster                                                    |
| sympy_sum                  | 100 ms                                                      | 90.9 ms: 1.10x faster                                                    |
| tomli_loads                | 1.46 sec                                                    | 1.32 sec: 1.10x faster                                                   |
| async_tree_none_tg         | 309 ms                                                      | 281 ms: 1.10x faster                                                     |
| sympy_str                  | 185 ms                                                      | 169 ms: 1.09x faster                                                     |
| async_tree_io              | 808 ms                                                      | 738 ms: 1.09x faster                                                     |
| chameleon                  | 5.26 ms                                                     | 4.82 ms: 1.09x faster                                                    |
| dulwich_log                | 46.4 ms                                                     | 42.5 ms: 1.09x faster                                                    |
| logging_format             | 7.16 us                                                     | 6.58 us: 1.09x faster                                                    |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 488 ms: 1.07x faster                                                     |
| pprint_pformat             | 1.09 sec                                                    | 1.01 sec: 1.07x faster                                                   |
| float                      | 54.4 ms                                                     | 50.8 ms: 1.07x faster                                                    |
| deepcopy_reduce            | 2.06 us                                                     | 1.93 us: 1.07x faster                                                    |
| unpack_sequence            | 46.9 ns                                                     | 43.9 ns: 1.07x faster                                                    |
| async_tree_io_tg           | 829 ms                                                      | 777 ms: 1.07x faster                                                     |
| tornado_http               | 92.8 ms                                                     | 87.3 ms: 1.06x faster                                                    |
| pprint_safe_repr           | 529 ms                                                      | 499 ms: 1.06x faster                                                     |
| sqlglot_normalize          | 190 ms                                                      | 181 ms: 1.05x faster                                                     |
| scimark_sor                | 78.1 ms                                                     | 74.4 ms: 1.05x faster                                                    |
| mypy2                      | 459 ms                                                      | 441 ms: 1.04x faster                                                     |
| crypto_pyaes               | 48.9 ms                                                     | 47.0 ms: 1.04x faster                                                    |
| sympy_integrate            | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                                    |
| dask                       | 273 ms                                                      | 264 ms: 1.04x faster                                                     |
| sympy_expand               | 299 ms                                                      | 290 ms: 1.03x faster                                                     |
| pickle_dict                | 18.5 us                                                     | 18.0 us: 1.03x faster                                                    |
| fannkuch                   | 253 ms                                                      | 247 ms: 1.03x faster                                                     |
| pycparser                  | 720 ms                                                      | 701 ms: 1.03x faster                                                     |
| xml_etree_parse            | 97.6 ms                                                     | 95.2 ms: 1.03x faster                                                    |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                   |
| bench_thread_pool          | 872 us                                                      | 855 us: 1.02x faster                                                     |
| spectral_norm              | 68.3 ms                                                     | 67.7 ms: 1.01x faster                                                    |
| go                         | 101 ms                                                      | 100 ms: 1.01x faster                                                     |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                    |
| xml_etree_iterparse        | 65.6 ms                                                     | 66.6 ms: 1.02x slower                                                    |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.02x slower                                                     |
| pidigits                   | 150 ms                                                      | 152 ms: 1.02x slower                                                     |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                                    |
| pickle_list                | 2.70 us                                                     | 2.78 us: 1.03x slower                                                    |
| meteor_contest             | 75.2 ms                                                     | 77.5 ms: 1.03x slower                                                    |
| create_gc_cycles           | 713 us                                                      | 736 us: 1.03x slower                                                     |
| gc_traversal               | 1.49 ms                                                     | 1.55 ms: 1.04x slower                                                    |
| 2to3                       | 214 ms                                                      | 223 ms: 1.05x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                    |
| mdp                        | 1.59 sec                                                    | 1.68 sec: 1.05x slower                                                   |
| unpickle_list              | 2.59 us                                                     | 2.76 us: 1.07x slower                                                    |
| xml_etree_generate         | 52.5 ms                                                     | 56.3 ms: 1.07x slower                                                    |
| python_startup             | 19.8 ms                                                     | 21.3 ms: 1.08x slower                                                    |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.79 ms: 1.08x slower                                                    |
| json_loads                 | 13.0 us                                                     | 14.1 us: 1.08x slower                                                    |
| coverage                   | 43.4 ms                                                     | 47.3 ms: 1.09x slower                                                    |
| scimark_fft                | 179 ms                                                      | 197 ms: 1.10x slower                                                     |
| pickle                     | 6.64 us                                                     | 7.30 us: 1.10x slower                                                    |
| bench_mp_pool              | 63.2 ms                                                     | 70.0 ms: 1.11x slower                                                    |
| telco                      | 4.06 ms                                                     | 4.57 ms: 1.12x slower                                                    |
| python_startup_no_site     | 16.8 ms                                                     | 19.2 ms: 1.14x slower                                                    |
| pathlib                    | 70.9 ms                                                     | 82.0 ms: 1.16x slower                                                    |
| unpickle                   | 7.57 us                                                     | 8.82 us: 1.16x slower                                                    |
| hexiom                     | 4.55 ms                                                     | 5.52 ms: 1.21x slower                                                    |
| regex_v8                   | 14.2 ms                                                     | 17.2 ms: 1.22x slower                                                    |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.6 ms: 1.25x slower                                                    |
| async_generators           | 177 ms                                                      | 248 ms: 1.40x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                             |

Benchmark hidden because not significant (2): json, pyflate
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown