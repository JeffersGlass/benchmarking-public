
# Results vs. 3.11.0

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-amd64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 85.0 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 337 ms: 1.18x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 343 ms: 1.18x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 266 ms: 1.16x faster                                                        |
| async_tree_io              | 808 ms                                                      | 709 ms: 1.14x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 466 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 746 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 61.4 ms: 1.15x faster                                                       |
| float          | 54.4 ms                                                     | 50.5 ms: 1.08x faster                                                       |
| pidigits       | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 80.1 ms: 1.14x faster                                                       |
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 126 us: 1.24x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.18x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 91.5 ms: 1.07x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 52.0 ms: 1.01x faster                                                       |
| pickle_list          | 2.70 us                                                     | 2.73 us: 1.01x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.04x slower                                                       |
| pickle               | 6.64 us                                                     | 7.31 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.46 us: 1.12x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.92 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.66 ms: 1.14x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 70.1 us: 4.65x faster                                                       |
| generators                 | 34.0 ms                                                     | 19.9 ms: 1.71x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 469 ms: 1.55x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.56 ms: 1.46x faster                                                       |
| comprehensions             | 15.6 us                                                     | 10.8 us: 1.45x faster                                                       |
| richards_super             | 38.7 ms                                                     | 28.4 ms: 1.36x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 1.99 ms: 1.36x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 54.6 ns: 1.31x faster                                                       |
| async_tree_none            | 332 ms                                                      | 261 ms: 1.27x faster                                                        |
| raytrace                   | 213 ms                                                      | 171 ms: 1.25x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 763 us: 1.25x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 126 us: 1.24x faster                                                        |
| richards                   | 31.4 ms                                                     | 25.8 ms: 1.22x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.67 sec: 1.21x faster                                                      |
| sqlglot_transpile          | 1.16 ms                                                     | 975 us: 1.19x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.49 us: 1.19x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 447 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 337 ms: 1.18x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.18x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 343 ms: 1.18x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 85.4 ms: 1.17x faster                                                       |
| sympy_str                  | 185 ms                                                      | 158 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 266 ms: 1.16x faster                                                        |
| chaos                      | 48.4 ms                                                     | 41.9 ms: 1.15x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.95 us: 1.15x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 59.3 ms: 1.15x faster                                                       |
| nbody                      | 70.3 ms                                                     | 61.4 ms: 1.15x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 40.5 ms: 1.15x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 22.8 us: 1.14x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.14x faster                                                       |
| async_tree_io              | 808 ms                                                      | 709 ms: 1.14x faster                                                        |
| mako                       | 7.58 ms                                                     | 6.66 ms: 1.14x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 80.1 ms: 1.14x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| unpack_sequence            | 46.9 ns                                                     | 41.6 ns: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 466 ms: 1.12x faster                                                        |
| deepcopy                   | 246 us                                                      | 220 us: 1.12x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 170 ms: 1.12x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 56.4 ms: 1.11x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 746 ms: 1.11x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.45 us: 1.11x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 988 ms: 1.10x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 85.0 ms: 1.09x faster                                                       |
| pprint_safe_repr           | 529 ms                                                      | 486 ms: 1.09x faster                                                        |
| mypy2                      | 459 ms                                                      | 422 ms: 1.09x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.0 ms: 1.08x faster                                                       |
| float                      | 54.4 ms                                                     | 50.5 ms: 1.08x faster                                                       |
| dask                       | 273 ms                                                      | 253 ms: 1.08x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 63.8 ms: 1.07x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 91.5 ms: 1.07x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.94 us: 1.06x faster                                                       |
| sympy_expand               | 299 ms                                                      | 281 ms: 1.06x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| go                         | 101 ms                                                      | 96.0 ms: 1.05x faster                                                       |
| fannkuch                   | 253 ms                                                      | 241 ms: 1.05x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 46.4 ms: 1.05x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.6 us: 1.05x faster                                                       |
| pycparser                  | 720 ms                                                      | 691 ms: 1.04x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 838 us: 1.04x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.0 ms: 1.03x faster                                                       |
| pyflate                    | 312 ms                                                      | 309 ms: 1.01x faster                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 52.0 ms: 1.01x faster                                                       |
| scimark_sor                | 78.1 ms                                                     | 77.8 ms: 1.00x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.60 sec: 1.00x slower                                                      |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| pickle_list                | 2.70 us                                                     | 2.73 us: 1.01x slower                                                       |
| pidigits                   | 150 ms                                                      | 152 ms: 1.01x slower                                                        |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.63 ms: 1.02x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 732 us: 1.03x slower                                                        |
| meteor_contest             | 75.2 ms                                                     | 77.3 ms: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 66.3 ms: 1.05x slower                                                       |
| scimark_fft                | 179 ms                                                      | 190 ms: 1.06x slower                                                        |
| pathlib                    | 70.9 ms                                                     | 75.4 ms: 1.06x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.3 ms: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.3 ms: 1.09x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.31 us: 1.10x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.46 us: 1.12x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.15 ms: 1.13x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.92 us: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.60 ms: 1.13x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 56.9 ms: 1.26x slower                                                       |
| async_generators           | 177 ms                                                      | 236 ms: 1.34x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown