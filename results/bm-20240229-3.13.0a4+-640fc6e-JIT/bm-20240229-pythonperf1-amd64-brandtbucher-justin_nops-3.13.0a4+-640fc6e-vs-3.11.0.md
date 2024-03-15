# Results vs. 3.11.0

- fork: brandtbucher
- ref: justin_nops
- machine: windows-amd64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 226 ms: 1.06x slower                                                     |
| chameleon      | 5.26 ms                                                     | 4.76 ms: 1.10x faster                                                    |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                   |
| html5lib       | 38.9 ms                                                     | 36.1 ms: 1.08x faster                                                    |
| tornado_http   | 92.8 ms                                                     | 84.8 ms: 1.09x faster                                                    |
| Geometric mean | (ref)                                                       | 1.05x faster                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_none            | 332 ms                                                      | 276 ms: 1.21x faster                                                     |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 460 ms: 1.15x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 349 ms: 1.14x faster                                                     |
| async_tree_memoization_tg  | 405 ms                                                      | 355 ms: 1.14x faster                                                     |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                                     |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 474 ms: 1.10x faster                                                     |
| async_tree_io              | 808 ms                                                      | 736 ms: 1.10x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 765 ms: 1.08x faster                                                     |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                    |
| float          | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                    |
| Geometric mean | (ref)                                                       | 1.09x faster                                                             |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.2 ms: 1.11x faster                                                    |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.03x slower                                                    |
| regex_dna      | 116 ms                                                      | 121 ms: 1.05x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                    |
| Geometric mean | (ref)                                                       | 1.00x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                    |
| tomli_loads          | 1.46 sec                                                    | 1.20 sec: 1.21x faster                                                   |
| unpickle_pure_python | 157 us                                                      | 130 us: 1.21x faster                                                     |
| pickle_pure_python   | 208 us                                                      | 176 us: 1.18x faster                                                     |
| xml_etree_parse      | 97.6 ms                                                     | 93.6 ms: 1.04x faster                                                    |
| pickle_dict          | 18.5 us                                                     | 17.7 us: 1.04x faster                                                    |
| xml_etree_process    | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                    |
| xml_etree_iterparse  | 65.6 ms                                                     | 64.1 ms: 1.02x faster                                                    |
| xml_etree_generate   | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                    |
| pickle_list          | 2.70 us                                                     | 2.84 us: 1.05x slower                                                    |
| json_loads           | 13.0 us                                                     | 13.9 us: 1.07x slower                                                    |
| unpickle_list        | 2.59 us                                                     | 2.77 us: 1.07x slower                                                    |
| pickle               | 6.64 us                                                     | 7.42 us: 1.12x slower                                                    |
| unpickle             | 7.57 us                                                     | 8.47 us: 1.12x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                             |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 24.1 ms: 1.22x slower                                                    |
| python_startup_no_site | 16.8 ms                                                     | 21.9 ms: 1.30x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.26x slower                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 5.78 ms: 1.31x faster                                                    |
| genshi_text     | 18.4 ms                                                     | 15.5 ms: 1.19x faster                                                    |
| genshi_xml      | 39.9 ms                                                     | 34.7 ms: 1.15x faster                                                    |
| django_template | 24.4 ms                                                     | 21.6 ms: 1.13x faster                                                    |
| Geometric mean  | (ref)                                                       | 1.19x faster                                                             |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 69.2 us: 4.71x faster                                                    |
| generators                 | 34.0 ms                                                     | 20.8 ms: 1.63x faster                                                    |
| asyncio_tcp                | 726 ms                                                      | 465 ms: 1.56x faster                                                     |
| pylint                     | 323 ms                                                      | 210 ms: 1.54x faster                                                     |
| comprehensions             | 15.6 us                                                     | 10.4 us: 1.50x faster                                                    |
| json_dumps                 | 8.09 ms                                                     | 5.59 ms: 1.45x faster                                                    |
| deltablue                  | 2.70 ms                                                     | 2.04 ms: 1.32x faster                                                    |
| spectral_norm              | 68.3 ms                                                     | 51.9 ms: 1.32x faster                                                    |
| mako                       | 7.58 ms                                                     | 5.78 ms: 1.31x faster                                                    |
| logging_silent             | 71.8 ns                                                     | 55.2 ns: 1.30x faster                                                    |
| sqlglot_parse              | 953 us                                                      | 767 us: 1.24x faster                                                     |
| richards_super             | 38.7 ms                                                     | 31.3 ms: 1.24x faster                                                    |
| chaos                      | 48.4 ms                                                     | 39.9 ms: 1.21x faster                                                    |
| tomli_loads                | 1.46 sec                                                    | 1.20 sec: 1.21x faster                                                   |
| unpickle_pure_python       | 157 us                                                      | 130 us: 1.21x faster                                                     |
| async_tree_none            | 332 ms                                                      | 276 ms: 1.21x faster                                                     |
| raytrace                   | 213 ms                                                      | 178 ms: 1.20x faster                                                     |
| genshi_text                | 18.4 ms                                                     | 15.5 ms: 1.19x faster                                                    |
| pickle_pure_python         | 208 us                                                      | 176 us: 1.18x faster                                                     |
| nbody                      | 70.3 ms                                                     | 59.5 ms: 1.18x faster                                                    |
| sqlglot_transpile          | 1.16 ms                                                     | 988 us: 1.18x faster                                                     |
| logging_simple             | 6.86 us                                                     | 5.86 us: 1.17x faster                                                    |
| deepcopy_memo              | 26.0 us                                                     | 22.3 us: 1.16x faster                                                    |
| sympy_sum                  | 100 ms                                                      | 86.2 ms: 1.16x faster                                                    |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 460 ms: 1.15x faster                                                     |
| genshi_xml                 | 39.9 ms                                                     | 34.7 ms: 1.15x faster                                                    |
| fannkuch                   | 253 ms                                                      | 221 ms: 1.15x faster                                                     |
| async_tree_memoization     | 399 ms                                                      | 349 ms: 1.14x faster                                                     |
| crypto_pyaes               | 48.9 ms                                                     | 42.8 ms: 1.14x faster                                                    |
| async_tree_memoization_tg  | 405 ms                                                      | 355 ms: 1.14x faster                                                     |
| sympy_str                  | 185 ms                                                      | 163 ms: 1.14x faster                                                     |
| logging_format             | 7.16 us                                                     | 6.29 us: 1.14x faster                                                    |
| django_template            | 24.4 ms                                                     | 21.6 ms: 1.13x faster                                                    |
| sqlite_synth               | 1.77 us                                                     | 1.56 us: 1.13x faster                                                    |
| dulwich_log                | 46.4 ms                                                     | 41.2 ms: 1.13x faster                                                    |
| richards                   | 31.4 ms                                                     | 28.0 ms: 1.12x faster                                                    |
| coroutines                 | 15.0 ms                                                     | 13.3 ms: 1.12x faster                                                    |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.31 ms: 1.12x faster                                                    |
| deepcopy                   | 246 us                                                      | 222 us: 1.11x faster                                                     |
| regex_compile              | 91.0 ms                                                     | 82.2 ms: 1.11x faster                                                    |
| async_tree_none_tg         | 309 ms                                                      | 279 ms: 1.11x faster                                                     |
| chameleon                  | 5.26 ms                                                     | 4.76 ms: 1.10x faster                                                    |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 474 ms: 1.10x faster                                                     |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.84 sec: 1.10x faster                                                   |
| pprint_pformat             | 1.09 sec                                                    | 988 ms: 1.10x faster                                                     |
| float                      | 54.4 ms                                                     | 49.5 ms: 1.10x faster                                                    |
| pyflate                    | 312 ms                                                      | 284 ms: 1.10x faster                                                     |
| async_tree_io              | 808 ms                                                      | 736 ms: 1.10x faster                                                     |
| tornado_http               | 92.8 ms                                                     | 84.8 ms: 1.09x faster                                                    |
| nqueens                    | 68.3 ms                                                     | 62.7 ms: 1.09x faster                                                    |
| sqlglot_normalize          | 190 ms                                                      | 175 ms: 1.08x faster                                                     |
| async_tree_io_tg           | 829 ms                                                      | 765 ms: 1.08x faster                                                     |
| pprint_safe_repr           | 529 ms                                                      | 491 ms: 1.08x faster                                                     |
| html5lib                   | 38.9 ms                                                     | 36.1 ms: 1.08x faster                                                    |
| sympy_expand               | 299 ms                                                      | 278 ms: 1.08x faster                                                     |
| unpack_sequence            | 46.9 ns                                                     | 43.8 ns: 1.07x faster                                                    |
| sympy_integrate            | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                                    |
| deepcopy_reduce            | 2.06 us                                                     | 1.93 us: 1.07x faster                                                    |
| go                         | 101 ms                                                      | 95.4 ms: 1.06x faster                                                    |
| mypy2                      | 459 ms                                                      | 435 ms: 1.06x faster                                                     |
| scimark_monte_carlo        | 45.3 ms                                                     | 43.0 ms: 1.05x faster                                                    |
| xml_etree_parse            | 97.6 ms                                                     | 93.6 ms: 1.04x faster                                                    |
| pickle_dict                | 18.5 us                                                     | 17.7 us: 1.04x faster                                                    |
| bench_thread_pool          | 872 us                                                      | 838 us: 1.04x faster                                                     |
| mdp                        | 1.59 sec                                                    | 1.54 sec: 1.03x faster                                                   |
| docutils                   | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                   |
| scimark_fft                | 179 ms                                                      | 173 ms: 1.03x faster                                                     |
| meteor_contest             | 75.2 ms                                                     | 72.9 ms: 1.03x faster                                                    |
| pycparser                  | 720 ms                                                      | 697 ms: 1.03x faster                                                     |
| hexiom                     | 4.55 ms                                                     | 4.43 ms: 1.03x faster                                                    |
| xml_etree_process          | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                    |
| xml_etree_iterparse        | 65.6 ms                                                     | 64.1 ms: 1.02x faster                                                    |
| sqlglot_optimize           | 34.5 ms                                                     | 34.4 ms: 1.00x faster                                                    |
| xml_etree_generate         | 52.5 ms                                                     | 53.3 ms: 1.01x slower                                                    |
| aiohttp                    | 883 us                                                      | 904 us: 1.02x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.03x slower                                                    |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.05x slower                                                     |
| scimark_sor                | 78.1 ms                                                     | 81.7 ms: 1.05x slower                                                    |
| create_gc_cycles           | 713 us                                                      | 749 us: 1.05x slower                                                     |
| regex_effbot               | 1.50 ms                                                     | 1.58 ms: 1.05x slower                                                    |
| pickle_list                | 2.70 us                                                     | 2.84 us: 1.05x slower                                                    |
| 2to3                       | 214 ms                                                      | 226 ms: 1.06x slower                                                     |
| pathlib                    | 70.9 ms                                                     | 75.3 ms: 1.06x slower                                                    |
| json_loads                 | 13.0 us                                                     | 13.9 us: 1.07x slower                                                    |
| json                       | 2.98 ms                                                     | 3.18 ms: 1.07x slower                                                    |
| unpickle_list              | 2.59 us                                                     | 2.77 us: 1.07x slower                                                    |
| coverage                   | 43.4 ms                                                     | 47.6 ms: 1.10x slower                                                    |
| bench_mp_pool              | 63.2 ms                                                     | 70.3 ms: 1.11x slower                                                    |
| pickle                     | 6.64 us                                                     | 7.42 us: 1.12x slower                                                    |
| unpickle                   | 7.57 us                                                     | 8.47 us: 1.12x slower                                                    |
| scimark_lu                 | 62.8 ms                                                     | 72.8 ms: 1.16x slower                                                    |
| telco                      | 4.06 ms                                                     | 4.74 ms: 1.17x slower                                                    |
| python_startup             | 19.8 ms                                                     | 24.1 ms: 1.22x slower                                                    |
| python_startup_no_site     | 16.8 ms                                                     | 21.9 ms: 1.30x slower                                                    |
| dask                       | 273 ms                                                      | 362 ms: 1.33x slower                                                     |
| async_generators           | 177 ms                                                      | 240 ms: 1.35x slower                                                     |
| thrift                     | 494 us                                                      | 8.88 ms: 17.98x slower                                                   |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                             |

Benchmark hidden because not significant (2): pidigits, gc_traversal
Ignored benchmarks (3) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown