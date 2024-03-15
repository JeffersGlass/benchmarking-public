
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 225 ms: 1.09x faster                                                        |
| chameleon      | 5.79 ms                                                     | 5.07 ms: 1.14x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.66 sec: 1.15x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.2 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 271 ms: 1.60x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 345 ms: 1.52x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 458 ms: 1.39x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.51x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 59.0 ms: 1.05x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 81.4 ms: 1.14x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 118 ms: 1.15x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| regex_compile  | 106 ms                                                      | 102 ms: 1.03x faster                                                        |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.68 ms: 1.61x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 186 us: 1.45x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 38.8 ms: 1.14x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.32 us: 1.09x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 168 us: 1.09x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.58 sec: 1.06x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.01x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 56.8 ms: 1.02x slower                                                       |
| pickle               | 6.85 us                                                     | 7.03 us: 1.03x slower                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 68.6 ms: 1.06x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.20 us: 1.16x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 17.9 ms: 1.16x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 7.55 ms: 1.20x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 75.3 us: 4.46x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.35 ms: 1.78x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.9 ns: 1.66x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.68 ms: 1.61x faster                                                       |
| async_tree_none          | 435 ms                                                      | 271 ms: 1.60x faster                                                        |
| generators               | 32.4 ms                                                     | 20.6 ms: 1.57x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 466 ms: 1.57x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 345 ms: 1.52x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| richards_super           | 52.2 ms                                                     | 35.7 ms: 1.47x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 835 us: 1.46x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 186 us: 1.45x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 458 ms: 1.39x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.06 ms: 1.39x faster                                                       |
| raytrace                 | 273 ms                                                      | 202 ms: 1.36x faster                                                        |
| chaos                    | 61.7 ms                                                     | 45.7 ms: 1.35x faster                                                       |
| go                       | 139 ms                                                      | 104 ms: 1.33x faster                                                        |
| richards                 | 42.4 ms                                                     | 31.9 ms: 1.33x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 47.9 ms: 1.31x faster                                                       |
| tornado_http             | 108 ms                                                      | 86.2 ms: 1.26x faster                                                       |
| mypy2                    | 555 ms                                                      | 445 ms: 1.25x faster                                                        |
| pycparser                | 930 ms                                                      | 746 ms: 1.25x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.46 sec: 1.22x faster                                                      |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.76 sec: 1.20x faster                                                      |
| mako                     | 9.03 ms                                                     | 7.55 ms: 1.20x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.60 us: 1.20x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 24.8 us: 1.16x faster                                                       |
| pyflate                  | 409 ms                                                      | 352 ms: 1.16x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 43.6 ms: 1.16x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.66 sec: 1.15x faster                                                      |
| regex_dna                | 136 ms                                                      | 118 ms: 1.15x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 38.8 ms: 1.14x faster                                                       |
| chameleon                | 5.79 ms                                                     | 5.07 ms: 1.14x faster                                                       |
| comprehensions           | 16.5 us                                                     | 14.5 us: 1.14x faster                                                       |
| sympy_sum                | 107 ms                                                      | 94.0 ms: 1.14x faster                                                       |
| scimark_sor              | 106 ms                                                      | 94.1 ms: 1.13x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 863 us: 1.11x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 2.01 us: 1.10x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.32 us: 1.09x faster                                                       |
| deepcopy                 | 255 us                                                      | 234 us: 1.09x faster                                                        |
| 2to3                     | 246 ms                                                      | 225 ms: 1.09x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 168 us: 1.09x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 36.6 ms: 1.09x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 14.1 ms: 1.09x faster                                                       |
| sympy_str                | 194 ms                                                      | 179 ms: 1.09x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 189 ms: 1.08x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 738 us: 1.08x faster                                                        |
| json                     | 3.14 ms                                                     | 2.91 ms: 1.08x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.58 sec: 1.06x faster                                                      |
| scimark_lu               | 85.8 ms                                                     | 81.1 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| sympy_expand             | 314 ms                                                      | 300 ms: 1.05x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 54.7 ms: 1.05x faster                                                       |
| float                    | 61.7 ms                                                     | 59.0 ms: 1.05x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.17 sec: 1.04x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 569 ms: 1.04x faster                                                        |
| regex_compile            | 106 ms                                                      | 102 ms: 1.03x faster                                                        |
| python_startup           | 20.6 ms                                                     | 19.9 ms: 1.03x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 5.61 ms: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.01x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.75 us: 1.01x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 76.9 ms: 1.01x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 76.8 ms: 1.01x slower                                                       |
| logging_format           | 6.76 us                                                     | 6.86 us: 1.02x slower                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 56.8 ms: 1.02x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.03 us: 1.03x slower                                                       |
| logging_simple           | 6.22 us                                                     | 6.42 us: 1.03x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 65.0 ms: 1.05x slower                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 68.6 ms: 1.06x slower                                                       |
| fannkuch                 | 256 ms                                                      | 273 ms: 1.07x slower                                                        |
| unpack_sequence          | 39.6 ns                                                     | 42.4 ns: 1.07x slower                                                       |
| nqueens                  | 66.6 ms                                                     | 71.4 ms: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 237 ms: 1.07x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| spectral_norm            | 77.3 ms                                                     | 83.5 ms: 1.08x slower                                                       |
| nbody                    | 71.3 ms                                                     | 81.4 ms: 1.14x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.9 ms: 1.16x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.20 us: 1.16x slower                                                       |
| scimark_fft              | 187 ms                                                      | 219 ms: 1.17x slower                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 3.22 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.5 ms: 1.22x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.85 ms: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.14x faster                                                                |

Benchmark hidden because not significant (1): regex_v8
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6-PYTHON_UOPS/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.07x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown