
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 212 ms: 1.16x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.98 ms: 1.16x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 84.0 ms: 1.29x faster                                                       |
| Geometric mean | (ref)                                                       | 1.21x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 341 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 738 ms: 1.50x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 453 ms: 1.41x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.3 ms: 1.14x faster                                                       |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 72.9 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 79.8 ms: 1.33x faster                                                       |
| regex_dna      | 136 ms                                                      | 120 ms: 1.13x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.6 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 185 us: 1.46x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 133 us: 1.38x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.41 sec: 1.18x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.58 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 64.1 ms: 1.01x faster                                                       |
| json_loads           | 14.0 us                                                     | 14.0 us: 1.01x faster                                                       |
| pickle               | 6.85 us                                                     | 7.14 us: 1.04x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.00 us: 1.09x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 17.6 ms: 1.14x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.05x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.49 ms: 1.39x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.8 us: 4.61x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.03 ms: 2.06x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.5 ns: 1.70x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.3 ms: 1.67x faster                                                       |
| raytrace                 | 273 ms                                                      | 166 ms: 1.65x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| async_tree_none          | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| go                       | 139 ms                                                      | 85.7 ms: 1.62x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 52.9 ms: 1.62x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 463 ms: 1.58x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.6 us: 1.56x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 781 us: 1.56x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 341 ms: 1.54x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.7 ms: 1.53x faster                                                       |
| chaos                    | 61.7 ms                                                     | 40.4 ms: 1.53x faster                                                       |
| generators               | 32.4 ms                                                     | 21.5 ms: 1.51x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 738 ms: 1.50x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.89 ms: 1.48x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.00 ms: 1.47x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 185 us: 1.46x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 44.3 ms: 1.41x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 453 ms: 1.41x faster                                                        |
| pyflate                  | 409 ms                                                      | 291 ms: 1.40x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 41.0 ms: 1.40x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.49 ms: 1.39x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 133 us: 1.38x faster                                                        |
| scimark_sor              | 106 ms                                                      | 77.2 ms: 1.37x faster                                                       |
| mypy2                    | 555 ms                                                      | 415 ms: 1.34x faster                                                        |
| regex_compile            | 106 ms                                                      | 79.8 ms: 1.33x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.37 sec: 1.30x faster                                                      |
| deepcopy_memo            | 28.8 us                                                     | 22.3 us: 1.29x faster                                                       |
| tornado_http             | 108 ms                                                      | 84.0 ms: 1.29x faster                                                       |
| sympy_sum                | 107 ms                                                      | 83.7 ms: 1.28x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 40.4 ms: 1.25x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.57 sec: 1.23x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 12.5 ms: 1.22x faster                                                       |
| sympy_str                | 194 ms                                                      | 160 ms: 1.22x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| pycparser                | 930 ms                                                      | 770 ms: 1.21x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.75 sec: 1.21x faster                                                      |
| sqlite_synth             | 1.91 us                                                     | 1.59 us: 1.20x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 64.4 ms: 1.20x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 33.4 ms: 1.19x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.03 sec: 1.19x faster                                                      |
| tomli_loads              | 1.67 sec                                                    | 1.41 sec: 1.18x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 501 ms: 1.18x faster                                                        |
| coroutines               | 16.0 ms                                                     | 13.5 ms: 1.18x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 177 ms: 1.16x faster                                                        |
| 2to3                     | 246 ms                                                      | 212 ms: 1.16x faster                                                        |
| chameleon                | 5.79 ms                                                     | 4.98 ms: 1.16x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 828 us: 1.16x faster                                                        |
| sympy_expand             | 314 ms                                                      | 275 ms: 1.14x faster                                                        |
| float                    | 61.7 ms                                                     | 54.3 ms: 1.14x faster                                                       |
| regex_dna                | 136 ms                                                      | 120 ms: 1.13x faster                                                        |
| deepcopy                 | 255 us                                                      | 227 us: 1.12x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 714 us: 1.12x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 59.8 ms: 1.11x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.45 ms: 1.11x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 1.99 us: 1.11x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 36.7 ns: 1.08x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.58 us: 1.06x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 71.9 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                       |
| scimark_fft              | 187 ms                                                      | 179 ms: 1.04x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.51 us: 1.04x faster                                                       |
| python_startup           | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.1 ms: 1.03x faster                                                       |
| fannkuch                 | 256 ms                                                      | 249 ms: 1.03x faster                                                        |
| logging_simple           | 6.22 us                                                     | 6.06 us: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 64.1 ms: 1.01x faster                                                       |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                                        |
| json_loads               | 14.0 us                                                     | 14.0 us: 1.01x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 76.1 ms: 1.01x slower                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.6 ms: 1.01x slower                                                       |
| async_generators         | 222 ms                                                      | 226 ms: 1.02x slower                                                        |
| nbody                    | 71.3 ms                                                     | 72.9 ms: 1.02x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 64.0 ms: 1.03x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.14 us: 1.04x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.2 us: 1.06x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.00 us: 1.09x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.6 ms: 1.14x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.2 ms: 1.21x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.86 ms: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                                |

Benchmark hidden because not significant (2): unpickle_list, json
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown