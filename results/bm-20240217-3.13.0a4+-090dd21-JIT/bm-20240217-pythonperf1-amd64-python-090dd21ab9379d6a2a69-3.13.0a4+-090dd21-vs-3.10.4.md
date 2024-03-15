
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.74 ms: 1.22x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 84.6 ms: 1.28x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 266 ms: 1.64x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 731 ms: 1.52x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 449 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.2 ms: 1.23x faster                                                       |
| nbody          | 71.3 ms                                                     | 59.8 ms: 1.19x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 79.2 ms: 1.34x faster                                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 175 us: 1.54x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 126 us: 1.46x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.29 sec: 1.29x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.44 us: 1.08x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.7 ms: 1.05x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 64.0 ms: 1.02x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 17.4 us: 1.01x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.81 us: 1.04x slower                                                       |
| pickle               | 6.85 us                                                     | 7.47 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.4 ms: 1.01x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.58 ms: 1.37x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.0 us: 4.80x faster                                                       |
| deltablue                | 4.19 ms                                                     | 1.98 ms: 2.11x faster                                                       |
| richards_super           | 52.2 ms                                                     | 28.4 ms: 1.84x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.2 ns: 1.74x faster                                                       |
| richards                 | 42.4 ms                                                     | 25.8 ms: 1.65x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| async_tree_none          | 435 ms                                                      | 266 ms: 1.64x faster                                                        |
| raytrace                 | 273 ms                                                      | 167 ms: 1.63x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 759 us: 1.60x faster                                                        |
| generators               | 32.4 ms                                                     | 20.7 ms: 1.57x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 472 ms: 1.55x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 175 us: 1.54x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 55.9 ms: 1.54x faster                                                       |
| comprehensions           | 16.5 us                                                     | 10.8 us: 1.53x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 971 us: 1.52x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 731 ms: 1.52x faster                                                        |
| chaos                    | 61.7 ms                                                     | 41.6 ms: 1.48x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 126 us: 1.46x faster                                                        |
| go                       | 139 ms                                                      | 95.8 ms: 1.45x faster                                                       |
| scimark_sor              | 106 ms                                                      | 74.3 ms: 1.43x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 449 ms: 1.42x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 45.4 ms: 1.38x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.58 ms: 1.37x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 21.4 us: 1.35x faster                                                       |
| pyflate                  | 409 ms                                                      | 306 ms: 1.34x faster                                                        |
| regex_compile            | 106 ms                                                      | 79.2 ms: 1.34x faster                                                       |
| mypy2                    | 555 ms                                                      | 423 ms: 1.31x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.29 sec: 1.29x faster                                                      |
| tornado_http             | 108 ms                                                      | 84.6 ms: 1.28x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.49 us: 1.28x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 40.3 ms: 1.25x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 978 ms: 1.25x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 476 ms: 1.24x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| dask                     | 313 ms                                                      | 254 ms: 1.23x faster                                                        |
| sympy_sum                | 107 ms                                                      | 87.0 ms: 1.23x faster                                                       |
| float                    | 61.7 ms                                                     | 50.2 ms: 1.23x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.74 ms: 1.22x faster                                                       |
| pycparser                | 930 ms                                                      | 764 ms: 1.22x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.73 sec: 1.22x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 64.1 ms: 1.20x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.7 ms: 1.20x faster                                                       |
| nbody                    | 71.3 ms                                                     | 59.8 ms: 1.19x faster                                                       |
| sympy_str                | 194 ms                                                      | 163 ms: 1.19x faster                                                        |
| coroutines               | 16.0 ms                                                     | 13.5 ms: 1.18x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 174 ms: 1.18x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 33.9 ms: 1.18x faster                                                       |
| deepcopy                 | 255 us                                                      | 218 us: 1.17x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.91 us: 1.15x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 837 us: 1.14x faster                                                        |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 59.0 ms: 1.13x faster                                                       |
| regex_dna                | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| sympy_expand             | 314 ms                                                      | 280 ms: 1.12x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.11 ms: 1.12x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.61 sec: 1.10x faster                                                      |
| create_gc_cycles         | 800 us                                                      | 729 us: 1.10x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.44 us: 1.08x faster                                                       |
| fannkuch                 | 256 ms                                                      | 240 ms: 1.07x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.39 us: 1.06x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 91.6 ms: 1.06x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.7 ms: 1.05x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.96 us: 1.04x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 38.6 ns: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 64.0 ms: 1.02x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.4 ms: 1.02x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.4 ms: 1.01x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 74.9 ms: 1.01x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.70 ms: 1.01x faster                                                       |
| scimark_fft              | 187 ms                                                      | 186 ms: 1.01x faster                                                        |
| pickle_list              | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 17.4 us: 1.01x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| unpickle_list            | 2.71 us                                                     | 2.81 us: 1.04x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.07x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 66.7 ms: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 240 ms: 1.08x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.47 us: 1.09x slower                                                       |
| coverage                 | 39.0 ms                                                     | 45.6 ms: 1.17x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.67 ms: 1.19x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                                |

Benchmark hidden because not significant (3): json, regex_effbot, meteor_contest
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown