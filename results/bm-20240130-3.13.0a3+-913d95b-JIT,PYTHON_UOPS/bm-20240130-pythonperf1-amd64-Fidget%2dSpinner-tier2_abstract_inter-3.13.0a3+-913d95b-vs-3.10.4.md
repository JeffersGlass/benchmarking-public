
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.21x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| chameleon      | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                                 |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                                |
| tornado_http   | 108 ms                                                      | 86.7 ms: 1.25x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 272 ms: 1.60x faster                                                                  |
| async_tree_memoization  | 526 ms                                                      | 346 ms: 1.52x faster                                                                  |
| async_tree_io           | 1.11 sec                                                    | 733 ms: 1.51x faster                                                                  |
| async_tree_cpu_io_mixed | 638 ms                                                      | 455 ms: 1.40x faster                                                                  |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 52.1 ms: 1.18x faster                                                                 |
| nbody          | 71.3 ms                                                     | 62.2 ms: 1.15x faster                                                                 |
| pidigits       | 149 ms                                                      | 154 ms: 1.03x slower                                                                  |
| Geometric mean | (ref)                                                       | 1.10x faster                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 82.7 ms: 1.28x faster                                                                 |
| regex_dna      | 136 ms                                                      | 122 ms: 1.11x faster                                                                  |
| regex_v8       | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                                 |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.44 ms: 1.69x faster                                                                 |
| pickle_pure_python   | 270 us                                                      | 177 us: 1.53x faster                                                                  |
| unpickle_pure_python | 183 us                                                      | 131 us: 1.40x faster                                                                  |
| tomli_loads          | 1.67 sec                                                    | 1.28 sec: 1.30x faster                                                                |
| xml_etree_process    | 44.5 ms                                                     | 35.8 ms: 1.24x faster                                                                 |
| unpickle             | 9.09 us                                                     | 8.44 us: 1.08x faster                                                                 |
| xml_etree_generate   | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                                 |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                                                 |
| xml_etree_parse      | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                                 |
| pickle_list          | 2.75 us                                                     | 2.82 us: 1.02x slower                                                                 |
| pickle_dict          | 17.2 us                                                     | 17.7 us: 1.03x slower                                                                 |
| unpickle_list        | 2.71 us                                                     | 2.84 us: 1.05x slower                                                                 |
| pickle               | 6.85 us                                                     | 7.31 us: 1.07x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                                          |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 21.1 ms: 1.02x slower                                                                 |
| python_startup_no_site | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.12x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.86 ms: 1.32x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 68.1 us: 4.93x faster                                                                 |
| deltablue                | 4.19 ms                                                     | 2.10 ms: 2.00x faster                                                                 |
| richards_super           | 52.2 ms                                                     | 28.3 ms: 1.84x faster                                                                 |
| logging_silent           | 94.6 ns                                                     | 52.2 ns: 1.81x faster                                                                 |
| richards                 | 42.4 ms                                                     | 24.9 ms: 1.70x faster                                                                 |
| json_dumps               | 9.16 ms                                                     | 5.44 ms: 1.69x faster                                                                 |
| sqlglot_parse            | 1.22 ms                                                     | 760 us: 1.60x faster                                                                  |
| async_tree_none          | 435 ms                                                      | 272 ms: 1.60x faster                                                                  |
| raytrace                 | 273 ms                                                      | 172 ms: 1.59x faster                                                                  |
| scimark_lu               | 85.8 ms                                                     | 55.2 ms: 1.56x faster                                                                 |
| generators               | 32.4 ms                                                     | 20.9 ms: 1.55x faster                                                                 |
| pickle_pure_python       | 270 us                                                      | 177 us: 1.53x faster                                                                  |
| async_tree_memoization   | 526 ms                                                      | 346 ms: 1.52x faster                                                                  |
| asyncio_tcp              | 732 ms                                                      | 483 ms: 1.52x faster                                                                  |
| async_tree_io            | 1.11 sec                                                    | 733 ms: 1.51x faster                                                                  |
| sqlglot_transpile        | 1.48 ms                                                     | 984 us: 1.50x faster                                                                  |
| chaos                    | 61.7 ms                                                     | 42.5 ms: 1.45x faster                                                                 |
| go                       | 139 ms                                                      | 97.4 ms: 1.43x faster                                                                 |
| comprehensions           | 16.5 us                                                     | 11.7 us: 1.41x faster                                                                 |
| unpickle_pure_python     | 183 us                                                      | 131 us: 1.40x faster                                                                  |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 455 ms: 1.40x faster                                                                  |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.52 sec: 1.38x faster                                                                |
| scimark_sor              | 106 ms                                                      | 77.6 ms: 1.37x faster                                                                 |
| deepcopy_memo            | 28.8 us                                                     | 21.2 us: 1.36x faster                                                                 |
| pycparser                | 930 ms                                                      | 703 ms: 1.32x faster                                                                  |
| mako                     | 9.03 ms                                                     | 6.86 ms: 1.32x faster                                                                 |
| crypto_pyaes             | 62.5 ms                                                     | 47.9 ms: 1.31x faster                                                                 |
| tomli_loads              | 1.67 sec                                                    | 1.28 sec: 1.30x faster                                                                |
| pyflate                  | 409 ms                                                      | 316 ms: 1.29x faster                                                                  |
| regex_compile            | 106 ms                                                      | 82.7 ms: 1.28x faster                                                                 |
| mypy2                    | 555 ms                                                      | 435 ms: 1.28x faster                                                                  |
| tornado_http             | 108 ms                                                      | 86.7 ms: 1.25x faster                                                                 |
| xml_etree_process        | 44.5 ms                                                     | 35.8 ms: 1.24x faster                                                                 |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.23x faster                                                                 |
| spectral_norm            | 77.3 ms                                                     | 62.9 ms: 1.23x faster                                                                 |
| chameleon                | 5.79 ms                                                     | 4.77 ms: 1.21x faster                                                                 |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                                |
| dulwich_log              | 50.5 ms                                                     | 42.2 ms: 1.20x faster                                                                 |
| pprint_safe_repr         | 592 ms                                                      | 498 ms: 1.19x faster                                                                  |
| float                    | 61.7 ms                                                     | 52.1 ms: 1.18x faster                                                                 |
| coroutines               | 16.0 ms                                                     | 13.5 ms: 1.18x faster                                                                 |
| dask                     | 313 ms                                                      | 265 ms: 1.18x faster                                                                  |
| sympy_sum                | 107 ms                                                      | 90.7 ms: 1.18x faster                                                                 |
| pprint_pformat           | 1.22 sec                                                    | 1.03 sec: 1.18x faster                                                                |
| deepcopy                 | 255 us                                                      | 218 us: 1.17x faster                                                                  |
| nbody                    | 71.3 ms                                                     | 62.2 ms: 1.15x faster                                                                 |
| sympy_str                | 194 ms                                                      | 170 ms: 1.14x faster                                                                  |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                                                 |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                                                  |
| deepcopy_reduce          | 2.20 us                                                     | 1.93 us: 1.14x faster                                                                 |
| sympy_expand             | 314 ms                                                      | 279 ms: 1.13x faster                                                                  |
| nqueens                  | 66.6 ms                                                     | 59.7 ms: 1.12x faster                                                                 |
| bench_thread_pool        | 958 us                                                      | 859 us: 1.11x faster                                                                  |
| regex_dna                | 136 ms                                                      | 122 ms: 1.11x faster                                                                  |
| sympy_integrate          | 15.3 ms                                                     | 13.9 ms: 1.10x faster                                                                 |
| 2to3                     | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| mdp                      | 1.78 sec                                                    | 1.62 sec: 1.10x faster                                                                |
| unpickle                 | 9.09 us                                                     | 8.44 us: 1.08x faster                                                                 |
| create_gc_cycles         | 800 us                                                      | 745 us: 1.07x faster                                                                  |
| xml_etree_generate       | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                                 |
| regex_v8                 | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                                 |
| hexiom                   | 5.74 ms                                                     | 5.44 ms: 1.06x faster                                                                 |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                                 |
| logging_format           | 6.76 us                                                     | 6.48 us: 1.04x faster                                                                 |
| json_loads               | 14.0 us                                                     | 13.5 us: 1.04x faster                                                                 |
| logging_simple           | 6.22 us                                                     | 6.02 us: 1.03x faster                                                                 |
| fannkuch                 | 256 ms                                                      | 251 ms: 1.02x faster                                                                  |
| xml_etree_parse          | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                                 |
| unpack_sequence          | 39.6 ns                                                     | 39.1 ns: 1.01x faster                                                                 |
| scimark_monte_carlo      | 57.3 ms                                                     | 58.3 ms: 1.02x slower                                                                 |
| python_startup           | 20.6 ms                                                     | 21.1 ms: 1.02x slower                                                                 |
| pickle_list              | 2.75 us                                                     | 2.82 us: 1.02x slower                                                                 |
| pickle_dict              | 17.2 us                                                     | 17.7 us: 1.03x slower                                                                 |
| pidigits                 | 149 ms                                                      | 154 ms: 1.03x slower                                                                  |
| scimark_fft              | 187 ms                                                      | 195 ms: 1.04x slower                                                                  |
| unpickle_list            | 2.71 us                                                     | 2.84 us: 1.05x slower                                                                 |
| pathlib                  | 75.7 ms                                                     | 79.8 ms: 1.05x slower                                                                 |
| meteor_contest           | 75.9 ms                                                     | 80.1 ms: 1.05x slower                                                                 |
| json                     | 3.14 ms                                                     | 3.33 ms: 1.06x slower                                                                 |
| pickle                   | 6.85 us                                                     | 7.31 us: 1.07x slower                                                                 |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.07x slower                                                                 |
| async_generators         | 222 ms                                                      | 242 ms: 1.09x slower                                                                  |
| bench_mp_pool            | 62.0 ms                                                     | 71.4 ms: 1.15x slower                                                                 |
| telco                    | 3.94 ms                                                     | 4.59 ms: 1.17x slower                                                                 |
| coverage                 | 39.0 ms                                                     | 45.8 ms: 1.17x slower                                                                 |
| python_startup_no_site   | 15.5 ms                                                     | 19.1 ms: 1.23x slower                                                                 |
| Geometric mean           | (ref)                                                       | 1.21x faster                                                                          |

Benchmark hidden because not significant (2): xml_etree_iterparse, scimark_sparse_mat_mult
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240130-3.13.0a3+-913d95b-JIT,PYTHON_UOPS/bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.16x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: unknown