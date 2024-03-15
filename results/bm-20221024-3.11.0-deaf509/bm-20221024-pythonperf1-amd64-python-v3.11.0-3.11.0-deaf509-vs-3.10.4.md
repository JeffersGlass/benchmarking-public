
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0
- machine: windows-amd64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.12x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 214 ms: 1.15x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.26 ms: 1.10x faster                                       |
| docutils       | 1.92 sec                                                    | 1.64 sec: 1.17x faster                                      |
| html5lib       | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                       |
| tornado_http   | 108 ms                                                      | 92.8 ms: 1.17x faster                                       |
| Geometric mean | (ref)                                                       | 1.18x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 808 ms: 1.37x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 399 ms: 1.32x faster                                        |
| async_tree_none         | 435 ms                                                      | 332 ms: 1.31x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 530 ms: 1.20x faster                                        |
| Geometric mean          | (ref)                                                       | 1.30x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.4 ms: 1.13x faster                                       |
| nbody          | 71.3 ms                                                     | 70.3 ms: 1.01x faster                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 116 ms: 1.17x faster                                        |
| regex_compile  | 106 ms                                                      | 91.0 ms: 1.16x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.50 ms: 1.11x faster                                       |
| regex_v8       | 15.4 ms                                                     | 14.2 ms: 1.09x faster                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 208 us: 1.29x faster                                        |
| unpickle             | 9.09 us                                                     | 7.57 us: 1.20x faster                                       |
| xml_etree_process    | 44.5 ms                                                     | 37.2 ms: 1.20x faster                                       |
| unpickle_pure_python | 183 us                                                      | 157 us: 1.17x faster                                        |
| tomli_loads          | 1.67 sec                                                    | 1.46 sec: 1.15x faster                                      |
| json_dumps           | 9.16 ms                                                     | 8.09 ms: 1.13x faster                                       |
| json_loads           | 14.0 us                                                     | 13.0 us: 1.08x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.59 us: 1.05x faster                                       |
| pickle               | 6.85 us                                                     | 6.64 us: 1.03x faster                                       |
| pickle_list          | 2.75 us                                                     | 2.70 us: 1.02x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                       |
| pickle_dict          | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 19.8 ms: 1.04x faster                                       |
| python_startup_no_site | 15.5 ms                                                     | 16.8 ms: 1.08x slower                                       |
| Geometric mean         | (ref)                                                       | 1.02x slower                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.58 ms: 1.19x faster                                       |
| django_template | 28.9 ms                                                     | 24.4 ms: 1.18x faster                                       |
| genshi_text     | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 39.9 ms: 1.03x faster                                       |
| Geometric mean  | (ref)                                                       | 1.12x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.70 ms: 1.55x faster                                       |
| go                       | 139 ms                                                      | 101 ms: 1.37x faster                                        |
| async_tree_io            | 1.11 sec                                                    | 808 ms: 1.37x faster                                        |
| scimark_lu               | 85.8 ms                                                     | 62.8 ms: 1.37x faster                                       |
| scimark_sor              | 106 ms                                                      | 78.1 ms: 1.36x faster                                       |
| richards                 | 42.4 ms                                                     | 31.4 ms: 1.35x faster                                       |
| richards_super           | 52.2 ms                                                     | 38.7 ms: 1.35x faster                                       |
| async_tree_memoization   | 526 ms                                                      | 399 ms: 1.32x faster                                        |
| logging_silent           | 94.6 ns                                                     | 71.8 ns: 1.32x faster                                       |
| html5lib                 | 51.0 ms                                                     | 38.9 ms: 1.31x faster                                       |
| async_tree_none          | 435 ms                                                      | 332 ms: 1.31x faster                                        |
| pyflate                  | 409 ms                                                      | 312 ms: 1.31x faster                                        |
| pickle_pure_python       | 270 us                                                      | 208 us: 1.29x faster                                        |
| pycparser                | 930 ms                                                      | 720 ms: 1.29x faster                                        |
| raytrace                 | 273 ms                                                      | 213 ms: 1.28x faster                                        |
| crypto_pyaes             | 62.5 ms                                                     | 48.9 ms: 1.28x faster                                       |
| chaos                    | 61.7 ms                                                     | 48.4 ms: 1.28x faster                                       |
| sqlglot_parse            | 1.22 ms                                                     | 953 us: 1.27x faster                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.16 ms: 1.27x faster                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 45.3 ms: 1.26x faster                                       |
| hexiom                   | 5.74 ms                                                     | 4.55 ms: 1.26x faster                                       |
| async_generators         | 222 ms                                                      | 177 ms: 1.25x faster                                        |
| thrift                   | 617 us                                                      | 494 us: 1.25x faster                                        |
| mypy2                    | 555 ms                                                      | 459 ms: 1.21x faster                                        |
| sqlalchemy_declarative   | 103 ms                                                      | 85.6 ms: 1.21x faster                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 530 ms: 1.20x faster                                        |
| unpickle                 | 9.09 us                                                     | 7.57 us: 1.20x faster                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.2 ms: 1.20x faster                                       |
| mako                     | 9.03 ms                                                     | 7.58 ms: 1.19x faster                                       |
| django_template          | 28.9 ms                                                     | 24.4 ms: 1.18x faster                                       |
| regex_dna                | 136 ms                                                      | 116 ms: 1.17x faster                                        |
| docutils                 | 1.92 sec                                                    | 1.64 sec: 1.17x faster                                      |
| unpickle_pure_python     | 183 us                                                      | 157 us: 1.17x faster                                        |
| tornado_http             | 108 ms                                                      | 92.8 ms: 1.17x faster                                       |
| regex_compile            | 106 ms                                                      | 91.0 ms: 1.16x faster                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 34.5 ms: 1.15x faster                                       |
| 2to3                     | 246 ms                                                      | 214 ms: 1.15x faster                                        |
| tomli_loads              | 1.67 sec                                                    | 1.46 sec: 1.15x faster                                      |
| dask                     | 313 ms                                                      | 273 ms: 1.15x faster                                        |
| float                    | 61.7 ms                                                     | 54.4 ms: 1.13x faster                                       |
| json_dumps               | 9.16 ms                                                     | 8.09 ms: 1.13x faster                                       |
| spectral_norm            | 77.3 ms                                                     | 68.3 ms: 1.13x faster                                       |
| aiohttp                  | 995 us                                                      | 883 us: 1.13x faster                                        |
| pprint_pformat           | 1.22 sec                                                    | 1.09 sec: 1.12x faster                                      |
| create_gc_cycles         | 800 us                                                      | 713 us: 1.12x faster                                        |
| pprint_safe_repr         | 592 ms                                                      | 529 ms: 1.12x faster                                        |
| mdp                      | 1.78 sec                                                    | 1.59 sec: 1.12x faster                                      |
| deepcopy_memo            | 28.8 us                                                     | 26.0 us: 1.11x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.50 ms: 1.11x faster                                       |
| chameleon                | 5.79 ms                                                     | 5.26 ms: 1.10x faster                                       |
| bench_thread_pool        | 958 us                                                      | 872 us: 1.10x faster                                        |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.4 ms: 1.09x faster                                       |
| regex_v8                 | 15.4 ms                                                     | 14.2 ms: 1.09x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 14.0 ms: 1.09x faster                                       |
| dulwich_log              | 50.5 ms                                                     | 46.4 ms: 1.09x faster                                       |
| pylint                   | 350 ms                                                      | 323 ms: 1.08x faster                                        |
| sqlite_synth             | 1.91 us                                                     | 1.77 us: 1.08x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 190 ms: 1.08x faster                                        |
| json_loads               | 14.0 us                                                     | 13.0 us: 1.08x faster                                       |
| genshi_text              | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.06 us: 1.07x faster                                       |
| sympy_sum                | 107 ms                                                      | 100 ms: 1.07x faster                                        |
| coroutines               | 16.0 ms                                                     | 15.0 ms: 1.07x faster                                       |
| pathlib                  | 75.7 ms                                                     | 70.9 ms: 1.07x faster                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.58 ms: 1.06x faster                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.5 ms: 1.06x faster                                       |
| comprehensions           | 16.5 us                                                     | 15.6 us: 1.06x faster                                       |
| json                     | 3.14 ms                                                     | 2.98 ms: 1.05x faster                                       |
| sympy_expand             | 314 ms                                                      | 299 ms: 1.05x faster                                        |
| sympy_str                | 194 ms                                                      | 185 ms: 1.05x faster                                        |
| unpickle_list            | 2.71 us                                                     | 2.59 us: 1.05x faster                                       |
| scimark_fft              | 187 ms                                                      | 179 ms: 1.05x faster                                        |
| python_startup           | 20.6 ms                                                     | 19.8 ms: 1.04x faster                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 2.03 sec: 1.04x faster                                      |
| deepcopy                 | 255 us                                                      | 246 us: 1.04x faster                                        |
| pickle                   | 6.85 us                                                     | 6.64 us: 1.03x faster                                       |
| typing_runtime_protocols | 336 us                                                      | 326 us: 1.03x faster                                        |
| genshi_xml               | 41.0 ms                                                     | 39.9 ms: 1.03x faster                                       |
| pickle_list              | 2.75 us                                                     | 2.70 us: 1.02x faster                                       |
| nbody                    | 71.3 ms                                                     | 70.3 ms: 1.01x faster                                       |
| fannkuch                 | 256 ms                                                      | 253 ms: 1.01x faster                                        |
| meteor_contest           | 75.9 ms                                                     | 75.2 ms: 1.01x faster                                       |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                        |
| xml_etree_iterparse      | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                       |
| bench_mp_pool            | 62.0 ms                                                     | 63.2 ms: 1.02x slower                                       |
| nqueens                  | 66.6 ms                                                     | 68.3 ms: 1.03x slower                                       |
| telco                    | 3.94 ms                                                     | 4.06 ms: 1.03x slower                                       |
| generators               | 32.4 ms                                                     | 34.0 ms: 1.05x slower                                       |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                       |
| logging_format           | 6.76 us                                                     | 7.16 us: 1.06x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| python_startup_no_site   | 15.5 ms                                                     | 16.8 ms: 1.08x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.86 us: 1.10x slower                                       |
| coverage                 | 39.0 ms                                                     | 43.4 ms: 1.11x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 46.9 ns: 1.18x slower                                       |
| Geometric mean           | (ref)                                                       | 1.12x faster                                                |

Benchmark hidden because not significant (3): asyncio_tcp, flaskblogging, xml_etree_parse
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.11x
- 95% likely to have a speedup of 1.10x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown