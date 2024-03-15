
# Results vs. 3.10.4

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 210 ms: 1.17x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.81 ms: 1.20x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.8 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 275 ms: 1.58x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 353 ms: 1.49x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 751 ms: 1.48x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 465 ms: 1.37x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                       |
| nbody          | 71.3 ms                                                     | 72.3 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 76.9 ms: 1.38x faster                                                       |
| regex_dna      | 136 ms                                                      | 118 ms: 1.15x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.63 ms: 1.63x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 185 us: 1.46x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 130 us: 1.41x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.68 us: 1.05x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.88 us: 1.05x slower                                                       |
| pickle               | 6.85 us                                                     | 7.25 us: 1.06x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.65 ms: 1.36x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 73.1 us: 4.60x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.01 ms: 2.08x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.5 ns: 1.70x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.0 ms: 1.68x faster                                                       |
| raytrace                 | 273 ms                                                      | 166 ms: 1.65x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.63 ms: 1.63x faster                                                       |
| go                       | 139 ms                                                      | 85.5 ms: 1.63x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 53.8 ms: 1.59x faster                                                       |
| async_tree_none          | 435 ms                                                      | 275 ms: 1.58x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 778 us: 1.56x faster                                                        |
| chaos                    | 61.7 ms                                                     | 39.6 ms: 1.56x faster                                                       |
| generators               | 32.4 ms                                                     | 21.3 ms: 1.52x faster                                                       |
| comprehensions           | 16.5 us                                                     | 10.9 us: 1.52x faster                                                       |
| richards                 | 42.4 ms                                                     | 28.0 ms: 1.52x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 981 us: 1.50x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.84 ms: 1.49x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 491 ms: 1.49x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 353 ms: 1.49x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 42.3 ms: 1.48x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 751 ms: 1.48x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 185 us: 1.46x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 130 us: 1.41x faster                                                        |
| pyflate                  | 409 ms                                                      | 293 ms: 1.40x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.0 ms: 1.40x faster                                                       |
| regex_compile            | 106 ms                                                      | 76.9 ms: 1.38x faster                                                       |
| scimark_sor              | 106 ms                                                      | 77.4 ms: 1.37x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 465 ms: 1.37x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.65 ms: 1.36x faster                                                       |
| mypy2                    | 555 ms                                                      | 419 ms: 1.33x faster                                                        |
| pycparser                | 930 ms                                                      | 702 ms: 1.32x faster                                                        |
| sympy_sum                | 107 ms                                                      | 83.1 ms: 1.29x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 22.6 us: 1.27x faster                                                       |
| tornado_http             | 108 ms                                                      | 85.8 ms: 1.26x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.42 sec: 1.26x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 61.8 ms: 1.25x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.4 ms: 1.23x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| dulwich_log              | 50.5 ms                                                     | 41.4 ms: 1.22x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| sympy_str                | 194 ms                                                      | 161 ms: 1.21x faster                                                        |
| dask                     | 313 ms                                                      | 259 ms: 1.21x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.81 ms: 1.20x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 33.2 ms: 1.20x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.4 ms: 1.19x faster                                                       |
| 2to3                     | 246 ms                                                      | 210 ms: 1.17x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.17x faster                                                      |
| tomli_loads              | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 512 ms: 1.16x faster                                                        |
| float                    | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                       |
| regex_dna                | 136 ms                                                      | 118 ms: 1.15x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 179 ms: 1.15x faster                                                        |
| sympy_expand             | 314 ms                                                      | 276 ms: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 226 us: 1.13x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.97 us: 1.12x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.45 ms: 1.11x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 861 us: 1.11x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 60.2 ms: 1.11x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.93 sec: 1.10x faster                                                      |
| fannkuch                 | 256 ms                                                      | 235 ms: 1.09x faster                                                        |
| scimark_fft              | 187 ms                                                      | 177 ms: 1.06x faster                                                        |
| unpack_sequence          | 39.6 ns                                                     | 37.6 ns: 1.05x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 760 us: 1.05x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.68 us: 1.05x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.46 us: 1.05x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.7 ms: 1.03x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.16 us: 1.01x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| nbody                    | 71.3 ms                                                     | 72.3 ms: 1.01x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.88 us: 1.05x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.25 us: 1.06x slower                                                       |
| async_generators         | 222 ms                                                      | 235 ms: 1.06x slower                                                        |
| pathlib                  | 75.7 ms                                                     | 81.0 ms: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                                       |
| json                     | 3.14 ms                                                     | 3.39 ms: 1.08x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 67.9 ms: 1.09x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.2 ms: 1.19x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.71 ms: 1.20x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.22x faster                                                                |

Benchmark hidden because not significant (4): python_startup, pidigits, xml_etree_iterparse, regex_v8
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown