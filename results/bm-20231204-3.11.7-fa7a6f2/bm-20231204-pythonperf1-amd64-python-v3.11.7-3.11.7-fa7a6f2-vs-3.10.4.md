
# Results vs. 3.10.4

- fork: python
- ref: v3.11.7
- machine: windows-amd64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.14x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 209 ms: 1.18x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.02 ms: 1.15x faster                                       |
| docutils       | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                      |
| html5lib       | 51.0 ms                                                     | 38.5 ms: 1.33x faster                                       |
| tornado_http   | 108 ms                                                      | 89.7 ms: 1.21x faster                                       |
| Geometric mean | (ref)                                                       | 1.21x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 784 ms: 1.41x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 380 ms: 1.38x faster                                        |
| async_tree_none         | 435 ms                                                      | 317 ms: 1.37x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 523 ms: 1.22x faster                                        |
| Geometric mean          | (ref)                                                       | 1.35x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                       |
| nbody          | 71.3 ms                                                     | 70.8 ms: 1.01x faster                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 88.3 ms: 1.20x faster                                       |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                        |
| regex_v8       | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.54 ms: 1.08x faster                                       |
| Geometric mean | (ref)                                                       | 1.14x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 201 us: 1.34x faster                                        |
| unpickle_pure_python | 183 us                                                      | 149 us: 1.23x faster                                        |
| tomli_loads          | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.2 ms: 1.19x faster                                       |
| unpickle             | 9.09 us                                                     | 7.74 us: 1.17x faster                                       |
| json_dumps           | 9.16 ms                                                     | 7.86 ms: 1.17x faster                                       |
| json_loads           | 14.0 us                                                     | 12.8 us: 1.10x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                       |
| pickle               | 6.85 us                                                     | 6.55 us: 1.04x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.60 us: 1.04x faster                                       |
| pickle_list          | 2.75 us                                                     | 2.66 us: 1.03x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 64.3 ms: 1.01x faster                                       |
| xml_etree_parse      | 96.8 ms                                                     | 98.1 ms: 1.01x slower                                       |
| pickle_dict          | 17.2 us                                                     | 18.4 us: 1.07x slower                                       |
| Geometric mean       | (ref)                                                       | 1.10x faster                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 15.7 ms: 1.01x slower                                       |
| Geometric mean         | (ref)                                                       | 1.00x faster                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.29 ms: 1.24x faster                                       |
| django_template | 28.9 ms                                                     | 23.7 ms: 1.22x faster                                       |
| genshi_text     | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 38.0 ms: 1.08x faster                                       |
| Geometric mean  | (ref)                                                       | 1.17x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.62 ms: 1.60x faster                                       |
| scimark_sor              | 106 ms                                                      | 74.5 ms: 1.42x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 784 ms: 1.41x faster                                        |
| richards                 | 42.4 ms                                                     | 30.2 ms: 1.41x faster                                       |
| scimark_lu               | 85.8 ms                                                     | 61.5 ms: 1.40x faster                                       |
| async_tree_memoization   | 526 ms                                                      | 380 ms: 1.38x faster                                        |
| async_tree_none          | 435 ms                                                      | 317 ms: 1.37x faster                                        |
| richards_super           | 52.2 ms                                                     | 38.2 ms: 1.37x faster                                       |
| logging_silent           | 94.6 ns                                                     | 69.6 ns: 1.36x faster                                       |
| raytrace                 | 273 ms                                                      | 202 ms: 1.35x faster                                        |
| go                       | 139 ms                                                      | 103 ms: 1.35x faster                                        |
| pickle_pure_python       | 270 us                                                      | 201 us: 1.34x faster                                        |
| pyflate                  | 409 ms                                                      | 305 ms: 1.34x faster                                        |
| pycparser                | 930 ms                                                      | 697 ms: 1.34x faster                                        |
| html5lib                 | 51.0 ms                                                     | 38.5 ms: 1.33x faster                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.13 ms: 1.30x faster                                       |
| sqlglot_parse            | 1.22 ms                                                     | 933 us: 1.30x faster                                        |
| hexiom                   | 5.74 ms                                                     | 4.45 ms: 1.29x faster                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 44.4 ms: 1.29x faster                                       |
| async_generators         | 222 ms                                                      | 172 ms: 1.29x faster                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.6 ms: 1.29x faster                                       |
| chaos                    | 61.7 ms                                                     | 49.1 ms: 1.26x faster                                       |
| mako                     | 9.03 ms                                                     | 7.29 ms: 1.24x faster                                       |
| sqlalchemy_declarative   | 103 ms                                                      | 83.7 ms: 1.24x faster                                       |
| unpickle_pure_python     | 183 us                                                      | 149 us: 1.23x faster                                        |
| thrift                   | 617 us                                                      | 503 us: 1.23x faster                                        |
| mypy2                    | 555 ms                                                      | 454 ms: 1.22x faster                                        |
| django_template          | 28.9 ms                                                     | 23.7 ms: 1.22x faster                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 523 ms: 1.22x faster                                        |
| docutils                 | 1.92 sec                                                    | 1.58 sec: 1.21x faster                                      |
| tornado_http             | 108 ms                                                      | 89.7 ms: 1.21x faster                                       |
| regex_compile            | 106 ms                                                      | 88.3 ms: 1.20x faster                                       |
| tomli_loads              | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                      |
| xml_etree_process        | 44.5 ms                                                     | 37.2 ms: 1.19x faster                                       |
| dask                     | 313 ms                                                      | 264 ms: 1.19x faster                                        |
| 2to3                     | 246 ms                                                      | 209 ms: 1.18x faster                                        |
| unpickle                 | 9.09 us                                                     | 7.74 us: 1.17x faster                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.17x faster                                      |
| json_dumps               | 9.16 ms                                                     | 7.86 ms: 1.17x faster                                       |
| spectral_norm            | 77.3 ms                                                     | 66.3 ms: 1.17x faster                                       |
| deepcopy_memo            | 28.8 us                                                     | 24.7 us: 1.17x faster                                       |
| aiohttp                  | 995 us                                                      | 854 us: 1.17x faster                                        |
| pprint_safe_repr         | 592 ms                                                      | 509 ms: 1.16x faster                                        |
| genshi_text              | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                       |
| chameleon                | 5.79 ms                                                     | 5.02 ms: 1.15x faster                                       |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                       |
| float                    | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                       |
| bench_thread_pool        | 958 us                                                      | 842 us: 1.14x faster                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.70 us: 1.13x faster                                       |
| regex_v8                 | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                       |
| dulwich_log              | 50.5 ms                                                     | 45.0 ms: 1.12x faster                                       |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.2 ms: 1.11x faster                                       |
| pylint                   | 350 ms                                                      | 316 ms: 1.11x faster                                        |
| create_gc_cycles         | 800 us                                                      | 721 us: 1.11x faster                                        |
| json_loads               | 14.0 us                                                     | 12.8 us: 1.10x faster                                       |
| sympy_sum                | 107 ms                                                      | 98.9 ms: 1.08x faster                                       |
| mdp                      | 1.78 sec                                                    | 1.65 sec: 1.08x faster                                      |
| deepcopy_reduce          | 2.20 us                                                     | 2.04 us: 1.08x faster                                       |
| genshi_xml               | 41.0 ms                                                     | 38.0 ms: 1.08x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.54 ms: 1.08x faster                                       |
| coroutines               | 16.0 ms                                                     | 14.9 ms: 1.07x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 192 ms: 1.07x faster                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.56 ms: 1.07x faster                                       |
| pathlib                  | 75.7 ms                                                     | 71.2 ms: 1.06x faster                                       |
| deepcopy                 | 255 us                                                      | 242 us: 1.06x faster                                        |
| sympy_str                | 194 ms                                                      | 184 ms: 1.05x faster                                        |
| comprehensions           | 16.5 us                                                     | 15.7 us: 1.05x faster                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.9 ms: 1.05x faster                                       |
| scimark_fft              | 187 ms                                                      | 179 ms: 1.05x faster                                        |
| pickle                   | 6.85 us                                                     | 6.55 us: 1.04x faster                                       |
| unpickle_list            | 2.71 us                                                     | 2.60 us: 1.04x faster                                       |
| fannkuch                 | 256 ms                                                      | 245 ms: 1.04x faster                                        |
| nqueens                  | 66.6 ms                                                     | 64.1 ms: 1.04x faster                                       |
| sympy_expand             | 314 ms                                                      | 303 ms: 1.04x faster                                        |
| pickle_list              | 2.75 us                                                     | 2.66 us: 1.03x faster                                       |
| typing_runtime_protocols | 336 us                                                      | 327 us: 1.03x faster                                        |
| bench_mp_pool            | 62.0 ms                                                     | 60.8 ms: 1.02x faster                                       |
| telco                    | 3.94 ms                                                     | 3.89 ms: 1.01x faster                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 64.3 ms: 1.01x faster                                       |
| nbody                    | 71.3 ms                                                     | 70.8 ms: 1.01x faster                                       |
| flaskblogging            | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                      |
| python_startup_no_site   | 15.5 ms                                                     | 15.7 ms: 1.01x slower                                       |
| xml_etree_parse          | 96.8 ms                                                     | 98.1 ms: 1.01x slower                                       |
| gc_traversal             | 1.41 ms                                                     | 1.46 ms: 1.04x slower                                       |
| generators               | 32.4 ms                                                     | 34.0 ms: 1.05x slower                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 2.23 sec: 1.06x slower                                      |
| pickle_dict              | 17.2 us                                                     | 18.4 us: 1.07x slower                                       |
| logging_format           | 6.76 us                                                     | 7.25 us: 1.07x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.76 us: 1.09x slower                                       |
| coverage                 | 39.0 ms                                                     | 43.9 ms: 1.13x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 47.9 ns: 1.21x slower                                       |
| Geometric mean           | (ref)                                                       | 1.14x faster                                                |

Benchmark hidden because not significant (5): python_startup, asyncio_tcp, pidigits, meteor_contest, json
Ignored benchmarks (4) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-pythonperf1-amd64-python-v3.11.7-3.11.7-fa7a6f2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.12x
- 99% likely to have a speedup of 1.10x


# Memory

- memory change: unknown