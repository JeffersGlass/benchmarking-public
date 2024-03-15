
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin
- machine: windows-amd64
- commit hash: 4d3e207
- commit date: 2024-01-25
- overall geometric mean: 1.20x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 220 ms: 1.12x faster                                                |
| chameleon      | 5.79 ms                                                     | 4.91 ms: 1.18x faster                                               |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                              |
| tornado_http   | 108 ms                                                      | 86.0 ms: 1.26x faster                                               |
| Geometric mean | (ref)                                                       | 1.19x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 273 ms: 1.59x faster                                                |
| async_tree_memoization  | 526 ms                                                      | 346 ms: 1.52x faster                                                |
| async_tree_io           | 1.11 sec                                                    | 730 ms: 1.52x faster                                                |
| async_tree_cpu_io_mixed | 638 ms                                                      | 459 ms: 1.39x faster                                                |
| Geometric mean          | (ref)                                                       | 1.50x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.4 ms: 1.22x faster                                               |
| nbody          | 71.3 ms                                                     | 60.8 ms: 1.17x faster                                               |
| pidigits       | 149 ms                                                      | 154 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                       | 1.12x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.3 ms: 1.29x faster                                               |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                               |
| regex_v8       | 15.4 ms                                                     | 16.9 ms: 1.10x slower                                               |
| Geometric mean | (ref)                                                       | 1.09x faster                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                               |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                |
| unpickle_pure_python | 183 us                                                      | 131 us: 1.40x faster                                                |
| tomli_loads          | 1.67 sec                                                    | 1.35 sec: 1.24x faster                                              |
| xml_etree_process    | 44.5 ms                                                     | 36.6 ms: 1.22x faster                                               |
| xml_etree_generate   | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                               |
| unpickle             | 9.09 us                                                     | 8.61 us: 1.06x faster                                               |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                               |
| xml_etree_parse      | 96.8 ms                                                     | 94.6 ms: 1.02x faster                                               |
| unpickle_list        | 2.71 us                                                     | 2.75 us: 1.01x slower                                               |
| pickle               | 6.85 us                                                     | 7.35 us: 1.07x slower                                               |
| pickle_list          | 2.75 us                                                     | 2.96 us: 1.08x slower                                               |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                               |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                        |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.0 ms: 1.02x slower                                               |
| python_startup_no_site | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                               |
| Geometric mean         | (ref)                                                       | 1.12x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.98 ms: 1.29x faster                                               |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207 |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.1 us: 4.66x faster                                               |
| deltablue                | 4.19 ms                                                     | 2.08 ms: 2.02x faster                                               |
| richards_super           | 52.2 ms                                                     | 28.8 ms: 1.82x faster                                               |
| logging_silent           | 94.6 ns                                                     | 54.5 ns: 1.74x faster                                               |
| richards                 | 42.4 ms                                                     | 25.5 ms: 1.66x faster                                               |
| json_dumps               | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                               |
| generators               | 32.4 ms                                                     | 20.1 ms: 1.61x faster                                               |
| async_tree_none          | 435 ms                                                      | 273 ms: 1.59x faster                                                |
| raytrace                 | 273 ms                                                      | 175 ms: 1.56x faster                                                |
| sqlglot_parse            | 1.22 ms                                                     | 784 us: 1.55x faster                                                |
| scimark_lu               | 85.8 ms                                                     | 55.9 ms: 1.54x faster                                               |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                |
| async_tree_memoization   | 526 ms                                                      | 346 ms: 1.52x faster                                                |
| async_tree_io            | 1.11 sec                                                    | 730 ms: 1.52x faster                                                |
| asyncio_tcp              | 732 ms                                                      | 487 ms: 1.50x faster                                                |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                               |
| comprehensions           | 16.5 us                                                     | 11.4 us: 1.44x faster                                               |
| go                       | 139 ms                                                      | 97.4 ms: 1.43x faster                                               |
| chaos                    | 61.7 ms                                                     | 43.7 ms: 1.41x faster                                               |
| unpickle_pure_python     | 183 us                                                      | 131 us: 1.40x faster                                                |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 459 ms: 1.39x faster                                                |
| scimark_sor              | 106 ms                                                      | 78.7 ms: 1.35x faster                                               |
| crypto_pyaes             | 62.5 ms                                                     | 47.2 ms: 1.33x faster                                               |
| pycparser                | 930 ms                                                      | 705 ms: 1.32x faster                                                |
| deepcopy_memo            | 28.8 us                                                     | 22.1 us: 1.30x faster                                               |
| mako                     | 9.03 ms                                                     | 6.98 ms: 1.29x faster                                               |
| regex_compile            | 106 ms                                                      | 82.3 ms: 1.29x faster                                               |
| pyflate                  | 409 ms                                                      | 320 ms: 1.28x faster                                                |
| mypy2                    | 555 ms                                                      | 436 ms: 1.28x faster                                                |
| tornado_http             | 108 ms                                                      | 86.0 ms: 1.26x faster                                               |
| tomli_loads              | 1.67 sec                                                    | 1.35 sec: 1.24x faster                                              |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                               |
| float                    | 61.7 ms                                                     | 50.4 ms: 1.22x faster                                               |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.22x faster                                               |
| xml_etree_process        | 44.5 ms                                                     | 36.6 ms: 1.22x faster                                               |
| sympy_sum                | 107 ms                                                      | 88.9 ms: 1.20x faster                                               |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                              |
| spectral_norm            | 77.3 ms                                                     | 65.3 ms: 1.18x faster                                               |
| dask                     | 313 ms                                                      | 265 ms: 1.18x faster                                                |
| chameleon                | 5.79 ms                                                     | 4.91 ms: 1.18x faster                                               |
| pprint_safe_repr         | 592 ms                                                      | 504 ms: 1.17x faster                                                |
| nbody                    | 71.3 ms                                                     | 60.8 ms: 1.17x faster                                               |
| dulwich_log              | 50.5 ms                                                     | 43.2 ms: 1.17x faster                                               |
| pprint_pformat           | 1.22 sec                                                    | 1.05 sec: 1.17x faster                                              |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.82 sec: 1.16x faster                                              |
| sympy_str                | 194 ms                                                      | 168 ms: 1.16x faster                                                |
| deepcopy                 | 255 us                                                      | 221 us: 1.16x faster                                                |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                               |
| sqlglot_optimize         | 39.8 ms                                                     | 34.7 ms: 1.15x faster                                               |
| mdp                      | 1.78 sec                                                    | 1.55 sec: 1.15x faster                                              |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                                |
| deepcopy_reduce          | 2.20 us                                                     | 1.95 us: 1.13x faster                                               |
| nqueens                  | 66.6 ms                                                     | 59.1 ms: 1.13x faster                                               |
| sympy_expand             | 314 ms                                                      | 280 ms: 1.12x faster                                                |
| 2to3                     | 246 ms                                                      | 220 ms: 1.12x faster                                                |
| bench_thread_pool        | 958 us                                                      | 861 us: 1.11x faster                                                |
| json                     | 3.14 ms                                                     | 2.88 ms: 1.09x faster                                               |
| hexiom                   | 5.74 ms                                                     | 5.29 ms: 1.09x faster                                               |
| create_gc_cycles         | 800 us                                                      | 754 us: 1.06x faster                                                |
| xml_etree_generate       | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                               |
| unpickle                 | 9.09 us                                                     | 8.61 us: 1.06x faster                                               |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                               |
| logging_format           | 6.76 us                                                     | 6.47 us: 1.04x faster                                               |
| fannkuch                 | 256 ms                                                      | 247 ms: 1.04x faster                                                |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                               |
| logging_simple           | 6.22 us                                                     | 6.03 us: 1.03x faster                                               |
| xml_etree_parse          | 96.8 ms                                                     | 94.6 ms: 1.02x faster                                               |
| unpickle_list            | 2.71 us                                                     | 2.75 us: 1.01x slower                                               |
| python_startup           | 20.6 ms                                                     | 21.0 ms: 1.02x slower                                               |
| scimark_monte_carlo      | 57.3 ms                                                     | 58.7 ms: 1.03x slower                                               |
| pidigits                 | 149 ms                                                      | 154 ms: 1.03x slower                                                |
| meteor_contest           | 75.9 ms                                                     | 78.7 ms: 1.04x slower                                               |
| scimark_fft              | 187 ms                                                      | 196 ms: 1.04x slower                                                |
| pathlib                  | 75.7 ms                                                     | 80.1 ms: 1.06x slower                                               |
| pickle                   | 6.85 us                                                     | 7.35 us: 1.07x slower                                               |
| pickle_list              | 2.75 us                                                     | 2.96 us: 1.08x slower                                               |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                               |
| async_generators         | 222 ms                                                      | 241 ms: 1.09x slower                                                |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.09x slower                                               |
| regex_v8                 | 15.4 ms                                                     | 16.9 ms: 1.10x slower                                               |
| bench_mp_pool            | 62.0 ms                                                     | 69.2 ms: 1.12x slower                                               |
| telco                    | 3.94 ms                                                     | 4.58 ms: 1.16x slower                                               |
| coverage                 | 39.0 ms                                                     | 45.7 ms: 1.17x slower                                               |
| python_startup_no_site   | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                               |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                        |

Benchmark hidden because not significant (3): xml_etree_iterparse, unpack_sequence, scimark_sparse_mat_mult
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240125-3.13.0a3+-4d3e207-JIT/bm-20240125-pythonperf1-amd64-brandtbucher-justin-3.13.0a3+-4d3e207.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown