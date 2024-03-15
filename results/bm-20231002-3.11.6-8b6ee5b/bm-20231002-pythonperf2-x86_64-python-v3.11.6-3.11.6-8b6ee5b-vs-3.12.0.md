
# Results vs. 3.12.0

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| chameleon      | 7.23 ms                                                      | 7.64 ms: 1.06x slower                                        |
| docutils       | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                       |
| tornado_http   | 121 ms                                                       | 123 ms: 1.01x slower                                         |
| Geometric mean | (ref)                                                        | 1.01x slower                                                 |

Benchmark hidden because not significant (1): 2to3

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 696 ms                                                       | 751 ms: 1.08x slower                                         |
| async_tree_io           | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| async_tree_memoization  | 544 ms                                                       | 622 ms: 1.14x slower                                         |
| async_tree_none         | 452 ms                                                       | 519 ms: 1.15x slower                                         |
| Geometric mean          | (ref)                                                        | 1.12x slower                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pidigits       | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| nbody          | 88.0 ms                                                      | 96.9 ms: 1.10x slower                                        |
| Geometric mean | (ref)                                                        | 1.04x slower                                                 |

Benchmark hidden because not significant (1): float

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.29 ms: 1.09x faster                                        |
| regex_dna      | 239 ms                                                       | 220 ms: 1.09x faster                                         |
| regex_v8       | 23.6 ms                                                      | 23.2 ms: 1.02x faster                                        |
| regex_compile  | 144 ms                                                       | 157 ms: 1.09x slower                                         |
| Geometric mean | (ref)                                                        | 1.03x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_list          | 4.43 us                                                      | 3.77 us: 1.17x faster                                        |
| unpickle             | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| xml_etree_generate   | 86.1 ms                                                      | 79.8 ms: 1.08x faster                                        |
| pickle               | 10.5 us                                                      | 9.99 us: 1.05x faster                                        |
| xml_etree_process    | 58.4 ms                                                      | 55.8 ms: 1.05x faster                                        |
| pickle_dict          | 32.5 us                                                      | 32.1 us: 1.02x faster                                        |
| pickle_pure_python   | 318 us                                                       | 315 us: 1.01x faster                                         |
| unpickle_list        | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| json_loads           | 24.4 us                                                      | 24.6 us: 1.01x slower                                        |
| xml_etree_iterparse  | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| tomli_loads          | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| xml_etree_parse      | 144 ms                                                       | 159 ms: 1.11x slower                                         |
| unpickle_pure_python | 210 us                                                       | 239 us: 1.14x slower                                         |
| json_dumps           | 10.2 ms                                                      | 13.3 ms: 1.30x slower                                        |
| Geometric mean       | (ref)                                                        | 1.01x slower                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup_no_site | 8.64 ms                                                      | 7.81 ms: 1.11x faster                                        |
| python_startup         | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                        |
| Geometric mean         | (ref)                                                        | 1.09x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 38.2 ms                                                      | 40.5 ms: 1.06x slower                                        |
| mako            | 10.0 ms                                                      | 10.8 ms: 1.08x slower                                        |
| Geometric mean  | (ref)                                                        | 1.07x slower                                                 |

All benchmarks:
===============

| Benchmark                | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------------:|:------------------------------------------------------------:|
| async_generators         | 390 ms                                                       | 316 ms: 1.24x faster                                         |
| pickle_list              | 4.43 us                                                      | 3.77 us: 1.17x faster                                        |
| unpack_sequence          | 53.2 ns                                                      | 45.6 ns: 1.17x faster                                        |
| unpickle                 | 14.8 us                                                      | 13.3 us: 1.11x faster                                        |
| sqlite_synth             | 2.77 us                                                      | 2.50 us: 1.11x faster                                        |
| python_startup_no_site   | 8.64 ms                                                      | 7.81 ms: 1.11x faster                                        |
| regex_effbot             | 3.57 ms                                                      | 3.29 ms: 1.09x faster                                        |
| regex_dna                | 239 ms                                                       | 220 ms: 1.09x faster                                         |
| xml_etree_generate       | 86.1 ms                                                      | 79.8 ms: 1.08x faster                                        |
| python_startup           | 11.6 ms                                                      | 10.8 ms: 1.08x faster                                        |
| pickle                   | 10.5 us                                                      | 9.99 us: 1.05x faster                                        |
| scimark_fft              | 301 ms                                                       | 286 ms: 1.05x faster                                         |
| xml_etree_process        | 58.4 ms                                                      | 55.8 ms: 1.05x faster                                        |
| pprint_safe_repr         | 807 ms                                                       | 775 ms: 1.04x faster                                         |
| aiohttp                  | 1.02 ms                                                      | 984 us: 1.03x faster                                         |
| sqlalchemy_declarative   | 159 ms                                                       | 155 ms: 1.03x faster                                         |
| pprint_pformat           | 1.65 sec                                                     | 1.61 sec: 1.03x faster                                       |
| scimark_sparse_mat_mult  | 4.21 ms                                                      | 4.11 ms: 1.02x faster                                        |
| telco                    | 6.96 ms                                                      | 6.80 ms: 1.02x faster                                        |
| gunicorn                 | 1.00 ms                                                      | 977 us: 1.02x faster                                         |
| regex_v8                 | 23.6 ms                                                      | 23.2 ms: 1.02x faster                                        |
| pickle_dict              | 32.5 us                                                      | 32.1 us: 1.02x faster                                        |
| docutils                 | 2.87 sec                                                     | 2.83 sec: 1.01x faster                                       |
| pickle_pure_python       | 318 us                                                       | 315 us: 1.01x faster                                         |
| scimark_monte_carlo      | 69.0 ms                                                      | 68.3 ms: 1.01x faster                                        |
| deepcopy_reduce          | 3.37 us                                                      | 3.39 us: 1.01x slower                                        |
| unpickle_list            | 4.66 us                                                      | 4.69 us: 1.01x slower                                        |
| pyflate                  | 439 ms                                                       | 442 ms: 1.01x slower                                         |
| json_loads               | 24.4 us                                                      | 24.6 us: 1.01x slower                                        |
| raytrace                 | 298 ms                                                       | 301 ms: 1.01x slower                                         |
| pidigits                 | 265 ms                                                       | 268 ms: 1.01x slower                                         |
| tornado_http             | 121 ms                                                       | 123 ms: 1.01x slower                                         |
| pathlib                  | 18.9 ms                                                      | 19.2 ms: 1.02x slower                                        |
| deepcopy_memo            | 36.8 us                                                      | 37.5 us: 1.02x slower                                        |
| sqlglot_optimize         | 57.5 ms                                                      | 58.6 ms: 1.02x slower                                        |
| json                     | 5.12 ms                                                      | 5.23 ms: 1.02x slower                                        |
| xml_etree_iterparse      | 103 ms                                                       | 105 ms: 1.02x slower                                         |
| logging_format           | 7.48 us                                                      | 7.66 us: 1.02x slower                                        |
| crypto_pyaes             | 80.3 ms                                                      | 82.4 ms: 1.03x slower                                        |
| scimark_sor              | 109 ms                                                       | 112 ms: 1.03x slower                                         |
| pycparser                | 1.23 sec                                                     | 1.28 sec: 1.03x slower                                       |
| logging_simple           | 6.71 us                                                      | 6.96 us: 1.04x slower                                        |
| dask                     | 392 ms                                                       | 407 ms: 1.04x slower                                         |
| deepcopy                 | 368 us                                                       | 383 us: 1.04x slower                                         |
| sqlglot_normalize        | 116 ms                                                       | 121 ms: 1.05x slower                                         |
| sqlalchemy_imperative    | 18.7 ms                                                      | 19.7 ms: 1.05x slower                                        |
| bench_thread_pool        | 950 us                                                       | 1.00 ms: 1.05x slower                                        |
| tomli_loads              | 2.16 sec                                                     | 2.28 sec: 1.06x slower                                       |
| chameleon                | 7.23 ms                                                      | 7.64 ms: 1.06x slower                                        |
| django_template          | 38.2 ms                                                      | 40.5 ms: 1.06x slower                                        |
| spectral_norm            | 91.6 ms                                                      | 97.3 ms: 1.06x slower                                        |
| logging_silent           | 94.4 ns                                                      | 101 ns: 1.07x slower                                         |
| sqlglot_transpile        | 1.78 ms                                                      | 1.91 ms: 1.08x slower                                        |
| async_tree_cpu_io_mixed  | 696 ms                                                       | 751 ms: 1.08x slower                                         |
| mako                     | 10.0 ms                                                      | 10.8 ms: 1.08x slower                                        |
| go                       | 150 ms                                                       | 162 ms: 1.08x slower                                         |
| sympy_integrate          | 23.9 ms                                                      | 25.9 ms: 1.08x slower                                        |
| richards                 | 45.7 ms                                                      | 49.6 ms: 1.08x slower                                        |
| regex_compile            | 144 ms                                                       | 157 ms: 1.09x slower                                         |
| nbody                    | 88.0 ms                                                      | 96.9 ms: 1.10x slower                                        |
| xml_etree_parse          | 144 ms                                                       | 159 ms: 1.11x slower                                         |
| sympy_str                | 302 ms                                                       | 335 ms: 1.11x slower                                         |
| mdp                      | 2.57 sec                                                     | 2.86 sec: 1.11x slower                                       |
| sqlglot_parse            | 1.38 ms                                                      | 1.53 ms: 1.11x slower                                        |
| async_tree_io            | 1.04 sec                                                     | 1.17 sec: 1.12x slower                                       |
| nqueens                  | 89.9 ms                                                      | 101 ms: 1.13x slower                                         |
| comprehensions           | 21.9 us                                                      | 24.8 us: 1.13x slower                                        |
| sympy_expand             | 484 ms                                                       | 550 ms: 1.14x slower                                         |
| sympy_sum                | 162 ms                                                       | 184 ms: 1.14x slower                                         |
| unpickle_pure_python     | 210 us                                                       | 239 us: 1.14x slower                                         |
| gc_traversal             | 3.48 ms                                                      | 3.97 ms: 1.14x slower                                        |
| async_tree_memoization   | 544 ms                                                       | 622 ms: 1.14x slower                                         |
| chaos                    | 64.0 ms                                                      | 73.4 ms: 1.15x slower                                        |
| async_tree_none          | 452 ms                                                       | 519 ms: 1.15x slower                                         |
| scimark_lu               | 98.8 ms                                                      | 114 ms: 1.15x slower                                         |
| hexiom                   | 5.96 ms                                                      | 6.97 ms: 1.17x slower                                        |
| coroutines               | 23.0 ms                                                      | 27.9 ms: 1.21x slower                                        |
| deltablue                | 3.24 ms                                                      | 3.97 ms: 1.23x slower                                        |
| richards_super           | 51.3 ms                                                      | 63.6 ms: 1.24x slower                                        |
| fannkuch                 | 350 ms                                                       | 437 ms: 1.25x slower                                         |
| json_dumps               | 10.2 ms                                                      | 13.3 ms: 1.30x slower                                        |
| generators               | 37.4 ms                                                      | 54.3 ms: 1.45x slower                                        |
| asyncio_tcp_ssl          | 1.59 sec                                                     | 3.09 sec: 1.94x slower                                       |
| asyncio_tcp              | 378 ms                                                       | 747 ms: 1.98x slower                                         |
| typing_runtime_protocols | 152 us                                                       | 519 us: 3.42x slower                                         |
| Geometric mean           | (ref)                                                        | 1.07x slower                                                 |

Benchmark hidden because not significant (6): float, meteor_contest, dulwich_log, 2to3, bench_mp_pool, create_gc_cycles
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (6) of results/bm-20231002-3.11.6-8b6ee5b/bm-20231002-pythonperf2-x86_64-python-v3.11.6-3.11.6-8b6ee5b.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.91x