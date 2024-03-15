
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: windows-amd64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.19x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 214 ms: 1.15x faster                                                         |
| chameleon      | 5.79 ms                                                     | 4.71 ms: 1.23x faster                                                        |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                       |
| tornado_http   | 108 ms                                                      | 83.9 ms: 1.29x faster                                                        |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 261 ms: 1.67x faster                                                         |
| async_tree_memoization  | 526 ms                                                      | 334 ms: 1.58x faster                                                         |
| async_tree_io           | 1.11 sec                                                    | 714 ms: 1.55x faster                                                         |
| async_tree_cpu_io_mixed | 638 ms                                                      | 447 ms: 1.43x faster                                                         |
| Geometric mean          | (ref)                                                       | 1.55x faster                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                        |
| nbody          | 71.3 ms                                                     | 58.4 ms: 1.22x faster                                                        |
| pidigits       | 149 ms                                                      | 151 ms: 1.01x slower                                                         |
| Geometric mean | (ref)                                                       | 1.15x faster                                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 76.9 ms: 1.38x faster                                                        |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                         |
| regex_effbot   | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 15.1 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.53 ms: 1.66x faster                                                        |
| pickle_pure_python   | 270 us                                                      | 174 us: 1.55x faster                                                         |
| unpickle_pure_python | 183 us                                                      | 123 us: 1.49x faster                                                         |
| tomli_loads          | 1.67 sec                                                    | 1.19 sec: 1.41x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 36.1 ms: 1.23x faster                                                        |
| unpickle             | 9.09 us                                                     | 8.50 us: 1.07x faster                                                        |
| xml_etree_generate   | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                        |
| xml_etree_parse      | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                        |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                        |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                        |
| pickle_dict          | 17.2 us                                                     | 17.5 us: 1.02x slower                                                        |
| unpickle_list        | 2.71 us                                                     | 2.78 us: 1.02x slower                                                        |
| pickle               | 6.85 us                                                     | 7.10 us: 1.04x slower                                                        |
| pickle_list          | 2.75 us                                                     | 3.13 us: 1.14x slower                                                        |
| Geometric mean       | (ref)                                                       | 1.15x faster                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.1 ms: 1.03x faster                                                        |
| python_startup_no_site | 15.5 ms                                                     | 18.0 ms: 1.16x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 5.98 ms: 1.51x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:-----------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.5 us: 4.77x faster                                                        |
| deltablue                | 4.19 ms                                                     | 1.94 ms: 2.16x faster                                                        |
| richards_super           | 52.2 ms                                                     | 27.9 ms: 1.87x faster                                                        |
| logging_silent           | 94.6 ns                                                     | 52.0 ns: 1.82x faster                                                        |
| richards                 | 42.4 ms                                                     | 24.8 ms: 1.71x faster                                                        |
| async_tree_none          | 435 ms                                                      | 261 ms: 1.67x faster                                                         |
| json_dumps               | 9.16 ms                                                     | 5.53 ms: 1.66x faster                                                        |
| raytrace                 | 273 ms                                                      | 167 ms: 1.64x faster                                                         |
| sqlglot_parse            | 1.22 ms                                                     | 747 us: 1.63x faster                                                         |
| generators               | 32.4 ms                                                     | 19.9 ms: 1.63x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 54.4 ms: 1.58x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 334 ms: 1.58x faster                                                         |
| comprehensions           | 16.5 us                                                     | 10.6 us: 1.56x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 714 ms: 1.55x faster                                                         |
| asyncio_tcp              | 732 ms                                                      | 472 ms: 1.55x faster                                                         |
| pickle_pure_python       | 270 us                                                      | 174 us: 1.55x faster                                                         |
| go                       | 139 ms                                                      | 90.0 ms: 1.54x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 963 us: 1.53x faster                                                         |
| chaos                    | 61.7 ms                                                     | 40.6 ms: 1.52x faster                                                        |
| mako                     | 9.03 ms                                                     | 5.98 ms: 1.51x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 123 us: 1.49x faster                                                         |
| pyflate                  | 409 ms                                                      | 284 ms: 1.44x faster                                                         |
| crypto_pyaes             | 62.5 ms                                                     | 43.5 ms: 1.44x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 447 ms: 1.43x faster                                                         |
| spectral_norm            | 77.3 ms                                                     | 54.4 ms: 1.42x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.19 sec: 1.41x faster                                                       |
| scimark_sor              | 106 ms                                                      | 76.1 ms: 1.39x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 20.7 us: 1.39x faster                                                        |
| regex_compile            | 106 ms                                                      | 76.9 ms: 1.38x faster                                                        |
| pycparser                | 930 ms                                                      | 686 ms: 1.36x faster                                                         |
| mypy2                    | 555 ms                                                      | 420 ms: 1.32x faster                                                         |
| hexiom                   | 5.74 ms                                                     | 4.44 ms: 1.29x faster                                                        |
| tornado_http             | 108 ms                                                      | 83.9 ms: 1.29x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 950 ms: 1.28x faster                                                         |
| dulwich_log              | 50.5 ms                                                     | 39.6 ms: 1.27x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 465 ms: 1.27x faster                                                         |
| sqlite_synth             | 1.91 us                                                     | 1.51 us: 1.27x faster                                                        |
| coroutines               | 16.0 ms                                                     | 12.8 ms: 1.25x faster                                                        |
| float                    | 61.7 ms                                                     | 49.5 ms: 1.25x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.69 sec: 1.25x faster                                                       |
| sympy_sum                | 107 ms                                                      | 86.5 ms: 1.24x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.1 ms: 1.23x faster                                                        |
| dask                     | 313 ms                                                      | 254 ms: 1.23x faster                                                         |
| chameleon                | 5.79 ms                                                     | 4.71 ms: 1.23x faster                                                        |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                       |
| nbody                    | 71.3 ms                                                     | 58.4 ms: 1.22x faster                                                        |
| sympy_str                | 194 ms                                                      | 161 ms: 1.20x faster                                                         |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.6 ms: 1.20x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 33.3 ms: 1.20x faster                                                        |
| deepcopy                 | 255 us                                                      | 214 us: 1.19x faster                                                         |
| bench_thread_pool        | 958 us                                                      | 803 us: 1.19x faster                                                         |
| sympy_integrate          | 15.3 ms                                                     | 12.8 ms: 1.19x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 174 ms: 1.18x faster                                                         |
| fannkuch                 | 256 ms                                                      | 218 ms: 1.17x faster                                                         |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.33 ms: 1.17x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.54 sec: 1.15x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 1.91 us: 1.15x faster                                                        |
| 2to3                     | 246 ms                                                      | 214 ms: 1.15x faster                                                         |
| sympy_expand             | 314 ms                                                      | 275 ms: 1.15x faster                                                         |
| nqueens                  | 66.6 ms                                                     | 58.2 ms: 1.14x faster                                                        |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                         |
| create_gc_cycles         | 800 us                                                      | 735 us: 1.09x faster                                                         |
| unpickle                 | 9.09 us                                                     | 8.50 us: 1.07x faster                                                        |
| logging_simple           | 6.22 us                                                     | 5.84 us: 1.07x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.35 us: 1.06x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 52.2 ms: 1.06x faster                                                        |
| scimark_fft              | 187 ms                                                      | 176 ms: 1.06x faster                                                         |
| regex_effbot             | 1.66 ms                                                     | 1.58 ms: 1.05x faster                                                        |
| meteor_contest           | 75.9 ms                                                     | 72.4 ms: 1.05x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 92.7 ms: 1.04x faster                                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.7 ms: 1.04x faster                                                        |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                        |
| python_startup           | 20.6 ms                                                     | 20.1 ms: 1.03x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 15.1 ms: 1.02x faster                                                        |
| unpack_sequence          | 39.6 ns                                                     | 38.8 ns: 1.02x faster                                                        |
| pathlib                  | 75.7 ms                                                     | 75.2 ms: 1.01x faster                                                        |
| pidigits                 | 149 ms                                                      | 151 ms: 1.01x slower                                                         |
| pickle_dict              | 17.2 us                                                     | 17.5 us: 1.02x slower                                                        |
| unpickle_list            | 2.71 us                                                     | 2.78 us: 1.02x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.10 us: 1.04x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 65.6 ms: 1.06x slower                                                        |
| async_generators         | 222 ms                                                      | 235 ms: 1.06x slower                                                         |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                        |
| json                     | 3.14 ms                                                     | 3.38 ms: 1.08x slower                                                        |
| pickle_list              | 2.75 us                                                     | 3.13 us: 1.14x slower                                                        |
| telco                    | 3.94 ms                                                     | 4.53 ms: 1.15x slower                                                        |
| python_startup_no_site   | 15.5 ms                                                     | 18.0 ms: 1.16x slower                                                        |
| coverage                 | 39.0 ms                                                     | 47.0 ms: 1.21x slower                                                        |
| Geometric mean           | (ref)                                                       | 1.26x faster                                                                 |
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-6dafac2-JIT/bm-20240212-pythonperf1-amd64-brandtbucher-justin_continue-3.13.0a3+-6dafac2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.19x


# Memory

- memory change: unknown