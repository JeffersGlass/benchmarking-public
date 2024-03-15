
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: d226882
- commit date: 2024-01-28
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| chameleon      | 5.79 ms                                                     | 5.01 ms: 1.16x faster                                                                 |
| docutils       | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                                |
| tornado_http   | 108 ms                                                      | 85.8 ms: 1.26x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.18x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 276 ms: 1.58x faster                                                                  |
| async_tree_memoization  | 526 ms                                                      | 350 ms: 1.50x faster                                                                  |
| async_tree_io           | 1.11 sec                                                    | 744 ms: 1.49x faster                                                                  |
| async_tree_cpu_io_mixed | 638 ms                                                      | 464 ms: 1.37x faster                                                                  |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 58.1 ms: 1.06x faster                                                                 |
| nbody          | 71.3 ms                                                     | 78.8 ms: 1.11x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x slower                                                                          |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 85.8 ms: 1.24x faster                                                                 |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                                                  |
| regex_effbot   | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                                 |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.51 ms: 1.66x faster                                                                 |
| pickle_pure_python   | 270 us                                                      | 179 us: 1.50x faster                                                                  |
| unpickle_pure_python | 183 us                                                      | 137 us: 1.34x faster                                                                  |
| xml_etree_process    | 44.5 ms                                                     | 38.0 ms: 1.17x faster                                                                 |
| tomli_loads          | 1.67 sec                                                    | 1.46 sec: 1.15x faster                                                                |
| unpickle             | 9.09 us                                                     | 8.45 us: 1.08x faster                                                                 |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                                 |
| unpickle_list        | 2.71 us                                                     | 2.81 us: 1.03x slower                                                                 |
| pickle               | 6.85 us                                                     | 7.11 us: 1.04x slower                                                                 |
| pickle_list          | 2.75 us                                                     | 2.91 us: 1.06x slower                                                                 |
| xml_etree_iterparse  | 65.0 ms                                                     | 69.1 ms: 1.06x slower                                                                 |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                          |

Benchmark hidden because not significant (2): xml_etree_parse, xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                          |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.99 ms: 1.13x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882 |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 73.7 us: 4.56x faster                                                                 |
| richards_super           | 52.2 ms                                                     | 30.2 ms: 1.73x faster                                                                 |
| logging_silent           | 94.6 ns                                                     | 55.0 ns: 1.72x faster                                                                 |
| json_dumps               | 9.16 ms                                                     | 5.51 ms: 1.66x faster                                                                 |
| richards                 | 42.4 ms                                                     | 26.6 ms: 1.60x faster                                                                 |
| async_tree_none          | 435 ms                                                      | 276 ms: 1.58x faster                                                                  |
| sqlglot_parse            | 1.22 ms                                                     | 782 us: 1.55x faster                                                                  |
| generators               | 32.4 ms                                                     | 20.9 ms: 1.55x faster                                                                 |
| raytrace                 | 273 ms                                                      | 178 ms: 1.53x faster                                                                  |
| scimark_lu               | 85.8 ms                                                     | 55.9 ms: 1.53x faster                                                                 |
| deltablue                | 4.19 ms                                                     | 2.74 ms: 1.53x faster                                                                 |
| go                       | 139 ms                                                      | 92.3 ms: 1.50x faster                                                                 |
| async_tree_memoization   | 526 ms                                                      | 350 ms: 1.50x faster                                                                  |
| pickle_pure_python       | 270 us                                                      | 179 us: 1.50x faster                                                                  |
| asyncio_tcp              | 732 ms                                                      | 490 ms: 1.49x faster                                                                  |
| async_tree_io            | 1.11 sec                                                    | 744 ms: 1.49x faster                                                                  |
| sqlglot_transpile        | 1.48 ms                                                     | 1.01 ms: 1.46x faster                                                                 |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.49 sec: 1.42x faster                                                                |
| chaos                    | 61.7 ms                                                     | 44.1 ms: 1.40x faster                                                                 |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 464 ms: 1.37x faster                                                                  |
| pycparser                | 930 ms                                                      | 678 ms: 1.37x faster                                                                  |
| scimark_sor              | 106 ms                                                      | 77.7 ms: 1.37x faster                                                                 |
| unpickle_pure_python     | 183 us                                                      | 137 us: 1.34x faster                                                                  |
| crypto_pyaes             | 62.5 ms                                                     | 47.3 ms: 1.32x faster                                                                 |
| mypy2                    | 555 ms                                                      | 431 ms: 1.29x faster                                                                  |
| comprehensions           | 16.5 us                                                     | 13.0 us: 1.27x faster                                                                 |
| tornado_http             | 108 ms                                                      | 85.8 ms: 1.26x faster                                                                 |
| pyflate                  | 409 ms                                                      | 329 ms: 1.24x faster                                                                  |
| deepcopy_memo            | 28.8 us                                                     | 23.2 us: 1.24x faster                                                                 |
| regex_compile            | 106 ms                                                      | 85.8 ms: 1.24x faster                                                                 |
| mdp                      | 1.78 sec                                                    | 1.44 sec: 1.23x faster                                                                |
| sympy_sum                | 107 ms                                                      | 88.7 ms: 1.21x faster                                                                 |
| dask                     | 313 ms                                                      | 262 ms: 1.19x faster                                                                  |
| docutils                 | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                                |
| scimark_monte_carlo      | 57.3 ms                                                     | 48.2 ms: 1.19x faster                                                                 |
| dulwich_log              | 50.5 ms                                                     | 43.1 ms: 1.17x faster                                                                 |
| xml_etree_process        | 44.5 ms                                                     | 38.0 ms: 1.17x faster                                                                 |
| chameleon                | 5.79 ms                                                     | 5.01 ms: 1.16x faster                                                                 |
| coroutines               | 16.0 ms                                                     | 13.9 ms: 1.15x faster                                                                 |
| sqlite_synth             | 1.91 us                                                     | 1.66 us: 1.15x faster                                                                 |
| sympy_str                | 194 ms                                                      | 169 ms: 1.15x faster                                                                  |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                                 |
| tomli_loads              | 1.67 sec                                                    | 1.46 sec: 1.15x faster                                                                |
| hexiom                   | 5.74 ms                                                     | 5.01 ms: 1.15x faster                                                                 |
| deepcopy                 | 255 us                                                      | 223 us: 1.15x faster                                                                  |
| sqlglot_optimize         | 39.8 ms                                                     | 35.1 ms: 1.13x faster                                                                 |
| deepcopy_reduce          | 2.20 us                                                     | 1.94 us: 1.13x faster                                                                 |
| mako                     | 9.03 ms                                                     | 7.99 ms: 1.13x faster                                                                 |
| sympy_expand             | 314 ms                                                      | 280 ms: 1.12x faster                                                                  |
| pprint_safe_repr         | 592 ms                                                      | 527 ms: 1.12x faster                                                                  |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.12x faster                                                                |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                                                  |
| bench_thread_pool        | 958 us                                                      | 857 us: 1.12x faster                                                                  |
| sqlglot_normalize        | 205 ms                                                      | 186 ms: 1.11x faster                                                                  |
| 2to3                     | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| unpickle                 | 9.09 us                                                     | 8.45 us: 1.08x faster                                                                 |
| create_gc_cycles         | 800 us                                                      | 750 us: 1.07x faster                                                                  |
| float                    | 61.7 ms                                                     | 58.1 ms: 1.06x faster                                                                 |
| nqueens                  | 66.6 ms                                                     | 63.5 ms: 1.05x faster                                                                 |
| regex_effbot             | 1.66 ms                                                     | 1.60 ms: 1.04x faster                                                                 |
| unpack_sequence          | 39.6 ns                                                     | 38.7 ns: 1.02x faster                                                                 |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                                 |
| regex_v8                 | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                                 |
| logging_format           | 6.76 us                                                     | 6.67 us: 1.01x faster                                                                 |
| unpickle_list            | 2.71 us                                                     | 2.81 us: 1.03x slower                                                                 |
| meteor_contest           | 75.9 ms                                                     | 78.7 ms: 1.04x slower                                                                 |
| pickle                   | 6.85 us                                                     | 7.11 us: 1.04x slower                                                                 |
| spectral_norm            | 77.3 ms                                                     | 80.3 ms: 1.04x slower                                                                 |
| async_generators         | 222 ms                                                      | 230 ms: 1.04x slower                                                                  |
| fannkuch                 | 256 ms                                                      | 268 ms: 1.05x slower                                                                  |
| pathlib                  | 75.7 ms                                                     | 79.8 ms: 1.05x slower                                                                 |
| pickle_list              | 2.75 us                                                     | 2.91 us: 1.06x slower                                                                 |
| xml_etree_iterparse      | 65.0 ms                                                     | 69.1 ms: 1.06x slower                                                                 |
| json                     | 3.14 ms                                                     | 3.34 ms: 1.06x slower                                                                 |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                                                 |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                                                 |
| nbody                    | 71.3 ms                                                     | 78.8 ms: 1.11x slower                                                                 |
| bench_mp_pool            | 62.0 ms                                                     | 68.7 ms: 1.11x slower                                                                 |
| scimark_fft              | 187 ms                                                      | 209 ms: 1.11x slower                                                                  |
| coverage                 | 39.0 ms                                                     | 45.0 ms: 1.15x slower                                                                 |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.19 ms: 1.17x slower                                                                 |
| python_startup_no_site   | 15.5 ms                                                     | 18.4 ms: 1.19x slower                                                                 |
| telco                    | 3.94 ms                                                     | 4.74 ms: 1.20x slower                                                                 |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                          |

Benchmark hidden because not significant (5): xml_etree_parse, logging_simple, xml_etree_generate, python_startup, pidigits
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240128-3.13.0a3+-d226882-PYTHON_UOPS/bm-20240128-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-d226882.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown