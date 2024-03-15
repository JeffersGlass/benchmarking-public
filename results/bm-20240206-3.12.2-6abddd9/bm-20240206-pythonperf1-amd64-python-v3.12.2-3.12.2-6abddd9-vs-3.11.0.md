
# Results vs. 3.11.0

- fork: python
- ref: v3.12.2
- machine: windows-amd64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| chameleon      | 5.26 ms                                                     | 5.14 ms: 1.02x faster                                       |
| docutils       | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                      |
| tornado_http   | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                        |
| async_tree_none            | 332 ms                                                      | 289 ms: 1.15x faster                                        |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                        |
| async_tree_none_tg         | 309 ms                                                      | 277 ms: 1.11x faster                                        |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 478 ms: 1.11x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 486 ms: 1.08x faster                                        |
| Geometric mean             | (ref)                                                       | 1.13x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 54.4 ms                                                     | 56.1 ms: 1.03x slower                                       |
| nbody          | 70.3 ms                                                     | 74.3 ms: 1.06x slower                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 86.2 ms: 1.06x faster                                       |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                       |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                        |
| regex_effbot   | 1.50 ms                                                     | 1.61 ms: 1.08x slower                                       |
| Geometric mean | (ref)                                                       | 1.01x slower                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.69 ms: 1.42x faster                                       |
| unpickle_pure_python | 157 us                                                      | 139 us: 1.13x faster                                        |
| xml_etree_parse      | 97.6 ms                                                     | 89.8 ms: 1.09x faster                                       |
| pickle_pure_python   | 208 us                                                      | 200 us: 1.04x faster                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.2 ms: 1.04x faster                                       |
| tomli_loads          | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                      |
| pickle_dict          | 18.5 us                                                     | 18.9 us: 1.02x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.65 us: 1.02x slower                                       |
| xml_etree_process    | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                       |
| json_loads           | 13.0 us                                                     | 13.6 us: 1.05x slower                                       |
| pickle_list          | 2.70 us                                                     | 2.85 us: 1.06x slower                                       |
| unpickle             | 7.57 us                                                     | 8.03 us: 1.06x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 56.3 ms: 1.07x slower                                       |
| pickle               | 6.64 us                                                     | 7.29 us: 1.10x slower                                       |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.8 ms: 1.06x faster                                       |
| python_startup         | 19.8 ms                                                     | 19.0 ms: 1.04x faster                                       |
| Geometric mean         | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 6.93 ms: 1.09x faster                                       |
| django_template | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                       |
| Geometric mean  | (ref)                                                       | 1.06x faster                                                |

All benchmarks:
===============

| Benchmark                  | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| typing_runtime_protocols   | 326 us                                                      | 78.9 us: 4.13x faster                                       |
| asyncio_tcp                | 726 ms                                                      | 466 ms: 1.56x faster                                        |
| generators                 | 34.0 ms                                                     | 22.3 ms: 1.52x faster                                       |
| json_dumps                 | 8.09 ms                                                     | 5.69 ms: 1.42x faster                                       |
| deltablue                  | 2.70 ms                                                     | 2.15 ms: 1.25x faster                                       |
| richards_super             | 38.7 ms                                                     | 31.0 ms: 1.25x faster                                       |
| async_tree_memoization     | 399 ms                                                      | 338 ms: 1.18x faster                                        |
| async_tree_memoization_tg  | 405 ms                                                      | 350 ms: 1.16x faster                                        |
| sqlalchemy_imperative      | 10.4 ms                                                     | 9.02 ms: 1.16x faster                                       |
| sqlglot_parse              | 953 us                                                      | 830 us: 1.15x faster                                        |
| async_tree_none            | 332 ms                                                      | 289 ms: 1.15x faster                                        |
| logging_silent             | 71.8 ns                                                     | 62.6 ns: 1.15x faster                                       |
| richards                   | 31.4 ms                                                     | 27.4 ms: 1.15x faster                                       |
| mdp                        | 1.59 sec                                                    | 1.39 sec: 1.14x faster                                      |
| unpickle_pure_python       | 157 us                                                      | 139 us: 1.13x faster                                        |
| async_tree_io              | 808 ms                                                      | 716 ms: 1.13x faster                                        |
| sympy_sum                  | 100 ms                                                      | 89.1 ms: 1.12x faster                                       |
| go                         | 101 ms                                                      | 90.0 ms: 1.12x faster                                       |
| dulwich_log                | 46.4 ms                                                     | 41.4 ms: 1.12x faster                                       |
| async_tree_none_tg         | 309 ms                                                      | 277 ms: 1.11x faster                                        |
| mypy2                      | 459 ms                                                      | 412 ms: 1.11x faster                                        |
| comprehensions             | 15.6 us                                                     | 14.0 us: 1.11x faster                                       |
| sqlglot_transpile          | 1.16 ms                                                     | 1.05 ms: 1.11x faster                                       |
| async_tree_cpu_io_mixed    | 530 ms                                                      | 478 ms: 1.11x faster                                        |
| async_tree_io_tg           | 829 ms                                                      | 753 ms: 1.10x faster                                        |
| sympy_integrate            | 14.0 ms                                                     | 12.8 ms: 1.10x faster                                       |
| mako                       | 7.58 ms                                                     | 6.93 ms: 1.09x faster                                       |
| hexiom                     | 4.55 ms                                                     | 4.18 ms: 1.09x faster                                       |
| chaos                      | 48.4 ms                                                     | 44.5 ms: 1.09x faster                                       |
| xml_etree_parse            | 97.6 ms                                                     | 89.8 ms: 1.09x faster                                       |
| raytrace                   | 213 ms                                                      | 197 ms: 1.09x faster                                        |
| sympy_str                  | 185 ms                                                      | 171 ms: 1.09x faster                                        |
| coverage                   | 43.4 ms                                                     | 40.0 ms: 1.09x faster                                       |
| tornado_http               | 92.8 ms                                                     | 85.8 ms: 1.08x faster                                       |
| asyncio_tcp_ssl            | 2.03 sec                                                    | 1.88 sec: 1.08x faster                                      |
| sympy_expand               | 299 ms                                                      | 277 ms: 1.08x faster                                        |
| async_tree_cpu_io_mixed_tg | 523 ms                                                      | 486 ms: 1.08x faster                                        |
| dask                       | 273 ms                                                      | 254 ms: 1.07x faster                                        |
| logging_simple             | 6.86 us                                                     | 6.41 us: 1.07x faster                                       |
| nqueens                    | 68.3 ms                                                     | 63.8 ms: 1.07x faster                                       |
| python_startup_no_site     | 16.8 ms                                                     | 15.8 ms: 1.06x faster                                       |
| coroutines                 | 15.0 ms                                                     | 14.1 ms: 1.06x faster                                       |
| regex_compile              | 91.0 ms                                                     | 86.2 ms: 1.06x faster                                       |
| deepcopy_memo              | 26.0 us                                                     | 24.7 us: 1.05x faster                                       |
| logging_format             | 7.16 us                                                     | 6.82 us: 1.05x faster                                       |
| scimark_lu                 | 62.8 ms                                                     | 60.0 ms: 1.05x faster                                       |
| fannkuch                   | 253 ms                                                      | 242 ms: 1.05x faster                                        |
| pyflate                    | 312 ms                                                      | 299 ms: 1.05x faster                                        |
| pickle_pure_python         | 208 us                                                      | 200 us: 1.04x faster                                        |
| deepcopy                   | 246 us                                                      | 236 us: 1.04x faster                                        |
| bench_thread_pool          | 872 us                                                      | 836 us: 1.04x faster                                        |
| pycparser                  | 720 ms                                                      | 690 ms: 1.04x faster                                        |
| python_startup             | 19.8 ms                                                     | 19.0 ms: 1.04x faster                                       |
| crypto_pyaes               | 48.9 ms                                                     | 46.9 ms: 1.04x faster                                       |
| meteor_contest             | 75.2 ms                                                     | 72.4 ms: 1.04x faster                                       |
| aiohttp                    | 883 us                                                      | 851 us: 1.04x faster                                        |
| xml_etree_iterparse        | 65.6 ms                                                     | 63.2 ms: 1.04x faster                                       |
| tomli_loads                | 1.46 sec                                                    | 1.41 sec: 1.03x faster                                      |
| sqlglot_normalize          | 190 ms                                                      | 185 ms: 1.03x faster                                        |
| docutils                   | 1.64 sec                                                    | 1.60 sec: 1.03x faster                                      |
| django_template            | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                       |
| scimark_sparse_mat_mult    | 2.58 ms                                                     | 2.51 ms: 1.03x faster                                       |
| chameleon                  | 5.26 ms                                                     | 5.14 ms: 1.02x faster                                       |
| spectral_norm              | 68.3 ms                                                     | 67.2 ms: 1.02x faster                                       |
| unpack_sequence            | 46.9 ns                                                     | 46.3 ns: 1.01x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                       |
| sqlalchemy_declarative     | 85.6 ms                                                     | 84.7 ms: 1.01x faster                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.3 ms: 1.01x faster                                       |
| pprint_pformat             | 1.09 sec                                                    | 1.08 sec: 1.01x faster                                      |
| telco                      | 4.06 ms                                                     | 4.08 ms: 1.00x slower                                       |
| sqlite_synth               | 1.77 us                                                     | 1.78 us: 1.01x slower                                       |
| pprint_safe_repr           | 529 ms                                                      | 534 ms: 1.01x slower                                        |
| scimark_monte_carlo        | 45.3 ms                                                     | 46.1 ms: 1.02x slower                                       |
| pickle_dict                | 18.5 us                                                     | 18.9 us: 1.02x slower                                       |
| deepcopy_reduce            | 2.06 us                                                     | 2.11 us: 1.02x slower                                       |
| unpickle_list              | 2.59 us                                                     | 2.65 us: 1.02x slower                                       |
| xml_etree_process          | 37.2 ms                                                     | 38.2 ms: 1.03x slower                                       |
| scimark_fft                | 179 ms                                                      | 184 ms: 1.03x slower                                        |
| float                      | 54.4 ms                                                     | 56.1 ms: 1.03x slower                                       |
| bench_mp_pool              | 63.2 ms                                                     | 65.5 ms: 1.04x slower                                       |
| regex_dna                  | 116 ms                                                      | 121 ms: 1.04x slower                                        |
| json_loads                 | 13.0 us                                                     | 13.6 us: 1.05x slower                                       |
| nbody                      | 70.3 ms                                                     | 74.3 ms: 1.06x slower                                       |
| pickle_list                | 2.70 us                                                     | 2.85 us: 1.06x slower                                       |
| unpickle                   | 7.57 us                                                     | 8.03 us: 1.06x slower                                       |
| pathlib                    | 70.9 ms                                                     | 75.7 ms: 1.07x slower                                       |
| xml_etree_generate         | 52.5 ms                                                     | 56.3 ms: 1.07x slower                                       |
| scimark_sor                | 78.1 ms                                                     | 83.9 ms: 1.07x slower                                       |
| regex_effbot               | 1.50 ms                                                     | 1.61 ms: 1.08x slower                                       |
| pickle                     | 6.64 us                                                     | 7.29 us: 1.10x slower                                       |
| async_generators           | 177 ms                                                      | 231 ms: 1.31x slower                                        |
| Geometric mean             | (ref)                                                       | 1.07x faster                                                |

Benchmark hidden because not significant (5): json, gc_traversal, 2to3, pidigits, create_gc_cycles
Ignored benchmarks (6) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown