
# Results vs. 3.10.4

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.24x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 215 ms: 1.14x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.86 ms: 1.19x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| tornado_http   | 108 ms                                                      | 87.7 ms: 1.24x faster                                                       |
| Geometric mean | (ref)                                                       | 1.20x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 266 ms: 1.64x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 724 ms: 1.53x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 448 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.53x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 51.9 ms: 1.19x faster                                                       |
| nbody          | 71.3 ms                                                     | 69.5 ms: 1.03x faster                                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.00x slower                                                        |
| Geometric mean | (ref)                                                       | 1.07x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 77.9 ms: 1.36x faster                                                       |
| regex_dna      | 136 ms                                                      | 122 ms: 1.12x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.49 ms: 1.67x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 181 us: 1.49x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 129 us: 1.43x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.32 us: 1.09x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 92.0 ms: 1.05x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.0 ms: 1.03x faster                                                       |
| pickle               | 6.85 us                                                     | 7.02 us: 1.02x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.86 us: 1.04x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.3 us: 1.06x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.8 ms: 1.21x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.10x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.41 ms: 1.41x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 72.3 us: 4.65x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.01 ms: 2.09x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 53.8 ns: 1.76x faster                                                       |
| richards_super           | 52.2 ms                                                     | 31.2 ms: 1.68x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.49 ms: 1.67x faster                                                       |
| raytrace                 | 273 ms                                                      | 166 ms: 1.65x faster                                                        |
| async_tree_none          | 435 ms                                                      | 266 ms: 1.64x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 461 ms: 1.59x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 765 us: 1.59x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.5 us: 1.58x faster                                                       |
| chaos                    | 61.7 ms                                                     | 39.2 ms: 1.57x faster                                                       |
| go                       | 139 ms                                                      | 88.5 ms: 1.57x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 55.4 ms: 1.55x faster                                                       |
| richards                 | 42.4 ms                                                     | 27.5 ms: 1.54x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 342 ms: 1.54x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 724 ms: 1.53x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.80 ms: 1.51x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 980 us: 1.51x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 181 us: 1.49x faster                                                        |
| generators               | 32.4 ms                                                     | 22.1 ms: 1.47x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 43.3 ms: 1.45x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 40.1 ms: 1.43x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 129 us: 1.43x faster                                                        |
| pyflate                  | 409 ms                                                      | 287 ms: 1.42x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 448 ms: 1.42x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.41 ms: 1.41x faster                                                       |
| regex_compile            | 106 ms                                                      | 77.9 ms: 1.36x faster                                                       |
| mypy2                    | 555 ms                                                      | 414 ms: 1.34x faster                                                        |
| scimark_sor              | 106 ms                                                      | 79.9 ms: 1.33x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 21.9 us: 1.32x faster                                                       |
| pycparser                | 930 ms                                                      | 709 ms: 1.31x faster                                                        |
| sympy_sum                | 107 ms                                                      | 83.3 ms: 1.28x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 60.2 ms: 1.28x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.41 sec: 1.26x faster                                                      |
| tornado_http             | 108 ms                                                      | 87.7 ms: 1.24x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.4 ms: 1.23x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.56 sec: 1.23x faster                                                      |
| sqlite_synth             | 1.91 us                                                     | 1.56 us: 1.22x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 996 ms: 1.22x faster                                                        |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.22x faster                                                       |
| sympy_str                | 194 ms                                                      | 160 ms: 1.22x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 488 ms: 1.21x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.7 ms: 1.21x faster                                                       |
| dask                     | 313 ms                                                      | 258 ms: 1.21x faster                                                        |
| dulwich_log              | 50.5 ms                                                     | 41.9 ms: 1.20x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.40 sec: 1.19x faster                                                      |
| chameleon                | 5.79 ms                                                     | 4.86 ms: 1.19x faster                                                       |
| float                    | 61.7 ms                                                     | 51.9 ms: 1.19x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 33.8 ms: 1.18x faster                                                       |
| deepcopy                 | 255 us                                                      | 220 us: 1.16x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 177 ms: 1.16x faster                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.36 ms: 1.16x faster                                                       |
| sympy_expand             | 314 ms                                                      | 272 ms: 1.15x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.83 sec: 1.15x faster                                                      |
| nqueens                  | 66.6 ms                                                     | 58.1 ms: 1.15x faster                                                       |
| 2to3                     | 246 ms                                                      | 215 ms: 1.14x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.95 us: 1.13x faster                                                       |
| regex_dna                | 136 ms                                                      | 122 ms: 1.12x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 857 us: 1.12x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 727 us: 1.10x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.32 us: 1.09x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 36.4 ns: 1.09x faster                                                       |
| fannkuch                 | 256 ms                                                      | 240 ms: 1.07x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 92.0 ms: 1.05x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.47 us: 1.04x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.0 ms: 1.04x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.99 us: 1.04x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.61 ms: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.0 ms: 1.03x faster                                                       |
| scimark_fft              | 187 ms                                                      | 182 ms: 1.03x faster                                                        |
| nbody                    | 71.3 ms                                                     | 69.5 ms: 1.03x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.3 ms: 1.01x faster                                                       |
| pidigits                 | 149 ms                                                      | 150 ms: 1.00x slower                                                        |
| async_generators         | 222 ms                                                      | 224 ms: 1.01x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.02 us: 1.02x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.86 us: 1.04x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 79.8 ms: 1.06x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.3 us: 1.06x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 69.8 ms: 1.12x slower                                                       |
| coverage                 | 39.0 ms                                                     | 45.9 ms: 1.18x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.8 ms: 1.21x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.92 ms: 1.25x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.24x faster                                                                |

Benchmark hidden because not significant (3): json, unpickle_list, python_startup
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.18x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown