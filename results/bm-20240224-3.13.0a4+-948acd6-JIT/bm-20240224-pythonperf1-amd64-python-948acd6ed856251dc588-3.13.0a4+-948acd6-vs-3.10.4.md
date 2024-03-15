
# Results vs. 3.10.4

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 227 ms: 1.08x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.80 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.6 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 265 ms: 1.64x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 728 ms: 1.52x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 454 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.0 ms: 1.24x faster                                                       |
| nbody          | 71.3 ms                                                     | 61.9 ms: 1.15x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| regex_compile  | 106 ms                                                      | 104 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 176 us: 1.53x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 142 us: 1.29x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.32 sec: 1.27x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.9 ms: 1.20x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.50 us: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.3 ms: 1.05x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.8 us: 1.02x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.78 us: 1.02x slower                                                       |
| pickle               | 6.85 us                                                     | 7.33 us: 1.07x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.10 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.2 ms: 1.13x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 20.9 ms: 1.35x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.23x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.45 ms: 1.40x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 70.8 us: 4.75x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.18 ms: 1.92x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 55.4 ns: 1.71x faster                                                       |
| async_tree_none          | 435 ms                                                      | 265 ms: 1.64x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.59 ms: 1.64x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 339 ms: 1.55x faster                                                        |
| generators               | 32.4 ms                                                     | 20.9 ms: 1.55x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 475 ms: 1.54x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 176 us: 1.53x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 728 ms: 1.52x faster                                                        |
| richards_super           | 52.2 ms                                                     | 35.0 ms: 1.49x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 824 us: 1.48x faster                                                        |
| raytrace                 | 273 ms                                                      | 191 ms: 1.43x faster                                                        |
| chaos                    | 61.7 ms                                                     | 43.5 ms: 1.42x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.04 ms: 1.42x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 454 ms: 1.40x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.45 ms: 1.40x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 46.1 ms: 1.36x faster                                                       |
| richards                 | 42.4 ms                                                     | 31.4 ms: 1.35x faster                                                       |
| comprehensions           | 16.5 us                                                     | 12.2 us: 1.35x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 21.8 us: 1.32x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 142 us: 1.29x faster                                                        |
| go                       | 139 ms                                                      | 109 ms: 1.28x faster                                                        |
| pycparser                | 930 ms                                                      | 730 ms: 1.28x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.32 sec: 1.27x faster                                                      |
| tornado_http             | 108 ms                                                      | 85.6 ms: 1.27x faster                                                       |
| pyflate                  | 409 ms                                                      | 328 ms: 1.25x faster                                                        |
| float                    | 61.7 ms                                                     | 50.0 ms: 1.24x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.57 us: 1.22x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.2 ms: 1.21x faster                                                       |
| mypy2                    | 555 ms                                                      | 459 ms: 1.21x faster                                                        |
| chameleon                | 5.79 ms                                                     | 4.80 ms: 1.21x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 36.9 ms: 1.20x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 47.6 ms: 1.20x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 64.5 ms: 1.20x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.80 sec: 1.17x faster                                                      |
| dulwich_log              | 50.5 ms                                                     | 43.2 ms: 1.17x faster                                                       |
| nbody                    | 71.3 ms                                                     | 61.9 ms: 1.15x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.67 sec: 1.15x faster                                                      |
| regex_dna                | 136 ms                                                      | 119 ms: 1.15x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 517 ms: 1.15x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                      |
| deepcopy                 | 255 us                                                      | 224 us: 1.14x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 841 us: 1.14x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.94 us: 1.14x faster                                                       |
| sympy_sum                | 107 ms                                                      | 94.2 ms: 1.14x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 76.6 ms: 1.12x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 184 ms: 1.12x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 36.1 ms: 1.10x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 14.0 ms: 1.09x faster                                                       |
| sympy_str                | 194 ms                                                      | 179 ms: 1.09x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 738 us: 1.08x faster                                                        |
| 2to3                     | 246 ms                                                      | 227 ms: 1.08x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.50 us: 1.07x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.68 sec: 1.06x faster                                                      |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.06x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 92.3 ms: 1.05x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.3 ms: 1.04x faster                                                       |
| scimark_sor              | 106 ms                                                      | 102 ms: 1.04x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.53 us: 1.03x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.63 ms: 1.03x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 64.7 ms: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                       |
| regex_compile            | 106 ms                                                      | 104 ms: 1.02x faster                                                        |
| json_loads               | 14.0 us                                                     | 13.8 us: 1.02x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.13 us: 1.01x faster                                                       |
| sympy_expand             | 314 ms                                                      | 310 ms: 1.01x faster                                                        |
| pathlib                  | 75.7 ms                                                     | 76.1 ms: 1.01x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 76.9 ms: 1.01x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.6 us: 1.02x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.78 us: 1.02x slower                                                       |
| fannkuch                 | 256 ms                                                      | 263 ms: 1.03x slower                                                        |
| scimark_fft              | 187 ms                                                      | 194 ms: 1.03x slower                                                        |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.06x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.33 us: 1.07x slower                                                       |
| hexiom                   | 5.74 ms                                                     | 6.28 ms: 1.09x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 69.4 ms: 1.12x slower                                                       |
| python_startup           | 20.6 ms                                                     | 23.2 ms: 1.13x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.10 us: 1.13x slower                                                       |
| async_generators         | 222 ms                                                      | 255 ms: 1.15x slower                                                        |
| telco                    | 3.94 ms                                                     | 4.59 ms: 1.16x slower                                                       |
| coverage                 | 39.0 ms                                                     | 48.0 ms: 1.23x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 20.9 ms: 1.35x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 88.5 ns: 2.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.16x faster                                                                |

Benchmark hidden because not significant (2): json, regex_v8
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown