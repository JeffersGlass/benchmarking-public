
# Results vs. 3.10.4

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| tornado_http   | 108 ms                                                      | 86.3 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 278 ms: 1.57x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 356 ms: 1.48x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 763 ms: 1.45x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 473 ms: 1.35x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.46x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                                       |
| pidigits       | 149 ms                                                      | 149 ms: 1.00x faster                                                        |
| nbody          | 71.3 ms                                                     | 72.0 ms: 1.01x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 79.0 ms: 1.34x faster                                                       |
| regex_dna      | 136 ms                                                      | 117 ms: 1.16x faster                                                        |
| regex_v8       | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.05x faster                                                       |
| Geometric mean | (ref)                                                       | 1.15x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.61 ms: 1.63x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 184 us: 1.46x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 133 us: 1.38x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.42 sec: 1.17x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.45 us: 1.08x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 95.6 ms: 1.01x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| pickle               | 6.85 us                                                     | 7.15 us: 1.04x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.87 us: 1.04x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.9 us: 1.10x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (2): xml_etree_iterparse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 18.5 ms: 1.19x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.09x slower                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.75 ms: 1.34x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 71.4 us: 4.70x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.06 ms: 2.03x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.8 ns: 1.73x faster                                                       |
| raytrace                 | 273 ms                                                      | 163 ms: 1.68x faster                                                        |
| richards_super           | 52.2 ms                                                     | 31.6 ms: 1.65x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.61 ms: 1.63x faster                                                       |
| go                       | 139 ms                                                      | 85.7 ms: 1.62x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 775 us: 1.57x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.5 us: 1.57x faster                                                       |
| async_tree_none          | 435 ms                                                      | 278 ms: 1.57x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 55.2 ms: 1.55x faster                                                       |
| chaos                    | 61.7 ms                                                     | 39.8 ms: 1.55x faster                                                       |
| richards                 | 42.4 ms                                                     | 28.4 ms: 1.50x faster                                                       |
| generators               | 32.4 ms                                                     | 21.8 ms: 1.49x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 356 ms: 1.48x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.00 ms: 1.47x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 184 us: 1.46x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 503 ms: 1.46x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 763 ms: 1.45x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.97 ms: 1.45x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 40.8 ms: 1.40x faster                                                       |
| pyflate                  | 409 ms                                                      | 292 ms: 1.40x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 44.8 ms: 1.40x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 133 us: 1.38x faster                                                        |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 473 ms: 1.35x faster                                                        |
| regex_compile            | 106 ms                                                      | 79.0 ms: 1.34x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.75 ms: 1.34x faster                                                       |
| mypy2                    | 555 ms                                                      | 421 ms: 1.32x faster                                                        |
| pycparser                | 930 ms                                                      | 710 ms: 1.31x faster                                                        |
| scimark_sor              | 106 ms                                                      | 81.5 ms: 1.30x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.41 sec: 1.27x faster                                                      |
| sympy_sum                | 107 ms                                                      | 85.1 ms: 1.26x faster                                                       |
| tornado_http             | 108 ms                                                      | 86.3 ms: 1.26x faster                                                       |
| deepcopy_memo            | 28.8 us                                                     | 23.0 us: 1.25x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 62.2 ms: 1.24x faster                                                       |
| sympy_str                | 194 ms                                                      | 159 ms: 1.23x faster                                                        |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.22x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                      |
| sympy_integrate          | 15.3 ms                                                     | 12.7 ms: 1.21x faster                                                       |
| dask                     | 313 ms                                                      | 260 ms: 1.20x faster                                                        |
| sqlite_synth             | 1.91 us                                                     | 1.59 us: 1.20x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.02 sec: 1.20x faster                                                      |
| dulwich_log              | 50.5 ms                                                     | 42.5 ms: 1.19x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.6 ms: 1.18x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 501 ms: 1.18x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 33.9 ms: 1.17x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.42 sec: 1.17x faster                                                      |
| chameleon                | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 175 ms: 1.17x faster                                                        |
| regex_dna                | 136 ms                                                      | 117 ms: 1.16x faster                                                        |
| sympy_expand             | 314 ms                                                      | 275 ms: 1.14x faster                                                        |
| float                    | 61.7 ms                                                     | 54.1 ms: 1.14x faster                                                       |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 224 us: 1.14x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 58.6 ms: 1.14x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.87 sec: 1.13x faster                                                      |
| deepcopy_reduce          | 2.20 us                                                     | 2.02 us: 1.09x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 877 us: 1.09x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.45 us: 1.08x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.54 ms: 1.07x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 752 us: 1.06x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 14.6 ms: 1.06x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.05x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 72.8 ms: 1.04x faster                                                       |
| fannkuch                 | 256 ms                                                      | 246 ms: 1.04x faster                                                        |
| scimark_fft              | 187 ms                                                      | 180 ms: 1.04x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 53.9 ms: 1.03x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.06 us: 1.03x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.61 us: 1.02x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 39.0 ns: 1.02x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 95.6 ms: 1.01x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.9 us: 1.01x faster                                                       |
| pidigits                 | 149 ms                                                      | 149 ms: 1.00x faster                                                        |
| nbody                    | 71.3 ms                                                     | 72.0 ms: 1.01x slower                                                       |
| async_generators         | 222 ms                                                      | 229 ms: 1.03x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.15 us: 1.04x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.87 us: 1.04x slower                                                       |
| pathlib                  | 75.7 ms                                                     | 80.3 ms: 1.06x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.54 ms: 1.09x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 67.7 ms: 1.09x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.9 us: 1.10x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.61 ms: 1.17x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.5 ms: 1.19x slower                                                       |
| coverage                 | 39.0 ms                                                     | 48.0 ms: 1.23x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.22x faster                                                                |

Benchmark hidden because not significant (4): python_startup, xml_etree_iterparse, unpickle_list, json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown