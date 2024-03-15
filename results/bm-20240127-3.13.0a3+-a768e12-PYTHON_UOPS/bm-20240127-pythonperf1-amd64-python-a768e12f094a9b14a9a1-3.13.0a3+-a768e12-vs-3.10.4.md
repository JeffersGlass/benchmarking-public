
# Results vs. 3.10.4

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 222 ms: 1.11x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.01 ms: 1.16x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.8 ms: 1.25x faster                                                       |
| Geometric mean | (ref)                                                       | 1.18x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 278 ms: 1.57x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 354 ms: 1.49x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 750 ms: 1.48x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 457 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.00x slower                                                        |
| nbody          | 71.3 ms                                                     | 83.1 ms: 1.17x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 85.2 ms: 1.24x faster                                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.12x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 182 us: 1.48x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 137 us: 1.34x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.52 us: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 56.2 ms: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 68.0 ms: 1.05x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.85 us: 1.05x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.89 us: 1.05x slower                                                       |
| pickle               | 6.85 us                                                     | 7.20 us: 1.05x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.8 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.38 ms: 1.22x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 75.6 us: 4.44x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.1 ns: 1.75x faster                                                       |
| richards_super           | 52.2 ms                                                     | 30.4 ms: 1.72x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.59 ms: 1.62x faster                                                       |
| raytrace                 | 273 ms                                                      | 170 ms: 1.60x faster                                                        |
| richards                 | 42.4 ms                                                     | 26.8 ms: 1.58x faster                                                       |
| async_tree_none          | 435 ms                                                      | 278 ms: 1.57x faster                                                        |
| generators               | 32.4 ms                                                     | 21.0 ms: 1.54x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 789 us: 1.54x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 478 ms: 1.53x faster                                                        |
| go                       | 139 ms                                                      | 91.5 ms: 1.52x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 354 ms: 1.49x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 182 us: 1.48x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 750 ms: 1.48x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 58.8 ms: 1.46x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.45x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 457 ms: 1.40x faster                                                        |
| chaos                    | 61.7 ms                                                     | 44.4 ms: 1.39x faster                                                       |
| scimark_sor              | 106 ms                                                      | 78.7 ms: 1.35x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 137 us: 1.34x faster                                                        |
| pycparser                | 930 ms                                                      | 710 ms: 1.31x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.6 ms: 1.29x faster                                                       |
| mypy2                    | 555 ms                                                      | 432 ms: 1.28x faster                                                        |
| comprehensions           | 16.5 us                                                     | 13.0 us: 1.27x faster                                                       |
| pyflate                  | 409 ms                                                      | 325 ms: 1.26x faster                                                        |
| tornado_http             | 108 ms                                                      | 86.8 ms: 1.25x faster                                                       |
| regex_compile            | 106 ms                                                      | 85.2 ms: 1.24x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 23.4 us: 1.23x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.22x faster                                                       |
| mako                     | 9.03 ms                                                     | 7.38 ms: 1.22x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.7 ms: 1.20x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 4.80 ms: 1.20x faster                                                       |
| sympy_sum                | 107 ms                                                      | 89.6 ms: 1.19x faster                                                       |
| dask                     | 313 ms                                                      | 263 ms: 1.19x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| mdp                      | 1.78 sec                                                    | 1.53 sec: 1.17x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 43.7 ms: 1.16x faster                                                       |
| chameleon                | 5.79 ms                                                     | 5.01 ms: 1.16x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                       |
| sympy_str                | 194 ms                                                      | 170 ms: 1.14x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.86 sec: 1.14x faster                                                      |
| regex_dna                | 136 ms                                                      | 121 ms: 1.12x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 528 ms: 1.12x faster                                                        |
| deepcopy                 | 255 us                                                      | 229 us: 1.12x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 35.7 ms: 1.12x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.11x faster                                                      |
| 2to3                     | 246 ms                                                      | 222 ms: 1.11x faster                                                        |
| sympy_expand             | 314 ms                                                      | 284 ms: 1.11x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.01 us: 1.09x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 189 ms: 1.08x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 888 us: 1.08x faster                                                        |
| float                    | 61.7 ms                                                     | 57.2 ms: 1.08x faster                                                       |
| json                     | 3.14 ms                                                     | 2.93 ms: 1.07x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.52 us: 1.07x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 750 us: 1.07x faster                                                        |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 63.5 ms: 1.05x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.8 ms: 1.05x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.7 ms: 1.05x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.03x faster                                                       |
| pidigits                 | 149 ms                                                      | 150 ms: 1.00x slower                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 56.2 ms: 1.01x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 77.5 ms: 1.02x slower                                                       |
| fannkuch                 | 256 ms                                                      | 266 ms: 1.04x slower                                                        |
| async_generators         | 222 ms                                                      | 231 ms: 1.04x slower                                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 68.0 ms: 1.05x slower                                                       |
| spectral_norm            | 77.3 ms                                                     | 80.9 ms: 1.05x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.85 us: 1.05x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.89 us: 1.05x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.20 us: 1.05x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 80.2 ms: 1.06x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 42.1 ns: 1.06x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.8 us: 1.09x slower                                                       |
| scimark_fft              | 187 ms                                                      | 205 ms: 1.10x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 68.4 ms: 1.10x slower                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.07 ms: 1.13x slower                                                       |
| nbody                    | 71.3 ms                                                     | 83.1 ms: 1.17x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.3 ms: 1.19x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.75 ms: 1.20x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                |

Benchmark hidden because not significant (3): logging_format, logging_simple, python_startup
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown