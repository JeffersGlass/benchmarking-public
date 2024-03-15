
# Results vs. 3.10.4

- fork: python
- ref: v3.11.5
- machine: windows-amd64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 208 ms: 1.18x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.27 ms: 1.10x faster                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| html5lib       | 51.0 ms                                                     | 38.8 ms: 1.32x faster                                       |
| tornado_http   | 108 ms                                                      | 90.6 ms: 1.20x faster                                       |
| Geometric mean | (ref)                                                       | 1.20x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 779 ms: 1.42x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 375 ms: 1.40x faster                                        |
| async_tree_none         | 435 ms                                                      | 311 ms: 1.40x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 516 ms: 1.24x faster                                        |
| Geometric mean          | (ref)                                                       | 1.36x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.9 ms: 1.14x faster                                       |
| nbody          | 71.3 ms                                                     | 70.1 ms: 1.02x faster                                       |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.06x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 117 ms: 1.16x faster                                        |
| regex_compile  | 106 ms                                                      | 91.3 ms: 1.16x faster                                       |
| regex_v8       | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.49 ms: 1.12x faster                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 202 us: 1.34x faster                                        |
| unpickle_pure_python | 183 us                                                      | 151 us: 1.21x faster                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.9 ms: 1.20x faster                                       |
| json_dumps           | 9.16 ms                                                     | 7.63 ms: 1.20x faster                                       |
| tomli_loads          | 1.67 sec                                                    | 1.41 sec: 1.19x faster                                      |
| unpickle             | 9.09 us                                                     | 7.92 us: 1.15x faster                                       |
| json_loads           | 14.0 us                                                     | 13.0 us: 1.08x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 51.8 ms: 1.07x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.60 us: 1.04x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.4 ms: 1.03x faster                                       |
| pickle_dict          | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                |

Benchmark hidden because not significant (3): pickle_list, pickle, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.4 ms: 1.06x faster                                       |
| python_startup_no_site | 15.5 ms                                                     | 16.5 ms: 1.06x slower                                       |
| Geometric mean         | (ref)                                                       | 1.00x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.44 ms: 1.21x faster                                       |
| django_template | 28.9 ms                                                     | 23.9 ms: 1.21x faster                                       |
| genshi_text     | 19.8 ms                                                     | 17.5 ms: 1.13x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 38.0 ms: 1.08x faster                                       |
| Geometric mean  | (ref)                                                       | 1.16x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-pythonperf1-amd64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.61 ms: 1.60x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 779 ms: 1.42x faster                                        |
| richards                 | 42.4 ms                                                     | 30.1 ms: 1.41x faster                                       |
| go                       | 139 ms                                                      | 98.8 ms: 1.41x faster                                       |
| async_tree_memoization   | 526 ms                                                      | 375 ms: 1.40x faster                                        |
| async_tree_none          | 435 ms                                                      | 311 ms: 1.40x faster                                        |
| scimark_sor              | 106 ms                                                      | 76.5 ms: 1.39x faster                                       |
| richards_super           | 52.2 ms                                                     | 38.0 ms: 1.37x faster                                       |
| scimark_lu               | 85.8 ms                                                     | 62.7 ms: 1.37x faster                                       |
| pyflate                  | 409 ms                                                      | 302 ms: 1.35x faster                                        |
| logging_silent           | 94.6 ns                                                     | 70.0 ns: 1.35x faster                                       |
| raytrace                 | 273 ms                                                      | 203 ms: 1.34x faster                                        |
| pickle_pure_python       | 270 us                                                      | 202 us: 1.34x faster                                        |
| pycparser                | 930 ms                                                      | 699 ms: 1.33x faster                                        |
| html5lib                 | 51.0 ms                                                     | 38.8 ms: 1.32x faster                                       |
| sqlglot_parse            | 1.22 ms                                                     | 928 us: 1.31x faster                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.13 ms: 1.30x faster                                       |
| crypto_pyaes             | 62.5 ms                                                     | 48.1 ms: 1.30x faster                                       |
| thrift                   | 617 us                                                      | 488 us: 1.27x faster                                        |
| hexiom                   | 5.74 ms                                                     | 4.55 ms: 1.26x faster                                       |
| chaos                    | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 516 ms: 1.24x faster                                        |
| sqlalchemy_declarative   | 103 ms                                                      | 83.8 ms: 1.23x faster                                       |
| async_generators         | 222 ms                                                      | 180 ms: 1.23x faster                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.5 ms: 1.23x faster                                       |
| mako                     | 9.03 ms                                                     | 7.44 ms: 1.21x faster                                       |
| unpickle_pure_python     | 183 us                                                      | 151 us: 1.21x faster                                        |
| django_template          | 28.9 ms                                                     | 23.9 ms: 1.21x faster                                       |
| xml_etree_process        | 44.5 ms                                                     | 36.9 ms: 1.20x faster                                       |
| json_dumps               | 9.16 ms                                                     | 7.63 ms: 1.20x faster                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                      |
| tornado_http             | 108 ms                                                      | 90.6 ms: 1.20x faster                                       |
| tomli_loads              | 1.67 sec                                                    | 1.41 sec: 1.19x faster                                      |
| dask                     | 313 ms                                                      | 265 ms: 1.18x faster                                        |
| 2to3                     | 246 ms                                                      | 208 ms: 1.18x faster                                        |
| aiohttp                  | 995 us                                                      | 853 us: 1.17x faster                                        |
| deepcopy_memo            | 28.8 us                                                     | 24.7 us: 1.16x faster                                       |
| regex_dna                | 136 ms                                                      | 117 ms: 1.16x faster                                        |
| regex_compile            | 106 ms                                                      | 91.3 ms: 1.16x faster                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.05 sec: 1.16x faster                                      |
| dulwich_log              | 50.5 ms                                                     | 43.6 ms: 1.16x faster                                       |
| pprint_safe_repr         | 592 ms                                                      | 513 ms: 1.15x faster                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 34.5 ms: 1.15x faster                                       |
| unpickle                 | 9.09 us                                                     | 7.92 us: 1.15x faster                                       |
| spectral_norm            | 77.3 ms                                                     | 67.5 ms: 1.14x faster                                       |
| float                    | 61.7 ms                                                     | 53.9 ms: 1.14x faster                                       |
| genshi_text              | 19.8 ms                                                     | 17.5 ms: 1.13x faster                                       |
| create_gc_cycles         | 800 us                                                      | 709 us: 1.13x faster                                        |
| regex_v8                 | 15.4 ms                                                     | 13.8 ms: 1.12x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.49 ms: 1.12x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.72 us: 1.11x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.7 ms: 1.11x faster                                       |
| bench_thread_pool        | 958 us                                                      | 863 us: 1.11x faster                                        |
| coroutines               | 16.0 ms                                                     | 14.5 ms: 1.10x faster                                       |
| chameleon                | 5.79 ms                                                     | 5.27 ms: 1.10x faster                                       |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.4 ms: 1.10x faster                                       |
| pylint                   | 350 ms                                                      | 320 ms: 1.10x faster                                        |
| mdp                      | 1.78 sec                                                    | 1.63 sec: 1.09x faster                                      |
| pathlib                  | 75.7 ms                                                     | 69.7 ms: 1.09x faster                                       |
| json_loads               | 14.0 us                                                     | 13.0 us: 1.08x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 190 ms: 1.08x faster                                        |
| genshi_xml               | 41.0 ms                                                     | 38.0 ms: 1.08x faster                                       |
| xml_etree_generate       | 55.5 ms                                                     | 51.8 ms: 1.07x faster                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.06 us: 1.07x faster                                       |
| nqueens                  | 66.6 ms                                                     | 62.3 ms: 1.07x faster                                       |
| sympy_sum                | 107 ms                                                      | 100 ms: 1.07x faster                                        |
| sympy_str                | 194 ms                                                      | 183 ms: 1.06x faster                                        |
| python_startup           | 20.6 ms                                                     | 19.4 ms: 1.06x faster                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.57 ms: 1.06x faster                                       |
| deepcopy                 | 255 us                                                      | 241 us: 1.06x faster                                        |
| asyncio_tcp              | 732 ms                                                      | 694 ms: 1.06x faster                                        |
| sympy_expand             | 314 ms                                                      | 299 ms: 1.05x faster                                        |
| unpickle_list            | 2.71 us                                                     | 2.60 us: 1.04x faster                                       |
| comprehensions           | 16.5 us                                                     | 15.9 us: 1.04x faster                                       |
| scimark_fft              | 187 ms                                                      | 181 ms: 1.03x faster                                        |
| typing_runtime_protocols | 336 us                                                      | 327 us: 1.03x faster                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.4 ms: 1.03x faster                                       |
| nbody                    | 71.3 ms                                                     | 70.1 ms: 1.02x faster                                       |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| bench_mp_pool            | 62.0 ms                                                     | 61.5 ms: 1.01x faster                                       |
| flaskblogging            | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| telco                    | 3.94 ms                                                     | 3.96 ms: 1.01x slower                                       |
| meteor_contest           | 75.9 ms                                                     | 76.8 ms: 1.01x slower                                       |
| generators               | 32.4 ms                                                     | 33.8 ms: 1.04x slower                                       |
| logging_format           | 6.76 us                                                     | 7.06 us: 1.04x slower                                       |
| gc_traversal             | 1.41 ms                                                     | 1.48 ms: 1.05x slower                                       |
| fannkuch                 | 256 ms                                                      | 268 ms: 1.05x slower                                        |
| logging_simple           | 6.22 us                                                     | 6.56 us: 1.05x slower                                       |
| python_startup_no_site   | 15.5 ms                                                     | 16.5 ms: 1.06x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 45.5 ns: 1.15x slower                                       |
| coverage                 | 39.0 ms                                                     | 54.3 ms: 1.39x slower                                       |
| Geometric mean           | (ref)                                                       | 1.13x faster                                                |

Benchmark hidden because not significant (5): asyncio_tcp_ssl, json, pickle_list, pickle, xml_etree_parse
Ignored benchmarks (1) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown