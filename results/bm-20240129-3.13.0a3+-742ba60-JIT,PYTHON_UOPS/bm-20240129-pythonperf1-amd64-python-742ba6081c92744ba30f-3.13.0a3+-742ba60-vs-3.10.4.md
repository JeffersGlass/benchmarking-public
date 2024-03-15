
# Results vs. 3.10.4

- fork: python
- ref: 742ba6081c92744ba30f
- machine: windows-amd64
- commit hash: 742ba60
- commit date: 2024-01-29
- overall geometric mean: 1.21x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 221 ms: 1.11x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.79 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| tornado_http   | 108 ms                                                      | 87.6 ms: 1.24x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 273 ms: 1.59x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 340 ms: 1.55x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 741 ms: 1.50x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 460 ms: 1.39x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.50x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 51.0 ms: 1.21x faster                                                       |
| nbody          | 71.3 ms                                                     | 60.9 ms: 1.17x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 81.0 ms: 1.31x faster                                                       |
| regex_dna      | 136 ms                                                      | 124 ms: 1.10x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 21.9 ms: 1.42x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 173 us: 1.56x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 125 us: 1.47x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.29 sec: 1.29x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.5 ms: 1.04x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.6 ms: 1.02x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 65.9 ms: 1.01x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.87 us: 1.06x slower                                                       |
| pickle               | 6.85 us                                                     | 7.28 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.3 ms: 1.04x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.13x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.82 ms: 1.32x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.9 us: 4.81x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.09 ms: 2.00x faster                                                       |
| richards_super           | 52.2 ms                                                     | 28.1 ms: 1.86x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 53.5 ns: 1.77x faster                                                       |
| richards                 | 42.4 ms                                                     | 25.1 ms: 1.69x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| raytrace                 | 273 ms                                                      | 168 ms: 1.63x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 750 us: 1.62x faster                                                        |
| async_tree_none          | 435 ms                                                      | 273 ms: 1.59x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 54.1 ms: 1.58x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 173 us: 1.56x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 340 ms: 1.55x faster                                                        |
| generators               | 32.4 ms                                                     | 21.1 ms: 1.54x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 976 us: 1.51x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 741 ms: 1.50x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 492 ms: 1.49x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 125 us: 1.47x faster                                                        |
| chaos                    | 61.7 ms                                                     | 42.4 ms: 1.45x faster                                                       |
| comprehensions           | 16.5 us                                                     | 11.4 us: 1.45x faster                                                       |
| go                       | 139 ms                                                      | 96.0 ms: 1.45x faster                                                       |
| scimark_sor              | 106 ms                                                      | 74.7 ms: 1.42x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 460 ms: 1.39x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 21.4 us: 1.34x faster                                                       |
| pycparser                | 930 ms                                                      | 695 ms: 1.34x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 46.9 ms: 1.33x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.82 ms: 1.32x faster                                                       |
| pyflate                  | 409 ms                                                      | 312 ms: 1.31x faster                                                        |
| regex_compile            | 106 ms                                                      | 81.0 ms: 1.31x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.29 sec: 1.29x faster                                                      |
| mypy2                    | 555 ms                                                      | 432 ms: 1.28x faster                                                        |
| coroutines               | 16.0 ms                                                     | 12.9 ms: 1.24x faster                                                       |
| tornado_http             | 108 ms                                                      | 87.6 ms: 1.24x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.23x faster                                                       |
| float                    | 61.7 ms                                                     | 51.0 ms: 1.21x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.79 ms: 1.21x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| sympy_sum                | 107 ms                                                      | 88.8 ms: 1.20x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.02 sec: 1.19x faster                                                      |
| sympy_str                | 194 ms                                                      | 164 ms: 1.19x faster                                                        |
| dask                     | 313 ms                                                      | 263 ms: 1.19x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 173 ms: 1.18x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 500 ms: 1.18x faster                                                        |
| deepcopy                 | 255 us                                                      | 217 us: 1.18x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 65.8 ms: 1.17x faster                                                       |
| nbody                    | 71.3 ms                                                     | 60.9 ms: 1.17x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.1 ms: 1.17x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 821 us: 1.17x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 43.3 ms: 1.17x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 1.89 us: 1.16x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.55 sec: 1.15x faster                                                      |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.87 sec: 1.13x faster                                                      |
| nqueens                  | 66.6 ms                                                     | 59.0 ms: 1.13x faster                                                       |
| sympy_expand             | 314 ms                                                      | 279 ms: 1.13x faster                                                        |
| 2to3                     | 246 ms                                                      | 221 ms: 1.11x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.18 ms: 1.11x faster                                                       |
| regex_dna                | 136 ms                                                      | 124 ms: 1.10x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 742 us: 1.08x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.40 us: 1.06x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.89 us: 1.06x faster                                                       |
| fannkuch                 | 256 ms                                                      | 246 ms: 1.04x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 53.5 ms: 1.04x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.6 ms: 1.02x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pickle_list              | 2.75 us                                                     | 2.77 us: 1.01x slower                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.76 ms: 1.01x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 65.9 ms: 1.01x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| unpack_sequence          | 39.6 ns                                                     | 40.7 ns: 1.03x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 78.0 ms: 1.03x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 17.7 us: 1.03x slower                                                       |
| scimark_fft              | 187 ms                                                      | 193 ms: 1.03x slower                                                        |
| python_startup           | 20.6 ms                                                     | 21.3 ms: 1.04x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.87 us: 1.06x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.28 us: 1.06x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 81.7 ms: 1.08x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.09x slower                                                       |
| async_generators         | 222 ms                                                      | 244 ms: 1.10x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 69.1 ms: 1.11x slower                                                       |
| coverage                 | 39.0 ms                                                     | 45.5 ms: 1.17x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.67 ms: 1.18x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                                       |
| regex_v8                 | 15.4 ms                                                     | 21.9 ms: 1.42x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.21x faster                                                                |

Benchmark hidden because not significant (2): json, scimark_monte_carlo
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-742ba60-JIT,PYTHON_UOPS/bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown