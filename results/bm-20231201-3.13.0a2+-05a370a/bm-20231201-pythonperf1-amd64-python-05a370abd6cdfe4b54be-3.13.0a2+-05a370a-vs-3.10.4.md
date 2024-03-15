
# Results vs. 3.10.4

- fork: python
- ref: 05a370abd6cdfe4b54be
- machine: windows-amd64
- commit hash: 05a370a
- commit date: 2023-12-01
- overall geometric mean: 1.18x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.21 ms: 1.11x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                      |
| tornado_http   | 108 ms                                                      | 88.4 ms: 1.23x faster                                                       |
| Geometric mean | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 276 ms: 1.58x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 352 ms: 1.49x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 743 ms: 1.49x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 465 ms: 1.37x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.48x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 75.8 ms: 1.06x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 86.6 ms: 1.22x faster                                                       |
| regex_dna      | 136 ms                                                      | 120 ms: 1.14x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.86 ms: 1.56x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 195 us: 1.38x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 142 us: 1.29x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 39.9 ms: 1.11x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.51 sec: 1.11x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.44 us: 1.08x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.7 ms: 1.02x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.66 us: 1.02x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.81 us: 1.02x slower                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 57.8 ms: 1.04x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                                |

Benchmark hidden because not significant (2): pickle, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.3 ms: 1.02x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.2 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.07 ms: 1.28x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 80.1 us: 4.20x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.25 ms: 1.86x faster                                                       |
| async_tree_none          | 435 ms                                                      | 276 ms: 1.58x faster                                                        |
| raytrace                 | 273 ms                                                      | 173 ms: 1.58x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.86 ms: 1.56x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 480 ms: 1.52x faster                                                        |
| go                       | 139 ms                                                      | 92.1 ms: 1.51x faster                                                       |
| richards_super           | 52.2 ms                                                     | 34.7 ms: 1.50x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 63.1 ns: 1.50x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 352 ms: 1.49x faster                                                        |
| chaos                    | 61.7 ms                                                     | 41.3 ms: 1.49x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 743 ms: 1.49x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 824 us: 1.47x faster                                                        |
| comprehensions           | 16.5 us                                                     | 11.2 us: 1.47x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.05 ms: 1.41x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 61.0 ms: 1.41x faster                                                       |
| generators               | 32.4 ms                                                     | 23.3 ms: 1.39x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 195 us: 1.38x faster                                                        |
| richards                 | 42.4 ms                                                     | 30.9 ms: 1.37x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 465 ms: 1.37x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 45.8 ms: 1.36x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 4.29 ms: 1.34x faster                                                       |
| pyflate                  | 409 ms                                                      | 306 ms: 1.34x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 43.3 ms: 1.32x faster                                                       |
| mypy2                    | 555 ms                                                      | 426 ms: 1.31x faster                                                        |
| scimark_sor              | 106 ms                                                      | 82.0 ms: 1.29x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.38 sec: 1.29x faster                                                      |
| unpickle_pure_python     | 183 us                                                      | 142 us: 1.29x faster                                                        |
| mako                     | 9.03 ms                                                     | 7.07 ms: 1.28x faster                                                       |
| sympy_sum                | 107 ms                                                      | 85.1 ms: 1.26x faster                                                       |
| tornado_http             | 108 ms                                                      | 88.4 ms: 1.23x faster                                                       |
| regex_compile            | 106 ms                                                      | 86.6 ms: 1.22x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.22x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 12.8 ms: 1.19x faster                                                       |
| sympy_str                | 194 ms                                                      | 163 ms: 1.19x faster                                                        |
| dask                     | 313 ms                                                      | 264 ms: 1.18x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 65.6 ms: 1.18x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 43.2 ms: 1.17x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 25.2 us: 1.14x faster                                                       |
| float                    | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                                       |
| regex_dna                | 136 ms                                                      | 120 ms: 1.14x faster                                                        |
| 2to3                     | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 35.4 ms: 1.13x faster                                                       |
| sympy_expand             | 314 ms                                                      | 281 ms: 1.12x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.12x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 39.9 ms: 1.11x faster                                                       |
| pycparser                | 930 ms                                                      | 836 ms: 1.11x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.90 sec: 1.11x faster                                                      |
| chameleon                | 5.79 ms                                                     | 5.21 ms: 1.11x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 535 ms: 1.11x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.51 sec: 1.11x faster                                                      |
| bench_thread_pool        | 958 us                                                      | 868 us: 1.10x faster                                                        |
| coroutines               | 16.0 ms                                                     | 14.6 ms: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 733 us: 1.09x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 188 ms: 1.09x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.44 us: 1.08x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.57 ms: 1.06x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 63.1 ms: 1.05x faster                                                       |
| deepcopy                 | 255 us                                                      | 244 us: 1.05x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 14.7 ms: 1.05x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.13 us: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 38.5 ns: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.7 ms: 1.02x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.66 us: 1.02x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.3 ms: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| scimark_fft              | 187 ms                                                      | 186 ms: 1.01x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.88 us: 1.02x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.81 us: 1.02x slower                                                       |
| logging_simple           | 6.22 us                                                     | 6.47 us: 1.04x slower                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 57.8 ms: 1.04x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 64.7 ms: 1.04x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.48 ms: 1.05x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| nbody                    | 71.3 ms                                                     | 75.8 ms: 1.06x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 80.6 ms: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 236 ms: 1.07x slower                                                        |
| fannkuch                 | 256 ms                                                      | 275 ms: 1.07x slower                                                        |
| python_startup_no_site   | 15.5 ms                                                     | 18.2 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.0 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 5.01 ms: 1.27x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.18x faster                                                                |

Benchmark hidden because not significant (4): json, pickle, meteor_contest, xml_etree_iterparse
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231201-3.13.0a2+-05a370a/bm-20231201-pythonperf1-amd64-python-05a370abd6cdfe4b54be-3.13.0a2+-05a370a.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown