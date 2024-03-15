
# Results vs. 3.10.4

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: fcdc84c
- commit date: 2024-01-29
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| chameleon      | 5.79 ms                                                     | 5.05 ms: 1.14x faster                                                                 |
| docutils       | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                                |
| tornado_http   | 108 ms                                                      | 88.1 ms: 1.23x faster                                                                 |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 276 ms: 1.58x faster                                                                  |
| async_tree_memoization  | 526 ms                                                      | 355 ms: 1.48x faster                                                                  |
| async_tree_io           | 1.11 sec                                                    | 756 ms: 1.47x faster                                                                  |
| async_tree_cpu_io_mixed | 638 ms                                                      | 473 ms: 1.35x faster                                                                  |
| Geometric mean          | (ref)                                                       | 1.47x faster                                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                                 |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                                  |
| nbody          | 71.3 ms                                                     | 76.8 ms: 1.08x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.6 ms: 1.25x faster                                                                 |
| regex_dna      | 136 ms                                                      | 123 ms: 1.11x faster                                                                  |
| regex_effbot   | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                                                 |
| regex_v8       | 15.4 ms                                                     | 15.7 ms: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                       | 1.09x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.76 ms: 1.59x faster                                                                 |
| pickle_pure_python   | 270 us                                                      | 181 us: 1.49x faster                                                                  |
| unpickle_pure_python | 183 us                                                      | 135 us: 1.35x faster                                                                  |
| xml_etree_process    | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                                                 |
| tomli_loads          | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                                |
| unpickle             | 9.09 us                                                     | 8.48 us: 1.07x faster                                                                 |
| xml_etree_parse      | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                                 |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                                 |
| unpickle_list        | 2.71 us                                                     | 2.78 us: 1.02x slower                                                                 |
| xml_etree_iterparse  | 65.0 ms                                                     | 68.4 ms: 1.05x slower                                                                 |
| pickle               | 6.85 us                                                     | 7.37 us: 1.08x slower                                                                 |
| pickle_list          | 2.75 us                                                     | 2.99 us: 1.09x slower                                                                 |
| pickle_dict          | 17.2 us                                                     | 18.8 us: 1.09x slower                                                                 |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                          |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.8 ms: 1.01x slower                                                                 |
| python_startup_no_site | 15.5 ms                                                     | 18.8 ms: 1.21x slower                                                                 |
| Geometric mean         | (ref)                                                       | 1.11x slower                                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|-----------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.53 ms: 1.20x faster                                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c |
|--------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 75.3 us: 4.46x faster                                                                 |
| logging_silent           | 94.6 ns                                                     | 55.2 ns: 1.72x faster                                                                 |
| richards_super           | 52.2 ms                                                     | 30.6 ms: 1.71x faster                                                                 |
| json_dumps               | 9.16 ms                                                     | 5.76 ms: 1.59x faster                                                                 |
| deltablue                | 4.19 ms                                                     | 2.65 ms: 1.58x faster                                                                 |
| async_tree_none          | 435 ms                                                      | 276 ms: 1.58x faster                                                                  |
| raytrace                 | 273 ms                                                      | 174 ms: 1.57x faster                                                                  |
| richards                 | 42.4 ms                                                     | 27.3 ms: 1.55x faster                                                                 |
| sqlglot_parse            | 1.22 ms                                                     | 787 us: 1.54x faster                                                                  |
| go                       | 139 ms                                                      | 93.0 ms: 1.49x faster                                                                 |
| pickle_pure_python       | 270 us                                                      | 181 us: 1.49x faster                                                                  |
| async_tree_memoization   | 526 ms                                                      | 355 ms: 1.48x faster                                                                  |
| scimark_lu               | 85.8 ms                                                     | 57.9 ms: 1.48x faster                                                                 |
| asyncio_tcp              | 732 ms                                                      | 495 ms: 1.48x faster                                                                  |
| generators               | 32.4 ms                                                     | 22.0 ms: 1.47x faster                                                                 |
| async_tree_io            | 1.11 sec                                                    | 756 ms: 1.47x faster                                                                  |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.45x faster                                                                 |
| chaos                    | 61.7 ms                                                     | 43.1 ms: 1.43x faster                                                                 |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.52 sec: 1.39x faster                                                                |
| pycparser                | 930 ms                                                      | 687 ms: 1.35x faster                                                                  |
| unpickle_pure_python     | 183 us                                                      | 135 us: 1.35x faster                                                                  |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 473 ms: 1.35x faster                                                                  |
| scimark_sor              | 106 ms                                                      | 79.0 ms: 1.34x faster                                                                 |
| crypto_pyaes             | 62.5 ms                                                     | 48.1 ms: 1.30x faster                                                                 |
| comprehensions           | 16.5 us                                                     | 12.8 us: 1.28x faster                                                                 |
| mypy2                    | 555 ms                                                      | 437 ms: 1.27x faster                                                                  |
| pyflate                  | 409 ms                                                      | 322 ms: 1.27x faster                                                                  |
| regex_compile            | 106 ms                                                      | 84.6 ms: 1.25x faster                                                                 |
| mdp                      | 1.78 sec                                                    | 1.43 sec: 1.24x faster                                                                |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                                 |
| tornado_http             | 108 ms                                                      | 88.1 ms: 1.23x faster                                                                 |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.0 ms: 1.22x faster                                                                 |
| deepcopy_memo            | 28.8 us                                                     | 23.7 us: 1.21x faster                                                                 |
| sympy_sum                | 107 ms                                                      | 89.1 ms: 1.20x faster                                                                 |
| sqlite_synth             | 1.91 us                                                     | 1.59 us: 1.20x faster                                                                 |
| mako                     | 9.03 ms                                                     | 7.53 ms: 1.20x faster                                                                 |
| docutils                 | 1.92 sec                                                    | 1.61 sec: 1.19x faster                                                                |
| dask                     | 313 ms                                                      | 265 ms: 1.18x faster                                                                  |
| xml_etree_process        | 44.5 ms                                                     | 37.8 ms: 1.18x faster                                                                 |
| hexiom                   | 5.74 ms                                                     | 4.90 ms: 1.17x faster                                                                 |
| tomli_loads              | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                                                |
| sympy_str                | 194 ms                                                      | 166 ms: 1.17x faster                                                                  |
| dulwich_log              | 50.5 ms                                                     | 43.2 ms: 1.17x faster                                                                 |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                                 |
| chameleon                | 5.79 ms                                                     | 5.05 ms: 1.14x faster                                                                 |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                                |
| deepcopy                 | 255 us                                                      | 226 us: 1.13x faster                                                                  |
| pprint_safe_repr         | 592 ms                                                      | 523 ms: 1.13x faster                                                                  |
| sqlglot_optimize         | 39.8 ms                                                     | 35.7 ms: 1.12x faster                                                                 |
| regex_dna                | 136 ms                                                      | 123 ms: 1.11x faster                                                                  |
| sympy_expand             | 314 ms                                                      | 284 ms: 1.11x faster                                                                  |
| bench_thread_pool        | 958 us                                                      | 868 us: 1.10x faster                                                                  |
| deepcopy_reduce          | 2.20 us                                                     | 2.00 us: 1.10x faster                                                                 |
| sqlglot_normalize        | 205 ms                                                      | 186 ms: 1.10x faster                                                                  |
| 2to3                     | 246 ms                                                      | 224 ms: 1.10x faster                                                                  |
| float                    | 61.7 ms                                                     | 56.6 ms: 1.09x faster                                                                 |
| create_gc_cycles         | 800 us                                                      | 737 us: 1.09x faster                                                                  |
| unpickle                 | 9.09 us                                                     | 8.48 us: 1.07x faster                                                                 |
| regex_effbot             | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                                                 |
| nqueens                  | 66.6 ms                                                     | 64.7 ms: 1.03x faster                                                                 |
| xml_etree_parse          | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                                 |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                                 |
| unpack_sequence          | 39.6 ns                                                     | 39.0 ns: 1.02x faster                                                                 |
| logging_format           | 6.76 us                                                     | 6.66 us: 1.01x faster                                                                 |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                                                  |
| logging_simple           | 6.22 us                                                     | 6.20 us: 1.00x faster                                                                 |
| meteor_contest           | 75.9 ms                                                     | 76.5 ms: 1.01x slower                                                                 |
| python_startup           | 20.6 ms                                                     | 20.8 ms: 1.01x slower                                                                 |
| regex_v8                 | 15.4 ms                                                     | 15.7 ms: 1.02x slower                                                                 |
| unpickle_list            | 2.71 us                                                     | 2.78 us: 1.02x slower                                                                 |
| async_generators         | 222 ms                                                      | 228 ms: 1.03x slower                                                                  |
| spectral_norm            | 77.3 ms                                                     | 80.1 ms: 1.04x slower                                                                 |
| scimark_fft              | 187 ms                                                      | 195 ms: 1.04x slower                                                                  |
| fannkuch                 | 256 ms                                                      | 269 ms: 1.05x slower                                                                  |
| xml_etree_iterparse      | 65.0 ms                                                     | 68.4 ms: 1.05x slower                                                                 |
| pathlib                  | 75.7 ms                                                     | 81.1 ms: 1.07x slower                                                                 |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                                                 |
| pickle                   | 6.85 us                                                     | 7.37 us: 1.08x slower                                                                 |
| nbody                    | 71.3 ms                                                     | 76.8 ms: 1.08x slower                                                                 |
| pickle_list              | 2.75 us                                                     | 2.99 us: 1.09x slower                                                                 |
| pickle_dict              | 17.2 us                                                     | 18.8 us: 1.09x slower                                                                 |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.02 ms: 1.11x slower                                                                 |
| bench_mp_pool            | 62.0 ms                                                     | 69.2 ms: 1.12x slower                                                                 |
| telco                    | 3.94 ms                                                     | 4.64 ms: 1.18x slower                                                                 |
| python_startup_no_site   | 15.5 ms                                                     | 18.8 ms: 1.21x slower                                                                 |
| coverage                 | 39.0 ms                                                     | 47.7 ms: 1.22x slower                                                                 |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                          |

Benchmark hidden because not significant (2): json, xml_etree_generate
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240129-3.13.0a3+-fcdc84c-PYTHON_UOPS/bm-20240129-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-fcdc84c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown