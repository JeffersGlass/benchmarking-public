
# Results vs. 3.10.4

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 210 ms: 1.17x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.88 ms: 1.19x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.55 sec: 1.24x faster                                                      |
| tornado_http   | 108 ms                                                      | 84.5 ms: 1.28x faster                                                       |
| Geometric mean | (ref)                                                       | 1.22x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 350 ms: 1.50x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 456 ms: 1.40x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.50x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.3 ms: 1.16x faster                                                       |
| nbody          | 71.3 ms                                                     | 70.0 ms: 1.02x faster                                                       |
| pidigits       | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 78.2 ms: 1.36x faster                                                       |
| regex_dna      | 136 ms                                                      | 116 ms: 1.18x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.55 ms: 1.07x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.16x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 183 us: 1.47x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 127 us: 1.45x faster                                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.5 ms: 1.19x faster                                                       |
| tomli_loads          | 1.67 sec                                                    | 1.45 sec: 1.16x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 90.8 ms: 1.07x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 54.1 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| pickle               | 6.85 us                                                     | 7.24 us: 1.06x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.95 us: 1.07x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.12x faster                                                                |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 17.9 ms: 1.15x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.60 ms: 1.37x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 71.0 us: 4.73x faster                                                       |
| deltablue                | 4.19 ms                                                     | 1.99 ms: 2.10x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 54.2 ns: 1.74x faster                                                       |
| raytrace                 | 273 ms                                                      | 165 ms: 1.66x faster                                                        |
| richards_super           | 52.2 ms                                                     | 31.8 ms: 1.64x faster                                                       |
| go                       | 139 ms                                                      | 85.5 ms: 1.63x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.65 ms: 1.62x faster                                                       |
| async_tree_none          | 435 ms                                                      | 272 ms: 1.60x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 470 ms: 1.56x faster                                                        |
| comprehensions           | 16.5 us                                                     | 10.7 us: 1.55x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 55.6 ms: 1.54x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 788 us: 1.54x faster                                                        |
| chaos                    | 61.7 ms                                                     | 40.5 ms: 1.52x faster                                                       |
| async_tree_io            | 1.11 sec                                                    | 729 ms: 1.52x faster                                                        |
| generators               | 32.4 ms                                                     | 21.3 ms: 1.52x faster                                                       |
| richards                 | 42.4 ms                                                     | 28.1 ms: 1.51x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 350 ms: 1.50x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 3.87 ms: 1.48x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 183 us: 1.47x faster                                                        |
| sqlglot_transpile        | 1.48 ms                                                     | 1.00 ms: 1.47x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 39.5 ms: 1.45x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 127 us: 1.45x faster                                                        |
| pyflate                  | 409 ms                                                      | 288 ms: 1.42x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 44.1 ms: 1.42x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 456 ms: 1.40x faster                                                        |
| scimark_sor              | 106 ms                                                      | 76.3 ms: 1.39x faster                                                       |
| mako                     | 9.03 ms                                                     | 6.60 ms: 1.37x faster                                                       |
| regex_compile            | 106 ms                                                      | 78.2 ms: 1.36x faster                                                       |
| mypy2                    | 555 ms                                                      | 413 ms: 1.35x faster                                                        |
| pycparser                | 930 ms                                                      | 713 ms: 1.31x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 22.4 us: 1.29x faster                                                       |
| sympy_sum                | 107 ms                                                      | 83.3 ms: 1.28x faster                                                       |
| tornado_http             | 108 ms                                                      | 84.5 ms: 1.28x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 39.8 ms: 1.27x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.52 us: 1.26x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.55 sec: 1.24x faster                                                      |
| spectral_norm            | 77.3 ms                                                     | 62.6 ms: 1.23x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.0 ms: 1.23x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 12.4 ms: 1.23x faster                                                       |
| dask                     | 313 ms                                                      | 254 ms: 1.23x faster                                                        |
| sympy_str                | 194 ms                                                      | 160 ms: 1.22x faster                                                        |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.76 sec: 1.20x faster                                                      |
| mdp                      | 1.78 sec                                                    | 1.48 sec: 1.20x faster                                                      |
| pprint_pformat           | 1.22 sec                                                    | 1.02 sec: 1.20x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 496 ms: 1.19x faster                                                        |
| chameleon                | 5.79 ms                                                     | 4.88 ms: 1.19x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.5 ms: 1.19x faster                                                       |
| regex_dna                | 136 ms                                                      | 116 ms: 1.18x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 34.0 ms: 1.17x faster                                                       |
| 2to3                     | 246 ms                                                      | 210 ms: 1.17x faster                                                        |
| float                    | 61.7 ms                                                     | 53.3 ms: 1.16x faster                                                       |
| sympy_expand             | 314 ms                                                      | 272 ms: 1.16x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.45 sec: 1.16x faster                                                      |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.36 ms: 1.15x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 831 us: 1.15x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 181 ms: 1.14x faster                                                        |
| deepcopy                 | 255 us                                                      | 228 us: 1.12x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 59.4 ms: 1.12x faster                                                       |
| unpack_sequence          | 39.6 ns                                                     | 36.2 ns: 1.10x faster                                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.04 us: 1.08x faster                                                       |
| scimark_fft              | 187 ms                                                      | 174 ms: 1.08x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 748 us: 1.07x faster                                                        |
| regex_effbot             | 1.66 ms                                                     | 1.55 ms: 1.07x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 90.8 ms: 1.07x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.06x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 72.7 ms: 1.04x faster                                                       |
| fannkuch                 | 256 ms                                                      | 247 ms: 1.04x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.52 us: 1.04x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.0 ms: 1.03x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.6 us: 1.03x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 54.1 ms: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.3 ms: 1.03x faster                                                       |
| logging_simple           | 6.22 us                                                     | 6.07 us: 1.03x faster                                                       |
| nbody                    | 71.3 ms                                                     | 70.0 ms: 1.02x faster                                                       |
| pidigits                 | 149 ms                                                      | 147 ms: 1.02x faster                                                        |
| pathlib                  | 75.7 ms                                                     | 75.1 ms: 1.01x faster                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 63.9 ms: 1.03x slower                                                       |
| async_generators         | 222 ms                                                      | 229 ms: 1.03x slower                                                        |
| pickle                   | 6.85 us                                                     | 7.24 us: 1.06x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.95 us: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.51 ms: 1.07x slower                                                       |
| pickle_dict              | 17.2 us                                                     | 18.6 us: 1.08x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.9 ms: 1.15x slower                                                       |
| coverage                 | 39.0 ms                                                     | 46.4 ms: 1.19x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.80 ms: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.24x faster                                                                |

Benchmark hidden because not significant (2): unpickle_list, json
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: unknown