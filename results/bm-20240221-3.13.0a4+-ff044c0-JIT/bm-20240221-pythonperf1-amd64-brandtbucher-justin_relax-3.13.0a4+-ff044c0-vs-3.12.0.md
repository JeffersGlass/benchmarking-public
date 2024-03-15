
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_relax
- machine: windows-amd64
- commit hash: ff044c0
- commit date: 2024-02-21
- overall geometric mean: 1.02x faster \*
- HPT reliability: 99.98%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 223 ms: 1.02x slower                                                      |
| chameleon      | 4.98 ms                                                     | 4.63 ms: 1.08x faster                                                     |
| docutils       | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                    |
| tornado_http   | 89.5 ms                                                     | 84.7 ms: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.04x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                      |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                      |
| async_tree_none_tg         | 285 ms                                                      | 267 ms: 1.07x faster                                                      |
| async_tree_io_tg           | 771 ms                                                      | 751 ms: 1.03x faster                                                      |
| async_tree_io              | 731 ms                                                      | 718 ms: 1.02x faster                                                      |
| Geometric mean             | (ref)                                                       | 1.06x faster                                                              |

Benchmark hidden because not significant (1): async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.6 ms: 1.21x faster                                                     |
| float          | 56.8 ms                                                     | 48.5 ms: 1.17x faster                                                     |
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.13x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 118 ms: 1.07x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                     |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_compile  | 87.5 ms                                                     | 89.9 ms: 1.03x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 175 us: 1.11x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                                     |
| tomli_loads          | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                                    |
| xml_etree_generate   | 55.8 ms                                                     | 53.6 ms: 1.04x faster                                                     |
| pickle               | 7.43 us                                                     | 7.15 us: 1.04x faster                                                     |
| xml_etree_process    | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| json_dumps           | 5.70 ms                                                     | 5.53 ms: 1.03x faster                                                     |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                     |
| pickle_list          | 2.83 us                                                     | 2.77 us: 1.02x faster                                                     |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                     |
| xml_etree_parse      | 93.0 ms                                                     | 92.0 ms: 1.01x faster                                                     |
| unpickle_pure_python | 133 us                                                      | 135 us: 1.02x slower                                                      |
| unpickle_list        | 2.75 us                                                     | 2.82 us: 1.03x slower                                                     |
| unpickle             | 8.18 us                                                     | 8.59 us: 1.05x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 23.9 ms: 1.23x slower                                                     |
| python_startup_no_site | 16.2 ms                                                     | 21.6 ms: 1.33x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.28x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako      | 7.09 ms                                                     | 5.95 ms: 1.19x faster                                                     |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240221-pythonperf1-amd64-brandtbucher-justin_relax-3.13.0a4+-ff044c0 |
|----------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols   | 95.1 us                                                     | 70.9 us: 1.34x faster                                                     |
| comprehensions             | 14.1 us                                                     | 10.8 us: 1.31x faster                                                     |
| asyncio_tcp_ssl            | 2.10 sec                                                    | 1.66 sec: 1.27x faster                                                    |
| spectral_norm              | 66.9 ms                                                     | 54.6 ms: 1.23x faster                                                     |
| nbody                      | 71.9 ms                                                     | 59.6 ms: 1.21x faster                                                     |
| mako                       | 7.09 ms                                                     | 5.95 ms: 1.19x faster                                                     |
| mypy2                      | 509 ms                                                      | 433 ms: 1.18x faster                                                      |
| float                      | 56.8 ms                                                     | 48.5 ms: 1.17x faster                                                     |
| sqlite_synth               | 1.76 us                                                     | 1.55 us: 1.14x faster                                                     |
| async_tree_none            | 291 ms                                                      | 261 ms: 1.12x faster                                                      |
| pickle_pure_python         | 195 us                                                      | 175 us: 1.11x faster                                                      |
| generators                 | 22.5 ms                                                     | 20.4 ms: 1.11x faster                                                     |
| crypto_pyaes               | 48.5 ms                                                     | 43.9 ms: 1.10x faster                                                     |
| coroutines                 | 14.3 ms                                                     | 13.0 ms: 1.10x faster                                                     |
| scimark_sparse_mat_mult    | 2.56 ms                                                     | 2.33 ms: 1.10x faster                                                     |
| async_tree_cpu_io_mixed    | 489 ms                                                      | 450 ms: 1.09x faster                                                      |
| logging_silent             | 60.5 ns                                                     | 55.7 ns: 1.09x faster                                                     |
| deepcopy_memo              | 23.7 us                                                     | 21.9 us: 1.08x faster                                                     |
| deepcopy                   | 238 us                                                      | 220 us: 1.08x faster                                                      |
| async_tree_memoization_tg  | 367 ms                                                      | 340 ms: 1.08x faster                                                      |
| async_tree_cpu_io_mixed_tg | 502 ms                                                      | 465 ms: 1.08x faster                                                      |
| deepcopy_reduce            | 2.09 us                                                     | 1.94 us: 1.08x faster                                                     |
| chameleon                  | 4.98 ms                                                     | 4.63 ms: 1.08x faster                                                     |
| dulwich_log                | 44.3 ms                                                     | 41.3 ms: 1.07x faster                                                     |
| async_tree_none_tg         | 285 ms                                                      | 267 ms: 1.07x faster                                                      |
| regex_dna                  | 126 ms                                                      | 118 ms: 1.07x faster                                                      |
| sqlglot_normalize          | 187 ms                                                      | 175 ms: 1.07x faster                                                      |
| logging_simple             | 6.28 us                                                     | 5.90 us: 1.06x faster                                                     |
| raytrace                   | 192 ms                                                      | 181 ms: 1.06x faster                                                      |
| chaos                      | 43.3 ms                                                     | 40.8 ms: 1.06x faster                                                     |
| tornado_http               | 89.5 ms                                                     | 84.7 ms: 1.06x faster                                                     |
| pathlib                    | 80.5 ms                                                     | 76.1 ms: 1.06x faster                                                     |
| sympy_str                  | 175 ms                                                      | 166 ms: 1.06x faster                                                      |
| pickle_dict                | 18.4 us                                                     | 17.4 us: 1.06x faster                                                     |
| tomli_loads                | 1.37 sec                                                    | 1.30 sec: 1.05x faster                                                    |
| logging_format             | 6.72 us                                                     | 6.41 us: 1.05x faster                                                     |
| asyncio_tcp                | 487 ms                                                      | 466 ms: 1.05x faster                                                      |
| sympy_sum                  | 91.5 ms                                                     | 87.8 ms: 1.04x faster                                                     |
| xml_etree_generate         | 55.8 ms                                                     | 53.6 ms: 1.04x faster                                                     |
| regex_effbot               | 1.62 ms                                                     | 1.55 ms: 1.04x faster                                                     |
| pickle                     | 7.43 us                                                     | 7.15 us: 1.04x faster                                                     |
| xml_etree_process          | 37.7 ms                                                     | 36.4 ms: 1.04x faster                                                     |
| docutils                   | 1.66 sec                                                    | 1.61 sec: 1.03x faster                                                    |
| scimark_fft                | 184 ms                                                      | 179 ms: 1.03x faster                                                      |
| json_dumps                 | 5.70 ms                                                     | 5.53 ms: 1.03x faster                                                     |
| async_tree_io_tg           | 771 ms                                                      | 751 ms: 1.03x faster                                                      |
| async_generators           | 239 ms                                                      | 233 ms: 1.03x faster                                                      |
| xml_etree_iterparse        | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                     |
| deltablue                  | 2.16 ms                                                     | 2.11 ms: 1.02x faster                                                     |
| bench_thread_pool          | 857 us                                                      | 839 us: 1.02x faster                                                      |
| nqueens                    | 62.8 ms                                                     | 61.5 ms: 1.02x faster                                                     |
| pickle_list                | 2.83 us                                                     | 2.77 us: 1.02x faster                                                     |
| async_tree_io              | 731 ms                                                      | 718 ms: 1.02x faster                                                      |
| pprint_safe_repr           | 513 ms                                                      | 506 ms: 1.01x faster                                                      |
| pidigits                   | 152 ms                                                      | 150 ms: 1.01x faster                                                      |
| create_gc_cycles           | 752 us                                                      | 742 us: 1.01x faster                                                      |
| json_loads                 | 13.9 us                                                     | 13.7 us: 1.01x faster                                                     |
| meteor_contest             | 74.6 ms                                                     | 73.7 ms: 1.01x faster                                                     |
| xml_etree_parse            | 93.0 ms                                                     | 92.0 ms: 1.01x faster                                                     |
| sympy_expand               | 284 ms                                                      | 286 ms: 1.01x slower                                                      |
| sqlglot_optimize           | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                     |
| sqlglot_transpile          | 1.02 ms                                                     | 1.03 ms: 1.01x slower                                                     |
| unpickle_pure_python       | 133 us                                                      | 135 us: 1.02x slower                                                      |
| bench_mp_pool              | 69.2 ms                                                     | 70.3 ms: 1.02x slower                                                     |
| sympy_integrate            | 13.0 ms                                                     | 13.2 ms: 1.02x slower                                                     |
| 2to3                       | 218 ms                                                      | 223 ms: 1.02x slower                                                      |
| unpickle_list              | 2.75 us                                                     | 2.82 us: 1.03x slower                                                     |
| regex_v8                   | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_compile              | 87.5 ms                                                     | 89.9 ms: 1.03x slower                                                     |
| scimark_monte_carlo        | 43.7 ms                                                     | 45.6 ms: 1.04x slower                                                     |
| unpickle                   | 8.18 us                                                     | 8.59 us: 1.05x slower                                                     |
| fannkuch                   | 247 ms                                                      | 259 ms: 1.05x slower                                                      |
| go                         | 91.6 ms                                                     | 98.1 ms: 1.07x slower                                                     |
| scimark_sor                | 78.8 ms                                                     | 84.4 ms: 1.07x slower                                                     |
| richards_super             | 32.1 ms                                                     | 35.2 ms: 1.10x slower                                                     |
| telco                      | 4.13 ms                                                     | 4.57 ms: 1.11x slower                                                     |
| mdp                        | 1.37 sec                                                    | 1.52 sec: 1.11x slower                                                    |
| richards                   | 28.4 ms                                                     | 31.7 ms: 1.12x slower                                                     |
| json                       | 3.05 ms                                                     | 3.55 ms: 1.17x slower                                                     |
| coverage                   | 40.8 ms                                                     | 48.1 ms: 1.18x slower                                                     |
| hexiom                     | 4.10 ms                                                     | 5.00 ms: 1.22x slower                                                     |
| python_startup             | 19.5 ms                                                     | 23.9 ms: 1.23x slower                                                     |
| scimark_lu                 | 58.9 ms                                                     | 74.5 ms: 1.26x slower                                                     |
| python_startup_no_site     | 16.2 ms                                                     | 21.6 ms: 1.33x slower                                                     |
| unpack_sequence            | 37.5 ns                                                     | 57.6 ns: 1.54x slower                                                     |
| Geometric mean             | (ref)                                                       | 1.02x faster                                                              |

Benchmark hidden because not significant (6): async_tree_memoization, gc_traversal, sqlglot_parse, pprint_pformat, pyflate, pycparser
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, dask, django_template, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 99.98% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown