
# Results vs. 3.11.0

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.09x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| chameleon      | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 86.3 ms: 1.08x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 278 ms: 1.19x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 356 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 473 ms: 1.12x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 368 ms: 1.10x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 484 ms: 1.08x faster                                                        |
| async_tree_io              | 808 ms                                                      | 763 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 787 ms: 1.05x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| nbody          | 70.3 ms                                                     | 72.0 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 79.0 ms: 1.15x faster                                                       |
| regex_dna      | 116 ms                                                      | 117 ms: 1.01x slower                                                        |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 133 us: 1.18x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 184 us: 1.13x faster                                                        |
| tomli_loads          | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 95.6 ms: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                                       |
| pickle_dict          | 18.5 us                                                     | 18.9 us: 1.02x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.72 us: 1.05x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.87 us: 1.07x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| pickle               | 6.64 us                                                     | 7.15 us: 1.08x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.45 us: 1.12x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.75 ms: 1.12x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 71.4 us: 4.56x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.8 ms: 1.56x faster                                                       |
| comprehensions             | 15.6 us                                                     | 10.5 us: 1.48x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 503 ms: 1.44x faster                                                        |
| json_dumps                 | 8.09 ms                                                     | 5.61 ms: 1.44x faster                                                       |
| raytrace                   | 213 ms                                                      | 163 ms: 1.31x faster                                                        |
| logging_silent             | 71.8 ns                                                     | 54.8 ns: 1.31x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 2.06 ms: 1.31x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 775 us: 1.23x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.6 ms: 1.23x faster                                                       |
| chaos                      | 48.4 ms                                                     | 39.8 ms: 1.22x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 39.0 ns: 1.20x faster                                                       |
| async_tree_none            | 332 ms                                                      | 278 ms: 1.19x faster                                                        |
| go                         | 101 ms                                                      | 85.7 ms: 1.18x faster                                                       |
| unpickle_pure_python       | 157 us                                                      | 133 us: 1.18x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 85.1 ms: 1.18x faster                                                       |
| nqueens                    | 68.3 ms                                                     | 58.6 ms: 1.17x faster                                                       |
| sympy_str                  | 185 ms                                                      | 159 ms: 1.17x faster                                                        |
| sqlglot_transpile          | 1.16 ms                                                     | 1.00 ms: 1.16x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 79.0 ms: 1.15x faster                                                       |
| hexiom                     | 4.55 ms                                                     | 3.97 ms: 1.15x faster                                                       |
| coroutines                 | 15.0 ms                                                     | 13.1 ms: 1.14x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 55.2 ms: 1.14x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.41 sec: 1.13x faster                                                      |
| logging_simple             | 6.86 us                                                     | 6.06 us: 1.13x faster                                                       |
| pickle_pure_python         | 208 us                                                      | 184 us: 1.13x faster                                                        |
| deepcopy_memo              | 26.0 us                                                     | 23.0 us: 1.13x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.75 ms: 1.12x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 356 ms: 1.12x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 473 ms: 1.12x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.59 us: 1.11x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 40.8 ms: 1.11x faster                                                       |
| sympy_integrate            | 14.0 ms                                                     | 12.7 ms: 1.11x faster                                                       |
| richards                   | 31.4 ms                                                     | 28.4 ms: 1.11x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 368 ms: 1.10x faster                                                        |
| deepcopy                   | 246 us                                                      | 224 us: 1.10x faster                                                        |
| spectral_norm              | 68.3 ms                                                     | 62.2 ms: 1.10x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 42.5 ms: 1.09x faster                                                       |
| crypto_pyaes               | 48.9 ms                                                     | 44.8 ms: 1.09x faster                                                       |
| mypy2                      | 459 ms                                                      | 421 ms: 1.09x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 283 ms: 1.09x faster                                                        |
| sympy_expand               | 299 ms                                                      | 275 ms: 1.09x faster                                                        |
| sqlglot_normalize          | 190 ms                                                      | 175 ms: 1.09x faster                                                        |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.87 sec: 1.08x faster                                                      |
| logging_format             | 7.16 us                                                     | 6.61 us: 1.08x faster                                                       |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 484 ms: 1.08x faster                                                        |
| tornado_http               | 92.8 ms                                                     | 86.3 ms: 1.08x faster                                                       |
| pyflate                    | 312 ms                                                      | 292 ms: 1.07x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.02 sec: 1.07x faster                                                      |
| chameleon                  | 5.26 ms                                                     | 4.93 ms: 1.07x faster                                                       |
| async_tree_io              | 808 ms                                                      | 763 ms: 1.06x faster                                                        |
| pprint_safe_repr           | 529 ms                                                      | 501 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 787 ms: 1.05x faster                                                        |
| dask                       | 273 ms                                                      | 260 ms: 1.05x faster                                                        |
| meteor_contest             | 75.2 ms                                                     | 72.8 ms: 1.03x faster                                                       |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| fannkuch                   | 253 ms                                                      | 246 ms: 1.03x faster                                                        |
| tomli_loads                | 1.46 sec                                                    | 1.42 sec: 1.02x faster                                                      |
| deepcopy_reduce            | 2.06 us                                                     | 2.02 us: 1.02x faster                                                       |
| xml_etree_parse            | 97.6 ms                                                     | 95.6 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 33.9 ms: 1.02x faster                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.54 ms: 1.01x faster                                                       |
| pidigits                   | 150 ms                                                      | 149 ms: 1.01x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                                       |
| 2to3                       | 214 ms                                                      | 216 ms: 1.01x slower                                                        |
| regex_dna                  | 116 ms                                                      | 117 ms: 1.01x slower                                                        |
| xml_etree_process          | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                                       |
| pickle_dict                | 18.5 us                                                     | 18.9 us: 1.02x slower                                                       |
| nbody                      | 70.3 ms                                                     | 72.0 ms: 1.02x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 53.9 ms: 1.03x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.54 ms: 1.03x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.5 ms: 1.04x slower                                                       |
| scimark_sor                | 78.1 ms                                                     | 81.5 ms: 1.04x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.72 us: 1.05x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 752 us: 1.05x slower                                                        |
| regex_effbot               | 1.50 ms                                                     | 1.59 ms: 1.06x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.87 us: 1.07x slower                                                       |
| json_loads                 | 13.0 us                                                     | 13.9 us: 1.07x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 67.7 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.15 us: 1.08x slower                                                       |
| json                       | 2.98 ms                                                     | 3.26 ms: 1.09x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 18.5 ms: 1.10x slower                                                       |
| coverage                   | 43.4 ms                                                     | 48.0 ms: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.45 us: 1.12x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 80.3 ms: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.61 ms: 1.13x slower                                                       |
| async_generators           | 177 ms                                                      | 229 ms: 1.29x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (4): pycparser, float, scimark_fft, bench_thread_pool
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown