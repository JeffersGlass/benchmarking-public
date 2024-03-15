
# Results vs. 3.10.4

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-amd64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 213 ms: 1.15x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.90 ms: 1.18x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.53 sec: 1.25x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.2 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                       | 1.21x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 264 ms: 1.65x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 716 ms: 1.55x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 446 ms: 1.43x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.54x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 51.3 ms: 1.20x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody          | 71.3 ms                                                     | 72.8 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 78.0 ms: 1.36x faster                                                       |
| regex_dna      | 136 ms                                                      | 117 ms: 1.17x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 128 us: 1.43x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.8 ms: 1.21x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 92.9 ms: 1.04x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.73 us: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.5 ms: 1.02x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                       |
| pickle_list          | 2.75 us                                                     | 2.82 us: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.18 us: 1.05x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.07x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.08x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.48 ms: 1.39x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 71.9 us: 4.67x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.03 ms: 2.07x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.0 ns: 1.72x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.2 ms: 1.67x faster                                                       |
| async_tree_none          | 435 ms                                                      | 264 ms: 1.65x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| raytrace                 | 273 ms                                                      | 169 ms: 1.62x faster                                                        |
| go                       | 139 ms                                                      | 86.0 ms: 1.62x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.6 us: 1.55x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 472 ms: 1.55x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 716 ms: 1.55x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 785 us: 1.55x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.5 ms: 1.54x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 55.7 ms: 1.54x faster                                                       |
| chaos                    | 61.7 ms                                                     | 40.1 ms: 1.54x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 180 us: 1.50x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.87 ms: 1.48x faster                                                       |
| generators               | 32.4 ms                                                     | 21.9 ms: 1.48x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 999 us: 1.48x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 43.1 ms: 1.45x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 128 us: 1.43x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 446 ms: 1.43x faster                                                        |
| pyflate                  | 409 ms                                                      | 287 ms: 1.42x faster                                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 40.9 ms: 1.40x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.48 ms: 1.39x faster                                                       |
| regex_compile            | 106 ms                                                      | 78.0 ms: 1.36x faster                                                       |
| mypy2                    | 555 ms                                                      | 413 ms: 1.35x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.34 sec: 1.33x faster                                                      |
| scimark_sor              | 106 ms                                                      | 80.2 ms: 1.32x faster                                                       |
| pycparser                | 930 ms                                                      | 713 ms: 1.31x faster                                                        |
| sympy_sum                | 107 ms                                                      | 82.4 ms: 1.30x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 22.4 us: 1.28x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 60.4 ms: 1.28x faster                                                       |
| tornado_http             | 108 ms                                                      | 86.2 ms: 1.26x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.53 sec: 1.25x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 12.3 ms: 1.24x faster                                                       |
| dask                     | 313 ms                                                      | 253 ms: 1.24x faster                                                        |
| sympy_str                | 194 ms                                                      | 159 ms: 1.22x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 41.4 ms: 1.22x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.22x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.21x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.01 sec: 1.21x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 36.8 ms: 1.21x faster                                                       |
| float                    | 61.7 ms                                                     | 51.3 ms: 1.20x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 493 ms: 1.20x faster                                                        |
| chameleon                | 5.79 ms                                                     | 4.90 ms: 1.18x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 33.9 ms: 1.17x faster                                                       |
| regex_dna                | 136 ms                                                      | 117 ms: 1.17x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.82 sec: 1.16x faster                                                      |
| sqlglot_normalize        | 205 ms                                                      | 178 ms: 1.16x faster                                                        |
| 2to3                     | 246 ms                                                      | 213 ms: 1.15x faster                                                        |
| sympy_expand             | 314 ms                                                      | 273 ms: 1.15x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 838 us: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 224 us: 1.14x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.94 us: 1.14x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 58.9 ms: 1.13x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 715 us: 1.12x faster                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.48 ms: 1.10x faster                                                       |
| json                     | 3.14 ms                                                     | 2.88 ms: 1.09x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 71.5 ms: 1.06x faster                                                       |
| fannkuch                 | 256 ms                                                      | 244 ms: 1.05x faster                                                        |
| scimark_fft              | 187 ms                                                      | 179 ms: 1.05x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 92.9 ms: 1.04x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.73 us: 1.04x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.50 us: 1.04x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.5 ms: 1.02x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.3 ms: 1.02x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.08 us: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.01x faster                                                        |
| nbody                    | 71.3 ms                                                     | 72.8 ms: 1.02x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.82 us: 1.03x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 79.2 ms: 1.05x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.18 us: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                                       |
| async_generators         | 222 ms                                                      | 235 ms: 1.06x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.07x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 66.7 ms: 1.07x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.3 ms: 1.18x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.2 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.80 ms: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.24x faster                                                                |

Benchmark hidden because not significant (3): unpickle_list, python_startup, unpack_sequence
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown