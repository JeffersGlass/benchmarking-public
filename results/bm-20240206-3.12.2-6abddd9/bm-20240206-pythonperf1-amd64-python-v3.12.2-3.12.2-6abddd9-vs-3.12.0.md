
# Results vs. 3.12.0

- fork: python
- ref: v3.12.2
- machine: windows-amd64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 214 ms: 1.02x faster                                        |
| chameleon      | 4.98 ms                                                     | 5.14 ms: 1.03x slower                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| tornado_http   | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_memoization_tg  | 367 ms                                                      | 350 ms: 1.05x faster                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 486 ms: 1.03x faster                                        |
| async_tree_none_tg         | 285 ms                                                      | 277 ms: 1.03x faster                                        |
| async_tree_io_tg           | 771 ms                                                      | 753 ms: 1.02x faster                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 478 ms: 1.02x faster                                        |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                        |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                        |
| float          | 56.8 ms                                                     | 56.1 ms: 1.01x faster                                       |
| nbody          | 71.9 ms                                                     | 74.3 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                        |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.02x faster                                       |
| regex_compile  | 87.5 ms                                                     | 86.2 ms: 1.02x faster                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| unpickle_list        | 2.75 us                                                     | 2.65 us: 1.04x faster                                       |
| xml_etree_parse      | 93.0 ms                                                     | 89.8 ms: 1.04x faster                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.2 ms: 1.03x faster                                       |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                       |
| unpickle             | 8.18 us                                                     | 8.03 us: 1.02x faster                                       |
| pickle               | 7.43 us                                                     | 7.29 us: 1.02x faster                                       |
| xml_etree_generate   | 55.8 ms                                                     | 56.3 ms: 1.01x slower                                       |
| pickle_list          | 2.83 us                                                     | 2.85 us: 1.01x slower                                       |
| xml_etree_process    | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                       |
| pickle_pure_python   | 195 us                                                      | 200 us: 1.02x slower                                        |
| pickle_dict          | 18.4 us                                                     | 18.9 us: 1.03x slower                                       |
| tomli_loads          | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                      |
| unpickle_pure_python | 133 us                                                      | 139 us: 1.04x slower                                        |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.8 ms: 1.03x faster                                       |
| python_startup         | 19.5 ms                                                     | 19.0 ms: 1.03x faster                                       |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.93 ms: 1.02x faster                                       |
| django_template | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                       |
| Geometric mean  | (ref)                                                       | 1.01x slower                                                |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240206-pythonperf1-amd64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mypy2                      | 509 ms                                                      | 412 ms: 1.23x faster                                        |
| typing_runtime_protocols   | 95.1 us                                                     | 78.9 us: 1.21x faster                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.88 sec: 1.12x faster                                      |
| dulwich_log                | 44.3 ms                                                     | 41.4 ms: 1.07x faster                                       |
| pathlib                    | 80.5 ms                                                     | 75.7 ms: 1.06x faster                                       |
| bench_mp_pool              | 69.2 ms                                                     | 65.5 ms: 1.06x faster                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 350 ms: 1.05x faster                                        |
| asyncio_tcp                | 487 ms                                                      | 466 ms: 1.05x faster                                        |
| tornado_http               | 89.5 ms                                                     | 85.8 ms: 1.04x faster                                       |
| create_gc_cycles           | 752 us                                                      | 721 us: 1.04x faster                                        |
| regex_dna                  | 126 ms                                                      | 121 ms: 1.04x faster                                        |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                      |
| aiohttp                    | 884 us                                                      | 851 us: 1.04x faster                                        |
| unpickle_list              | 2.75 us                                                     | 2.65 us: 1.04x faster                                       |
| xml_etree_parse            | 93.0 ms                                                     | 89.8 ms: 1.04x faster                                       |
| richards                   | 28.4 ms                                                     | 27.4 ms: 1.04x faster                                       |
| richards_super             | 32.1 ms                                                     | 31.0 ms: 1.04x faster                                       |
| async_generators           | 239 ms                                                      | 231 ms: 1.03x faster                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 486 ms: 1.03x faster                                        |
| crypto_pyaes               | 48.5 ms                                                     | 46.9 ms: 1.03x faster                                       |
| dask                       | 263 ms                                                      | 254 ms: 1.03x faster                                        |
| json                       | 3.05 ms                                                     | 2.95 ms: 1.03x faster                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.2 ms: 1.03x faster                                       |
| meteor_contest             | 74.6 ms                                                     | 72.4 ms: 1.03x faster                                       |
| async_tree_none_tg         | 285 ms                                                      | 277 ms: 1.03x faster                                        |
| sqlalchemy_imperative      | 9.29 ms                                                     | 9.02 ms: 1.03x faster                                       |
| python_startup_no_site     | 16.2 ms                                                     | 15.8 ms: 1.03x faster                                       |
| sympy_sum                  | 91.5 ms                                                     | 89.1 ms: 1.03x faster                                       |
| sympy_str                  | 175 ms                                                      | 171 ms: 1.03x faster                                        |
| python_startup             | 19.5 ms                                                     | 19.0 ms: 1.03x faster                                       |
| sympy_expand               | 284 ms                                                      | 277 ms: 1.03x faster                                        |
| bench_thread_pool          | 857 us                                                      | 836 us: 1.02x faster                                        |
| async_tree_io_tg           | 771 ms                                                      | 753 ms: 1.02x faster                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 478 ms: 1.02x faster                                        |
| gc_traversal               | 1.52 ms                                                     | 1.49 ms: 1.02x faster                                       |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                       |
| mako                       | 7.09 ms                                                     | 6.93 ms: 1.02x faster                                       |
| 2to3                       | 218 ms                                                      | 214 ms: 1.02x faster                                        |
| coverage                   | 40.8 ms                                                     | 40.0 ms: 1.02x faster                                       |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                        |
| unpickle                   | 8.18 us                                                     | 8.03 us: 1.02x faster                                       |
| sqlalchemy_declarative     | 86.4 ms                                                     | 84.7 ms: 1.02x faster                                       |
| pickle                     | 7.43 us                                                     | 7.29 us: 1.02x faster                                       |
| fannkuch                   | 247 ms                                                      | 242 ms: 1.02x faster                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.51 ms: 1.02x faster                                       |
| go                         | 91.6 ms                                                     | 90.0 ms: 1.02x faster                                       |
| regex_v8                   | 14.2 ms                                                     | 14.0 ms: 1.02x faster                                       |
| regex_compile              | 87.5 ms                                                     | 86.2 ms: 1.02x faster                                       |
| coroutines                 | 14.3 ms                                                     | 14.1 ms: 1.01x faster                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                        |
| pycparser                  | 699 ms                                                      | 690 ms: 1.01x faster                                        |
| float                      | 56.8 ms                                                     | 56.1 ms: 1.01x faster                                       |
| sqlglot_normalize          | 187 ms                                                      | 185 ms: 1.01x faster                                        |
| telco                      | 4.13 ms                                                     | 4.08 ms: 1.01x faster                                       |
| sympy_integrate            | 13.0 ms                                                     | 12.8 ms: 1.01x faster                                       |
| deepcopy                   | 238 us                                                      | 236 us: 1.01x faster                                        |
| generators                 | 22.5 ms                                                     | 22.3 ms: 1.01x faster                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.3 ms: 1.01x faster                                       |
| comprehensions             | 14.1 us                                                     | 14.0 us: 1.01x faster                                       |
| spectral_norm              | 66.9 ms                                                     | 67.2 ms: 1.00x slower                                       |
| deepcopy_reduce            | 2.09 us                                                     | 2.11 us: 1.01x slower                                       |
| xml_etree_generate         | 55.8 ms                                                     | 56.3 ms: 1.01x slower                                       |
| pickle_list                | 2.83 us                                                     | 2.85 us: 1.01x slower                                       |
| sqlite_synth               | 1.76 us                                                     | 1.78 us: 1.01x slower                                       |
| xml_etree_process          | 37.7 ms                                                     | 38.2 ms: 1.01x slower                                       |
| pyflate                    | 295 ms                                                      | 299 ms: 1.01x slower                                        |
| mdp                        | 1.37 sec                                                    | 1.39 sec: 1.02x slower                                      |
| logging_format             | 6.72 us                                                     | 6.82 us: 1.02x slower                                       |
| nqueens                    | 62.8 ms                                                     | 63.8 ms: 1.02x slower                                       |
| scimark_lu                 | 58.9 ms                                                     | 60.0 ms: 1.02x slower                                       |
| hexiom                     | 4.10 ms                                                     | 4.18 ms: 1.02x slower                                       |
| logging_simple             | 6.28 us                                                     | 6.41 us: 1.02x slower                                       |
| pickle_pure_python         | 195 us                                                      | 200 us: 1.02x slower                                        |
| raytrace                   | 192 ms                                                      | 197 ms: 1.02x slower                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.05 ms: 1.03x slower                                       |
| pickle_dict                | 18.4 us                                                     | 18.9 us: 1.03x slower                                       |
| chaos                      | 43.3 ms                                                     | 44.5 ms: 1.03x slower                                       |
| tomli_loads                | 1.37 sec                                                    | 1.41 sec: 1.03x slower                                      |
| chameleon                  | 4.98 ms                                                     | 5.14 ms: 1.03x slower                                       |
| sqlglot_parse              | 804 us                                                      | 830 us: 1.03x slower                                        |
| pprint_pformat             | 1.05 sec                                                    | 1.08 sec: 1.03x slower                                      |
| nbody                      | 71.9 ms                                                     | 74.3 ms: 1.03x slower                                       |
| logging_silent             | 60.5 ns                                                     | 62.6 ns: 1.03x slower                                       |
| django_template            | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                       |
| pprint_safe_repr           | 513 ms                                                      | 534 ms: 1.04x slower                                        |
| deepcopy_memo              | 23.7 us                                                     | 24.7 us: 1.04x slower                                       |
| unpickle_pure_python       | 133 us                                                      | 139 us: 1.04x slower                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 46.1 ms: 1.05x slower                                       |
| scimark_sor                | 78.8 ms                                                     | 83.9 ms: 1.07x slower                                       |
| unpack_sequence            | 37.5 ns                                                     | 46.3 ns: 1.23x slower                                       |
| Geometric mean             | (ref)                                                       | 1.01x faster                                                |

Benchmark hidden because not significant (6): async_tree_none, async_tree_memoization, deltablue, regex_effbot, scimark_fft, json_dumps


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown