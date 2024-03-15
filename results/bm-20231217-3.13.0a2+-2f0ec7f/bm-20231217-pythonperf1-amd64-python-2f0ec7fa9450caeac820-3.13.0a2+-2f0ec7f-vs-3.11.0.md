
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.11x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 215 ms: 1.01x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.86 ms: 1.08x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 87.7 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 448 ms: 1.18x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 463 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 724 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 51.9 ms: 1.05x faster                                                       |
| nbody          | 70.3 ms                                                     | 69.5 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 77.9 ms: 1.17x faster                                                       |
| regex_dna      | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.49 ms: 1.47x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 129 us: 1.22x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 181 us: 1.15x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 92.0 ms: 1.06x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.0 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.69 us: 1.04x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.04x slower                                                       |
| pickle               | 6.64 us                                                     | 7.02 us: 1.06x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.86 us: 1.06x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.32 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.8 ms: 1.12x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.41 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 72.3 us: 4.51x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 461 ms: 1.58x faster                                                        |
| generators                 | 34.0 ms                                                     | 22.1 ms: 1.54x faster                                                       |
| comprehensions             | 15.6 us                                                     | 10.5 us: 1.49x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.49 ms: 1.47x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.01 ms: 1.35x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 53.8 ns: 1.33x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 36.4 ns: 1.29x faster                                                       |
| raytrace                   | 213 ms                                                      | 166 ms: 1.29x faster                                                        |
| async_tree_none            | 332 ms                                                      | 266 ms: 1.25x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 765 us: 1.25x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.2 ms: 1.24x faster                                                       |
| chaos                      | 48.4 ms                                                     | 39.2 ms: 1.23x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 129 us: 1.22x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 83.3 ms: 1.20x faster                                                       |
| hexiom                     | 4.55 ms                                                     | 3.80 ms: 1.20x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 980 us: 1.19x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 21.9 us: 1.19x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.41 ms: 1.18x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 448 ms: 1.18x faster                                                        |
| nqueens                    | 68.3 ms                                                     | 58.1 ms: 1.18x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 77.9 ms: 1.17x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 342 ms: 1.17x faster                                                        |
| sympy_str                  | 185 ms                                                      | 160 ms: 1.16x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 181 us: 1.15x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.15x faster                                                       |
| logging_simple             | 6.86 us                                                     | 5.99 us: 1.15x faster                                                       |
| go                         | 101 ms                                                      | 88.5 ms: 1.14x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.5 ms: 1.14x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 60.2 ms: 1.13x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 55.4 ms: 1.13x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.41 sec: 1.13x faster                                                      |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.4 ms: 1.13x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 40.1 ms: 1.13x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 43.3 ms: 1.13x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 463 ms: 1.13x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 275 ms: 1.12x faster                                                        |
| deepcopy                   | 246 us                                                      | 220 us: 1.12x faster                                                        |
| async_tree_io              | 808 ms                                                      | 724 ms: 1.11x faster                                                        |
| mypy2                      | 459 ms                                                      | 414 ms: 1.11x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 748 ms: 1.11x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.47 us: 1.11x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 41.9 ms: 1.11x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.83 sec: 1.11x faster                                                      |
| sympy_expand               | 299 ms                                                      | 272 ms: 1.10x faster                                                        |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.36 ms: 1.09x faster                                                       |
| pprint_pformat             | 1.09 sec                                                    | 996 ms: 1.09x faster                                                        |
| pyflate                    | 312 ms                                                      | 287 ms: 1.09x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 488 ms: 1.08x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.86 ms: 1.08x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 177 ms: 1.07x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 92.0 ms: 1.06x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 87.7 ms: 1.06x faster                                                       |
| fannkuch                   | 253 ms                                                      | 240 ms: 1.06x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 1.95 us: 1.06x faster                                                       |
| dask                       | 273 ms                                                      | 258 ms: 1.06x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                      |
| float                      | 54.4 ms                                                     | 51.9 ms: 1.05x faster                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.0 ms: 1.04x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.40 sec: 1.04x faster                                                      |
| meteor_contest             | 75.2 ms                                                     | 73.0 ms: 1.03x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.8 ms: 1.02x faster                                                       |
| xml_etree_process          | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| nbody                      | 70.3 ms                                                     | 69.5 ms: 1.01x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.3 us: 1.01x faster                                                       |
| 2to3                       | 214 ms                                                      | 215 ms: 1.01x slower                                                        |
| xml_etree_generate         | 52.5 ms                                                     | 53.1 ms: 1.01x slower                                                       |
| scimark_fft                | 179 ms                                                      | 182 ms: 1.02x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 727 us: 1.02x slower                                                        |
| scimark_sor                | 78.1 ms                                                     | 79.9 ms: 1.02x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.69 us: 1.04x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.04x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                                       |
| regex_dna                  | 116 ms                                                      | 122 ms: 1.05x slower                                                        |
| coverage                   | 43.4 ms                                                     | 45.9 ms: 1.06x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.02 us: 1.06x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.86 us: 1.06x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.61 ms: 1.07x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 15.3 ms: 1.08x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.32 us: 1.10x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 69.8 ms: 1.10x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.8 ms: 1.12x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 79.8 ms: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.92 ms: 1.21x slower                                                       |
| async_generators           | 177 ms                                                      | 224 ms: 1.27x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (5): bench_thread_pool, pycparser, gc_traversal, pidigits, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown