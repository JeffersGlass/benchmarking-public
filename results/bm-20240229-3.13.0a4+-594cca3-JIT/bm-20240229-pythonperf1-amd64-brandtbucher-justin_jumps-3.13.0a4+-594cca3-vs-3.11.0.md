# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_jumps
- machine: windows-amd64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 222 ms: 1.04x slower                                                      |
| chameleon      | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                     |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                    |
| tornado_http   | 92.8 ms                                                     | 84.6 ms: 1.10x faster                                                     |
| Geometric mean | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                      |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.17x faster                                                      |
| async_tree_memoization_tg  | 405 ms                                                      | 349 ms: 1.16x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                      |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                      |
| async_tree_io_tg           | 829 ms                                                      | 760 ms: 1.09x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 480 ms: 1.09x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 60.2 ms: 1.17x faster                                                     |
| float          | 54.4 ms                                                     | 48.7 ms: 1.12x faster                                                     |
| pidigits       | 150 ms                                                      | 151 ms: 1.00x slower                                                      |
| Geometric mean | (ref)                                                       | 1.09x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 83.6 ms: 1.09x faster                                                     |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.43 ms: 1.49x faster                                                     |
| tomli_loads          | 1.46 sec                                                    | 1.17 sec: 1.24x faster                                                    |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.21x faster                                                      |
| pickle_pure_python   | 208 us                                                      | 178 us: 1.17x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 92.2 ms: 1.06x faster                                                     |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                     |
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.05x faster                                                     |
| xml_etree_process    | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 53.4 ms: 1.02x slower                                                     |
| json_loads           | 13.0 us                                                     | 13.8 us: 1.06x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.83 us: 1.09x slower                                                     |
| pickle               | 6.64 us                                                     | 7.60 us: 1.15x slower                                                     |
| unpickle             | 7.57 us                                                     | 8.69 us: 1.15x slower                                                     |
| pickle_list          | 2.70 us                                                     | 3.12 us: 1.16x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                     |
| python_startup_no_site | 16.8 ms                                                     | 21.7 ms: 1.29x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 5.63 ms: 1.35x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.9 us: 4.66x faster                                                     |
| generators                 | 34.0 ms                                                     | 20.2 ms: 1.68x faster                                                     |
| asyncio_tcp                | 726 ms                                                      | 464 ms: 1.56x faster                                                      |
| comprehensions             | 15.6 us                                                     | 10.3 us: 1.52x faster                                                     |
| json_dumps                 | 8.09 ms                                                     | 5.43 ms: 1.49x faster                                                     |
| mako                       | 7.58 ms                                                     | 5.63 ms: 1.35x faster                                                     |
| spectral_norm              | 68.3 ms                                                     | 51.1 ms: 1.34x faster                                                     |
| deltablue                  | 2.70 ms                                                     | 2.05 ms: 1.32x faster                                                     |
| logging_silent             | 71.8 ns                                                     | 54.7 ns: 1.31x faster                                                     |
| async_tree_none            | 332 ms                                                      | 263 ms: 1.26x faster                                                      |
| tomli_loads                | 1.46 sec                                                    | 1.17 sec: 1.24x faster                                                    |
| chaos                      | 48.4 ms                                                     | 39.3 ms: 1.23x faster                                                     |
| sqlglot_parse              | 953 us                                                      | 778 us: 1.22x faster                                                      |
| richards_super             | 38.7 ms                                                     | 31.8 ms: 1.22x faster                                                     |
| unpickle_pure_python       | 157 us                                                      | 130 us: 1.21x faster                                                      |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.69 sec: 1.20x faster                                                    |
| raytrace                   | 213 ms                                                      | 179 ms: 1.19x faster                                                      |
| logging_simple             | 6.86 us                                                     | 5.80 us: 1.18x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                      |
| deepcopy_memo              | 26.0 us                                                     | 22.1 us: 1.18x faster                                                     |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 451 ms: 1.17x faster                                                      |
| pickle_pure_python         | 208 us                                                      | 178 us: 1.17x faster                                                      |
| nbody                      | 70.3 ms                                                     | 60.2 ms: 1.17x faster                                                     |
| async_tree_memoization_tg  | 405 ms                                                      | 349 ms: 1.16x faster                                                      |
| sqlglot_transpile          | 1.16 ms                                                     | 1.01 ms: 1.16x faster                                                     |
| sympy_sum                  | 100 ms                                                      | 86.6 ms: 1.16x faster                                                     |
| logging_format             | 7.16 us                                                     | 6.24 us: 1.15x faster                                                     |
| fannkuch                   | 253 ms                                                      | 221 ms: 1.15x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.14x faster                                                      |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.13x faster                                                      |
| coroutines                 | 15.0 ms                                                     | 13.2 ms: 1.13x faster                                                     |
| crypto_pyaes               | 48.9 ms                                                     | 43.5 ms: 1.12x faster                                                     |
| dulwich_log                | 46.4 ms                                                     | 41.3 ms: 1.12x faster                                                     |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.29 ms: 1.12x faster                                                     |
| pprint_pformat             | 1.09 sec                                                    | 969 ms: 1.12x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                     |
| float                      | 54.4 ms                                                     | 48.7 ms: 1.12x faster                                                     |
| nqueens                    | 68.3 ms                                                     | 61.3 ms: 1.12x faster                                                     |
| pprint_safe_repr           | 529 ms                                                      | 475 ms: 1.11x faster                                                      |
| async_tree_io              | 808 ms                                                      | 725 ms: 1.11x faster                                                      |
| chameleon                  | 5.26 ms                                                     | 4.77 ms: 1.10x faster                                                     |
| deepcopy                   | 246 us                                                      | 224 us: 1.10x faster                                                      |
| richards                   | 31.4 ms                                                     | 28.5 ms: 1.10x faster                                                     |
| tornado_http               | 92.8 ms                                                     | 84.6 ms: 1.10x faster                                                     |
| scimark_monte_carlo        | 45.3 ms                                                     | 41.5 ms: 1.09x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 760 ms: 1.09x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 480 ms: 1.09x faster                                                      |
| pyflate                    | 312 ms                                                      | 287 ms: 1.09x faster                                                      |
| regex_compile              | 91.0 ms                                                     | 83.6 ms: 1.09x faster                                                     |
| sympy_integrate            | 14.0 ms                                                     | 13.0 ms: 1.08x faster                                                     |
| sqlglot_normalize          | 190 ms                                                      | 177 ms: 1.07x faster                                                      |
| sympy_expand               | 299 ms                                                      | 280 ms: 1.07x faster                                                      |
| scimark_fft                | 179 ms                                                      | 169 ms: 1.06x faster                                                      |
| xml_etree_parse            | 97.6 ms                                                     | 92.2 ms: 1.06x faster                                                     |
| deepcopy_reduce            | 2.06 us                                                     | 1.95 us: 1.06x faster                                                     |
| mypy2                      | 459 ms                                                      | 436 ms: 1.05x faster                                                      |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                     |
| mdp                        | 1.59 sec                                                    | 1.52 sec: 1.05x faster                                                    |
| pickle_dict                | 18.5 us                                                     | 17.7 us: 1.05x faster                                                     |
| go                         | 101 ms                                                      | 96.8 ms: 1.04x faster                                                     |
| meteor_contest             | 75.2 ms                                                     | 72.2 ms: 1.04x faster                                                     |
| unpack_sequence            | 46.9 ns                                                     | 45.2 ns: 1.04x faster                                                     |
| hexiom                     | 4.55 ms                                                     | 4.39 ms: 1.04x faster                                                     |
| pycparser                  | 720 ms                                                      | 696 ms: 1.03x faster                                                      |
| bench_thread_pool          | 872 us                                                      | 845 us: 1.03x faster                                                      |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                    |
| xml_etree_process          | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| pidigits                   | 150 ms                                                      | 151 ms: 1.00x slower                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                     |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                     |
| xml_etree_generate         | 52.5 ms                                                     | 53.4 ms: 1.02x slower                                                     |
| regex_dna                  | 116 ms                                                      | 120 ms: 1.03x slower                                                      |
| create_gc_cycles           | 713 us                                                      | 738 us: 1.04x slower                                                      |
| 2to3                       | 214 ms                                                      | 222 ms: 1.04x slower                                                      |
| regex_v8                   | 14.2 ms                                                     | 14.8 ms: 1.04x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                     |
| coverage                   | 43.4 ms                                                     | 45.7 ms: 1.05x slower                                                     |
| json_loads                 | 13.0 us                                                     | 13.8 us: 1.06x slower                                                     |
| pathlib                    | 70.9 ms                                                     | 76.0 ms: 1.07x slower                                                     |
| scimark_sor                | 78.1 ms                                                     | 84.6 ms: 1.08x slower                                                     |
| unpickle_list              | 2.59 us                                                     | 2.83 us: 1.09x slower                                                     |
| bench_mp_pool              | 63.2 ms                                                     | 69.8 ms: 1.10x slower                                                     |
| telco                      | 4.06 ms                                                     | 4.57 ms: 1.12x slower                                                     |
| pickle                     | 6.64 us                                                     | 7.60 us: 1.15x slower                                                     |
| unpickle                   | 7.57 us                                                     | 8.69 us: 1.15x slower                                                     |
| pickle_list                | 2.70 us                                                     | 3.12 us: 1.16x slower                                                     |
| scimark_lu                 | 62.8 ms                                                     | 73.0 ms: 1.16x slower                                                     |
| python_startup             | 19.8 ms                                                     | 23.8 ms: 1.20x slower                                                     |
| python_startup_no_site     | 16.8 ms                                                     | 21.7 ms: 1.29x slower                                                     |
| async_generators           | 177 ms                                                      | 240 ms: 1.36x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                              |

Benchmark hidden because not significant (1): json
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown