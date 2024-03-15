
# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_relax
- machine: windows-amd64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.05x slower                                                      |
| chameleon      | 5.26 ms                                                     | 4.63 ms: 1.14x faster                                                     |
| docutils       | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                    |
| tornado_http   | 92.8 ms                                                     | 84.7 ms: 1.10x faster                                                     |
| Geometric mean | (ref)                                                       | 1.05x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                      |
| async_tree_memoization     | 399 ms                                                      | 335 ms: 1.19x faster                                                      |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 267 ms: 1.16x faster                                                      |
| async_tree_io              | 808 ms                                                      | 718 ms: 1.12x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.12x faster                                                      |
| async_tree_io_tg           | 829 ms                                                      | 751 ms: 1.10x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.6 ms: 1.18x faster                                                     |
| float          | 54.4 ms                                                     | 48.5 ms: 1.12x faster                                                     |
| Geometric mean | (ref)                                                       | 1.10x faster                                                              |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 89.9 ms: 1.01x faster                                                     |
| regex_dna      | 116 ms                                                      | 118 ms: 1.02x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.55 ms: 1.04x slower                                                     |
| Geometric mean | (ref)                                                       | 1.02x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.53 ms: 1.46x faster                                                     |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                                      |
| tomli_loads          | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                    |
| xml_etree_parse      | 97.6 ms                                                     | 92.0 ms: 1.06x faster                                                     |
| pickle_dict          | 18.5 us                                                     | 17.4 us: 1.06x faster                                                     |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                     |
| xml_etree_process    | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| xml_etree_generate   | 52.5 ms                                                     | 53.6 ms: 1.02x slower                                                     |
| pickle_list          | 2.70 us                                                     | 2.77 us: 1.03x slower                                                     |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                     |
| pickle               | 6.64 us                                                     | 7.15 us: 1.08x slower                                                     |
| unpickle_list        | 2.59 us                                                     | 2.82 us: 1.09x slower                                                     |
| unpickle             | 7.57 us                                                     | 8.59 us: 1.13x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 23.9 ms: 1.21x slower                                                     |
| python_startup_no_site | 16.8 ms                                                     | 21.6 ms: 1.28x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.24x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 5.95 ms: 1.28x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.9 us: 4.60x faster                                                     |
| generators                 | 34.0 ms                                                     | 20.4 ms: 1.67x faster                                                     |
| asyncio_tcp                | 726 ms                                                      | 466 ms: 1.56x faster                                                      |
| json_dumps                 | 8.09 ms                                                     | 5.53 ms: 1.46x faster                                                     |
| comprehensions             | 15.6 us                                                     | 10.8 us: 1.45x faster                                                     |
| logging_silent             | 71.8 ns                                                     | 55.7 ns: 1.29x faster                                                     |
| deltablue                  | 2.70 ms                                                     | 2.11 ms: 1.28x faster                                                     |
| mako                       | 7.58 ms                                                     | 5.95 ms: 1.28x faster                                                     |
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                      |
| spectral_norm              | 68.3 ms                                                     | 54.6 ms: 1.25x faster                                                     |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.66 sec: 1.22x faster                                                    |
| async_tree_memoization     | 399 ms                                                      | 335 ms: 1.19x faster                                                      |
| async_tree_memoization_tg  | 405 ms                                                      | 340 ms: 1.19x faster                                                      |
| sqlglot_parse              | 953 us                                                      | 801 us: 1.19x faster                                                      |
| pickle_pure_python         | 208 us                                                      | 175 us: 1.19x faster                                                      |
| deepcopy_memo              | 26.0 us                                                     | 21.9 us: 1.19x faster                                                     |
| chaos                      | 48.4 ms                                                     | 40.8 ms: 1.18x faster                                                     |
| nbody                      | 70.3 ms                                                     | 59.6 ms: 1.18x faster                                                     |
| raytrace                   | 213 ms                                                      | 181 ms: 1.18x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 450 ms: 1.18x faster                                                      |
| logging_simple             | 6.86 us                                                     | 5.90 us: 1.16x faster                                                     |
| unpickle_pure_python       | 157 us                                                      | 135 us: 1.16x faster                                                      |
| async_tree_none_tg         | 309 ms                                                      | 267 ms: 1.16x faster                                                      |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                     |
| sqlite_synth               | 1.77 us                                                     | 1.55 us: 1.14x faster                                                     |
| sympy_sum                  | 100 ms                                                      | 87.8 ms: 1.14x faster                                                     |
| chameleon                  | 5.26 ms                                                     | 4.63 ms: 1.14x faster                                                     |
| sqlglot_transpile          | 1.16 ms                                                     | 1.03 ms: 1.13x faster                                                     |
| async_tree_io              | 808 ms                                                      | 718 ms: 1.12x faster                                                      |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.12x faster                                                      |
| dulwich_log                | 46.4 ms                                                     | 41.3 ms: 1.12x faster                                                     |
| tomli_loads                | 1.46 sec                                                    | 1.30 sec: 1.12x faster                                                    |
| float                      | 54.4 ms                                                     | 48.5 ms: 1.12x faster                                                     |
| deepcopy                   | 246 us                                                      | 220 us: 1.12x faster                                                      |
| logging_format             | 7.16 us                                                     | 6.41 us: 1.12x faster                                                     |
| sympy_str                  | 185 ms                                                      | 166 ms: 1.12x faster                                                      |
| crypto_pyaes               | 48.9 ms                                                     | 43.9 ms: 1.11x faster                                                     |
| nqueens                    | 68.3 ms                                                     | 61.5 ms: 1.11x faster                                                     |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.33 ms: 1.11x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 751 ms: 1.10x faster                                                      |
| richards_super             | 38.7 ms                                                     | 35.2 ms: 1.10x faster                                                     |
| tornado_http               | 92.8 ms                                                     | 84.7 ms: 1.10x faster                                                     |
| sqlglot_normalize          | 190 ms                                                      | 175 ms: 1.09x faster                                                      |
| xml_etree_parse            | 97.6 ms                                                     | 92.0 ms: 1.06x faster                                                     |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                     |
| mypy2                      | 459 ms                                                      | 433 ms: 1.06x faster                                                      |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.06x faster                                                     |
| pickle_dict                | 18.5 us                                                     | 17.4 us: 1.06x faster                                                     |
| pyflate                    | 312 ms                                                      | 296 ms: 1.05x faster                                                      |
| mdp                        | 1.59 sec                                                    | 1.52 sec: 1.05x faster                                                    |
| pprint_safe_repr           | 529 ms                                                      | 506 ms: 1.05x faster                                                      |
| sympy_expand               | 299 ms                                                      | 286 ms: 1.05x faster                                                      |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                                    |
| bench_thread_pool          | 872 us                                                      | 839 us: 1.04x faster                                                      |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                     |
| go                         | 101 ms                                                      | 98.1 ms: 1.03x faster                                                     |
| docutils                   | 1.64 sec                                                    | 1.61 sec: 1.02x faster                                                    |
| xml_etree_process          | 37.2 ms                                                     | 36.4 ms: 1.02x faster                                                     |
| meteor_contest             | 75.2 ms                                                     | 73.7 ms: 1.02x faster                                                     |
| regex_compile              | 91.0 ms                                                     | 89.9 ms: 1.01x faster                                                     |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                     |
| richards                   | 31.4 ms                                                     | 31.7 ms: 1.01x slower                                                     |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                     |
| regex_dna                  | 116 ms                                                      | 118 ms: 1.02x slower                                                      |
| xml_etree_generate         | 52.5 ms                                                     | 53.6 ms: 1.02x slower                                                     |
| fannkuch                   | 253 ms                                                      | 259 ms: 1.02x slower                                                      |
| pickle_list                | 2.70 us                                                     | 2.77 us: 1.03x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.55 ms: 1.04x slower                                                     |
| create_gc_cycles           | 713 us                                                      | 742 us: 1.04x slower                                                      |
| 2to3                       | 214 ms                                                      | 223 ms: 1.05x slower                                                      |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                     |
| pathlib                    | 70.9 ms                                                     | 76.1 ms: 1.07x slower                                                     |
| pickle                     | 6.64 us                                                     | 7.15 us: 1.08x slower                                                     |
| scimark_sor                | 78.1 ms                                                     | 84.4 ms: 1.08x slower                                                     |
| unpickle_list              | 2.59 us                                                     | 2.82 us: 1.09x slower                                                     |
| hexiom                     | 4.55 ms                                                     | 5.00 ms: 1.10x slower                                                     |
| coverage                   | 43.4 ms                                                     | 48.1 ms: 1.11x slower                                                     |
| bench_mp_pool              | 63.2 ms                                                     | 70.3 ms: 1.11x slower                                                     |
| telco                      | 4.06 ms                                                     | 4.57 ms: 1.13x slower                                                     |
| unpickle                   | 7.57 us                                                     | 8.59 us: 1.13x slower                                                     |
| scimark_lu                 | 62.8 ms                                                     | 74.5 ms: 1.19x slower                                                     |
| json                       | 2.98 ms                                                     | 3.55 ms: 1.19x slower                                                     |
| python_startup             | 19.8 ms                                                     | 23.9 ms: 1.21x slower                                                     |
| unpack_sequence            | 46.9 ns                                                     | 57.6 ns: 1.23x slower                                                     |
| python_startup_no_site     | 16.8 ms                                                     | 21.6 ms: 1.28x slower                                                     |
| async_generators           | 177 ms                                                      | 233 ms: 1.32x slower                                                      |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                              |

Benchmark hidden because not significant (4): scimark_fft, pidigits, scimark_monte_carlo, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown