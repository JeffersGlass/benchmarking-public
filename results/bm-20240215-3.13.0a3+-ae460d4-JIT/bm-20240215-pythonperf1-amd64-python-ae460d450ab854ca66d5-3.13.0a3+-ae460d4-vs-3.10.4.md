
# Results vs. 3.10.4

- fork: python
- ref: ae460d450ab854ca66d5
- machine: windows-amd64
- commit hash: ae460d4
- commit date: 2024-02-15
- overall geometric mean: 1.23x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.80 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.0 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.21x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 261 ms: 1.67x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 709 ms: 1.56x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 337 ms: 1.56x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 447 ms: 1.43x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.55x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.5 ms: 1.22x faster                                                       |
| nbody          | 71.3 ms                                                     | 61.4 ms: 1.16x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 80.1 ms: 1.32x faster                                                       |
| regex_dna      | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 126 us: 1.45x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.46 us: 1.07x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.0 ms: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 91.5 ms: 1.06x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| pickle               | 6.85 us                                                     | 7.31 us: 1.07x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.92 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.66 ms: 1.36x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.1 us: 4.79x faster                                                       |
| deltablue                | 4.19 ms                                                     | 1.99 ms: 2.10x faster                                                       |
| richards_super           | 52.2 ms                                                     | 28.4 ms: 1.84x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.6 ns: 1.73x faster                                                       |
| async_tree_none          | 435 ms                                                      | 261 ms: 1.67x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.56 ms: 1.65x faster                                                       |
| richards                 | 42.4 ms                                                     | 25.8 ms: 1.65x faster                                                       |
| generators               | 32.4 ms                                                     | 19.9 ms: 1.63x faster                                                       |
| raytrace                 | 273 ms                                                      | 171 ms: 1.60x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 763 us: 1.59x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 709 ms: 1.56x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 337 ms: 1.56x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 469 ms: 1.56x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.8 us: 1.53x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 56.4 ms: 1.52x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 975 us: 1.51x faster                                                        |
| chaos                    | 61.7 ms                                                     | 41.9 ms: 1.47x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 126 us: 1.45x faster                                                        |
| go                       | 139 ms                                                      | 96.0 ms: 1.45x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 447 ms: 1.43x faster                                                        |
| scimark_sor              | 106 ms                                                      | 77.8 ms: 1.36x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.66 ms: 1.36x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 46.4 ms: 1.35x faster                                                       |
| pycparser                | 930 ms                                                      | 691 ms: 1.35x faster                                                        |
| regex_compile            | 106 ms                                                      | 80.1 ms: 1.32x faster                                                       |
| pyflate                  | 409 ms                                                      | 309 ms: 1.32x faster                                                        |
| mypy2                    | 555 ms                                                      | 422 ms: 1.32x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| sqlite_synth             | 1.91 us                                                     | 1.49 us: 1.28x faster                                                       |
| tornado_http             | 108 ms                                                      | 85.0 ms: 1.27x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.67 sec: 1.26x faster                                                      |
| deepcopy_memo            | 28.8 us                                                     | 22.8 us: 1.26x faster                                                       |
| sympy_sum                | 107 ms                                                      | 85.4 ms: 1.25x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 40.5 ms: 1.25x faster                                                       |
| dask                     | 313 ms                                                      | 253 ms: 1.24x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.0 ms: 1.24x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 988 ms: 1.23x faster                                                        |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| sympy_str                | 194 ms                                                      | 158 ms: 1.23x faster                                                        |
| float                    | 61.7 ms                                                     | 50.5 ms: 1.22x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.22x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 486 ms: 1.22x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 63.8 ms: 1.21x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.80 ms: 1.21x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 170 ms: 1.20x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 33.3 ms: 1.20x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.0 ms: 1.17x faster                                                       |
| nbody                    | 71.3 ms                                                     | 61.4 ms: 1.16x faster                                                       |
| deepcopy                 | 255 us                                                      | 220 us: 1.16x faster                                                        |
| regex_dna                | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 838 us: 1.14x faster                                                        |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.94 us: 1.14x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 59.3 ms: 1.12x faster                                                       |
| sympy_expand             | 314 ms                                                      | 281 ms: 1.12x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.15 ms: 1.12x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.60 sec: 1.11x faster                                                      |
| create_gc_cycles         | 800 us                                                      | 732 us: 1.09x faster                                                        |
| json                     | 3.14 ms                                                     | 2.89 ms: 1.08x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.46 us: 1.07x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.0 ms: 1.07x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| fannkuch                 | 256 ms                                                      | 241 ms: 1.06x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 91.5 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.45 us: 1.05x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.95 us: 1.04x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.63 ms: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| pickle_list              | 2.75 us                                                     | 2.73 us: 1.01x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.9 ms: 1.01x faster                                                       |
| scimark_fft              | 187 ms                                                      | 190 ms: 1.01x slower                                                        |
| meteor_contest           | 75.9 ms                                                     | 77.3 ms: 1.02x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 41.6 ns: 1.05x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.31 us: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 236 ms: 1.07x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 66.3 ms: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.92 us: 1.08x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.60 ms: 1.17x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.3 ms: 1.19x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.23x faster                                                                |

Benchmark hidden because not significant (2): python_startup, pathlib
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240215-3.13.0a3+-ae460d4-JIT/bm-20240215-pythonperf1-amd64-python-ae460d450ab854ca66d5-3.13.0a3+-ae460d4.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown