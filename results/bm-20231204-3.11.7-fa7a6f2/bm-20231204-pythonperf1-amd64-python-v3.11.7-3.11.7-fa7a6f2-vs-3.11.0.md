
# Results vs. 3.11.0

- fork: python
- ref: v3.11.7
- machine: windows-amd64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.02x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 209 ms: 1.02x faster                                        |
| chameleon      | 5.26 ms                                                     | 5.02 ms: 1.05x faster                                       |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                      |
| tornado_http   | 92.8 ms                                                     | 89.7 ms: 1.04x faster                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization_tg  | 405 ms                                                      | 378 ms: 1.07x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                        |
| async_tree_memoization     | 399 ms                                                      | 380 ms: 1.05x faster                                        |
| async_tree_none            | 332 ms                                                      | 317 ms: 1.05x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 294 ms: 1.05x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 500 ms: 1.05x faster                                        |
| async_tree_io              | 808 ms                                                      | 784 ms: 1.03x faster                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                        |
| nbody          | 70.3 ms                                                     | 70.8 ms: 1.01x slower                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.03x faster                                       |
| regex_compile  | 91.0 ms                                                     | 88.3 ms: 1.03x faster                                       |
| regex_dna      | 116 ms                                                      | 119 ms: 1.02x slower                                        |
| regex_effbot   | 1.50 ms                                                     | 1.54 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| unpickle_pure_python | 157 us                                                      | 149 us: 1.06x faster                                        |
| tomli_loads          | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                      |
| pickle_pure_python   | 208 us                                                      | 201 us: 1.04x faster                                        |
| json_dumps           | 8.09 ms                                                     | 7.86 ms: 1.03x faster                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.3 ms: 1.02x faster                                       |
| json_loads           | 13.0 us                                                     | 12.8 us: 1.02x faster                                       |
| pickle               | 6.64 us                                                     | 6.55 us: 1.01x faster                                       |
| xml_etree_generate   | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                       |
| unpickle             | 7.57 us                                                     | 7.74 us: 1.02x slower                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (5): pickle_list, pickle_dict, xml_etree_process, unpickle_list, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.7 ms: 1.07x faster                                       |
| python_startup         | 19.8 ms                                                     | 20.3 ms: 1.03x slower                                       |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                       |
| genshi_xml      | 39.9 ms                                                     | 38.0 ms: 1.05x faster                                       |
| mako            | 7.58 ms                                                     | 7.29 ms: 1.04x faster                                       |
| django_template | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                       |
| Geometric mean  | (ref)                                                       | 1.05x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_text                | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                       |
| python_startup_no_site     | 16.8 ms                                                     | 15.7 ms: 1.07x faster                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 378 ms: 1.07x faster                                        |
| nqueens                    | 68.3 ms                                                     | 64.1 ms: 1.07x faster                                       |
| async_tree_io_tg           | 829 ms                                                      | 783 ms: 1.06x faster                                        |
| raytrace                   | 213 ms                                                      | 202 ms: 1.06x faster                                        |
| unpickle_pure_python       | 157 us                                                      | 149 us: 1.06x faster                                        |
| deepcopy_memo              | 26.0 us                                                     | 24.7 us: 1.05x faster                                       |
| genshi_xml                 | 39.9 ms                                                     | 38.0 ms: 1.05x faster                                       |
| async_tree_memoization     | 399 ms                                                      | 380 ms: 1.05x faster                                        |
| async_tree_none            | 332 ms                                                      | 317 ms: 1.05x faster                                        |
| scimark_sor                | 78.1 ms                                                     | 74.5 ms: 1.05x faster                                       |
| async_tree_none_tg         | 309 ms                                                      | 294 ms: 1.05x faster                                        |
| chameleon                  | 5.26 ms                                                     | 5.02 ms: 1.05x faster                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 500 ms: 1.05x faster                                        |
| telco                      | 4.06 ms                                                     | 3.89 ms: 1.04x faster                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                      |
| sqlite_synth               | 1.77 us                                                     | 1.70 us: 1.04x faster                                       |
| tomli_loads                | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                      |
| mako                       | 7.58 ms                                                     | 7.29 ms: 1.04x faster                                       |
| sympy_integrate            | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                       |
| richards                   | 31.4 ms                                                     | 30.2 ms: 1.04x faster                                       |
| bench_mp_pool              | 63.2 ms                                                     | 60.8 ms: 1.04x faster                                       |
| pprint_safe_repr           | 529 ms                                                      | 509 ms: 1.04x faster                                        |
| pickle_pure_python         | 208 us                                                      | 201 us: 1.04x faster                                        |
| docutils                   | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                      |
| bench_thread_pool          | 872 us                                                      | 842 us: 1.04x faster                                        |
| tornado_http               | 92.8 ms                                                     | 89.7 ms: 1.04x faster                                       |
| dask                       | 273 ms                                                      | 264 ms: 1.03x faster                                        |
| aiohttp                    | 883 us                                                      | 854 us: 1.03x faster                                        |
| django_template            | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                       |
| pycparser                  | 720 ms                                                      | 697 ms: 1.03x faster                                        |
| fannkuch                   | 253 ms                                                      | 245 ms: 1.03x faster                                        |
| regex_v8                   | 14.2 ms                                                     | 13.7 ms: 1.03x faster                                       |
| logging_silent             | 71.8 ns                                                     | 69.6 ns: 1.03x faster                                       |
| deltablue                  | 2.70 ms                                                     | 2.62 ms: 1.03x faster                                       |
| spectral_norm              | 68.3 ms                                                     | 66.3 ms: 1.03x faster                                       |
| regex_compile              | 91.0 ms                                                     | 88.3 ms: 1.03x faster                                       |
| dulwich_log                | 46.4 ms                                                     | 45.0 ms: 1.03x faster                                       |
| json_dumps                 | 8.09 ms                                                     | 7.86 ms: 1.03x faster                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.13 ms: 1.03x faster                                       |
| async_tree_io              | 808 ms                                                      | 784 ms: 1.03x faster                                        |
| async_generators           | 177 ms                                                      | 172 ms: 1.03x faster                                        |
| pylint                     | 323 ms                                                      | 316 ms: 1.02x faster                                        |
| hexiom                     | 4.55 ms                                                     | 4.45 ms: 1.02x faster                                       |
| sqlalchemy_declarative     | 85.6 ms                                                     | 83.7 ms: 1.02x faster                                       |
| pyflate                    | 312 ms                                                      | 305 ms: 1.02x faster                                        |
| 2to3                       | 214 ms                                                      | 209 ms: 1.02x faster                                        |
| sqlglot_parse              | 953 us                                                      | 933 us: 1.02x faster                                        |
| scimark_lu                 | 62.8 ms                                                     | 61.5 ms: 1.02x faster                                       |
| gc_traversal               | 1.49 ms                                                     | 1.46 ms: 1.02x faster                                       |
| deepcopy                   | 246 us                                                      | 242 us: 1.02x faster                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.3 ms: 1.02x faster                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 44.4 ms: 1.02x faster                                       |
| sqlalchemy_imperative      | 10.4 ms                                                     | 10.2 ms: 1.02x faster                                       |
| json_loads                 | 13.0 us                                                     | 12.8 us: 1.02x faster                                       |
| logging_simple             | 6.86 us                                                     | 6.76 us: 1.02x faster                                       |
| richards_super             | 38.7 ms                                                     | 38.2 ms: 1.01x faster                                       |
| pickle                     | 6.64 us                                                     | 6.55 us: 1.01x faster                                       |
| sympy_sum                  | 100 ms                                                      | 98.9 ms: 1.01x faster                                       |
| mypy2                      | 459 ms                                                      | 454 ms: 1.01x faster                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.04 us: 1.01x faster                                       |
| pidigits                   | 150 ms                                                      | 149 ms: 1.01x faster                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.56 ms: 1.01x faster                                       |
| crypto_pyaes               | 48.9 ms                                                     | 48.6 ms: 1.00x faster                                       |
| pathlib                    | 70.9 ms                                                     | 71.2 ms: 1.01x slower                                       |
| xml_etree_generate         | 52.5 ms                                                     | 52.9 ms: 1.01x slower                                       |
| sqlglot_normalize          | 190 ms                                                      | 192 ms: 1.01x slower                                        |
| nbody                      | 70.3 ms                                                     | 70.8 ms: 1.01x slower                                       |
| flaskblogging              | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                      |
| meteor_contest             | 75.2 ms                                                     | 75.9 ms: 1.01x slower                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                       |
| coverage                   | 43.4 ms                                                     | 43.9 ms: 1.01x slower                                       |
| logging_format             | 7.16 us                                                     | 7.25 us: 1.01x slower                                       |
| sympy_expand               | 299 ms                                                      | 303 ms: 1.01x slower                                        |
| chaos                      | 48.4 ms                                                     | 49.1 ms: 1.01x slower                                       |
| thrift                     | 494 us                                                      | 503 us: 1.02x slower                                        |
| go                         | 101 ms                                                      | 103 ms: 1.02x slower                                        |
| unpack_sequence            | 46.9 ns                                                     | 47.9 ns: 1.02x slower                                       |
| unpickle                   | 7.57 us                                                     | 7.74 us: 1.02x slower                                       |
| regex_dna                  | 116 ms                                                      | 119 ms: 1.02x slower                                        |
| python_startup             | 19.8 ms                                                     | 20.3 ms: 1.03x slower                                       |
| regex_effbot               | 1.50 ms                                                     | 1.54 ms: 1.03x slower                                       |
| mdp                        | 1.59 sec                                                    | 1.65 sec: 1.03x slower                                      |
| json                       | 2.98 ms                                                     | 3.22 ms: 1.08x slower                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 2.23 sec: 1.10x slower                                      |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (16): pickle_list, async_tree_cpu_io_mixed, html5lib, float, sympy_str, pickle_dict, coroutines, scimark_fft, generators, xml_etree_process, typing_runtime_protocols, comprehensions, unpickle_list, xml_etree_parse, asyncio_tcp, create_gc_cycles


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown