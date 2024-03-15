
# Results vs. 3.10.4

- fork: python
- ref: 1aec0644447e69e981d5
- machine: windows-amd64
- commit hash: 1aec064
- commit date: 2024-02-01
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 219 ms: 1.12x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.89 ms: 1.18x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.62 sec: 1.18x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.9 ms: 1.25x faster                                                       |
| Geometric mean | (ref)                                                       | 1.18x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 721 ms: 1.54x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.4 ms: 1.22x faster                                                       |
| nbody          | 71.3 ms                                                     | 61.0 ms: 1.17x faster                                                       |
| pidigits       | 149 ms                                                      | 153 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 81.0 ms: 1.31x faster                                                       |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 21.8 ms: 1.41x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.48 ms: 1.67x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 179 us: 1.51x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 127 us: 1.44x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.9 ms: 1.21x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.8 ms: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.81 us: 1.03x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.82 us: 1.02x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.1 us: 1.05x slower                                                       |
| pickle               | 6.85 us                                                     | 7.48 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.9 ms: 1.01x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.9 ms: 1.22x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.79 ms: 1.33x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.9 us: 4.74x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.06 ms: 2.04x faster                                                       |
| richards_super           | 52.2 ms                                                     | 29.6 ms: 1.76x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 53.9 ns: 1.76x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.48 ms: 1.67x faster                                                       |
| richards                 | 42.4 ms                                                     | 25.9 ms: 1.64x faster                                                       |
| generators               | 32.4 ms                                                     | 19.9 ms: 1.63x faster                                                       |
| async_tree_none          | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| raytrace                 | 273 ms                                                      | 171 ms: 1.59x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 764 us: 1.59x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 721 ms: 1.54x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 179 us: 1.51x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 977 us: 1.51x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 57.2 ms: 1.50x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 499 ms: 1.47x faster                                                        |
| chaos                    | 61.7 ms                                                     | 42.6 ms: 1.45x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 127 us: 1.44x faster                                                        |
| comprehensions           | 16.5 us                                                     | 11.5 us: 1.43x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 450 ms: 1.42x faster                                                        |
| go                       | 139 ms                                                      | 99.3 ms: 1.40x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 45.3 ms: 1.38x faster                                                       |
| scimark_sor              | 106 ms                                                      | 77.9 ms: 1.36x faster                                                       |
| pycparser                | 930 ms                                                      | 695 ms: 1.34x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.79 ms: 1.33x faster                                                       |
| regex_compile            | 106 ms                                                      | 81.0 ms: 1.31x faster                                                       |
| pyflate                  | 409 ms                                                      | 315 ms: 1.30x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.30 sec: 1.28x faster                                                      |
| deepcopy_memo            | 28.8 us                                                     | 22.6 us: 1.27x faster                                                       |
| mypy2                    | 555 ms                                                      | 439 ms: 1.26x faster                                                        |
| tornado_http             | 108 ms                                                      | 86.9 ms: 1.25x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.54 us: 1.24x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| float                    | 61.7 ms                                                     | 50.4 ms: 1.22x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 36.9 ms: 1.21x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 42.6 ms: 1.19x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.62 sec: 1.18x faster                                                      |
| chameleon                | 5.79 ms                                                     | 4.89 ms: 1.18x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 501 ms: 1.18x faster                                                        |
| sympy_sum                | 107 ms                                                      | 91.0 ms: 1.18x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.18x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 65.8 ms: 1.17x faster                                                       |
| dask                     | 313 ms                                                      | 268 ms: 1.17x faster                                                        |
| nbody                    | 71.3 ms                                                     | 61.0 ms: 1.17x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 57.5 ms: 1.16x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.84 sec: 1.15x faster                                                      |
| sympy_str                | 194 ms                                                      | 169 ms: 1.15x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.4 ms: 1.14x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 35.2 ms: 1.13x faster                                                       |
| deepcopy                 | 255 us                                                      | 226 us: 1.13x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.96 us: 1.13x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 183 ms: 1.12x faster                                                        |
| 2to3                     | 246 ms                                                      | 219 ms: 1.12x faster                                                        |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                                        |
| sympy_expand             | 314 ms                                                      | 284 ms: 1.11x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 876 us: 1.09x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.27 ms: 1.09x faster                                                       |
| json                     | 3.14 ms                                                     | 2.89 ms: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 742 us: 1.08x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.68 sec: 1.06x faster                                                      |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.43 us: 1.05x faster                                                       |
| fannkuch                 | 256 ms                                                      | 244 ms: 1.05x faster                                                        |
| logging_simple           | 6.22 us                                                     | 5.98 us: 1.04x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.8 ms: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.81 us: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 38.7 ns: 1.02x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.8 ms: 1.02x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 76.2 ms: 1.00x slower                                                       |
| python_startup           | 20.6 ms                                                     | 20.9 ms: 1.01x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.82 us: 1.02x slower                                                       |
| pidigits                 | 149 ms                                                      | 153 ms: 1.02x slower                                                        |
| scimark_fft              | 187 ms                                                      | 195 ms: 1.04x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 18.1 us: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 81.5 ms: 1.08x slower                                                       |
| async_generators         | 222 ms                                                      | 241 ms: 1.09x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.48 us: 1.09x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.46 ms: 1.13x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 70.2 ms: 1.13x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.9 ms: 1.22x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.6 ms: 1.22x slower                                                       |
| regex_v8                 | 15.4 ms                                                     | 21.8 ms: 1.41x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                                |

Benchmark hidden because not significant (3): scimark_monte_carlo, scimark_sparse_mat_mult, unpickle_list
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240201-3.13.0a3+-1aec064-JIT/bm-20240201-pythonperf1-amd64-python-1aec0644447e69e981d5-3.13.0a3+-1aec064.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown