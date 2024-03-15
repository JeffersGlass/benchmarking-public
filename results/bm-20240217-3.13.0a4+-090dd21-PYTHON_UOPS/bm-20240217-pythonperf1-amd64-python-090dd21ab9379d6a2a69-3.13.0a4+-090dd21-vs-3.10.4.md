
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.19x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 220 ms: 1.12x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.12 ms: 1.13x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.20x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.4 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.18x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 270 ms: 1.61x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 346 ms: 1.52x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 458 ms: 1.39x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 58.3 ms: 1.06x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 75.6 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| regex_dna      | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 184 us: 1.46x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 140 us: 1.31x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.4 ms: 1.19x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.51 sec: 1.11x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.43 us: 1.08x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.9 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.0 ms: 1.03x faster                                                       |
| pickle               | 6.85 us                                                     | 7.10 us: 1.04x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.85 us: 1.04x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 67.4 ms: 1.04x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.86 us: 1.05x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.0 ms: 1.16x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 74.0 us: 4.54x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.15 ms: 1.95x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.0 ns: 1.69x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.0 ms: 1.68x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| async_tree_none          | 435 ms                                                      | 270 ms: 1.61x faster                                                        |
| generators               | 32.4 ms                                                     | 20.3 ms: 1.59x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 465 ms: 1.57x faster                                                        |
| raytrace                 | 273 ms                                                      | 174 ms: 1.57x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.3 ms: 1.55x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 790 us: 1.54x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 346 ms: 1.52x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 56.9 ms: 1.51x faster                                                       |
| go                       | 139 ms                                                      | 93.7 ms: 1.48x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 184 us: 1.46x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 458 ms: 1.39x faster                                                        |
| chaos                    | 61.7 ms                                                     | 44.5 ms: 1.39x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 47.5 ms: 1.32x faster                                                       |
| comprehensions           | 16.5 us                                                     | 12.5 us: 1.32x faster                                                       |
| mypy2                    | 555 ms                                                      | 424 ms: 1.31x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 140 us: 1.31x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.64 sec: 1.29x faster                                                      |
| tornado_http             | 108 ms                                                      | 85.4 ms: 1.27x faster                                                       |
| scimark_sor              | 106 ms                                                      | 83.8 ms: 1.27x faster                                                       |
| regex_compile            | 106 ms                                                      | 84.8 ms: 1.25x faster                                                       |
| pyflate                  | 409 ms                                                      | 328 ms: 1.25x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 23.2 us: 1.24x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 41.5 ms: 1.22x faster                                                       |
| dask                     | 313 ms                                                      | 257 ms: 1.22x faster                                                        |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                       |
| sympy_sum                | 107 ms                                                      | 88.4 ms: 1.21x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.47 sec: 1.21x faster                                                      |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.20x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 37.4 ms: 1.19x faster                                                       |
| mako                     | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.0 ms: 1.18x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 49.4 ms: 1.16x faster                                                       |
| sympy_str                | 194 ms                                                      | 168 ms: 1.16x faster                                                        |
| regex_dna                | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.00 ms: 1.15x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.8 ms: 1.14x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 843 us: 1.14x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.08 sec: 1.13x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 523 ms: 1.13x faster                                                        |
| chameleon                | 5.79 ms                                                     | 5.12 ms: 1.13x faster                                                       |
| pycparser                | 930 ms                                                      | 823 ms: 1.13x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 182 ms: 1.13x faster                                                        |
| 2to3                     | 246 ms                                                      | 220 ms: 1.12x faster                                                        |
| deepcopy                 | 255 us                                                      | 231 us: 1.11x faster                                                        |
| sympy_expand             | 314 ms                                                      | 284 ms: 1.11x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.51 sec: 1.11x faster                                                      |
| deepcopy_reduce          | 2.20 us                                                     | 1.99 us: 1.11x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 738 us: 1.08x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.43 us: 1.08x faster                                                       |
| float                    | 61.7 ms                                                     | 58.3 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 37.9 ns: 1.05x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.9 ms: 1.04x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 64.4 ms: 1.03x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.0 ms: 1.03x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| logging_simple           | 6.22 us                                                     | 6.29 us: 1.01x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.10 us: 1.04x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.85 us: 1.04x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 67.4 ms: 1.04x slower                                                       |
| fannkuch                 | 256 ms                                                      | 266 ms: 1.04x slower                                                        |
| async_generators         | 222 ms                                                      | 231 ms: 1.04x slower                                                        |
| spectral_norm            | 77.3 ms                                                     | 81.0 ms: 1.05x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 65.1 ms: 1.05x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.86 us: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.05x slower                                                       |
| nbody                    | 71.3 ms                                                     | 75.6 ms: 1.06x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.06x slower                                                       |
| scimark_fft              | 187 ms                                                      | 205 ms: 1.10x slower                                                        |
| python_startup_no_site   | 15.5 ms                                                     | 18.0 ms: 1.16x slower                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.22 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.0 ms: 1.21x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.87 ms: 1.24x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                                |

Benchmark hidden because not significant (4): json, logging_format, pathlib, meteor_contest
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown