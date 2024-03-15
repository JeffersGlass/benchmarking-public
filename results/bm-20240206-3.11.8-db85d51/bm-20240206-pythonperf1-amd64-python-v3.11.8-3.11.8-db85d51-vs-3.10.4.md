
# Results vs. 3.10.4

- fork: python
- ref: v3.11.8
- machine: windows-amd64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.14x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 206 ms: 1.19x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.18 ms: 1.12x faster                                       |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                      |
| html5lib       | 51.0 ms                                                     | 38.6 ms: 1.32x faster                                       |
| tornado_http   | 108 ms                                                      | 88.0 ms: 1.23x faster                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 785 ms: 1.41x faster                                        |
| async_tree_none         | 435 ms                                                      | 312 ms: 1.40x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 379 ms: 1.39x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 521 ms: 1.22x faster                                        |
| Geometric mean          | (ref)                                                       | 1.35x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.6 ms: 1.15x faster                                       |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 88.2 ms: 1.20x faster                                       |
| regex_dna      | 136 ms                                                      | 117 ms: 1.16x faster                                        |
| regex_v8       | 15.4 ms                                                     | 13.6 ms: 1.14x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.49 ms: 1.11x faster                                       |
| Geometric mean | (ref)                                                       | 1.15x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 201 us: 1.34x faster                                        |
| unpickle_pure_python | 183 us                                                      | 150 us: 1.22x faster                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                       |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                      |
| json_dumps           | 9.16 ms                                                     | 7.80 ms: 1.17x faster                                       |
| unpickle             | 9.09 us                                                     | 7.78 us: 1.17x faster                                       |
| json_loads           | 14.0 us                                                     | 12.9 us: 1.09x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.7 ms: 1.05x faster                                       |
| unpickle_list        | 2.71 us                                                     | 2.61 us: 1.04x faster                                       |
| pickle_list          | 2.75 us                                                     | 2.71 us: 1.02x faster                                       |
| pickle               | 6.85 us                                                     | 6.78 us: 1.01x faster                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                       |
| xml_etree_parse      | 96.8 ms                                                     | 102 ms: 1.05x slower                                        |
| pickle_dict          | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| Geometric mean       | (ref)                                                       | 1.09x faster                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                       |
| python_startup_no_site | 15.5 ms                                                     | 15.3 ms: 1.02x faster                                       |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 7.47 ms: 1.21x faster                                       |
| django_template | 28.9 ms                                                     | 23.9 ms: 1.21x faster                                       |
| genshi_text     | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 38.3 ms: 1.07x faster                                       |
| Geometric mean  | (ref)                                                       | 1.16x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51 |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.62 ms: 1.60x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 785 ms: 1.41x faster                                        |
| scimark_lu               | 85.8 ms                                                     | 61.0 ms: 1.41x faster                                       |
| richards                 | 42.4 ms                                                     | 30.3 ms: 1.40x faster                                       |
| async_tree_none          | 435 ms                                                      | 312 ms: 1.40x faster                                        |
| async_tree_memoization   | 526 ms                                                      | 379 ms: 1.39x faster                                        |
| richards_super           | 52.2 ms                                                     | 37.6 ms: 1.39x faster                                       |
| scimark_sor              | 106 ms                                                      | 76.6 ms: 1.39x faster                                       |
| pycparser                | 930 ms                                                      | 684 ms: 1.36x faster                                        |
| raytrace                 | 273 ms                                                      | 202 ms: 1.36x faster                                        |
| logging_silent           | 94.6 ns                                                     | 69.9 ns: 1.35x faster                                       |
| go                       | 139 ms                                                      | 103 ms: 1.34x faster                                        |
| pickle_pure_python       | 270 us                                                      | 201 us: 1.34x faster                                        |
| pyflate                  | 409 ms                                                      | 305 ms: 1.34x faster                                        |
| html5lib                 | 51.0 ms                                                     | 38.6 ms: 1.32x faster                                       |
| crypto_pyaes             | 62.5 ms                                                     | 47.7 ms: 1.31x faster                                       |
| sqlglot_parse            | 1.22 ms                                                     | 929 us: 1.31x faster                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.14 ms: 1.30x faster                                       |
| thrift                   | 617 us                                                      | 485 us: 1.27x faster                                        |
| chaos                    | 61.7 ms                                                     | 48.5 ms: 1.27x faster                                       |
| hexiom                   | 5.74 ms                                                     | 4.51 ms: 1.27x faster                                       |
| async_generators         | 222 ms                                                      | 178 ms: 1.25x faster                                        |
| sqlalchemy_declarative   | 103 ms                                                      | 83.4 ms: 1.24x faster                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.5 ms: 1.23x faster                                       |
| tornado_http             | 108 ms                                                      | 88.0 ms: 1.23x faster                                       |
| mypy2                    | 555 ms                                                      | 452 ms: 1.23x faster                                        |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                      |
| unpickle_pure_python     | 183 us                                                      | 150 us: 1.22x faster                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 521 ms: 1.22x faster                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                       |
| mako                     | 9.03 ms                                                     | 7.47 ms: 1.21x faster                                       |
| django_template          | 28.9 ms                                                     | 23.9 ms: 1.21x faster                                       |
| regex_compile            | 106 ms                                                      | 88.2 ms: 1.20x faster                                       |
| dask                     | 313 ms                                                      | 263 ms: 1.19x faster                                        |
| 2to3                     | 246 ms                                                      | 206 ms: 1.19x faster                                        |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.18x faster                                      |
| aiohttp                  | 995 us                                                      | 846 us: 1.18x faster                                        |
| json_dumps               | 9.16 ms                                                     | 7.80 ms: 1.17x faster                                       |
| unpickle                 | 9.09 us                                                     | 7.78 us: 1.17x faster                                       |
| deepcopy_memo            | 28.8 us                                                     | 24.6 us: 1.17x faster                                       |
| regex_dna                | 136 ms                                                      | 117 ms: 1.16x faster                                        |
| genshi_text              | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                       |
| float                    | 61.7 ms                                                     | 53.6 ms: 1.15x faster                                       |
| spectral_norm            | 77.3 ms                                                     | 67.3 ms: 1.15x faster                                       |
| dulwich_log              | 50.5 ms                                                     | 44.0 ms: 1.15x faster                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.07 sec: 1.14x faster                                      |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                       |
| regex_v8                 | 15.4 ms                                                     | 13.6 ms: 1.14x faster                                       |
| pylint                   | 350 ms                                                      | 308 ms: 1.14x faster                                        |
| pprint_safe_repr         | 592 ms                                                      | 522 ms: 1.13x faster                                        |
| pathlib                  | 75.7 ms                                                     | 66.9 ms: 1.13x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.5 ms: 1.13x faster                                       |
| bench_thread_pool        | 958 us                                                      | 849 us: 1.13x faster                                        |
| create_gc_cycles         | 800 us                                                      | 713 us: 1.12x faster                                        |
| python_startup           | 20.6 ms                                                     | 18.4 ms: 1.12x faster                                       |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.2 ms: 1.12x faster                                       |
| chameleon                | 5.79 ms                                                     | 5.18 ms: 1.12x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.71 us: 1.12x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.49 ms: 1.11x faster                                       |
| mdp                      | 1.78 sec                                                    | 1.61 sec: 1.10x faster                                      |
| json_loads               | 14.0 us                                                     | 12.9 us: 1.09x faster                                       |
| sympy_sum                | 107 ms                                                      | 98.5 ms: 1.09x faster                                       |
| comprehensions           | 16.5 us                                                     | 15.2 us: 1.08x faster                                       |
| coroutines               | 16.0 ms                                                     | 14.8 ms: 1.08x faster                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.96 sec: 1.08x faster                                      |
| genshi_xml               | 41.0 ms                                                     | 38.3 ms: 1.07x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 192 ms: 1.07x faster                                        |
| sympy_str                | 194 ms                                                      | 183 ms: 1.06x faster                                        |
| fannkuch                 | 256 ms                                                      | 241 ms: 1.06x faster                                        |
| deepcopy                 | 255 us                                                      | 242 us: 1.06x faster                                        |
| xml_etree_generate       | 55.5 ms                                                     | 52.7 ms: 1.05x faster                                       |
| sympy_expand             | 314 ms                                                      | 300 ms: 1.05x faster                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.61 ms: 1.04x faster                                       |
| unpickle_list            | 2.71 us                                                     | 2.61 us: 1.04x faster                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.13 us: 1.03x faster                                       |
| asyncio_tcp              | 732 ms                                                      | 709 ms: 1.03x faster                                        |
| scimark_fft              | 187 ms                                                      | 182 ms: 1.03x faster                                        |
| nqueens                  | 66.6 ms                                                     | 64.7 ms: 1.03x faster                                       |
| typing_runtime_protocols | 336 us                                                      | 328 us: 1.02x faster                                        |
| meteor_contest           | 75.9 ms                                                     | 74.7 ms: 1.02x faster                                       |
| pickle_list              | 2.75 us                                                     | 2.71 us: 1.02x faster                                       |
| python_startup_no_site   | 15.5 ms                                                     | 15.3 ms: 1.02x faster                                       |
| pickle                   | 6.85 us                                                     | 6.78 us: 1.01x faster                                       |
| bench_mp_pool            | 62.0 ms                                                     | 61.4 ms: 1.01x faster                                       |
| pidigits                 | 149 ms                                                      | 148 ms: 1.01x faster                                        |
| flaskblogging            | 2.03 sec                                                    | 2.03 sec: 1.00x slower                                      |
| xml_etree_iterparse      | 65.0 ms                                                     | 65.6 ms: 1.01x slower                                       |
| generators               | 32.4 ms                                                     | 33.5 ms: 1.03x slower                                       |
| xml_etree_parse          | 96.8 ms                                                     | 102 ms: 1.05x slower                                        |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.05x slower                                       |
| logging_format           | 6.76 us                                                     | 7.13 us: 1.05x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.5 us: 1.08x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.75 us: 1.08x slower                                       |
| coverage                 | 39.0 ms                                                     | 44.8 ms: 1.15x slower                                       |
| unpack_sequence          | 39.6 ns                                                     | 47.3 ns: 1.19x slower                                       |
| Geometric mean           | (ref)                                                       | 1.14x faster                                                |

Benchmark hidden because not significant (3): json, telco, nbody
Ignored benchmarks (4) of results/bm-20240206-3.11.8-db85d51/bm-20240206-pythonperf1-amd64-python-v3.11.8-3.11.8-db85d51.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown