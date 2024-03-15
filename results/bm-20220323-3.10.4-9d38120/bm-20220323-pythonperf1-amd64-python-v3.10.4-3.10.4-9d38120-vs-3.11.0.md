
# Results vs. 3.11.0

- fork: python
- ref: v3.10.4
- machine: windows-amd64
- commit hash: 9d38120
- commit date: 2022-03-23
- overall geometric mean: 1.12x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 246 ms: 1.15x slower                                        |
| chameleon      | 5.26 ms                                                     | 5.79 ms: 1.10x slower                                       |
| docutils       | 1.64 sec                                                    | 1.92 sec: 1.17x slower                                      |
| html5lib       | 38.9 ms                                                     | 51.0 ms: 1.31x slower                                       |
| tornado_http   | 92.8 ms                                                     | 108 ms: 1.17x slower                                        |
| Geometric mean | (ref)                                                       | 1.18x slower                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 638 ms: 1.20x slower                                        |
| async_tree_none         | 332 ms                                                      | 435 ms: 1.31x slower                                        |
| async_tree_memoization  | 399 ms                                                      | 526 ms: 1.32x slower                                        |
| async_tree_io           | 808 ms                                                      | 1.11 sec: 1.37x slower                                      |
| Geometric mean          | (ref)                                                       | 1.30x slower                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 149 ms: 1.01x faster                                        |
| nbody          | 70.3 ms                                                     | 71.3 ms: 1.01x slower                                       |
| float          | 54.4 ms                                                     | 61.7 ms: 1.13x slower                                       |
| Geometric mean | (ref)                                                       | 1.05x slower                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 15.4 ms: 1.09x slower                                       |
| regex_effbot   | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                       |
| regex_compile  | 91.0 ms                                                     | 106 ms: 1.16x slower                                        |
| regex_dna      | 116 ms                                                      | 136 ms: 1.17x slower                                        |
| Geometric mean | (ref)                                                       | 1.13x slower                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 17.2 us: 1.08x faster                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                       |
| pickle_list          | 2.70 us                                                     | 2.75 us: 1.02x slower                                       |
| pickle               | 6.64 us                                                     | 6.85 us: 1.03x slower                                       |
| unpickle_list        | 2.59 us                                                     | 2.71 us: 1.05x slower                                       |
| xml_etree_generate   | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                       |
| json_loads           | 13.0 us                                                     | 14.0 us: 1.08x slower                                       |
| json_dumps           | 8.09 ms                                                     | 9.16 ms: 1.13x slower                                       |
| tomli_loads          | 1.46 sec                                                    | 1.67 sec: 1.15x slower                                      |
| unpickle_pure_python | 157 us                                                      | 183 us: 1.17x slower                                        |
| xml_etree_process    | 37.2 ms                                                     | 44.5 ms: 1.20x slower                                       |
| unpickle             | 7.57 us                                                     | 9.09 us: 1.20x slower                                       |
| pickle_pure_python   | 208 us                                                      | 270 us: 1.29x slower                                        |
| Geometric mean       | (ref)                                                       | 1.09x slower                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.5 ms: 1.08x faster                                       |
| python_startup         | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                       |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| genshi_xml      | 39.9 ms                                                     | 41.0 ms: 1.03x slower                                       |
| genshi_text     | 18.4 ms                                                     | 19.8 ms: 1.07x slower                                       |
| django_template | 24.4 ms                                                     | 28.9 ms: 1.18x slower                                       |
| mako            | 7.58 ms                                                     | 9.03 ms: 1.19x slower                                       |
| Geometric mean  | (ref)                                                       | 1.12x slower                                                |

All benchmarks:
===============

| Benchmark                | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| unpack_sequence          | 46.9 ns                                                     | 39.6 ns: 1.18x faster                                       |
| coverage                 | 43.4 ms                                                     | 39.0 ms: 1.11x faster                                       |
| logging_simple           | 6.86 us                                                     | 6.22 us: 1.10x faster                                       |
| python_startup_no_site   | 16.8 ms                                                     | 15.5 ms: 1.08x faster                                       |
| pickle_dict              | 18.5 us                                                     | 17.2 us: 1.08x faster                                       |
| logging_format           | 7.16 us                                                     | 6.76 us: 1.06x faster                                       |
| gc_traversal             | 1.49 ms                                                     | 1.41 ms: 1.06x faster                                       |
| generators               | 34.0 ms                                                     | 32.4 ms: 1.05x faster                                       |
| telco                    | 4.06 ms                                                     | 3.94 ms: 1.03x faster                                       |
| nqueens                  | 68.3 ms                                                     | 66.6 ms: 1.03x faster                                       |
| bench_mp_pool            | 63.2 ms                                                     | 62.0 ms: 1.02x faster                                       |
| xml_etree_iterparse      | 65.6 ms                                                     | 65.0 ms: 1.01x faster                                       |
| pidigits                 | 150 ms                                                      | 149 ms: 1.01x faster                                        |
| meteor_contest           | 75.2 ms                                                     | 75.9 ms: 1.01x slower                                       |
| fannkuch                 | 253 ms                                                      | 256 ms: 1.01x slower                                        |
| nbody                    | 70.3 ms                                                     | 71.3 ms: 1.01x slower                                       |
| pickle_list              | 2.70 us                                                     | 2.75 us: 1.02x slower                                       |
| genshi_xml               | 39.9 ms                                                     | 41.0 ms: 1.03x slower                                       |
| typing_runtime_protocols | 326 us                                                      | 336 us: 1.03x slower                                        |
| pickle                   | 6.64 us                                                     | 6.85 us: 1.03x slower                                       |
| deepcopy                 | 246 us                                                      | 255 us: 1.04x slower                                        |
| asyncio_tcp_ssl          | 2.03 sec                                                    | 2.11 sec: 1.04x slower                                      |
| python_startup           | 19.8 ms                                                     | 20.6 ms: 1.04x slower                                       |
| scimark_fft              | 179 ms                                                      | 187 ms: 1.05x slower                                        |
| unpickle_list            | 2.59 us                                                     | 2.71 us: 1.05x slower                                       |
| sympy_str                | 185 ms                                                      | 194 ms: 1.05x slower                                        |
| sympy_expand             | 299 ms                                                      | 314 ms: 1.05x slower                                        |
| json                     | 2.98 ms                                                     | 3.14 ms: 1.05x slower                                       |
| comprehensions           | 15.6 us                                                     | 16.5 us: 1.06x slower                                       |
| xml_etree_generate       | 52.5 ms                                                     | 55.5 ms: 1.06x slower                                       |
| scimark_sparse_mat_mult  | 2.58 ms                                                     | 2.72 ms: 1.06x slower                                       |
| pathlib                  | 70.9 ms                                                     | 75.7 ms: 1.07x slower                                       |
| coroutines               | 15.0 ms                                                     | 16.0 ms: 1.07x slower                                       |
| sympy_sum                | 100 ms                                                      | 107 ms: 1.07x slower                                        |
| deepcopy_reduce          | 2.06 us                                                     | 2.20 us: 1.07x slower                                       |
| genshi_text              | 18.4 ms                                                     | 19.8 ms: 1.07x slower                                       |
| json_loads               | 13.0 us                                                     | 14.0 us: 1.08x slower                                       |
| sqlglot_normalize        | 190 ms                                                      | 205 ms: 1.08x slower                                        |
| sqlite_synth             | 1.77 us                                                     | 1.91 us: 1.08x slower                                       |
| pylint                   | 323 ms                                                      | 350 ms: 1.08x slower                                        |
| dulwich_log              | 46.4 ms                                                     | 50.5 ms: 1.09x slower                                       |
| sympy_integrate          | 14.0 ms                                                     | 15.3 ms: 1.09x slower                                       |
| regex_v8                 | 14.2 ms                                                     | 15.4 ms: 1.09x slower                                       |
| sqlalchemy_imperative    | 10.4 ms                                                     | 11.4 ms: 1.09x slower                                       |
| bench_thread_pool        | 872 us                                                      | 958 us: 1.10x slower                                        |
| chameleon                | 5.26 ms                                                     | 5.79 ms: 1.10x slower                                       |
| regex_effbot             | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                       |
| deepcopy_memo            | 26.0 us                                                     | 28.8 us: 1.11x slower                                       |
| mdp                      | 1.59 sec                                                    | 1.78 sec: 1.12x slower                                      |
| pprint_safe_repr         | 529 ms                                                      | 592 ms: 1.12x slower                                        |
| create_gc_cycles         | 713 us                                                      | 800 us: 1.12x slower                                        |
| pprint_pformat           | 1.09 sec                                                    | 1.22 sec: 1.12x slower                                      |
| aiohttp                  | 883 us                                                      | 995 us: 1.13x slower                                        |
| spectral_norm            | 68.3 ms                                                     | 77.3 ms: 1.13x slower                                       |
| json_dumps               | 8.09 ms                                                     | 9.16 ms: 1.13x slower                                       |
| float                    | 54.4 ms                                                     | 61.7 ms: 1.13x slower                                       |
| dask                     | 273 ms                                                      | 313 ms: 1.15x slower                                        |
| tomli_loads              | 1.46 sec                                                    | 1.67 sec: 1.15x slower                                      |
| 2to3                     | 214 ms                                                      | 246 ms: 1.15x slower                                        |
| sqlglot_optimize         | 34.5 ms                                                     | 39.8 ms: 1.15x slower                                       |
| regex_compile            | 91.0 ms                                                     | 106 ms: 1.16x slower                                        |
| tornado_http             | 92.8 ms                                                     | 108 ms: 1.17x slower                                        |
| unpickle_pure_python     | 157 us                                                      | 183 us: 1.17x slower                                        |
| docutils                 | 1.64 sec                                                    | 1.92 sec: 1.17x slower                                      |
| regex_dna                | 116 ms                                                      | 136 ms: 1.17x slower                                        |
| django_template          | 24.4 ms                                                     | 28.9 ms: 1.18x slower                                       |
| mako                     | 7.58 ms                                                     | 9.03 ms: 1.19x slower                                       |
| xml_etree_process        | 37.2 ms                                                     | 44.5 ms: 1.20x slower                                       |
| unpickle                 | 7.57 us                                                     | 9.09 us: 1.20x slower                                       |
| async_tree_cpu_io_mixed  | 530 ms                                                      | 638 ms: 1.20x slower                                        |
| sqlalchemy_declarative   | 85.6 ms                                                     | 103 ms: 1.21x slower                                        |
| mypy2                    | 459 ms                                                      | 555 ms: 1.21x slower                                        |
| thrift                   | 494 us                                                      | 617 us: 1.25x slower                                        |
| async_generators         | 177 ms                                                      | 222 ms: 1.25x slower                                        |
| hexiom                   | 4.55 ms                                                     | 5.74 ms: 1.26x slower                                       |
| scimark_monte_carlo      | 45.3 ms                                                     | 57.3 ms: 1.26x slower                                       |
| sqlglot_transpile        | 1.16 ms                                                     | 1.48 ms: 1.27x slower                                       |
| sqlglot_parse            | 953 us                                                      | 1.22 ms: 1.27x slower                                       |
| chaos                    | 48.4 ms                                                     | 61.7 ms: 1.28x slower                                       |
| crypto_pyaes             | 48.9 ms                                                     | 62.5 ms: 1.28x slower                                       |
| raytrace                 | 213 ms                                                      | 273 ms: 1.28x slower                                        |
| pycparser                | 720 ms                                                      | 930 ms: 1.29x slower                                        |
| pickle_pure_python       | 208 us                                                      | 270 us: 1.29x slower                                        |
| pyflate                  | 312 ms                                                      | 409 ms: 1.31x slower                                        |
| async_tree_none          | 332 ms                                                      | 435 ms: 1.31x slower                                        |
| html5lib                 | 38.9 ms                                                     | 51.0 ms: 1.31x slower                                       |
| logging_silent           | 71.8 ns                                                     | 94.6 ns: 1.32x slower                                       |
| async_tree_memoization   | 399 ms                                                      | 526 ms: 1.32x slower                                        |
| richards_super           | 38.7 ms                                                     | 52.2 ms: 1.35x slower                                       |
| richards                 | 31.4 ms                                                     | 42.4 ms: 1.35x slower                                       |
| scimark_sor              | 78.1 ms                                                     | 106 ms: 1.36x slower                                        |
| scimark_lu               | 62.8 ms                                                     | 85.8 ms: 1.37x slower                                       |
| async_tree_io            | 808 ms                                                      | 1.11 sec: 1.37x slower                                      |
| go                       | 101 ms                                                      | 139 ms: 1.37x slower                                        |
| deltablue                | 2.70 ms                                                     | 4.19 ms: 1.55x slower                                       |
| Geometric mean           | (ref)                                                       | 1.12x slower                                                |

Benchmark hidden because not significant (3): xml_etree_parse, flaskblogging, asyncio_tcp
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.10x
- 99% likely to have a slowdown of 1.08x


# Memory

- memory change: unknown