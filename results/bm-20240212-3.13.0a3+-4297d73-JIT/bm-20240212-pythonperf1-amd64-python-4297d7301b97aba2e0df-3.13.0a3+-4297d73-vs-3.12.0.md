
# Results vs. 3.12.0

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-amd64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| chameleon      | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 84.9 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                        |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.09x faster                                                        |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 466 ms: 1.08x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 269 ms: 1.06x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 746 ms: 1.03x faster                                                        |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                                        |
| async_tree_memoization     | 339 ms                                                      | 333 ms: 1.02x faster                                                        |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 61.7 ms: 1.16x faster                                                       |
| float          | 56.8 ms                                                     | 50.0 ms: 1.13x faster                                                       |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 79.9 ms: 1.09x faster                                                       |
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| regex_effbot   | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 173 us: 1.13x faster                                                        |
| tomli_loads          | 1.37 sec                                                    | 1.27 sec: 1.08x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 125 us: 1.07x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 17.6 us: 1.04x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                       |
| pickle               | 7.43 us                                                     | 7.16 us: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                       |
| json_dumps           | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 93.9 ms: 1.01x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| pickle_list          | 2.83 us                                                     | 3.12 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                                       |
| python_startup_no_site | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 6.44 ms: 1.10x faster                                                       |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 69.1 us: 1.38x faster                                                       |
| comprehensions             | 14.1 us                                                     | 11.3 us: 1.25x faster                                                       |
| mypy2                      | 509 ms                                                      | 425 ms: 1.20x faster                                                        |
| sqlite_synth               | 1.76 us                                                     | 1.51 us: 1.17x faster                                                       |
| nbody                      | 71.9 ms                                                     | 61.7 ms: 1.16x faster                                                       |
| logging_silent             | 60.5 ns                                                     | 52.2 ns: 1.16x faster                                                       |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.84 sec: 1.14x faster                                                      |
| richards_super             | 32.1 ms                                                     | 28.2 ms: 1.14x faster                                                       |
| richards                   | 28.4 ms                                                     | 25.0 ms: 1.14x faster                                                       |
| float                      | 56.8 ms                                                     | 50.0 ms: 1.13x faster                                                       |
| pickle_pure_python         | 195 us                                                      | 173 us: 1.13x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.0 ms: 1.13x faster                                                       |
| raytrace                   | 192 ms                                                      | 172 ms: 1.12x faster                                                        |
| deepcopy_reduce            | 2.09 us                                                     | 1.89 us: 1.11x faster                                                       |
| async_tree_none            | 291 ms                                                      | 263 ms: 1.11x faster                                                        |
| deepcopy_memo              | 23.7 us                                                     | 21.5 us: 1.10x faster                                                       |
| coroutines                 | 14.3 ms                                                     | 12.9 ms: 1.10x faster                                                       |
| mako                       | 7.09 ms                                                     | 6.44 ms: 1.10x faster                                                       |
| dulwich_log                | 44.3 ms                                                     | 40.2 ms: 1.10x faster                                                       |
| deltablue                  | 2.16 ms                                                     | 1.96 ms: 1.10x faster                                                       |
| deepcopy                   | 238 us                                                      | 217 us: 1.10x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 79.9 ms: 1.09x faster                                                       |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 451 ms: 1.09x faster                                                        |
| pathlib                    | 80.5 ms                                                     | 74.5 ms: 1.08x faster                                                       |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 466 ms: 1.08x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.83 us: 1.08x faster                                                       |
| tomli_loads                | 1.37 sec                                                    | 1.27 sec: 1.08x faster                                                      |
| logging_format             | 6.72 us                                                     | 6.28 us: 1.07x faster                                                       |
| pprint_safe_repr           | 513 ms                                                      | 480 ms: 1.07x faster                                                        |
| sqlglot_parse              | 804 us                                                      | 754 us: 1.07x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 125 us: 1.07x faster                                                        |
| nqueens                    | 62.8 ms                                                     | 58.8 ms: 1.07x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 45.5 ms: 1.07x faster                                                       |
| xml_etree_generate         | 55.8 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| async_tree_none_tg         | 285 ms                                                      | 269 ms: 1.06x faster                                                        |
| regex_dna                  | 126 ms                                                      | 119 ms: 1.06x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| pprint_pformat             | 1.05 sec                                                    | 991 ms: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 84.9 ms: 1.05x faster                                                       |
| scimark_lu                 | 58.9 ms                                                     | 55.9 ms: 1.05x faster                                                       |
| sympy_str                  | 175 ms                                                      | 167 ms: 1.05x faster                                                        |
| asyncio_tcp                | 487 ms                                                      | 465 ms: 1.05x faster                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 66.1 ms: 1.05x faster                                                       |
| sqlglot_transpile          | 1.02 ms                                                     | 979 us: 1.04x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.6 us: 1.04x faster                                                       |
| chameleon                  | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                                       |
| xml_etree_process          | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                       |
| sqlglot_normalize          | 187 ms                                                      | 180 ms: 1.04x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 88.1 ms: 1.04x faster                                                       |
| pickle                     | 7.43 us                                                     | 7.16 us: 1.04x faster                                                       |
| bench_thread_pool          | 857 us                                                      | 826 us: 1.04x faster                                                        |
| create_gc_cycles           | 752 us                                                      | 728 us: 1.03x faster                                                        |
| async_tree_io_tg           | 771 ms                                                      | 746 ms: 1.03x faster                                                        |
| dask                       | 263 ms                                                      | 255 ms: 1.03x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                       |
| json_dumps                 | 5.70 ms                                                     | 5.55 ms: 1.03x faster                                                       |
| chaos                      | 43.3 ms                                                     | 42.5 ms: 1.02x faster                                                       |
| async_tree_io              | 731 ms                                                      | 716 ms: 1.02x faster                                                        |
| scimark_sor                | 78.8 ms                                                     | 77.2 ms: 1.02x faster                                                       |
| pycparser                  | 699 ms                                                      | 685 ms: 1.02x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 65.7 ms: 1.02x faster                                                       |
| async_tree_memoization     | 339 ms                                                      | 333 ms: 1.02x faster                                                        |
| regex_effbot               | 1.62 ms                                                     | 1.59 ms: 1.02x faster                                                       |
| fannkuch                   | 247 ms                                                      | 243 ms: 1.01x faster                                                        |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                       |
| gc_traversal               | 1.52 ms                                                     | 1.50 ms: 1.01x faster                                                       |
| async_generators           | 239 ms                                                      | 237 ms: 1.01x faster                                                        |
| 2to3                       | 218 ms                                                      | 216 ms: 1.01x faster                                                        |
| sympy_expand               | 284 ms                                                      | 282 ms: 1.01x faster                                                        |
| xml_etree_parse            | 93.0 ms                                                     | 93.9 ms: 1.01x slower                                                       |
| meteor_contest             | 74.6 ms                                                     | 75.5 ms: 1.01x slower                                                       |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                       |
| python_startup             | 19.5 ms                                                     | 20.2 ms: 1.04x slower                                                       |
| unpickle                   | 8.18 us                                                     | 8.54 us: 1.04x slower                                                       |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.67 ms: 1.04x slower                                                       |
| pyflate                    | 295 ms                                                      | 310 ms: 1.05x slower                                                        |
| go                         | 91.6 ms                                                     | 97.1 ms: 1.06x slower                                                       |
| scimark_fft                | 184 ms                                                      | 196 ms: 1.06x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.06x slower                                                       |
| unpack_sequence            | 37.5 ns                                                     | 40.8 ns: 1.09x slower                                                       |
| pickle_list                | 2.83 us                                                     | 3.12 us: 1.10x slower                                                       |
| python_startup_no_site     | 16.2 ms                                                     | 18.1 ms: 1.11x slower                                                       |
| mdp                        | 1.37 sec                                                    | 1.54 sec: 1.13x slower                                                      |
| telco                      | 4.13 ms                                                     | 4.71 ms: 1.14x slower                                                       |
| coverage                   | 40.8 ms                                                     | 47.7 ms: 1.17x slower                                                       |
| json                       | 3.05 ms                                                     | 3.58 ms: 1.17x slower                                                       |
| hexiom                     | 4.10 ms                                                     | 5.22 ms: 1.27x slower                                                       |
| scimark_monte_carlo        | 43.7 ms                                                     | 56.7 ms: 1.30x slower                                                       |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (3): pidigits, sqlglot_optimize, unpickle_list
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown