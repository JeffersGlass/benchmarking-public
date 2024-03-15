
# Results vs. 3.10.4

- fork: python
- ref: v3.11.6
- machine: windows-amd64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 207 ms: 1.19x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.24 ms: 1.10x faster                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| html5lib       | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                       |
| tornado_http   | 108 ms                                                      | 90.5 ms: 1.20x faster                                       |
| Geometric mean | (ref)                                                       | 1.20x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 778 ms: 1.42x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 375 ms: 1.40x faster                                        |
| async_tree_none         | 435 ms                                                      | 311 ms: 1.40x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 515 ms: 1.24x faster                                        |
| Geometric mean          | (ref)                                                       | 1.36x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.3 ms: 1.14x faster                                       |
| nbody          | 71.3 ms                                                     | 69.7 ms: 1.02x faster                                       |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 91.7 ms: 1.16x faster                                       |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                        |
| regex_v8       | 15.4 ms                                                     | 14.2 ms: 1.09x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.53 ms: 1.08x faster                                       |
| Geometric mean | (ref)                                                       | 1.11x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 203 us: 1.33x faster                                        |
| unpickle_pure_python | 183 us                                                      | 151 us: 1.21x faster                                        |
| unpickle             | 9.09 us                                                     | 7.67 us: 1.19x faster                                       |
| json_dumps           | 9.16 ms                                                     | 7.74 ms: 1.18x faster                                       |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                       |
| json_loads           | 14.0 us                                                     | 13.2 us: 1.06x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.64 us: 1.03x faster                                       |
| pickle               | 6.85 us                                                     | 6.67 us: 1.03x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                       |
| pickle_list          | 2.75 us                                                     | 2.70 us: 1.02x faster                                       |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup | 20.6 ms                                                     | 18.6 ms: 1.11x faster                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.31 ms: 1.24x faster                                       |
| django_template | 28.9 ms                                                     | 23.6 ms: 1.23x faster                                       |
| genshi_text     | 19.8 ms                                                     | 17.2 ms: 1.15x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 38.1 ms: 1.08x faster                                       |
| Geometric mean  | (ref)                                                       | 1.17x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231002-pythonperf1-amd64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.63 ms: 1.59x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 778 ms: 1.42x faster                                        |
| async_tree_memoization   | 526 ms                                                      | 375 ms: 1.40x faster                                        |
| async_tree_none          | 435 ms                                                      | 311 ms: 1.40x faster                                        |
| scimark_lu               | 85.8 ms                                                     | 61.9 ms: 1.39x faster                                       |
| richards                 | 42.4 ms                                                     | 30.6 ms: 1.39x faster                                       |
| scimark_sor              | 106 ms                                                      | 76.8 ms: 1.38x faster                                       |
| go                       | 139 ms                                                      | 102 ms: 1.36x faster                                        |
| richards_super           | 52.2 ms                                                     | 38.4 ms: 1.36x faster                                       |
| raytrace                 | 273 ms                                                      | 203 ms: 1.35x faster                                        |
| pyflate                  | 409 ms                                                      | 305 ms: 1.34x faster                                        |
| pycparser                | 930 ms                                                      | 694 ms: 1.34x faster                                        |
| logging_silent           | 94.6 ns                                                     | 70.7 ns: 1.34x faster                                       |
| pickle_pure_python       | 270 us                                                      | 203 us: 1.33x faster                                        |
| html5lib                 | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                       |
| sqlglot_parse            | 1.22 ms                                                     | 938 us: 1.29x faster                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.14 ms: 1.29x faster                                       |
| crypto_pyaes             | 62.5 ms                                                     | 49.3 ms: 1.27x faster                                       |
| thrift                   | 617 us                                                      | 487 us: 1.27x faster                                        |
| hexiom                   | 5.74 ms                                                     | 4.55 ms: 1.26x faster                                       |
| chaos                    | 61.7 ms                                                     | 49.7 ms: 1.24x faster                                       |
| async_generators         | 222 ms                                                      | 179 ms: 1.24x faster                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 515 ms: 1.24x faster                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.3 ms: 1.24x faster                                       |
| mako                     | 9.03 ms                                                     | 7.31 ms: 1.24x faster                                       |
| sqlalchemy_declarative   | 103 ms                                                      | 83.8 ms: 1.23x faster                                       |
| django_template          | 28.9 ms                                                     | 23.6 ms: 1.23x faster                                       |
| unpickle_pure_python     | 183 us                                                      | 151 us: 1.21x faster                                        |
| tornado_http             | 108 ms                                                      | 90.5 ms: 1.20x faster                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| dask                     | 313 ms                                                      | 263 ms: 1.19x faster                                        |
| 2to3                     | 246 ms                                                      | 207 ms: 1.19x faster                                        |
| unpickle                 | 9.09 us                                                     | 7.67 us: 1.19x faster                                       |
| json_dumps               | 9.16 ms                                                     | 7.74 ms: 1.18x faster                                       |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                      |
| xml_etree_process        | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                       |
| aiohttp                  | 995 us                                                      | 853 us: 1.17x faster                                        |
| regex_compile            | 106 ms                                                      | 91.7 ms: 1.16x faster                                       |
| genshi_text              | 19.8 ms                                                     | 17.2 ms: 1.15x faster                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.06 sec: 1.15x faster                                      |
| pprint_safe_repr         | 592 ms                                                      | 517 ms: 1.15x faster                                        |
| spectral_norm            | 77.3 ms                                                     | 67.5 ms: 1.14x faster                                       |
| deepcopy_memo            | 28.8 us                                                     | 25.3 us: 1.14x faster                                       |
| float                    | 61.7 ms                                                     | 54.3 ms: 1.14x faster                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 35.1 ms: 1.14x faster                                       |
| create_gc_cycles         | 800 us                                                      | 708 us: 1.13x faster                                        |
| bench_thread_pool        | 958 us                                                      | 852 us: 1.12x faster                                        |
| dulwich_log              | 50.5 ms                                                     | 45.0 ms: 1.12x faster                                       |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                        |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.3 ms: 1.11x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.72 us: 1.11x faster                                       |
| python_startup           | 20.6 ms                                                     | 18.6 ms: 1.11x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.8 ms: 1.11x faster                                       |
| chameleon                | 5.79 ms                                                     | 5.24 ms: 1.10x faster                                       |
| pathlib                  | 75.7 ms                                                     | 68.5 ms: 1.10x faster                                       |
| pylint                   | 350 ms                                                      | 318 ms: 1.10x faster                                        |
| coroutines               | 16.0 ms                                                     | 14.7 ms: 1.09x faster                                       |
| regex_v8                 | 15.4 ms                                                     | 14.2 ms: 1.09x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.53 ms: 1.08x faster                                       |
| genshi_xml               | 41.0 ms                                                     | 38.1 ms: 1.08x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 192 ms: 1.07x faster                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.55 ms: 1.07x faster                                       |
| json_loads               | 14.0 us                                                     | 13.2 us: 1.06x faster                                       |
| fannkuch                 | 256 ms                                                      | 241 ms: 1.06x faster                                        |
| bench_mp_pool            | 62.0 ms                                                     | 58.7 ms: 1.06x faster                                       |
| sympy_sum                | 107 ms                                                      | 102 ms: 1.05x faster                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.10 us: 1.05x faster                                       |
| comprehensions           | 16.5 us                                                     | 15.7 us: 1.05x faster                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                       |
| nqueens                  | 66.6 ms                                                     | 63.7 ms: 1.05x faster                                       |
| mdp                      | 1.78 sec                                                    | 1.71 sec: 1.04x faster                                      |
| sympy_str                | 194 ms                                                      | 187 ms: 1.04x faster                                        |
| deepcopy                 | 255 us                                                      | 246 us: 1.04x faster                                        |
| typing_runtime_protocols | 336 us                                                      | 324 us: 1.04x faster                                        |
| scimark_fft              | 187 ms                                                      | 181 ms: 1.04x faster                                        |
| sympy_expand             | 314 ms                                                      | 305 ms: 1.03x faster                                        |
| unpickle_list            | 2.71 us                                                     | 2.64 us: 1.03x faster                                       |
| pickle                   | 6.85 us                                                     | 6.67 us: 1.03x faster                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                       |
| nbody                    | 71.3 ms                                                     | 69.7 ms: 1.02x faster                                       |
| pickle_list              | 2.75 us                                                     | 2.70 us: 1.02x faster                                       |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| flaskblogging            | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| generators               | 32.4 ms                                                     | 33.7 ms: 1.04x slower                                       |
| gc_traversal             | 1.41 ms                                                     | 1.48 ms: 1.05x slower                                       |
| logging_format           | 6.76 us                                                     | 7.18 us: 1.06x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.72 us: 1.08x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 46.3 ns: 1.17x slower                                       |
| coverage                 | 39.0 ms                                                     | 53.6 ms: 1.37x slower                                       |
| Geometric mean           | (ref)                                                       | 1.13x faster                                                |

Benchmark hidden because not significant (7): json, asyncio_tcp_ssl, asyncio_tcp, telco, meteor_contest, xml_etree_parse, python_startup_no_site
Ignored benchmarks (1) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown