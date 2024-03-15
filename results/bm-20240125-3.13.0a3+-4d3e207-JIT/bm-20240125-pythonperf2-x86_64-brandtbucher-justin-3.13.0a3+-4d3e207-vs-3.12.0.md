
# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin
- machine: linux-x86_64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.92x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 299 ms: 1.05x slower                                                 |
| chameleon      | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                |
| docutils       | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                               |
| tornado_http   | 121 ms                                                       | 124 ms: 1.02x slower                                                 |
| Geometric mean | (ref)                                                        | 1.03x slower                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none    | 452 ms                                                       | 434 ms: 1.04x faster                                                 |
| async_tree_none_tg | 431 ms                                                       | 435 ms: 1.01x slower                                                 |
| async_tree_io_tg   | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                               |
| async_tree_io      | 1.04 sec                                                     | 1.07 sec: 1.02x slower                                               |
| Geometric mean     | (ref)                                                        | 1.00x slower                                                         |

Benchmark hidden because not significant (4): async_tree_memoization, async_tree_cpu_io_mixed, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 263 ms: 1.01x faster                                                 |
| float          | 76.6 ms                                                      | 82.4 ms: 1.07x slower                                                |
| nbody          | 88.0 ms                                                      | 107 ms: 1.21x slower                                                 |
| Geometric mean | (ref)                                                        | 1.09x slower                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 144 ms                                                       | 147 ms: 1.02x slower                                                 |
| regex_dna      | 239 ms                                                       | 246 ms: 1.03x slower                                                 |
| regex_v8       | 23.6 ms                                                      | 26.7 ms: 1.13x slower                                                |
| Geometric mean | (ref)                                                        | 1.05x slower                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.4 us: 1.04x faster                                                |
| pickle_pure_python   | 318 us                                                       | 310 us: 1.03x faster                                                 |
| xml_etree_generate   | 86.1 ms                                                      | 84.9 ms: 1.01x faster                                                |
| pickle_list          | 4.43 us                                                      | 4.38 us: 1.01x faster                                                |
| xml_etree_process    | 58.4 ms                                                      | 58.7 ms: 1.01x slower                                                |
| pickle               | 10.5 us                                                      | 10.6 us: 1.01x slower                                                |
| json_loads           | 24.4 us                                                      | 24.8 us: 1.02x slower                                                |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                                 |
| unpickle             | 14.8 us                                                      | 15.5 us: 1.05x slower                                                |
| json_dumps           | 10.2 ms                                                      | 10.7 ms: 1.05x slower                                                |
| tomli_loads          | 2.16 sec                                                     | 2.30 sec: 1.07x slower                                               |
| unpickle_list        | 4.66 us                                                      | 5.09 us: 1.09x slower                                                |
| unpickle_pure_python | 210 us                                                       | 235 us: 1.12x slower                                                 |
| Geometric mean       | (ref)                                                        | 1.02x slower                                                         |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 11.9 ms: 1.19x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240125-pythonperf2-x86_64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 152 us                                                       | 119 us: 1.28x faster                                                 |
| unpack_sequence          | 53.2 ns                                                      | 42.9 ns: 1.24x faster                                                |
| generators               | 37.4 ms                                                      | 33.7 ms: 1.11x faster                                                |
| raytrace                 | 298 ms                                                       | 278 ms: 1.07x faster                                                 |
| async_generators         | 390 ms                                                       | 367 ms: 1.06x faster                                                 |
| comprehensions           | 21.9 us                                                      | 20.8 us: 1.05x faster                                                |
| async_tree_none          | 452 ms                                                       | 434 ms: 1.04x faster                                                 |
| create_gc_cycles         | 1.59 ms                                                      | 1.53 ms: 1.04x faster                                                |
| pickle_dict              | 32.5 us                                                      | 31.4 us: 1.04x faster                                                |
| asyncio_tcp              | 378 ms                                                       | 367 ms: 1.03x faster                                                 |
| pickle_pure_python       | 318 us                                                       | 310 us: 1.03x faster                                                 |
| sympy_sum                | 162 ms                                                       | 159 ms: 1.02x faster                                                 |
| xml_etree_generate       | 86.1 ms                                                      | 84.9 ms: 1.01x faster                                                |
| gc_traversal             | 3.48 ms                                                      | 3.43 ms: 1.01x faster                                                |
| sympy_str                | 302 ms                                                       | 298 ms: 1.01x faster                                                 |
| deepcopy_reduce          | 3.37 us                                                      | 3.33 us: 1.01x faster                                                |
| pickle_list              | 4.43 us                                                      | 4.38 us: 1.01x faster                                                |
| logging_format           | 7.48 us                                                      | 7.41 us: 1.01x faster                                                |
| pidigits                 | 265 ms                                                       | 263 ms: 1.01x faster                                                 |
| sqlite_synth             | 2.77 us                                                      | 2.75 us: 1.01x faster                                                |
| pathlib                  | 18.9 ms                                                      | 18.8 ms: 1.01x faster                                                |
| mdp                      | 2.57 sec                                                     | 2.56 sec: 1.00x faster                                               |
| docutils                 | 2.87 sec                                                     | 2.88 sec: 1.00x slower                                               |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 1.60 sec: 1.00x slower                                               |
| xml_etree_process        | 58.4 ms                                                      | 58.7 ms: 1.01x slower                                                |
| pickle                   | 10.5 us                                                      | 10.6 us: 1.01x slower                                                |
| async_tree_none_tg       | 431 ms                                                       | 435 ms: 1.01x slower                                                 |
| async_tree_io_tg         | 1.05 sec                                                     | 1.06 sec: 1.01x slower                                               |
| sqlglot_transpile        | 1.78 ms                                                      | 1.79 ms: 1.01x slower                                                |
| sympy_integrate          | 23.9 ms                                                      | 24.3 ms: 1.01x slower                                                |
| json_loads               | 24.4 us                                                      | 24.8 us: 1.02x slower                                                |
| tornado_http             | 121 ms                                                       | 124 ms: 1.02x slower                                                 |
| sqlglot_normalize        | 116 ms                                                       | 118 ms: 1.02x slower                                                 |
| xml_etree_iterparse      | 103 ms                                                       | 105 ms: 1.02x slower                                                 |
| logging_silent           | 94.4 ns                                                      | 96.7 ns: 1.02x slower                                                |
| regex_compile            | 144 ms                                                       | 147 ms: 1.02x slower                                                 |
| json                     | 5.12 ms                                                      | 5.24 ms: 1.02x slower                                                |
| async_tree_io            | 1.04 sec                                                     | 1.07 sec: 1.02x slower                                               |
| dask                     | 392 ms                                                       | 403 ms: 1.03x slower                                                 |
| scimark_lu               | 98.8 ms                                                      | 102 ms: 1.03x slower                                                 |
| deepcopy_memo            | 36.8 us                                                      | 37.8 us: 1.03x slower                                                |
| regex_dna                | 239 ms                                                       | 246 ms: 1.03x slower                                                 |
| crypto_pyaes             | 80.3 ms                                                      | 82.9 ms: 1.03x slower                                                |
| sympy_expand             | 484 ms                                                       | 501 ms: 1.03x slower                                                 |
| bench_thread_pool        | 950 us                                                       | 982 us: 1.03x slower                                                 |
| meteor_contest           | 128 ms                                                       | 133 ms: 1.03x slower                                                 |
| dulwich_log              | 65.4 ms                                                      | 67.9 ms: 1.04x slower                                                |
| chameleon                | 7.23 ms                                                      | 7.53 ms: 1.04x slower                                                |
| unpickle                 | 14.8 us                                                      | 15.5 us: 1.05x slower                                                |
| 2to3                     | 285 ms                                                       | 299 ms: 1.05x slower                                                 |
| json_dumps               | 10.2 ms                                                      | 10.7 ms: 1.05x slower                                                |
| sqlglot_optimize         | 57.5 ms                                                      | 61.0 ms: 1.06x slower                                                |
| bench_mp_pool            | 4.76 ms                                                      | 5.07 ms: 1.07x slower                                                |
| tomli_loads              | 2.16 sec                                                     | 2.30 sec: 1.07x slower                                               |
| pprint_safe_repr         | 807 ms                                                       | 864 ms: 1.07x slower                                                 |
| pycparser                | 1.23 sec                                                     | 1.32 sec: 1.07x slower                                               |
| float                    | 76.6 ms                                                      | 82.4 ms: 1.07x slower                                                |
| python_startup           | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                |
| pprint_pformat           | 1.65 sec                                                     | 1.80 sec: 1.08x slower                                               |
| unpickle_list            | 4.66 us                                                      | 5.09 us: 1.09x slower                                                |
| nqueens                  | 89.9 ms                                                      | 98.5 ms: 1.10x slower                                                |
| chaos                    | 64.0 ms                                                      | 70.7 ms: 1.11x slower                                                |
| richards                 | 45.7 ms                                                      | 50.9 ms: 1.11x slower                                                |
| unpickle_pure_python     | 210 us                                                       | 235 us: 1.12x slower                                                 |
| regex_v8                 | 23.6 ms                                                      | 26.7 ms: 1.13x slower                                                |
| richards_super           | 51.3 ms                                                      | 58.4 ms: 1.14x slower                                                |
| scimark_monte_carlo      | 69.0 ms                                                      | 79.3 ms: 1.15x slower                                                |
| go                       | 150 ms                                                       | 178 ms: 1.19x slower                                                 |
| mako                     | 10.0 ms                                                      | 11.9 ms: 1.19x slower                                                |
| fannkuch                 | 350 ms                                                       | 418 ms: 1.19x slower                                                 |
| telco                    | 6.96 ms                                                      | 8.37 ms: 1.20x slower                                                |
| nbody                    | 88.0 ms                                                      | 107 ms: 1.21x slower                                                 |
| scimark_fft              | 301 ms                                                       | 368 ms: 1.22x slower                                                 |
| deltablue                | 3.24 ms                                                      | 3.99 ms: 1.23x slower                                                |
| pyflate                  | 439 ms                                                       | 542 ms: 1.23x slower                                                 |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 5.24 ms: 1.25x slower                                                |
| spectral_norm            | 91.6 ms                                                      | 116 ms: 1.27x slower                                                 |
| python_startup_no_site   | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                |
| scimark_sor              | 109 ms                                                       | 142 ms: 1.31x slower                                                 |
| coverage                 | 66.7 ms                                                      | 88.0 ms: 1.32x slower                                                |
| hexiom                   | 5.96 ms                                                      | 7.91 ms: 1.33x slower                                                |
| Geometric mean           | (ref)                                                        | 1.05x slower                                                         |

Benchmark hidden because not significant (12): async_tree_memoization, asyncio_websockets, async_tree_cpu_io_mixed, deepcopy, xml_etree_parse, coroutines, regex_effbot, sqlglot_parse, logging_simple, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.92x