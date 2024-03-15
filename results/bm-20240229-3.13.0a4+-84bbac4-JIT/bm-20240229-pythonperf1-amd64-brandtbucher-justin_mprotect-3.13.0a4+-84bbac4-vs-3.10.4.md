# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_mprotect
- machine: windows-amd64
- commit hash: 84bbac4
- commit date: 2024-02-29
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                         |
| chameleon      | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                                        |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                       |
| tornado_http   | 108 ms                                                      | 85.0 ms: 1.27x faster                                                        |
| Geometric mean | (ref)                                                       | 1.20x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 267 ms: 1.63x faster                                                         |
| async_tree_memoization  | 526 ms                                                      | 341 ms: 1.54x faster                                                         |
| async_tree_io           | 1.11 sec                                                    | 725 ms: 1.53x faster                                                         |
| async_tree_cpu_io_mixed | 638 ms                                                      | 450 ms: 1.42x faster                                                         |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.1 ms: 1.26x faster                                                        |
| nbody          | 71.3 ms                                                     | 57.7 ms: 1.24x faster                                                        |
| pidigits       | 149 ms                                                      | 150 ms: 1.00x slower                                                         |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.2 ms: 1.29x faster                                                        |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                                         |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.01x faster                                                        |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.52 ms: 1.66x faster                                                        |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                         |
| unpickle_pure_python | 183 us                                                      | 127 us: 1.44x faster                                                         |
| tomli_loads          | 1.67 sec                                                    | 1.19 sec: 1.41x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 35.8 ms: 1.24x faster                                                        |
| xml_etree_generate   | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                                        |
| unpickle             | 9.09 us                                                     | 8.68 us: 1.05x faster                                                        |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.1 ms: 1.05x faster                                                        |
| xml_etree_parse      | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                        |
| pickle_dict          | 17.2 us                                                     | 17.3 us: 1.01x slower                                                        |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                                        |
| pickle               | 6.85 us                                                     | 7.16 us: 1.05x slower                                                        |
| pickle_list          | 2.75 us                                                     | 2.90 us: 1.05x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.15x faster                                                                 |

Benchmark hidden because not significant (1): json_loads

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.8 ms: 1.16x slower                                                        |
| python_startup_no_site | 15.5 ms                                                     | 21.5 ms: 1.39x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.27x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 5.66 ms: 1.59x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4 |
|--------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.4 us: 4.77x faster                                                        |
| deltablue                | 4.19 ms                                                     | 2.13 ms: 1.96x faster                                                        |
| logging_silent           | 94.6 ns                                                     | 55.8 ns: 1.69x faster                                                        |
| richards_super           | 52.2 ms                                                     | 31.2 ms: 1.67x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.52 ms: 1.66x faster                                                        |
| async_tree_none          | 435 ms                                                      | 267 ms: 1.63x faster                                                         |
| mako                     | 9.03 ms                                                     | 5.66 ms: 1.59x faster                                                        |
| generators               | 32.4 ms                                                     | 20.4 ms: 1.59x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 774 us: 1.57x faster                                                         |
| comprehensions           | 16.5 us                                                     | 10.6 us: 1.56x faster                                                        |
| chaos                    | 61.7 ms                                                     | 39.6 ms: 1.56x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 471 ms: 1.56x faster                                                         |
| async_tree_memoization   | 526 ms                                                      | 341 ms: 1.54x faster                                                         |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                                         |
| async_tree_io            | 1.11 sec                                                    | 725 ms: 1.53x faster                                                         |
| richards                 | 42.4 ms                                                     | 27.8 ms: 1.53x faster                                                        |
| raytrace                 | 273 ms                                                      | 180 ms: 1.51x faster                                                         |
| spectral_norm            | 77.3 ms                                                     | 51.0 ms: 1.51x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 994 us: 1.48x faster                                                         |
| crypto_pyaes             | 62.5 ms                                                     | 42.7 ms: 1.46x faster                                                        |
| pyflate                  | 409 ms                                                      | 283 ms: 1.45x faster                                                         |
| unpickle_pure_python     | 183 us                                                      | 127 us: 1.44x faster                                                         |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 450 ms: 1.42x faster                                                         |
| go                       | 139 ms                                                      | 98.4 ms: 1.41x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.19 sec: 1.41x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.7 ms: 1.37x faster                                                        |
| scimark_sor              | 106 ms                                                      | 80.6 ms: 1.32x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 4.37 ms: 1.31x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 21.9 us: 1.31x faster                                                        |
| regex_compile            | 106 ms                                                      | 82.2 ms: 1.29x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.38 sec: 1.29x faster                                                       |
| tornado_http             | 108 ms                                                      | 85.0 ms: 1.27x faster                                                        |
| mypy2                    | 555 ms                                                      | 438 ms: 1.27x faster                                                         |
| pprint_pformat           | 1.22 sec                                                    | 962 ms: 1.27x faster                                                         |
| pprint_safe_repr         | 592 ms                                                      | 468 ms: 1.26x faster                                                         |
| pycparser                | 930 ms                                                      | 739 ms: 1.26x faster                                                         |
| float                    | 61.7 ms                                                     | 49.1 ms: 1.26x faster                                                        |
| sympy_sum                | 107 ms                                                      | 86.0 ms: 1.24x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 35.8 ms: 1.24x faster                                                        |
| nbody                    | 71.3 ms                                                     | 57.7 ms: 1.24x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 41.1 ms: 1.23x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 70.4 ms: 1.22x faster                                                        |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                        |
| chameleon                | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                                        |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                       |
| sympy_str                | 194 ms                                                      | 162 ms: 1.20x faster                                                         |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.27 ms: 1.20x faster                                                        |
| coroutines               | 16.0 ms                                                     | 13.4 ms: 1.19x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 174 ms: 1.18x faster                                                         |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.79 sec: 1.18x faster                                                       |
| deepcopy                 | 255 us                                                      | 217 us: 1.18x faster                                                         |
| sympy_integrate          | 15.3 ms                                                     | 13.1 ms: 1.17x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 821 us: 1.17x faster                                                         |
| sqlglot_optimize         | 39.8 ms                                                     | 34.2 ms: 1.16x faster                                                        |
| fannkuch                 | 256 ms                                                      | 220 ms: 1.16x faster                                                         |
| deepcopy_reduce          | 2.20 us                                                     | 1.93 us: 1.14x faster                                                        |
| sympy_expand             | 314 ms                                                      | 275 ms: 1.14x faster                                                         |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                                         |
| scimark_fft              | 187 ms                                                      | 169 ms: 1.11x faster                                                         |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                         |
| nqueens                  | 66.6 ms                                                     | 61.4 ms: 1.09x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.28 us: 1.08x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 748 us: 1.07x faster                                                         |
| logging_simple           | 6.22 us                                                     | 5.88 us: 1.06x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                                        |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.68 us: 1.05x faster                                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.1 ms: 1.05x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                        |
| meteor_contest           | 75.9 ms                                                     | 73.4 ms: 1.04x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 15.2 ms: 1.01x faster                                                        |
| pathlib                  | 75.7 ms                                                     | 75.0 ms: 1.01x faster                                                        |
| pidigits                 | 149 ms                                                      | 150 ms: 1.00x slower                                                         |
| pickle_dict              | 17.2 us                                                     | 17.3 us: 1.01x slower                                                        |
| unpickle_list            | 2.71 us                                                     | 2.79 us: 1.03x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.16 us: 1.05x slower                                                        |
| pickle_list              | 2.75 us                                                     | 2.90 us: 1.05x slower                                                        |
| gc_traversal             | 1.41 ms                                                     | 1.53 ms: 1.08x slower                                                        |
| async_generators         | 222 ms                                                      | 240 ms: 1.08x slower                                                         |
| bench_mp_pool            | 62.0 ms                                                     | 69.8 ms: 1.12x slower                                                        |
| dask                     | 313 ms                                                      | 360 ms: 1.15x slower                                                         |
| python_startup           | 20.6 ms                                                     | 23.8 ms: 1.16x slower                                                        |
| unpack_sequence          | 39.6 ns                                                     | 46.6 ns: 1.17x slower                                                        |
| telco                    | 3.94 ms                                                     | 4.66 ms: 1.18x slower                                                        |
| coverage                 | 39.0 ms                                                     | 46.4 ms: 1.19x slower                                                        |
| python_startup_no_site   | 15.5 ms                                                     | 21.5 ms: 1.39x slower                                                        |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                                 |

Benchmark hidden because not significant (2): json_loads, json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-84bbac4-JIT/bm-20240229-pythonperf1-amd64-brandtbucher-justin_mprotect-3.13.0a4+-84bbac4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown