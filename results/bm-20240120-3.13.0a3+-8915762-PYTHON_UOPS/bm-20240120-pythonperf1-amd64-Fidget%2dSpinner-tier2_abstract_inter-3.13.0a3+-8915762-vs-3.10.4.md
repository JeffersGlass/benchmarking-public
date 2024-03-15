
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 8915762
- commit date: 2024-01-20
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                                  |
| chameleon      | 5.79 ms                                                     | 5.03 ms: 1.15x faster                                                                 |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                                |
| tornado_http   | 108 ms                                                      | 88.5 ms: 1.22x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.17x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 271 ms: 1.61x faster                                                                  |
| async_tree_io           | 1.11 sec                                                    | 722 ms: 1.54x faster                                                                  |
| async_tree_memoization  | 526 ms                                                      | 344 ms: 1.53x faster                                                                  |
| async_tree_cpu_io_mixed | 638 ms                                                      | 457 ms: 1.40x faster                                                                  |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                                 |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                                  |
| nbody          | 71.3 ms                                                     | 81.4 ms: 1.14x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.4 ms: 1.26x faster                                                                 |
| regex_dna      | 136 ms                                                      | 118 ms: 1.16x faster                                                                  |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                                 |
| regex_v8       | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                                 |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                                  |
| unpickle_pure_python | 183 us                                                      | 137 us: 1.34x faster                                                                  |
| xml_etree_process    | 44.5 ms                                                     | 37.1 ms: 1.20x faster                                                                 |
| tomli_loads          | 1.67 sec                                                    | 1.44 sec: 1.16x faster                                                                |
| unpickle             | 9.09 us                                                     | 8.33 us: 1.09x faster                                                                 |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                                                 |
| xml_etree_parse      | 96.8 ms                                                     | 94.0 ms: 1.03x faster                                                                 |
| xml_etree_generate   | 55.5 ms                                                     | 54.5 ms: 1.02x faster                                                                 |
| xml_etree_iterparse  | 65.0 ms                                                     | 66.3 ms: 1.02x slower                                                                 |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                                                 |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.07x slower                                                                 |
| pickle               | 6.85 us                                                     | 7.41 us: 1.08x slower                                                                 |
| pickle_list          | 2.75 us                                                     | 3.09 us: 1.12x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.0 ms: 1.02x slower                                                                 |
| python_startup_no_site | 15.5 ms                                                     | 18.5 ms: 1.20x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.50 ms: 1.20x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762 |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.5 us: 4.63x faster                                                                 |
| logging_silent           | 94.6 ns                                                     | 55.3 ns: 1.71x faster                                                                 |
| richards_super           | 52.2 ms                                                     | 30.7 ms: 1.70x faster                                                                 |
| json_dumps               | 9.16 ms                                                     | 5.54 ms: 1.65x faster                                                                 |
| async_tree_none          | 435 ms                                                      | 271 ms: 1.61x faster                                                                  |
| raytrace                 | 273 ms                                                      | 173 ms: 1.58x faster                                                                  |
| sqlglot_parse            | 1.22 ms                                                     | 776 us: 1.57x faster                                                                  |
| asyncio_tcp              | 732 ms                                                      | 468 ms: 1.56x faster                                                                  |
| richards                 | 42.4 ms                                                     | 27.1 ms: 1.56x faster                                                                 |
| deltablue                | 4.19 ms                                                     | 2.73 ms: 1.54x faster                                                                 |
| async_tree_io            | 1.11 sec                                                    | 722 ms: 1.54x faster                                                                  |
| async_tree_memoization   | 526 ms                                                      | 344 ms: 1.53x faster                                                                  |
| scimark_lu               | 85.8 ms                                                     | 56.2 ms: 1.53x faster                                                                 |
| go                       | 139 ms                                                      | 92.3 ms: 1.51x faster                                                                 |
| generators               | 32.4 ms                                                     | 21.6 ms: 1.50x faster                                                                 |
| pickle_pure_python       | 270 us                                                      | 180 us: 1.50x faster                                                                  |
| sqlglot_transpile        | 1.48 ms                                                     | 1.00 ms: 1.47x faster                                                                 |
| chaos                    | 61.7 ms                                                     | 43.8 ms: 1.41x faster                                                                 |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 457 ms: 1.40x faster                                                                  |
| scimark_sor              | 106 ms                                                      | 79.0 ms: 1.34x faster                                                                 |
| unpickle_pure_python     | 183 us                                                      | 137 us: 1.34x faster                                                                  |
| pycparser                | 930 ms                                                      | 703 ms: 1.32x faster                                                                  |
| mdp                      | 1.78 sec                                                    | 1.36 sec: 1.31x faster                                                                |
| mypy2                    | 555 ms                                                      | 423 ms: 1.31x faster                                                                  |
| crypto_pyaes             | 62.5 ms                                                     | 47.9 ms: 1.31x faster                                                                 |
| comprehensions           | 16.5 us                                                     | 12.7 us: 1.30x faster                                                                 |
| deepcopy_memo            | 28.8 us                                                     | 22.5 us: 1.28x faster                                                                 |
| pyflate                  | 409 ms                                                      | 324 ms: 1.26x faster                                                                  |
| regex_compile            | 106 ms                                                      | 84.4 ms: 1.26x faster                                                                 |
| tornado_http             | 108 ms                                                      | 88.5 ms: 1.22x faster                                                                 |
| docutils                 | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                                |
| sympy_sum                | 107 ms                                                      | 88.3 ms: 1.21x faster                                                                 |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.75 sec: 1.20x faster                                                                |
| mako                     | 9.03 ms                                                     | 7.50 ms: 1.20x faster                                                                 |
| dask                     | 313 ms                                                      | 260 ms: 1.20x faster                                                                  |
| coroutines               | 16.0 ms                                                     | 13.3 ms: 1.20x faster                                                                 |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.7 ms: 1.20x faster                                                                 |
| dulwich_log              | 50.5 ms                                                     | 42.1 ms: 1.20x faster                                                                 |
| xml_etree_process        | 44.5 ms                                                     | 37.1 ms: 1.20x faster                                                                 |
| sqlite_synth             | 1.91 us                                                     | 1.61 us: 1.18x faster                                                                 |
| sympy_str                | 194 ms                                                      | 167 ms: 1.17x faster                                                                  |
| tomli_loads              | 1.67 sec                                                    | 1.44 sec: 1.16x faster                                                                |
| hexiom                   | 5.74 ms                                                     | 4.94 ms: 1.16x faster                                                                 |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                                 |
| regex_dna                | 136 ms                                                      | 118 ms: 1.16x faster                                                                  |
| chameleon                | 5.79 ms                                                     | 5.03 ms: 1.15x faster                                                                 |
| pprint_pformat           | 1.22 sec                                                    | 1.06 sec: 1.15x faster                                                                |
| deepcopy                 | 255 us                                                      | 223 us: 1.15x faster                                                                  |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                                                 |
| pprint_safe_repr         | 592 ms                                                      | 519 ms: 1.14x faster                                                                  |
| sqlglot_normalize        | 205 ms                                                      | 182 ms: 1.13x faster                                                                  |
| sympy_expand             | 314 ms                                                      | 280 ms: 1.12x faster                                                                  |
| bench_thread_pool        | 958 us                                                      | 856 us: 1.12x faster                                                                  |
| deepcopy_reduce          | 2.20 us                                                     | 1.99 us: 1.11x faster                                                                 |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                                  |
| unpickle                 | 9.09 us                                                     | 8.33 us: 1.09x faster                                                                 |
| float                    | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                                 |
| create_gc_cycles         | 800 us                                                      | 742 us: 1.08x faster                                                                  |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                                 |
| regex_v8                 | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                                 |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                                                 |
| xml_etree_parse          | 96.8 ms                                                     | 94.0 ms: 1.03x faster                                                                 |
| xml_etree_generate       | 55.5 ms                                                     | 54.5 ms: 1.02x faster                                                                 |
| nqueens                  | 66.6 ms                                                     | 65.5 ms: 1.02x faster                                                                 |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                                                  |
| python_startup           | 20.6 ms                                                     | 21.0 ms: 1.02x slower                                                                 |
| xml_etree_iterparse      | 65.0 ms                                                     | 66.3 ms: 1.02x slower                                                                 |
| unpickle_list            | 2.71 us                                                     | 2.79 us: 1.03x slower                                                                 |
| fannkuch                 | 256 ms                                                      | 267 ms: 1.04x slower                                                                  |
| spectral_norm            | 77.3 ms                                                     | 80.6 ms: 1.04x slower                                                                 |
| pathlib                  | 75.7 ms                                                     | 79.3 ms: 1.05x slower                                                                 |
| async_generators         | 222 ms                                                      | 236 ms: 1.06x slower                                                                  |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.07x slower                                                                 |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                                 |
| scimark_fft              | 187 ms                                                      | 202 ms: 1.08x slower                                                                  |
| pickle                   | 6.85 us                                                     | 7.41 us: 1.08x slower                                                                 |
| pickle_list              | 2.75 us                                                     | 3.09 us: 1.12x slower                                                                 |
| bench_mp_pool            | 62.0 ms                                                     | 69.7 ms: 1.12x slower                                                                 |
| nbody                    | 71.3 ms                                                     | 81.4 ms: 1.14x slower                                                                 |
| coverage                 | 39.0 ms                                                     | 45.0 ms: 1.15x slower                                                                 |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.19 ms: 1.17x slower                                                                 |
| python_startup_no_site   | 15.5 ms                                                     | 18.5 ms: 1.20x slower                                                                 |
| telco                    | 3.94 ms                                                     | 4.80 ms: 1.22x slower                                                                 |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                                          |

Benchmark hidden because not significant (5): json, unpack_sequence, logging_format, meteor_contest, logging_simple
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-8915762-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-8915762.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown