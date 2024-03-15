
# Results vs. 3.11.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.06x faster
- HPT reliability: 99.02%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 217 ms: 1.02x slower                                                        |
| chameleon      | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 87.5 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 269 ms: 1.23x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.17x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.13x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 754 ms: 1.10x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 58.1 ms: 1.07x slower                                                       |
| nbody          | 70.3 ms                                                     | 82.6 ms: 1.17x slower                                                       |
| Geometric mean | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| regex_dna      | 116 ms                                                      | 117 ms: 1.00x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 135 us: 1.16x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 180 us: 1.16x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                       |
| unpickle_list        | 2.59 us                                                     | 2.56 us: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.00x slower                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.48 sec: 1.01x slower                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 66.5 ms: 1.01x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.3 us: 1.02x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.9 ms: 1.05x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.28 us: 1.09x slower                                                       |
| pickle               | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| pickle_list          | 2.70 us                                                     | 3.36 us: 1.24x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 75.4 us: 4.32x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 464 ms: 1.56x faster                                                        |
| generators                 | 34.0 ms                                                     | 22.0 ms: 1.54x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.58 ms: 1.45x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 55.3 ns: 1.30x faster                                                       |
| richards_super             | 38.7 ms                                                     | 31.0 ms: 1.25x faster                                                       |
| async_tree_none            | 332 ms                                                      | 269 ms: 1.23x faster                                                        |
| sqlglot_parse              | 953 us                                                      | 773 us: 1.23x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.65 sec: 1.23x faster                                                      |
| raytrace                   | 213 ms                                                      | 175 ms: 1.22x faster                                                        |
| comprehensions             | 15.6 us                                                     | 13.3 us: 1.18x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 340 ms: 1.17x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 455 ms: 1.17x faster                                                        |
| unpack_sequence            | 46.9 ns                                                     | 40.3 ns: 1.16x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 12.9 ms: 1.16x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 135 us: 1.16x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.00 ms: 1.16x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 180 us: 1.16x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 87.0 ms: 1.15x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 352 ms: 1.15x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 22.9 us: 1.14x faster                                                       |
| sqlite_synth               | 1.77 us                                                     | 1.57 us: 1.13x faster                                                       |
| richards                   | 31.4 ms                                                     | 27.9 ms: 1.13x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 274 ms: 1.13x faster                                                        |
| scimark_lu                 | 62.8 ms                                                     | 55.9 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 471 ms: 1.11x faster                                                        |
| sympy_str                  | 185 ms                                                      | 167 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 733 ms: 1.10x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.24 us: 1.10x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 754 ms: 1.10x faster                                                        |
| mypy2                      | 459 ms                                                      | 420 ms: 1.09x faster                                                        |
| go                         | 101 ms                                                      | 93.0 ms: 1.09x faster                                                       |
| deepcopy                   | 246 us                                                      | 227 us: 1.08x faster                                                        |
| dulwich_log                | 46.4 ms                                                     | 42.9 ms: 1.08x faster                                                       |
| sympy_expand               | 299 ms                                                      | 277 ms: 1.08x faster                                                        |
| regex_compile              | 91.0 ms                                                     | 84.8 ms: 1.07x faster                                                       |
| logging_format             | 7.16 us                                                     | 6.68 us: 1.07x faster                                                       |
| chaos                      | 48.4 ms                                                     | 45.2 ms: 1.07x faster                                                       |
| dask                       | 273 ms                                                      | 255 ms: 1.07x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 13.2 ms: 1.07x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 87.5 ms: 1.06x faster                                                       |
| chameleon                  | 5.26 ms                                                     | 5.01 ms: 1.05x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| pycparser                  | 720 ms                                                      | 693 ms: 1.04x faster                                                        |
| mdp                        | 1.59 sec                                                    | 1.53 sec: 1.04x faster                                                      |
| xml_etree_parse            | 97.6 ms                                                     | 94.0 ms: 1.04x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 65.9 ms: 1.04x faster                                                       |
| deepcopy_reduce            | 2.06 us                                                     | 1.99 us: 1.04x faster                                                       |
| sqlglot_normalize          | 190 ms                                                      | 185 ms: 1.03x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 855 us: 1.02x faster                                                        |
| unpickle_list              | 2.59 us                                                     | 2.56 us: 1.01x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.00x slower                                                       |
| regex_dna                  | 116 ms                                                      | 117 ms: 1.00x slower                                                        |
| mako                       | 7.58 ms                                                     | 7.67 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.48 sec: 1.01x slower                                                      |
| meteor_contest             | 75.2 ms                                                     | 76.3 ms: 1.01x slower                                                       |
| xml_etree_iterparse        | 65.6 ms                                                     | 66.5 ms: 1.01x slower                                                       |
| 2to3                       | 214 ms                                                      | 217 ms: 1.02x slower                                                        |
| create_gc_cycles           | 713 us                                                      | 728 us: 1.02x slower                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 35.4 ms: 1.02x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.3 us: 1.02x slower                                                       |
| deltablue                  | 2.70 ms                                                     | 2.77 ms: 1.03x slower                                                       |
| coverage                   | 43.4 ms                                                     | 44.7 ms: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.4 ms: 1.03x slower                                                       |
| pyflate                    | 312 ms                                                      | 323 ms: 1.03x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.7 ms: 1.04x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 81.1 ms: 1.04x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.56 ms: 1.04x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 54.9 ms: 1.05x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 66.7 ms: 1.06x slower                                                       |
| fannkuch                   | 253 ms                                                      | 268 ms: 1.06x slower                                                        |
| float                      | 54.4 ms                                                     | 58.1 ms: 1.07x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.2 ms: 1.08x slower                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 49.5 ms: 1.09x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.28 us: 1.09x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.30 us: 1.10x slower                                                       |
| hexiom                     | 4.55 ms                                                     | 5.07 ms: 1.11x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 79.1 ms: 1.12x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.72 ms: 1.16x slower                                                       |
| scimark_fft                | 179 ms                                                      | 210 ms: 1.17x slower                                                        |
| nbody                      | 70.3 ms                                                     | 82.6 ms: 1.17x slower                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 3.12 ms: 1.21x slower                                                       |
| spectral_norm              | 68.3 ms                                                     | 85.0 ms: 1.24x slower                                                       |
| pickle_list                | 2.70 us                                                     | 3.36 us: 1.24x slower                                                       |
| async_generators           | 177 ms                                                      | 229 ms: 1.30x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmark hidden because not significant (6): pprint_pformat, crypto_pyaes, xml_etree_process, pprint_safe_repr, pidigits, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 99.02% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown