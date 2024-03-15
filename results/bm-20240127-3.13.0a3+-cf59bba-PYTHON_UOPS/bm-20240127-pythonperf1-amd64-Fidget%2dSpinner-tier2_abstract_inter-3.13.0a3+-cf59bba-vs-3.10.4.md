
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: cf59bba
- commit date: 2024-01-27
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 229 ms: 1.07x faster                                                                  |
| chameleon      | 5.79 ms                                                     | 5.05 ms: 1.15x faster                                                                 |
| docutils       | 1.92 sec                                                    | 1.63 sec: 1.18x faster                                                                |
| tornado_http   | 108 ms                                                      | 87.4 ms: 1.24x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 273 ms: 1.60x faster                                                                  |
| async_tree_memoization  | 526 ms                                                      | 343 ms: 1.53x faster                                                                  |
| async_tree_io           | 1.11 sec                                                    | 747 ms: 1.48x faster                                                                  |
| async_tree_cpu_io_mixed | 638 ms                                                      | 466 ms: 1.37x faster                                                                  |
| Geometric mean          | (ref)                                                       | 1.49x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.7 ms: 1.09x faster                                                                 |
| nbody          | 71.3 ms                                                     | 77.0 ms: 1.08x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.6 ms: 1.25x faster                                                                 |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                                                  |
| regex_effbot   | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                                 |
| regex_v8       | 15.4 ms                                                     | 15.7 ms: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                                 |
| pickle_pure_python   | 270 us                                                      | 186 us: 1.45x faster                                                                  |
| unpickle_pure_python | 183 us                                                      | 139 us: 1.31x faster                                                                  |
| tomli_loads          | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                                                |
| xml_etree_process    | 44.5 ms                                                     | 38.0 ms: 1.17x faster                                                                 |
| unpickle             | 9.09 us                                                     | 8.30 us: 1.10x faster                                                                 |
| xml_etree_parse      | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                                 |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.01x faster                                                                 |
| pickle               | 6.85 us                                                     | 7.22 us: 1.05x slower                                                                 |
| xml_etree_iterparse  | 65.0 ms                                                     | 68.9 ms: 1.06x slower                                                                 |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                                                 |
| pickle_list          | 2.75 us                                                     | 2.98 us: 1.08x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                          |

Benchmark hidden because not significant (2): xml_etree_generate, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.8 ms: 1.01x slower                                                                 |
| python_startup_no_site | 15.5 ms                                                     | 18.9 ms: 1.22x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 74.8 us: 4.49x faster                                                                 |
| richards_super           | 52.2 ms                                                     | 30.9 ms: 1.69x faster                                                                 |
| logging_silent           | 94.6 ns                                                     | 56.3 ns: 1.68x faster                                                                 |
| json_dumps               | 9.16 ms                                                     | 5.66 ms: 1.62x faster                                                                 |
| deltablue                | 4.19 ms                                                     | 2.61 ms: 1.60x faster                                                                 |
| async_tree_none          | 435 ms                                                      | 273 ms: 1.60x faster                                                                  |
| sqlglot_parse            | 1.22 ms                                                     | 780 us: 1.56x faster                                                                  |
| raytrace                 | 273 ms                                                      | 176 ms: 1.55x faster                                                                  |
| richards                 | 42.4 ms                                                     | 27.6 ms: 1.54x faster                                                                 |
| async_tree_memoization   | 526 ms                                                      | 343 ms: 1.53x faster                                                                  |
| asyncio_tcp              | 732 ms                                                      | 491 ms: 1.49x faster                                                                  |
| async_tree_io            | 1.11 sec                                                    | 747 ms: 1.48x faster                                                                  |
| go                       | 139 ms                                                      | 93.7 ms: 1.48x faster                                                                 |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                                                 |
| pickle_pure_python       | 270 us                                                      | 186 us: 1.45x faster                                                                  |
| generators               | 32.4 ms                                                     | 22.6 ms: 1.43x faster                                                                 |
| chaos                    | 61.7 ms                                                     | 43.5 ms: 1.42x faster                                                                 |
| scimark_lu               | 85.8 ms                                                     | 62.6 ms: 1.37x faster                                                                 |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 466 ms: 1.37x faster                                                                  |
| comprehensions           | 16.5 us                                                     | 12.5 us: 1.32x faster                                                                 |
| unpickle_pure_python     | 183 us                                                      | 139 us: 1.31x faster                                                                  |
| pycparser                | 930 ms                                                      | 708 ms: 1.31x faster                                                                  |
| crypto_pyaes             | 62.5 ms                                                     | 48.1 ms: 1.30x faster                                                                 |
| mypy2                    | 555 ms                                                      | 432 ms: 1.29x faster                                                                  |
| scimark_sor              | 106 ms                                                      | 83.8 ms: 1.27x faster                                                                 |
| pyflate                  | 409 ms                                                      | 326 ms: 1.25x faster                                                                  |
| regex_compile            | 106 ms                                                      | 84.6 ms: 1.25x faster                                                                 |
| mako                     | 9.03 ms                                                     | 7.22 ms: 1.25x faster                                                                 |
| tornado_http             | 108 ms                                                      | 87.4 ms: 1.24x faster                                                                 |
| mdp                      | 1.78 sec                                                    | 1.44 sec: 1.24x faster                                                                |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.72 sec: 1.23x faster                                                                |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                                 |
| hexiom                   | 5.74 ms                                                     | 4.78 ms: 1.20x faster                                                                 |
| sympy_sum                | 107 ms                                                      | 89.1 ms: 1.20x faster                                                                 |
| scimark_monte_carlo      | 57.3 ms                                                     | 48.0 ms: 1.19x faster                                                                 |
| tomli_loads              | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                                                |
| dask                     | 313 ms                                                      | 263 ms: 1.19x faster                                                                  |
| deepcopy_memo            | 28.8 us                                                     | 24.4 us: 1.18x faster                                                                 |
| docutils                 | 1.92 sec                                                    | 1.63 sec: 1.18x faster                                                                |
| coroutines               | 16.0 ms                                                     | 13.6 ms: 1.17x faster                                                                 |
| xml_etree_process        | 44.5 ms                                                     | 38.0 ms: 1.17x faster                                                                 |
| sympy_str                | 194 ms                                                      | 167 ms: 1.16x faster                                                                  |
| dulwich_log              | 50.5 ms                                                     | 43.7 ms: 1.15x faster                                                                 |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                                 |
| chameleon                | 5.79 ms                                                     | 5.05 ms: 1.15x faster                                                                 |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                                                 |
| pprint_pformat           | 1.22 sec                                                    | 1.08 sec: 1.13x faster                                                                |
| pprint_safe_repr         | 592 ms                                                      | 523 ms: 1.13x faster                                                                  |
| sqlglot_normalize        | 205 ms                                                      | 182 ms: 1.13x faster                                                                  |
| deepcopy                 | 255 us                                                      | 227 us: 1.13x faster                                                                  |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                                                  |
| sympy_expand             | 314 ms                                                      | 284 ms: 1.11x faster                                                                  |
| unpickle                 | 9.09 us                                                     | 8.30 us: 1.10x faster                                                                 |
| deepcopy_reduce          | 2.20 us                                                     | 2.01 us: 1.09x faster                                                                 |
| float                    | 61.7 ms                                                     | 56.7 ms: 1.09x faster                                                                 |
| bench_thread_pool        | 958 us                                                      | 881 us: 1.09x faster                                                                  |
| create_gc_cycles         | 800 us                                                      | 740 us: 1.08x faster                                                                  |
| 2to3                     | 246 ms                                                      | 229 ms: 1.07x faster                                                                  |
| nqueens                  | 66.6 ms                                                     | 63.8 ms: 1.04x faster                                                                 |
| regex_effbot             | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                                 |
| xml_etree_parse          | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                                 |
| logging_format           | 6.76 us                                                     | 6.59 us: 1.03x faster                                                                 |
| unpack_sequence          | 39.6 ns                                                     | 39.1 ns: 1.01x faster                                                                 |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.01x faster                                                                 |
| spectral_norm            | 77.3 ms                                                     | 76.2 ms: 1.01x faster                                                                 |
| logging_simple           | 6.22 us                                                     | 6.15 us: 1.01x faster                                                                 |
| python_startup           | 20.6 ms                                                     | 20.8 ms: 1.01x slower                                                                 |
| meteor_contest           | 75.9 ms                                                     | 77.0 ms: 1.01x slower                                                                 |
| regex_v8                 | 15.4 ms                                                     | 15.7 ms: 1.02x slower                                                                 |
| pickle                   | 6.85 us                                                     | 7.22 us: 1.05x slower                                                                 |
| scimark_fft              | 187 ms                                                      | 198 ms: 1.05x slower                                                                  |
| xml_etree_iterparse      | 65.0 ms                                                     | 68.9 ms: 1.06x slower                                                                 |
| async_generators         | 222 ms                                                      | 236 ms: 1.06x slower                                                                  |
| fannkuch                 | 256 ms                                                      | 272 ms: 1.06x slower                                                                  |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.91 ms: 1.07x slower                                                                 |
| pathlib                  | 75.7 ms                                                     | 80.9 ms: 1.07x slower                                                                 |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                                                 |
| nbody                    | 71.3 ms                                                     | 77.0 ms: 1.08x slower                                                                 |
| pickle_list              | 2.75 us                                                     | 2.98 us: 1.08x slower                                                                 |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.09x slower                                                                 |
| bench_mp_pool            | 62.0 ms                                                     | 70.8 ms: 1.14x slower                                                                 |
| telco                    | 3.94 ms                                                     | 4.73 ms: 1.20x slower                                                                 |
| python_startup_no_site   | 15.5 ms                                                     | 18.9 ms: 1.22x slower                                                                 |
| coverage                 | 39.0 ms                                                     | 47.8 ms: 1.23x slower                                                                 |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                          |

Benchmark hidden because not significant (4): json, xml_etree_generate, pidigits, unpickle_list
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240127-3.13.0a3+-cf59bba-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-cf59bba.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown