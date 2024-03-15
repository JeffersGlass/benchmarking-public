
# Results vs. 3.10.4

- fork: python
- ref: 384429d1c0cf011dcf88
- machine: windows-amd64
- commit hash: 384429d
- commit date: 2024-01-24
- overall geometric mean: 1.17x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.12 ms: 1.13x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.62 sec: 1.18x faster                                                      |
| tornado_http   | 108 ms                                                      | 88.3 ms: 1.23x faster                                                       |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 349 ms: 1.51x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 742 ms: 1.49x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 472 ms: 1.35x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.3 ms: 1.10x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 78.4 ms: 1.10x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.4 ms: 1.26x faster                                                       |
| regex_dna      | 136 ms                                                      | 118 ms: 1.16x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.70 ms: 1.61x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 183 us: 1.47x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 137 us: 1.34x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.35 us: 1.09x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.65 us: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.02x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 56.0 ms: 1.01x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 68.2 ms: 1.05x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.89 us: 1.05x slower                                                       |
| pickle               | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.24 ms: 1.25x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 75.7 us: 4.44x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.1 ns: 1.69x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.0 ms: 1.69x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.70 ms: 1.61x faster                                                       |
| async_tree_none          | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| raytrace                 | 273 ms                                                      | 174 ms: 1.57x faster                                                        |
| deltablue                | 4.19 ms                                                     | 2.68 ms: 1.56x faster                                                       |
| richards                 | 42.4 ms                                                     | 27.6 ms: 1.54x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 349 ms: 1.51x faster                                                        |
| go                       | 139 ms                                                      | 92.4 ms: 1.50x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 810 us: 1.50x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 742 ms: 1.49x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 491 ms: 1.49x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 183 us: 1.47x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 59.2 ms: 1.45x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.44x faster                                                       |
| generators               | 32.4 ms                                                     | 22.6 ms: 1.43x faster                                                       |
| chaos                    | 61.7 ms                                                     | 44.1 ms: 1.40x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 472 ms: 1.35x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 137 us: 1.34x faster                                                        |
| pycparser                | 930 ms                                                      | 721 ms: 1.29x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.6 ms: 1.29x faster                                                       |
| mypy2                    | 555 ms                                                      | 434 ms: 1.28x faster                                                        |
| comprehensions           | 16.5 us                                                     | 13.0 us: 1.27x faster                                                       |
| scimark_sor              | 106 ms                                                      | 84.4 ms: 1.26x faster                                                       |
| regex_compile            | 106 ms                                                      | 84.4 ms: 1.26x faster                                                       |
| pyflate                  | 409 ms                                                      | 326 ms: 1.25x faster                                                        |
| mako                     | 9.03 ms                                                     | 7.24 ms: 1.25x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 23.2 us: 1.24x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.44 sec: 1.24x faster                                                      |
| tornado_http             | 108 ms                                                      | 88.3 ms: 1.23x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| sympy_sum                | 107 ms                                                      | 89.2 ms: 1.20x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.8 ms: 1.20x faster                                                       |
| dask                     | 313 ms                                                      | 264 ms: 1.19x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 4.85 ms: 1.19x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.62 sec: 1.18x faster                                                      |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 38.2 ms: 1.16x faster                                                       |
| sympy_str                | 194 ms                                                      | 167 ms: 1.16x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 43.5 ms: 1.16x faster                                                       |
| regex_dna                | 136 ms                                                      | 118 ms: 1.16x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.08 sec: 1.13x faster                                                      |
| chameleon                | 5.79 ms                                                     | 5.12 ms: 1.13x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 525 ms: 1.13x faster                                                        |
| deepcopy                 | 255 us                                                      | 228 us: 1.12x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 183 ms: 1.12x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 35.6 ms: 1.12x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.90 sec: 1.11x faster                                                      |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| sympy_expand             | 314 ms                                                      | 285 ms: 1.10x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 871 us: 1.10x faster                                                        |
| float                    | 61.7 ms                                                     | 56.3 ms: 1.10x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.01 us: 1.09x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.35 us: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 748 us: 1.07x faster                                                        |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 64.9 ms: 1.03x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.65 us: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 95.2 ms: 1.02x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.69 us: 1.01x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 75.3 ms: 1.01x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.18 us: 1.01x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 39.9 ns: 1.01x slower                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 56.0 ms: 1.01x slower                                                       |
| fannkuch                 | 256 ms                                                      | 264 ms: 1.03x slower                                                        |
| async_generators         | 222 ms                                                      | 232 ms: 1.05x slower                                                        |
| spectral_norm            | 77.3 ms                                                     | 81.0 ms: 1.05x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 68.2 ms: 1.05x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.89 us: 1.05x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 80.5 ms: 1.06x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.30 us: 1.07x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.09x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 68.2 ms: 1.10x slower                                                       |
| nbody                    | 71.3 ms                                                     | 78.4 ms: 1.10x slower                                                       |
| scimark_fft              | 187 ms                                                      | 207 ms: 1.10x slower                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.05 ms: 1.12x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.67 ms: 1.19x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.7 ms: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.17x faster                                                                |

Benchmark hidden because not significant (2): python_startup, json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240124-3.13.0a3+-384429d-PYTHON_UOPS/bm-20240124-pythonperf1-amd64-python-384429d1c0cf011dcf88-3.13.0a3+-384429d.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown