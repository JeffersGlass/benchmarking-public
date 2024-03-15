
# Results vs. 3.10.4

- fork: python
- ref: 4297d7301b97aba2e0df
- machine: windows-amd64
- commit hash: 4297d73
- commit date: 2024-02-12
- overall geometric mean: 1.22x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| tornado_http   | 108 ms                                                      | 84.9 ms: 1.28x faster                                                       |
| Geometric mean | (ref)                                                       | 1.21x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 263 ms: 1.65x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 333 ms: 1.58x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 716 ms: 1.55x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 451 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.55x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.0 ms: 1.23x faster                                                       |
| nbody          | 71.3 ms                                                     | 61.7 ms: 1.15x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 79.9 ms: 1.33x faster                                                       |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 173 us: 1.56x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 125 us: 1.47x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.27 sec: 1.32x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.3 ms: 1.23x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.9 ms: 1.03x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.4 ms: 1.02x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| unpickle_list        | 2.71 us                                                     | 2.76 us: 1.02x slower                                                       |
| pickle_dict          | 17.2 us                                                     | 17.6 us: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.16 us: 1.05x slower                                                       |
| pickle_list          | 2.75 us                                                     | 3.12 us: 1.13x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 20.2 ms: 1.02x faster                                                       |
| python_startup_no_site | 15.5 ms                                                     | 18.1 ms: 1.16x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.07x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.44 ms: 1.40x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.1 us: 4.86x faster                                                       |
| deltablue                | 4.19 ms                                                     | 1.96 ms: 2.13x faster                                                       |
| richards_super           | 52.2 ms                                                     | 28.2 ms: 1.85x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 52.2 ns: 1.81x faster                                                       |
| richards                 | 42.4 ms                                                     | 25.0 ms: 1.70x faster                                                       |
| async_tree_none          | 435 ms                                                      | 263 ms: 1.65x faster                                                        |
| json_dumps               | 9.16 ms                                                     | 5.55 ms: 1.65x faster                                                       |
| generators               | 32.4 ms                                                     | 20.0 ms: 1.62x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 754 us: 1.61x faster                                                        |
| raytrace                 | 273 ms                                                      | 172 ms: 1.59x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 333 ms: 1.58x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 465 ms: 1.57x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 173 us: 1.56x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 716 ms: 1.55x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 55.9 ms: 1.53x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 979 us: 1.51x faster                                                        |
| unpickle_pure_python     | 183 us                                                      | 125 us: 1.47x faster                                                        |
| comprehensions           | 16.5 us                                                     | 11.3 us: 1.46x faster                                                       |
| chaos                    | 61.7 ms                                                     | 42.5 ms: 1.45x faster                                                       |
| go                       | 139 ms                                                      | 97.1 ms: 1.43x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 451 ms: 1.42x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.44 ms: 1.40x faster                                                       |
| scimark_sor              | 106 ms                                                      | 77.2 ms: 1.38x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 45.5 ms: 1.37x faster                                                       |
| pycparser                | 930 ms                                                      | 685 ms: 1.36x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 21.5 us: 1.34x faster                                                       |
| regex_compile            | 106 ms                                                      | 79.9 ms: 1.33x faster                                                       |
| pyflate                  | 409 ms                                                      | 310 ms: 1.32x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.27 sec: 1.32x faster                                                      |
| mypy2                    | 555 ms                                                      | 425 ms: 1.31x faster                                                        |
| tornado_http             | 108 ms                                                      | 84.9 ms: 1.28x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.51 us: 1.27x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 40.2 ms: 1.25x faster                                                       |
| coroutines               | 16.0 ms                                                     | 12.9 ms: 1.24x faster                                                       |
| float                    | 61.7 ms                                                     | 50.0 ms: 1.23x faster                                                       |
| pprint_safe_repr         | 592 ms                                                      | 480 ms: 1.23x faster                                                        |
| pprint_pformat           | 1.22 sec                                                    | 991 ms: 1.23x faster                                                        |
| dask                     | 313 ms                                                      | 255 ms: 1.23x faster                                                        |
| xml_etree_process        | 44.5 ms                                                     | 36.3 ms: 1.23x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.57 sec: 1.22x faster                                                      |
| sympy_sum                | 107 ms                                                      | 88.1 ms: 1.21x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.78 ms: 1.21x faster                                                       |
| spectral_norm            | 77.3 ms                                                     | 65.7 ms: 1.18x faster                                                       |
| deepcopy                 | 255 us                                                      | 217 us: 1.18x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.89 us: 1.17x faster                                                       |
| sympy_str                | 194 ms                                                      | 167 ms: 1.16x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.2 ms: 1.16x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 826 us: 1.16x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 34.5 ms: 1.15x faster                                                       |
| nbody                    | 71.3 ms                                                     | 61.7 ms: 1.15x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.54 sec: 1.15x faster                                                      |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.84 sec: 1.15x faster                                                      |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                                        |
| 2to3                     | 246 ms                                                      | 216 ms: 1.14x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 58.8 ms: 1.13x faster                                                       |
| sympy_expand             | 314 ms                                                      | 282 ms: 1.12x faster                                                        |
| hexiom                   | 5.74 ms                                                     | 5.22 ms: 1.10x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 728 us: 1.10x faster                                                        |
| logging_format           | 6.76 us                                                     | 6.28 us: 1.08x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.83 us: 1.07x faster                                                       |
| unpickle                 | 9.09 us                                                     | 8.54 us: 1.06x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| fannkuch                 | 256 ms                                                      | 243 ms: 1.05x faster                                                        |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 93.9 ms: 1.03x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 63.4 ms: 1.02x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| python_startup           | 20.6 ms                                                     | 20.2 ms: 1.02x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.67 ms: 1.02x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 74.5 ms: 1.02x faster                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 56.7 ms: 1.01x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 75.5 ms: 1.01x faster                                                       |
| unpickle_list            | 2.71 us                                                     | 2.76 us: 1.02x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.6 us: 1.03x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 40.8 ns: 1.03x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.16 us: 1.05x slower                                                       |
| scimark_fft              | 187 ms                                                      | 196 ms: 1.05x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 66.1 ms: 1.07x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 237 ms: 1.07x slower                                                        |
| pickle_list              | 2.75 us                                                     | 3.12 us: 1.13x slower                                                       |
| json                     | 3.14 ms                                                     | 3.58 ms: 1.14x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 18.1 ms: 1.16x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.71 ms: 1.20x slower                                                       |
| coverage                 | 39.0 ms                                                     | 47.7 ms: 1.22x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.22x faster                                                                |
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-4297d73-JIT/bm-20240212-pythonperf1-amd64-python-4297d7301b97aba2e0df-3.13.0a3+-4297d73.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: unknown