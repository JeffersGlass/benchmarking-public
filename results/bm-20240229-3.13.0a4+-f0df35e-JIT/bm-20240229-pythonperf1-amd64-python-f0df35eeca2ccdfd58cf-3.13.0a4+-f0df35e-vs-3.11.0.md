# Results vs. 3.11.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-amd64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.08x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 84.8 ms: 1.09x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 346 ms: 1.17x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 757 ms: 1.09x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| float          | 54.4 ms                                                     | 48.8 ms: 1.11x faster                                                       |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 116 ms                                                      | 114 ms: 1.02x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.49 ms: 1.47x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                        |
| unpickle_pure_python | 157 us                                                      | 138 us: 1.13x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 91.8 ms: 1.06x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 17.5 us: 1.06x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.5 ms: 1.05x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.2 ms: 1.03x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.88 us: 1.07x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.78 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.19 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.50 us: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 24.0 ms: 1.21x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 21.7 ms: 1.29x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.25x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 5.90 ms: 1.29x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.9 us: 4.66x faster                                                       |
| generators                 | 34.0 ms                                                     | 20.1 ms: 1.69x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 468 ms: 1.55x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.49 ms: 1.47x faster                                                       |
| comprehensions             | 15.6 us                                                     | 11.1 us: 1.40x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.09 ms: 1.29x faster                                                       |
| mako                       | 7.58 ms                                                     | 5.90 ms: 1.29x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 56.0 ns: 1.28x faster                                                       |
| async_tree_none            | 332 ms                                                      | 264 ms: 1.26x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 56.3 ms: 1.21x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 792 us: 1.20x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.71 sec: 1.18x faster                                                      |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 449 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                                        |
| nbody                      | 70.3 ms                                                     | 59.9 ms: 1.17x faster                                                       |
| chaos                      | 48.4 ms                                                     | 41.2 ms: 1.17x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 346 ms: 1.17x faster                                                        |
| raytrace                   | 213 ms                                                      | 183 ms: 1.17x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 180 us: 1.16x faster                                                        |
| logging_simple             | 6.86 us                                                     | 5.96 us: 1.15x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.15x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.02 ms: 1.14x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 22.7 us: 1.14x faster                                                       |
| sympy_sum                  | 100 ms                                                      | 88.2 ms: 1.14x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 272 ms: 1.13x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 138 us: 1.13x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.29 sec: 1.13x faster                                                      |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.29 ms: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 465 ms: 1.13x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.38 us: 1.12x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.58 us: 1.12x faster                                                       |
| async_tree_io              | 808 ms                                                      | 722 ms: 1.12x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.43 sec: 1.11x faster                                                      |
| float                      | 54.4 ms                                                     | 48.8 ms: 1.11x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 61.4 ms: 1.11x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 41.8 ms: 1.11x faster                                                       |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                        |
| richards_super             | 38.7 ms                                                     | 35.0 ms: 1.10x faster                                                       |
| deepcopy                   | 246 us                                                      | 223 us: 1.10x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 44.2 ms: 1.10x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 4.80 ms: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 757 ms: 1.09x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 84.8 ms: 1.09x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 176 ms: 1.08x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 91.8 ms: 1.06x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.3 ms: 1.06x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 17.5 us: 1.06x faster                                                       |
| pyflate                    | 312 ms                                                      | 298 ms: 1.05x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 62.5 ms: 1.05x faster                                                       |
| mypy2                      | 459 ms                                                      | 438 ms: 1.05x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 840 us: 1.04x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 510 ms: 1.04x faster                                                        |
| sympy_expand               | 299 ms                                                      | 288 ms: 1.04x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.99 us: 1.04x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.2 ms: 1.03x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.06 sec: 1.03x faster                                                      |
| meteor_contest             | 75.2 ms                                                     | 73.3 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.02x faster                                                      |
| regex_dna                  | 116 ms                                                      | 114 ms: 1.02x faster                                                        |
| go                         | 101 ms                                                      | 99.8 ms: 1.01x faster                                                       |
| richards                   | 31.4 ms                                                     | 31.6 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.50 ms: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 46.3 ms: 1.02x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| fannkuch                   | 253 ms                                                      | 261 ms: 1.03x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 742 us: 1.04x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| 2to3                       | 214 ms                                                      | 223 ms: 1.04x slower                                                        |
| coverage                   | 43.4 ms                                                     | 45.8 ms: 1.06x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.7 us: 1.06x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.88 us: 1.07x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.78 us: 1.07x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 76.1 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.19 us: 1.08x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.01 ms: 1.10x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 69.9 ms: 1.11x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 87.1 ms: 1.12x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.50 us: 1.12x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.65 ms: 1.14x slower                                                       |
| scimark_lu                 | 62.8 ms                                                     | 72.0 ms: 1.15x slower                                                       |
| python_startup             | 19.8 ms                                                     | 24.0 ms: 1.21x slower                                                       |
| unpack_sequence            | 46.9 ns                                                     | 58.3 ns: 1.24x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 21.7 ms: 1.29x slower                                                       |
| async_generators           | 177 ms                                                      | 242 ms: 1.36x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.08x faster                                                                |

Benchmark hidden because not significant (5): scimark_fft, regex_compile, pidigits, json, pycparser
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown