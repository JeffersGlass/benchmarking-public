
# Results vs. 3.10.4

- fork: python
- ref: 2feec0fc7fd0b9caae7a
- machine: windows-amd64
- commit hash: 2feec0f
- commit date: 2023-12-18
- overall geometric mean: 1.19x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| tornado_http   | 108 ms                                                      | 88.0 ms: 1.23x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 341 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 456 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 57.1 ms: 1.08x faster                                                       |
| pidigits       | 149 ms                                                      | 151 ms: 1.01x slower                                                        |
| nbody          | 71.3 ms                                                     | 82.3 ms: 1.15x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 84.4 ms: 1.26x faster                                                       |
| regex_dna      | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.1 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.11x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.62 ms: 1.63x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 181 us: 1.49x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 135 us: 1.35x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.1 ms: 1.20x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.47 sec: 1.14x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.37 us: 1.09x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.3 us: 1.05x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 94.2 ms: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.8 ms: 1.01x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.19 us: 1.05x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.39 us: 1.23x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.3 ms: 1.02x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.1 ms: 1.17x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.96 ms: 1.30x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 74.3 us: 4.52x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.8 ns: 1.73x faster                                                       |
| richards_super           | 52.2 ms                                                     | 30.7 ms: 1.70x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.62 ms: 1.63x faster                                                       |
| async_tree_none          | 435 ms                                                      | 268 ms: 1.62x faster                                                        |
| raytrace                 | 273 ms                                                      | 173 ms: 1.58x faster                                                        |
| deltablue                | 4.19 ms                                                     | 2.67 ms: 1.57x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 775 us: 1.57x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 341 ms: 1.54x faster                                                        |
| richards                 | 42.4 ms                                                     | 27.6 ms: 1.54x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 478 ms: 1.53x faster                                                        |
| go                       | 139 ms                                                      | 91.2 ms: 1.52x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 56.5 ms: 1.52x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 733 ms: 1.51x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 181 us: 1.49x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 997 us: 1.48x faster                                                        |
| generators               | 32.4 ms                                                     | 22.2 ms: 1.46x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 456 ms: 1.40x faster                                                        |
| chaos                    | 61.7 ms                                                     | 44.6 ms: 1.38x faster                                                       |
| scimark_sor              | 106 ms                                                      | 77.1 ms: 1.38x faster                                                       |
| pycparser                | 930 ms                                                      | 684 ms: 1.36x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 135 us: 1.35x faster                                                        |
| mypy2                    | 555 ms                                                      | 420 ms: 1.32x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 47.8 ms: 1.31x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.96 ms: 1.30x faster                                                       |
| comprehensions           | 16.5 us                                                     | 12.8 us: 1.28x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 22.6 us: 1.27x faster                                                       |
| pyflate                  | 409 ms                                                      | 321 ms: 1.27x faster                                                        |
| regex_compile            | 106 ms                                                      | 84.4 ms: 1.26x faster                                                       |
| coroutines               | 16.0 ms                                                     | 12.8 ms: 1.25x faster                                                       |
| sympy_sum                | 107 ms                                                      | 86.1 ms: 1.24x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.44 sec: 1.23x faster                                                      |
| tornado_http             | 108 ms                                                      | 88.0 ms: 1.23x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.23x faster                                                       |
| dask                     | 313 ms                                                      | 256 ms: 1.22x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.74 sec: 1.22x faster                                                      |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 37.1 ms: 1.20x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| sympy_str                | 194 ms                                                      | 167 ms: 1.17x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 43.3 ms: 1.17x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.1 ms: 1.16x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 49.5 ms: 1.16x faster                                                       |
| hexiom                   | 5.74 ms                                                     | 4.99 ms: 1.15x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.47 sec: 1.14x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 520 ms: 1.14x faster                                                        |
| sympy_expand             | 314 ms                                                      | 276 ms: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 226 us: 1.13x faster                                                        |
| 2to3                     | 246 ms                                                      | 218 ms: 1.13x faster                                                        |
| regex_dna                | 136 ms                                                      | 121 ms: 1.13x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 183 ms: 1.12x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.97 us: 1.12x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 876 us: 1.09x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.37 us: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 739 us: 1.08x faster                                                        |
| float                    | 61.7 ms                                                     | 57.1 ms: 1.08x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.57 ms: 1.05x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.3 us: 1.05x faster                                                       |
| nqueens                  | 66.6 ms                                                     | 63.9 ms: 1.04x faster                                                       |
| json                     | 3.14 ms                                                     | 3.01 ms: 1.04x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 94.2 ms: 1.03x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.58 us: 1.03x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.1 ms: 1.02x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.3 ms: 1.02x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.8 ms: 1.01x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 39.2 ns: 1.01x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.16 us: 1.01x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 75.6 ms: 1.00x faster                                                       |
| pidigits                 | 149 ms                                                      | 151 ms: 1.01x slower                                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 67.0 ms: 1.03x slower                                                       |
| async_generators         | 222 ms                                                      | 230 ms: 1.04x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.19 us: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.48 ms: 1.05x slower                                                       |
| spectral_norm            | 77.3 ms                                                     | 82.6 ms: 1.07x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 81.9 ms: 1.08x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 67.5 ms: 1.09x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.7 us: 1.09x slower                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.98 ms: 1.09x slower                                                       |
| scimark_fft              | 187 ms                                                      | 209 ms: 1.11x slower                                                        |
| fannkuch                 | 256 ms                                                      | 291 ms: 1.14x slower                                                        |
| coverage                 | 39.0 ms                                                     | 44.9 ms: 1.15x slower                                                       |
| nbody                    | 71.3 ms                                                     | 82.3 ms: 1.15x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.1 ms: 1.17x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.75 ms: 1.21x slower                                                       |
| pickle_list              | 2.75 us                                                     | 3.39 us: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.19x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231218-3.13.0a2+-2feec0f-PYTHON_UOPS/bm-20231218-pythonperf1-amd64-python-2feec0fc7fd0b9caae7a-3.13.0a2+-2feec0f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.14x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: unknown