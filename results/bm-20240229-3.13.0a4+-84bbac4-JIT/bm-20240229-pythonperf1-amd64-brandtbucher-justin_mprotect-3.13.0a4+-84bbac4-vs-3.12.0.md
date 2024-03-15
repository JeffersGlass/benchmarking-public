# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-amd64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                         |
| chameleon      | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                                        |
| docutils       | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                       |
| tornado_http   | 89.5 ms                                                     | 85.0 ms: 1.05x faster                                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 267 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                                         |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                         |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                         |
| async_tree_io_tg           | 771 ms                                                      | 759 ms: 1.02x faster                                                         |
| Geometric mean             | (ref)                                                       | 1.05x faster                                                                 |

Benchmark hidden because not significant (2): async_tree_io, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 57.7 ms: 1.25x faster                                                        |
| float          | 56.8 ms                                                     | 49.1 ms: 1.16x faster                                                        |
| pidigits       | 152 ms                                                      | 150 ms: 1.02x faster                                                         |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 82.2 ms: 1.06x faster                                                        |
| regex_dna      | 126 ms                                                      | 122 ms: 1.04x faster                                                         |
| regex_effbot   | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                        |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| tomli_loads          | 1.37 sec                                                    | 1.19 sec: 1.15x faster                                                       |
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                                         |
| pickle_dict          | 18.4 us                                                     | 17.3 us: 1.06x faster                                                        |
| xml_etree_generate   | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                                        |
| xml_etree_process    | 37.7 ms                                                     | 35.8 ms: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.1 ms: 1.05x faster                                                        |
| unpickle_pure_python | 133 us                                                      | 127 us: 1.05x faster                                                         |
| pickle               | 7.43 us                                                     | 7.16 us: 1.04x faster                                                        |
| json_dumps           | 5.70 ms                                                     | 5.52 ms: 1.03x faster                                                        |
| unpickle_list        | 2.75 us                                                     | 2.79 us: 1.01x slower                                                        |
| unpickle             | 8.18 us                                                     | 8.68 us: 1.06x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.04x faster                                                                 |

Benchmark hidden because not significant (3): xml_etree_parse, json_loads, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                        |
| python_startup_no_site | 16.2 ms                                                     | 21.5 ms: 1.32x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 5.66 ms: 1.25x faster                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.4 us: 1.35x faster                                                        |
| comprehensions             | 14.1 us                                                     | 10.6 us: 1.33x faster                                                        |
| spectral_norm              | 66.9 ms                                                     | 51.0 ms: 1.31x faster                                                        |
| mako                       | 7.09 ms                                                     | 5.66 ms: 1.25x faster                                                        |
| nbody                      | 71.9 ms                                                     | 57.7 ms: 1.25x faster                                                        |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.79 sec: 1.17x faster                                                       |
| mypy2                      | 509 ms                                                      | 438 ms: 1.16x faster                                                         |
| float                      | 56.8 ms                                                     | 49.1 ms: 1.16x faster                                                        |
| tomli_loads                | 1.37 sec                                                    | 1.19 sec: 1.15x faster                                                       |
| crypto_pyaes               | 48.5 ms                                                     | 42.7 ms: 1.14x faster                                                        |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.27 ms: 1.13x faster                                                        |
| fannkuch                   | 247 ms                                                      | 220 ms: 1.12x faster                                                         |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.12x faster                                                         |
| sqlite_synth               | 1.76 us                                                     | 1.58 us: 1.11x faster                                                        |
| generators                 | 22.5 ms                                                     | 20.4 ms: 1.11x faster                                                        |
| deepcopy                   | 238 us                                                      | 217 us: 1.10x faster                                                         |
| pprint_safe_repr           | 513 ms                                                      | 468 ms: 1.10x faster                                                         |
| chaos                      | 43.3 ms                                                     | 39.6 ms: 1.09x faster                                                        |
| async_tree_none            | 291 ms                                                      | 267 ms: 1.09x faster                                                         |
| scimark_fft                | 184 ms                                                      | 169 ms: 1.09x faster                                                         |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                         |
| pprint_pformat             | 1.05 sec                                                    | 962 ms: 1.09x faster                                                         |
| deepcopy_reduce            | 2.09 us                                                     | 1.93 us: 1.09x faster                                                        |
| logging_silent             | 60.5 ns                                                     | 55.8 ns: 1.08x faster                                                        |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 464 ms: 1.08x faster                                                         |
| deepcopy_memo              | 23.7 us                                                     | 21.9 us: 1.08x faster                                                        |
| sympy_str                  | 175 ms                                                      | 162 ms: 1.08x faster                                                         |
| dulwich_log                | 44.3 ms                                                     | 41.1 ms: 1.08x faster                                                        |
| sqlglot_normalize          | 187 ms                                                      | 174 ms: 1.08x faster                                                         |
| pathlib                    | 80.5 ms                                                     | 75.0 ms: 1.07x faster                                                        |
| logging_format             | 6.72 us                                                     | 6.28 us: 1.07x faster                                                        |
| logging_simple             | 6.28 us                                                     | 5.88 us: 1.07x faster                                                        |
| raytrace                   | 192 ms                                                      | 180 ms: 1.07x faster                                                         |
| coroutines                 | 14.3 ms                                                     | 13.4 ms: 1.06x faster                                                        |
| regex_compile              | 87.5 ms                                                     | 82.2 ms: 1.06x faster                                                        |
| pickle_dict                | 18.4 us                                                     | 17.3 us: 1.06x faster                                                        |
| sympy_sum                  | 91.5 ms                                                     | 86.0 ms: 1.06x faster                                                        |
| xml_etree_generate         | 55.8 ms                                                     | 52.5 ms: 1.06x faster                                                        |
| xml_etree_process          | 37.7 ms                                                     | 35.8 ms: 1.05x faster                                                        |
| tornado_http               | 89.5 ms                                                     | 85.0 ms: 1.05x faster                                                        |
| xml_etree_iterparse        | 65.2 ms                                                     | 62.1 ms: 1.05x faster                                                        |
| async_tree_none_tg         | 285 ms                                                      | 272 ms: 1.05x faster                                                         |
| scimark_monte_carlo        | 43.7 ms                                                     | 41.7 ms: 1.05x faster                                                        |
| unpickle_pure_python       | 133 us                                                      | 127 us: 1.05x faster                                                         |
| bench_thread_pool          | 857 us                                                      | 821 us: 1.04x faster                                                         |
| pyflate                    | 295 ms                                                      | 283 ms: 1.04x faster                                                         |
| async_tree_memoization_tg  | 367 ms                                                      | 352 ms: 1.04x faster                                                         |
| chameleon                  | 4.98 ms                                                     | 4.78 ms: 1.04x faster                                                        |
| docutils                   | 1.66 sec                                                    | 1.60 sec: 1.04x faster                                                       |
| sqlglot_parse              | 804 us                                                      | 774 us: 1.04x faster                                                         |
| pickle                     | 7.43 us                                                     | 7.16 us: 1.04x faster                                                        |
| regex_dna                  | 126 ms                                                      | 122 ms: 1.04x faster                                                         |
| asyncio_tcp                | 487 ms                                                      | 471 ms: 1.04x faster                                                         |
| json_dumps                 | 5.70 ms                                                     | 5.52 ms: 1.03x faster                                                        |
| sympy_expand               | 284 ms                                                      | 275 ms: 1.03x faster                                                         |
| richards_super             | 32.1 ms                                                     | 31.2 ms: 1.03x faster                                                        |
| sqlglot_transpile          | 1.02 ms                                                     | 994 us: 1.03x faster                                                         |
| regex_effbot               | 1.62 ms                                                     | 1.58 ms: 1.02x faster                                                        |
| nqueens                    | 62.8 ms                                                     | 61.4 ms: 1.02x faster                                                        |
| richards                   | 28.4 ms                                                     | 27.8 ms: 1.02x faster                                                        |
| meteor_contest             | 74.6 ms                                                     | 73.4 ms: 1.02x faster                                                        |
| pidigits                   | 152 ms                                                      | 150 ms: 1.02x faster                                                         |
| async_tree_io_tg           | 771 ms                                                      | 759 ms: 1.02x faster                                                         |
| deltablue                  | 2.16 ms                                                     | 2.13 ms: 1.01x faster                                                        |
| sqlglot_optimize           | 34.5 ms                                                     | 34.2 ms: 1.01x faster                                                        |
| mdp                        | 1.37 sec                                                    | 1.38 sec: 1.01x slower                                                       |
| sympy_integrate            | 13.0 ms                                                     | 13.1 ms: 1.01x slower                                                        |
| bench_mp_pool              | 69.2 ms                                                     | 69.8 ms: 1.01x slower                                                        |
| unpickle_list              | 2.75 us                                                     | 2.79 us: 1.01x slower                                                        |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                         |
| scimark_sor                | 78.8 ms                                                     | 80.6 ms: 1.02x slower                                                        |
| json                       | 3.05 ms                                                     | 3.22 ms: 1.06x slower                                                        |
| pycparser                  | 699 ms                                                      | 739 ms: 1.06x slower                                                         |
| unpickle                   | 8.18 us                                                     | 8.68 us: 1.06x slower                                                        |
| hexiom                     | 4.10 ms                                                     | 4.37 ms: 1.07x slower                                                        |
| regex_v8                   | 14.2 ms                                                     | 15.2 ms: 1.07x slower                                                        |
| go                         | 91.6 ms                                                     | 98.4 ms: 1.07x slower                                                        |
| telco                      | 4.13 ms                                                     | 4.66 ms: 1.13x slower                                                        |
| coverage                   | 40.8 ms                                                     | 46.4 ms: 1.14x slower                                                        |
| scimark_lu                 | 58.9 ms                                                     | 70.4 ms: 1.20x slower                                                        |
| python_startup             | 19.5 ms                                                     | 23.8 ms: 1.22x slower                                                        |
| unpack_sequence            | 37.5 ns                                                     | 46.6 ns: 1.24x slower                                                        |
| python_startup_no_site     | 16.2 ms                                                     | 21.5 ms: 1.32x slower                                                        |
| dask                       | 263 ms                                                      | 360 ms: 1.37x slower                                                         |
| Geometric mean             | (ref)                                                       | 1.04x faster                                                                 |

Benchmark hidden because not significant (8): async_tree_io, create_gc_cycles, xml_etree_parse, gc_traversal, async_generators, json_loads, async_tree_memoization, pickle_list
Ignored benchmarks (4) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown