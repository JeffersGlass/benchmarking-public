
# Results vs. 3.11.0

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 210 ms: 1.01x faster                                                        |
| chameleon      | 5.26 ms                                                     | 4.88 ms: 1.08x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 84.5 ms: 1.10x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 456 ms: 1.16x faster                                                        |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 358 ms: 1.13x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| async_tree_none_tg         | 309 ms                                                      | 280 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 475 ms: 1.10x faster                                                        |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 53.3 ms: 1.02x faster                                                       |
| nbody          | 70.3 ms                                                     | 70.0 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 78.2 ms: 1.16x faster                                                       |
| regex_dna      | 116 ms                                                      | 116 ms: 1.01x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.03x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.55 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 127 us: 1.24x faster                                                        |
| pickle_pure_python   | 208 us                                                      | 183 us: 1.14x faster                                                        |
| xml_etree_parse      | 97.6 ms                                                     | 90.8 ms: 1.07x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                                       |
| tomli_loads          | 1.46 sec                                                    | 1.45 sec: 1.01x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_process    | 37.2 ms                                                     | 37.5 ms: 1.01x slower                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 54.1 ms: 1.03x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| unpickle_list        | 2.59 us                                                     | 2.73 us: 1.05x slower                                                       |
| pickle               | 6.64 us                                                     | 7.24 us: 1.09x slower                                                       |
| pickle_list          | 2.70 us                                                     | 2.95 us: 1.10x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| python_startup_no_site | 16.8 ms                                                     | 17.9 ms: 1.06x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.58 ms                                                     | 6.60 ms: 1.15x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 71.0 us: 4.59x faster                                                       |
| generators                 | 34.0 ms                                                     | 21.3 ms: 1.59x faster                                                       |
| asyncio_tcp                | 726 ms                                                      | 470 ms: 1.54x faster                                                        |
| comprehensions             | 15.6 us                                                     | 10.7 us: 1.47x faster                                                       |
| json_dumps                 | 8.09 ms                                                     | 5.65 ms: 1.43x faster                                                       |
| deltablue                  | 2.70 ms                                                     | 1.99 ms: 1.36x faster                                                       |
| logging_silent             | 71.8 ns                                                     | 54.2 ns: 1.32x faster                                                       |
| unpack_sequence            | 46.9 ns                                                     | 36.2 ns: 1.30x faster                                                       |
| raytrace                   | 213 ms                                                      | 165 ms: 1.29x faster                                                        |
| unpickle_pure_python       | 157 us                                                      | 127 us: 1.24x faster                                                        |
| async_tree_none            | 332 ms                                                      | 272 ms: 1.22x faster                                                        |
| richards_super             | 38.7 ms                                                     | 31.8 ms: 1.22x faster                                                       |
| sqlglot_parse              | 953 us                                                      | 788 us: 1.21x faster                                                        |
| sympy_sum                  | 100 ms                                                      | 83.3 ms: 1.20x faster                                                       |
| chaos                      | 48.4 ms                                                     | 40.5 ms: 1.20x faster                                                       |
| go                         | 101 ms                                                      | 85.5 ms: 1.18x faster                                                       |
| hexiom                     | 4.55 ms                                                     | 3.87 ms: 1.18x faster                                                       |
| dulwich_log                | 46.4 ms                                                     | 39.8 ms: 1.17x faster                                                       |
| regex_compile              | 91.0 ms                                                     | 78.2 ms: 1.16x faster                                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 456 ms: 1.16x faster                                                        |
| sqlite_synth               | 1.77 us                                                     | 1.52 us: 1.16x faster                                                       |
| deepcopy_memo              | 26.0 us                                                     | 22.4 us: 1.16x faster                                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.00 ms: 1.16x faster                                                       |
| sympy_str                  | 185 ms                                                      | 160 ms: 1.16x faster                                                        |
| coroutines                 | 15.0 ms                                                     | 13.0 ms: 1.15x faster                                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.76 sec: 1.15x faster                                                      |
| nqueens                    | 68.3 ms                                                     | 59.4 ms: 1.15x faster                                                       |
| mako                       | 7.58 ms                                                     | 6.60 ms: 1.15x faster                                                       |
| scimark_monte_carlo        | 45.3 ms                                                     | 39.5 ms: 1.15x faster                                                       |
| async_tree_memoization     | 399 ms                                                      | 350 ms: 1.14x faster                                                        |
| pickle_pure_python         | 208 us                                                      | 183 us: 1.14x faster                                                        |
| logging_simple             | 6.86 us                                                     | 6.07 us: 1.13x faster                                                       |
| async_tree_memoization_tg  | 405 ms                                                      | 358 ms: 1.13x faster                                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.4 ms: 1.13x faster                                                       |
| scimark_lu                 | 62.8 ms                                                     | 55.6 ms: 1.13x faster                                                       |
| richards                   | 31.4 ms                                                     | 28.1 ms: 1.12x faster                                                       |
| mypy2                      | 459 ms                                                      | 413 ms: 1.11x faster                                                        |
| async_tree_io              | 808 ms                                                      | 729 ms: 1.11x faster                                                        |
| crypto_pyaes               | 48.9 ms                                                     | 44.1 ms: 1.11x faster                                                       |
| async_tree_none_tg         | 309 ms                                                      | 280 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 475 ms: 1.10x faster                                                        |
| sympy_expand               | 299 ms                                                      | 272 ms: 1.10x faster                                                        |
| logging_format             | 7.16 us                                                     | 6.52 us: 1.10x faster                                                       |
| tornado_http               | 92.8 ms                                                     | 84.5 ms: 1.10x faster                                                       |
| spectral_norm              | 68.3 ms                                                     | 62.6 ms: 1.09x faster                                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.36 ms: 1.09x faster                                                       |
| pyflate                    | 312 ms                                                      | 288 ms: 1.08x faster                                                        |
| deepcopy                   | 246 us                                                      | 228 us: 1.08x faster                                                        |
| chameleon                  | 5.26 ms                                                     | 4.88 ms: 1.08x faster                                                       |
| async_tree_io_tg           | 829 ms                                                      | 770 ms: 1.08x faster                                                        |
| xml_etree_parse            | 97.6 ms                                                     | 90.8 ms: 1.07x faster                                                       |
| mdp                        | 1.59 sec                                                    | 1.48 sec: 1.07x faster                                                      |
| dask                       | 273 ms                                                      | 254 ms: 1.07x faster                                                        |
| pprint_pformat             | 1.09 sec                                                    | 1.02 sec: 1.07x faster                                                      |
| pprint_safe_repr           | 529 ms                                                      | 496 ms: 1.07x faster                                                        |
| docutils                   | 1.64 sec                                                    | 1.55 sec: 1.06x faster                                                      |
| sqlglot_normalize          | 190 ms                                                      | 181 ms: 1.05x faster                                                        |
| bench_thread_pool          | 872 us                                                      | 831 us: 1.05x faster                                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.3 ms: 1.04x faster                                                       |
| meteor_contest             | 75.2 ms                                                     | 72.7 ms: 1.03x faster                                                       |
| scimark_fft                | 179 ms                                                      | 174 ms: 1.03x faster                                                        |
| fannkuch                   | 253 ms                                                      | 247 ms: 1.03x faster                                                        |
| scimark_sor                | 78.1 ms                                                     | 76.3 ms: 1.02x faster                                                       |
| pidigits                   | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float                      | 54.4 ms                                                     | 53.3 ms: 1.02x faster                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.0 ms: 1.02x faster                                                       |
| 2to3                       | 214 ms                                                      | 210 ms: 1.01x faster                                                        |
| deepcopy_reduce            | 2.06 us                                                     | 2.04 us: 1.01x faster                                                       |
| tomli_loads                | 1.46 sec                                                    | 1.45 sec: 1.01x faster                                                      |
| regex_dna                  | 116 ms                                                      | 116 ms: 1.01x faster                                                        |
| nbody                      | 70.3 ms                                                     | 70.0 ms: 1.00x faster                                                       |
| pickle_dict                | 18.5 us                                                     | 18.6 us: 1.01x slower                                                       |
| xml_etree_process          | 37.2 ms                                                     | 37.5 ms: 1.01x slower                                                       |
| python_startup             | 19.8 ms                                                     | 20.0 ms: 1.01x slower                                                       |
| bench_mp_pool              | 63.2 ms                                                     | 63.9 ms: 1.01x slower                                                       |
| gc_traversal               | 1.49 ms                                                     | 1.51 ms: 1.01x slower                                                       |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.03x slower                                                       |
| xml_etree_generate         | 52.5 ms                                                     | 54.1 ms: 1.03x slower                                                       |
| regex_effbot               | 1.50 ms                                                     | 1.55 ms: 1.04x slower                                                       |
| create_gc_cycles           | 713 us                                                      | 748 us: 1.05x slower                                                        |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                                       |
| unpickle_list              | 2.59 us                                                     | 2.73 us: 1.05x slower                                                       |
| pathlib                    | 70.9 ms                                                     | 75.1 ms: 1.06x slower                                                       |
| python_startup_no_site     | 16.8 ms                                                     | 17.9 ms: 1.06x slower                                                       |
| coverage                   | 43.4 ms                                                     | 46.4 ms: 1.07x slower                                                       |
| pickle                     | 6.64 us                                                     | 7.24 us: 1.09x slower                                                       |
| pickle_list                | 2.70 us                                                     | 2.95 us: 1.10x slower                                                       |
| json                       | 2.98 ms                                                     | 3.32 ms: 1.11x slower                                                       |
| unpickle                   | 7.57 us                                                     | 8.54 us: 1.13x slower                                                       |
| telco                      | 4.06 ms                                                     | 4.80 ms: 1.18x slower                                                       |
| async_generators           | 177 ms                                                      | 229 ms: 1.29x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): pycparser
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown