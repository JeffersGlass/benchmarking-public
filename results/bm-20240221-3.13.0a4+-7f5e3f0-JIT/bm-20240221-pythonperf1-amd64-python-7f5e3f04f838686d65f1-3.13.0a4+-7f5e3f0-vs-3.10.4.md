
# Results vs. 3.10.4

- fork: python
- ref: 7f5e3f04f838686d65f1
- machine: windows-amd64
- commit hash: 7f5e3f0
- commit date: 2024-02-21
- overall geometric mean: 1.16x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 228 ms: 1.08x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.64 sec: 1.17x faster                                                      |
| tornado_http   | 108 ms                                                      | 85.6 ms: 1.27x faster                                                       |
| Geometric mean | (ref)                                                       | 1.17x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 261 ms: 1.67x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 335 ms: 1.57x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 718 ms: 1.54x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 445 ms: 1.43x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.55x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 50.8 ms: 1.22x faster                                                       |
| nbody          | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| pidigits       | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| regex_compile  | 106 ms                                                      | 101 ms: 1.05x faster                                                        |
| regex_effbot   | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.67 ms: 1.62x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 144 us: 1.27x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.34 sec: 1.25x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.6 ms: 1.04x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.4 us: 1.01x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.82 us: 1.02x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.79 us: 1.03x slower                                                       |
| pickle               | 6.85 us                                                     | 7.57 us: 1.11x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.11x faster                                                                |

Benchmark hidden because not significant (3): unpickle, json_loads, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 23.2 ms: 1.13x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 20.8 ms: 1.34x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.23x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 6.37 ms: 1.42x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0 |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 71.8 us: 4.68x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.21 ms: 1.89x faster                                                       |
| async_tree_none          | 435 ms                                                      | 261 ms: 1.67x faster                                                        |
| logging_silent           | 94.6 ns                                                     | 56.7 ns: 1.67x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.67 ms: 1.62x faster                                                       |
| generators               | 32.4 ms                                                     | 20.3 ms: 1.59x faster                                                       |
| async_tree_memoization   | 526 ms                                                      | 335 ms: 1.57x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 718 ms: 1.54x faster                                                        |
| asyncio_tcp              | 732 ms                                                      | 475 ms: 1.54x faster                                                        |
| pickle_pure_python       | 270 us                                                      | 180 us: 1.50x faster                                                        |
| richards_super           | 52.2 ms                                                     | 35.4 ms: 1.47x faster                                                       |
| sqlglot_parse            | 1.22 ms                                                     | 828 us: 1.47x faster                                                        |
| comprehensions           | 16.5 us                                                     | 11.4 us: 1.45x faster                                                       |
| chaos                    | 61.7 ms                                                     | 42.5 ms: 1.45x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 445 ms: 1.43x faster                                                        |
| raytrace                 | 273 ms                                                      | 191 ms: 1.43x faster                                                        |
| mako                     | 9.03 ms                                                     | 6.37 ms: 1.42x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.05 ms: 1.40x faster                                                       |
| crypto_pyaes             | 62.5 ms                                                     | 46.5 ms: 1.35x faster                                                       |
| richards                 | 42.4 ms                                                     | 31.9 ms: 1.33x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.65 sec: 1.28x faster                                                      |
| deepcopy_memo            | 28.8 us                                                     | 22.6 us: 1.27x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 144 us: 1.27x faster                                                        |
| tornado_http             | 108 ms                                                      | 85.6 ms: 1.27x faster                                                       |
| pycparser                | 930 ms                                                      | 741 ms: 1.26x faster                                                        |
| go                       | 139 ms                                                      | 111 ms: 1.25x faster                                                        |
| mypy2                    | 555 ms                                                      | 445 ms: 1.25x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 62.0 ms: 1.25x faster                                                       |
| tomli_loads              | 1.67 sec                                                    | 1.34 sec: 1.25x faster                                                      |
| pyflate                  | 409 ms                                                      | 331 ms: 1.23x faster                                                        |
| float                    | 61.7 ms                                                     | 50.8 ms: 1.22x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 42.0 ms: 1.20x faster                                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.0 ms: 1.20x faster                                                       |
| nbody                    | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.04 sec: 1.18x faster                                                      |
| sympy_sum                | 107 ms                                                      | 91.2 ms: 1.17x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.93 ms: 1.17x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.6 ms: 1.17x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.64 sec: 1.17x faster                                                      |
| pprint_safe_repr         | 592 ms                                                      | 512 ms: 1.16x faster                                                        |
| regex_dna                | 136 ms                                                      | 119 ms: 1.14x faster                                                        |
| sqlglot_normalize        | 205 ms                                                      | 180 ms: 1.14x faster                                                        |
| bench_thread_pool        | 958 us                                                      | 846 us: 1.13x faster                                                        |
| deepcopy                 | 255 us                                                      | 227 us: 1.12x faster                                                        |
| sympy_str                | 194 ms                                                      | 175 ms: 1.11x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.98 us: 1.11x faster                                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.8 ms: 1.11x faster                                                       |
| sqlglot_optimize         | 39.8 ms                                                     | 36.0 ms: 1.11x faster                                                       |
| scimark_lu               | 85.8 ms                                                     | 77.6 ms: 1.10x faster                                                       |
| mdp                      | 1.78 sec                                                    | 1.63 sec: 1.09x faster                                                      |
| 2to3                     | 246 ms                                                      | 228 ms: 1.08x faster                                                        |
| create_gc_cycles         | 800 us                                                      | 745 us: 1.07x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 62.3 ms: 1.07x faster                                                       |
| regex_compile            | 106 ms                                                      | 101 ms: 1.05x faster                                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.60 ms: 1.05x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.47 us: 1.04x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.96 us: 1.04x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.59 ms: 1.04x faster                                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.6 ms: 1.04x faster                                                       |
| sympy_expand             | 314 ms                                                      | 304 ms: 1.04x faster                                                        |
| xml_etree_parse          | 96.8 ms                                                     | 93.8 ms: 1.03x faster                                                       |
| scimark_sor              | 106 ms                                                      | 104 ms: 1.02x faster                                                        |
| regex_v8                 | 15.4 ms                                                     | 15.2 ms: 1.02x faster                                                       |
| scimark_fft              | 187 ms                                                      | 188 ms: 1.00x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.4 us: 1.01x slower                                                       |
| pidigits                 | 149 ms                                                      | 152 ms: 1.02x slower                                                        |
| pickle_list              | 2.75 us                                                     | 2.82 us: 1.02x slower                                                       |
| unpickle_list            | 2.71 us                                                     | 2.79 us: 1.03x slower                                                       |
| meteor_contest           | 75.9 ms                                                     | 78.0 ms: 1.03x slower                                                       |
| scimark_monte_carlo      | 57.3 ms                                                     | 59.6 ms: 1.04x slower                                                       |
| hexiom                   | 5.74 ms                                                     | 6.01 ms: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.49 ms: 1.06x slower                                                       |
| json                     | 3.14 ms                                                     | 3.38 ms: 1.08x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.57 us: 1.11x slower                                                       |
| bench_mp_pool            | 62.0 ms                                                     | 69.5 ms: 1.12x slower                                                       |
| python_startup           | 20.6 ms                                                     | 23.2 ms: 1.13x slower                                                       |
| async_generators         | 222 ms                                                      | 251 ms: 1.13x slower                                                        |
| telco                    | 3.94 ms                                                     | 4.53 ms: 1.15x slower                                                       |
| coverage                 | 39.0 ms                                                     | 48.1 ms: 1.23x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 20.8 ms: 1.34x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 89.7 ns: 2.26x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.16x faster                                                                |

Benchmark hidden because not significant (5): unpickle, json_loads, xml_etree_iterparse, fannkuch, pathlib
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240221-3.13.0a4+-7f5e3f0-JIT/bm-20240221-pythonperf1-amd64-python-7f5e3f04f838686d65f1-3.13.0a4+-7f5e3f0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.12x
- 95% likely to have a speedup of 1.11x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown