
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.06x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.03x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 214 ms: 1.02x faster                                                         |
| chameleon      | 4.98 ms                                                     | 4.71 ms: 1.06x faster                                                        |
| docutils       | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                       |
| tornado_http   | 89.5 ms                                                     | 83.9 ms: 1.07x faster                                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                         |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 462 ms: 1.09x faster                                                         |
| async_tree_memoization_tg  | 367 ms                                                      | 339 ms: 1.08x faster                                                         |
| async_tree_none_tg         | 285 ms                                                      | 268 ms: 1.07x faster                                                         |
| async_tree_io_tg           | 771 ms                                                      | 748 ms: 1.03x faster                                                         |
| async_tree_io              | 731 ms                                                      | 714 ms: 1.02x faster                                                         |
| async_tree_memoization     | 339 ms                                                      | 334 ms: 1.02x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 58.4 ms: 1.23x faster                                                        |
| float          | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                        |
| pidigits       | 152 ms                                                      | 151 ms: 1.01x faster                                                         |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 76.9 ms: 1.14x faster                                                        |
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                         |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.19 sec: 1.15x faster                                                       |
| pickle_pure_python   | 195 us                                                      | 174 us: 1.12x faster                                                         |
| unpickle_pure_python | 133 us                                                      | 123 us: 1.08x faster                                                         |
| xml_etree_generate   | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                        |
| pickle_dict          | 18.4 us                                                     | 17.5 us: 1.05x faster                                                        |
| pickle               | 7.43 us                                                     | 7.10 us: 1.05x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 36.1 ms: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                        |
| json_dumps           | 5.70 ms                                                     | 5.53 ms: 1.03x faster                                                        |
| json_loads           | 13.9 us                                                     | 13.6 us: 1.02x faster                                                        |
| unpickle_list        | 2.75 us                                                     | 2.78 us: 1.01x slower                                                        |
| unpickle             | 8.18 us                                                     | 8.50 us: 1.04x slower                                                        |
| pickle_list          | 2.83 us                                                     | 3.13 us: 1.11x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.1 ms: 1.03x slower                                                        |
| python_startup_no_site | 16.2 ms                                                     | 18.0 ms: 1.11x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 5.98 ms: 1.18x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.5 us: 1.35x faster                                                        |
| comprehensions             | 14.1 us                                                     | 10.6 us: 1.33x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.69 sec: 1.24x faster                                                       |
| spectral_norm              | 66.9 ms                                                     | 54.4 ms: 1.23x faster                                                        |
| nbody                      | 71.9 ms                                                     | 58.4 ms: 1.23x faster                                                        |
| mypy2                      | 509 ms                                                      | 420 ms: 1.21x faster                                                         |
| mako                       | 7.09 ms                                                     | 5.98 ms: 1.18x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.51 us: 1.17x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 52.0 ns: 1.16x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.19 sec: 1.15x faster                                                       |
| raytrace                   | 192 ms                                                      | 167 ms: 1.15x faster                                                         |
| richards_super             | 32.1 ms                                                     | 27.9 ms: 1.15x faster                                                        |
| float                      | 56.8 ms                                                     | 49.5 ms: 1.15x faster                                                        |
| richards                   | 28.4 ms                                                     | 24.8 ms: 1.15x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 20.7 us: 1.14x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 76.9 ms: 1.14x faster                                                        |
| generators                 | 22.5 ms                                                     | 19.9 ms: 1.13x faster                                                        |
| fannkuch                   | 247 ms                                                      | 218 ms: 1.13x faster                                                         |
| pickle_pure_python         | 195 us                                                      | 174 us: 1.12x faster                                                         |
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                         |
| dulwich_log                | 44.3 ms                                                     | 39.6 ms: 1.12x faster                                                        |
| coroutines                 | 14.3 ms                                                     | 12.8 ms: 1.12x faster                                                        |
| crypto_pyaes               | 48.5 ms                                                     | 43.5 ms: 1.11x faster                                                        |
| deltablue                  | 2.16 ms                                                     | 1.94 ms: 1.11x faster                                                        |
| deepcopy                   | 238 us                                                      | 214 us: 1.11x faster                                                         |
| pprint_safe_repr           | 513 ms                                                      | 465 ms: 1.10x faster                                                         |
| pprint_pformat             | 1.05 sec                                                    | 950 ms: 1.10x faster                                                         |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.33 ms: 1.10x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.91 us: 1.10x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 447 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 462 ms: 1.09x faster                                                         |
| sympy_str                  | 175 ms                                                      | 161 ms: 1.08x faster                                                         |
| scimark_lu                 | 58.9 ms                                                     | 54.4 ms: 1.08x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 339 ms: 1.08x faster                                                         |
| unpickle_pure_python       | 133 us                                                      | 123 us: 1.08x faster                                                         |
| nqueens                    | 62.8 ms                                                     | 58.2 ms: 1.08x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 747 us: 1.08x faster                                                         |
| sqlglot_normalize          | 187 ms                                                      | 174 ms: 1.07x faster                                                         |
| logging_simple             | 6.28 us                                                     | 5.84 us: 1.07x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 75.2 ms: 1.07x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.2 ms: 1.07x faster                                                        |
| chaos                      | 43.3 ms                                                     | 40.6 ms: 1.07x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 83.9 ms: 1.07x faster                                                        |
| bench_thread_pool          | 857 us                                                      | 803 us: 1.07x faster                                                         |
| async_tree_none_tg         | 285 ms                                                      | 268 ms: 1.07x faster                                                         |
| docutils                   | 1.66 sec                                                    | 1.56 sec: 1.06x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 963 us: 1.06x faster                                                         |
| chameleon                  | 4.98 ms                                                     | 4.71 ms: 1.06x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 86.5 ms: 1.06x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                         |
| logging_format             | 6.72 us                                                     | 6.35 us: 1.06x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 65.6 ms: 1.05x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.5 us: 1.05x faster                                                        |
| pickle                     | 7.43 us                                                     | 7.10 us: 1.05x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 36.1 ms: 1.05x faster                                                        |
| scimark_fft                | 184 ms                                                      | 176 ms: 1.04x faster                                                         |
| xml_etree_iterparse        | 65.2 ms                                                     | 62.7 ms: 1.04x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 33.3 ms: 1.04x faster                                                        |
| pyflate                    | 295 ms                                                      | 284 ms: 1.04x faster                                                         |
| scimark_sor                | 78.8 ms                                                     | 76.1 ms: 1.03x faster                                                        |
| sympy_expand               | 284 ms                                                      | 275 ms: 1.03x faster                                                         |
| dask                       | 263 ms                                                      | 254 ms: 1.03x faster                                                         |
| asyncio_tcp                | 487 ms                                                      | 472 ms: 1.03x faster                                                         |
| async_tree_io_tg           | 771 ms                                                      | 748 ms: 1.03x faster                                                         |
| meteor_contest             | 74.6 ms                                                     | 72.4 ms: 1.03x faster                                                        |
| json_dumps                 | 5.70 ms                                                     | 5.53 ms: 1.03x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                        |
| async_tree_io              | 731 ms                                                      | 714 ms: 1.02x faster                                                         |
| create_gc_cycles           | 752 us                                                      | 735 us: 1.02x faster                                                         |
| async_generators           | 239 ms                                                      | 235 ms: 1.02x faster                                                         |
| json_loads                 | 13.9 us                                                     | 13.6 us: 1.02x faster                                                        |
| pycparser                  | 699 ms                                                      | 686 ms: 1.02x faster                                                         |
| go                         | 91.6 ms                                                     | 90.0 ms: 1.02x faster                                                        |
| 2to3                       | 218 ms                                                      | 214 ms: 1.02x faster                                                         |
| async_tree_memoization     | 339 ms                                                      | 334 ms: 1.02x faster                                                         |
| pidigits                   | 152 ms                                                      | 151 ms: 1.01x faster                                                         |
| gc_traversal               | 1.52 ms                                                     | 1.51 ms: 1.01x faster                                                        |
| sympy_integrate            | 13.0 ms                                                     | 12.8 ms: 1.01x faster                                                        |
| unpickle_list              | 2.75 us                                                     | 2.78 us: 1.01x slower                                                        |
| python_startup             | 19.5 ms                                                     | 20.1 ms: 1.03x slower                                                        |
| unpack_sequence            | 37.5 ns                                                     | 38.8 ns: 1.04x slower                                                        |
| unpickle                   | 8.18 us                                                     | 8.50 us: 1.04x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.1 ms: 1.06x slower                                                        |
| hexiom                     | 4.10 ms                                                     | 4.44 ms: 1.08x slower                                                        |
| scimark_monte_carlo        | 43.7 ms                                                     | 47.6 ms: 1.09x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.53 ms: 1.10x slower                                                        |
| pickle_list                | 2.83 us                                                     | 3.13 us: 1.11x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 18.0 ms: 1.11x slower                                                        |
| json                       | 3.05 ms                                                     | 3.38 ms: 1.11x slower                                                        |
| mdp                        | 1.37 sec                                                    | 1.54 sec: 1.12x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.0 ms: 1.15x slower                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                 |

Benchmark hidden because not significant (1): xml_etree_parse
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.03x


# Memory

- memory change: unknown