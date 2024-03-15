# Results vs. 3.12.0

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-amd64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.82%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| chameleon      | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 84.8 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 346 ms: 1.06x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 757 ms: 1.02x faster                                                        |
| async_tree_io              | 731 ms                                                      | 722 ms: 1.01x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| float          | 56.8 ms                                                     | 48.8 ms: 1.16x faster                                                       |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 114 ms: 1.11x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| regex_compile  | 87.5 ms                                                     | 90.9 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 180 us: 1.08x faster                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.5 us: 1.05x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.5 ms: 1.04x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.2 ms: 1.04x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.49 ms: 1.04x faster                                                       |
| pickle               | 7.43 us                                                     | 7.19 us: 1.03x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 91.8 ms: 1.01x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.78 us: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.50 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 138 us: 1.04x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 24.0 ms: 1.23x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 21.7 ms: 1.33x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.28x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 5.90 ms: 1.20x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.9 us: 1.36x faster                                                       |
| comprehensions             | 14.1 us                                                     | 11.1 us: 1.27x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.71 sec: 1.22x faster                                                      |
| mako                       | 7.09 ms                                                     | 5.90 ms: 1.20x faster                                                       |
| nbody                      | 71.9 ms                                                     | 59.9 ms: 1.20x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 56.3 ms: 1.19x faster                                                       |
| float                      | 56.8 ms                                                     | 48.8 ms: 1.16x faster                                                       |
| mypy2                      | 509 ms                                                      | 438 ms: 1.16x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.1 ms: 1.12x faster                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.29 ms: 1.12x faster                                                       |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.12x faster                                                       |
| regex_dna                  | 126 ms                                                      | 114 ms: 1.11x faster                                                        |
| async_tree_none            | 291 ms                                                      | 264 ms: 1.10x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 44.2 ms: 1.10x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 13.1 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 449 ms: 1.09x faster                                                        |
| pickle_pure_python         | 195 us                                                      | 180 us: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 56.0 ns: 1.08x faster                                                       |
| deepcopy                   | 238 us                                                      | 223 us: 1.07x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.29 sec: 1.06x faster                                                      |
| sqlglot_normalize          | 187 ms                                                      | 176 ms: 1.06x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 346 ms: 1.06x faster                                                        |
| dulwich_log                | 44.3 ms                                                     | 41.8 ms: 1.06x faster                                                       |
| pathlib                    | 80.5 ms                                                     | 76.1 ms: 1.06x faster                                                       |
| tornado_http               | 89.5 ms                                                     | 84.8 ms: 1.06x faster                                                       |
| logging_simple             | 6.28 us                                                     | 5.96 us: 1.05x faster                                                       |
| raytrace                   | 192 ms                                                      | 183 ms: 1.05x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.38 us: 1.05x faster                                                       |
| deepcopy_reduce            | 2.09 us                                                     | 1.99 us: 1.05x faster                                                       |
| pickle_dict                | 18.4 us                                                     | 17.5 us: 1.05x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| chaos                      | 43.3 ms                                                     | 41.2 ms: 1.05x faster                                                       |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 22.7 us: 1.04x faster                                                       |
| xml_etree_iterparse        | 65.2 ms                                                     | 62.5 ms: 1.04x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.2 ms: 1.04x faster                                                       |
| asyncio_tcp                | 487 ms                                                      | 468 ms: 1.04x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.49 ms: 1.04x faster                                                       |
| sympy_sum                  | 91.5 ms                                                     | 88.2 ms: 1.04x faster                                                       |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                      |
| chameleon                  | 4.98 ms                                                     | 4.80 ms: 1.04x faster                                                       |
| regex_effbot               | 1.62 ms                                                     | 1.56 ms: 1.04x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 2.09 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.19 us: 1.03x faster                                                       |
| scimark_fft                | 184 ms                                                      | 179 ms: 1.03x faster                                                        |
| nqueens                    | 62.8 ms                                                     | 61.4 ms: 1.02x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 840 us: 1.02x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 757 ms: 1.02x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.3 ms: 1.02x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 792 us: 1.02x faster                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 91.8 ms: 1.01x faster                                                       |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 742 us: 1.01x faster                                                        |
| async_tree_io              | 731 ms                                                      | 722 ms: 1.01x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.01x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 510 ms: 1.01x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 1.02 ms: 1.00x faster                                                       |
| async_generators           | 239 ms                                                      | 242 ms: 1.01x slower                                                        |
| pyflate                    | 295 ms                                                      | 298 ms: 1.01x slower                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 69.9 ms: 1.01x slower                                                       |
| sqlglot_optimize           | 34.5 ms                                                     | 34.9 ms: 1.01x slower                                                       |
| unpickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                                       |
| pprint_pformat             | 1.05 sec                                                    | 1.06 sec: 1.01x slower                                                      |
| sympy_expand               | 284 ms                                                      | 288 ms: 1.02x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 14.5 ms: 1.02x slower                                                       |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                        |
| sympy_integrate            | 13.0 ms                                                     | 13.3 ms: 1.02x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.50 us: 1.04x slower                                                       |
| regex_compile              | 87.5 ms                                                     | 90.9 ms: 1.04x slower                                                       |
| unpickle_pure_python       | 133 us                                                      | 138 us: 1.04x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.43 sec: 1.04x slower                                                      |
| scimark_monte_carlo        | 43.7 ms                                                     | 46.3 ms: 1.06x slower                                                       |
| pycparser                  | 699 ms                                                      | 740 ms: 1.06x slower                                                        |
| fannkuch                   | 247 ms                                                      | 261 ms: 1.06x slower                                                        |
| go                         | 91.6 ms                                                     | 99.8 ms: 1.09x slower                                                       |
| richards_super             | 32.1 ms                                                     | 35.0 ms: 1.09x slower                                                       |
| scimark_sor                | 78.8 ms                                                     | 87.1 ms: 1.11x slower                                                       |
| richards                   | 28.4 ms                                                     | 31.6 ms: 1.11x slower                                                       |
| coverage                   | 40.8 ms                                                     | 45.8 ms: 1.12x slower                                                       |
| telco                      | 4.13 ms                                                     | 4.65 ms: 1.13x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.01 ms: 1.22x slower                                                       |
| scimark_lu                 | 58.9 ms                                                     | 72.0 ms: 1.22x slower                                                       |
| python_startup             | 19.5 ms                                                     | 24.0 ms: 1.23x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 21.7 ms: 1.33x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 58.3 ns: 1.55x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (3): json, async_tree_memoization, pickle_list
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.82% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown