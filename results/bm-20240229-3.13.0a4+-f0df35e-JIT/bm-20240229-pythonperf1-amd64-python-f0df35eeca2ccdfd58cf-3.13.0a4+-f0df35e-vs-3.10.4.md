# Results vs. 3.10.4

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: windows-amd64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.20x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| chameleon      | 5.79 ms                                                     | 4.80 ms: 1.20x faster                                                       |
| docutils       | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| tornado_http   | 108 ms                                                      | 84.8 ms: 1.28x faster                                                       |
| Geometric mean | (ref)                                                       | 1.19x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 435 ms                                                      | 264 ms: 1.65x faster                                                        |
| async_tree_memoization  | 526 ms                                                      | 338 ms: 1.56x faster                                                        |
| async_tree_io           | 1.11 sec                                                    | 722 ms: 1.54x faster                                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 449 ms: 1.42x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.54x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 48.8 ms: 1.26x faster                                                       |
| nbody          | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| pidigits       | 149 ms                                                      | 150 ms: 1.01x slower                                                        |
| Geometric mean | (ref)                                                       | 1.14x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 136 ms                                                      | 114 ms: 1.19x faster                                                        |
| regex_compile  | 106 ms                                                      | 90.9 ms: 1.17x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| regex_effbot   | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.49 ms: 1.67x faster                                                       |
| pickle_pure_python   | 270 us                                                      | 180 us: 1.50x faster                                                        |
| unpickle_pure_python | 183 us                                                      | 138 us: 1.32x faster                                                        |
| tomli_loads          | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| xml_etree_process    | 44.5 ms                                                     | 36.2 ms: 1.23x faster                                                       |
| unpickle             | 9.09 us                                                     | 8.50 us: 1.07x faster                                                       |
| xml_etree_parse      | 96.8 ms                                                     | 91.8 ms: 1.06x faster                                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| xml_etree_iterparse  | 65.0 ms                                                     | 62.5 ms: 1.04x faster                                                       |
| json_loads           | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pickle_dict          | 17.2 us                                                     | 17.5 us: 1.02x slower                                                       |
| unpickle_list        | 2.71 us                                                     | 2.78 us: 1.02x slower                                                       |
| pickle_list          | 2.75 us                                                     | 2.88 us: 1.05x slower                                                       |
| pickle               | 6.85 us                                                     | 7.19 us: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 24.0 ms: 1.16x slower                                                       |
| python_startup_no_site | 15.5 ms                                                     | 21.7 ms: 1.40x slower                                                       |
| Geometric mean         | (ref)                                                       | 1.28x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 9.03 ms                                                     | 5.90 ms: 1.53x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 336 us                                                      | 69.9 us: 4.81x faster                                                       |
| deltablue                | 4.19 ms                                                     | 2.09 ms: 2.01x faster                                                       |
| logging_silent           | 94.6 ns                                                     | 56.0 ns: 1.69x faster                                                       |
| json_dumps               | 9.16 ms                                                     | 5.49 ms: 1.67x faster                                                       |
| async_tree_none          | 435 ms                                                      | 264 ms: 1.65x faster                                                        |
| generators               | 32.4 ms                                                     | 20.1 ms: 1.61x faster                                                       |
| asyncio_tcp              | 732 ms                                                      | 468 ms: 1.57x faster                                                        |
| async_tree_memoization   | 526 ms                                                      | 338 ms: 1.56x faster                                                        |
| async_tree_io            | 1.11 sec                                                    | 722 ms: 1.54x faster                                                        |
| sqlglot_parse            | 1.22 ms                                                     | 792 us: 1.53x faster                                                        |
| mako                     | 9.03 ms                                                     | 5.90 ms: 1.53x faster                                                       |
| raytrace                 | 273 ms                                                      | 183 ms: 1.50x faster                                                        |
| chaos                    | 61.7 ms                                                     | 41.2 ms: 1.50x faster                                                       |
| pickle_pure_python       | 270 us                                                      | 180 us: 1.50x faster                                                        |
| richards_super           | 52.2 ms                                                     | 35.0 ms: 1.49x faster                                                       |
| comprehensions           | 16.5 us                                                     | 11.1 us: 1.48x faster                                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.02 ms: 1.45x faster                                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 449 ms: 1.42x faster                                                        |
| crypto_pyaes             | 62.5 ms                                                     | 44.2 ms: 1.41x faster                                                       |
| go                       | 139 ms                                                      | 99.8 ms: 1.39x faster                                                       |
| pyflate                  | 409 ms                                                      | 298 ms: 1.37x faster                                                        |
| spectral_norm            | 77.3 ms                                                     | 56.3 ms: 1.37x faster                                                       |
| richards                 | 42.4 ms                                                     | 31.6 ms: 1.34x faster                                                       |
| unpickle_pure_python     | 183 us                                                      | 138 us: 1.32x faster                                                        |
| tomli_loads              | 1.67 sec                                                    | 1.29 sec: 1.30x faster                                                      |
| tornado_http             | 108 ms                                                      | 84.8 ms: 1.28x faster                                                       |
| mypy2                    | 555 ms                                                      | 438 ms: 1.27x faster                                                        |
| deepcopy_memo            | 28.8 us                                                     | 22.7 us: 1.27x faster                                                       |
| float                    | 61.7 ms                                                     | 48.8 ms: 1.26x faster                                                       |
| pycparser                | 930 ms                                                      | 740 ms: 1.26x faster                                                        |
| mdp                      | 1.78 sec                                                    | 1.43 sec: 1.25x faster                                                      |
| scimark_monte_carlo      | 57.3 ms                                                     | 46.3 ms: 1.24x faster                                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 1.71 sec: 1.23x faster                                                      |
| xml_etree_process        | 44.5 ms                                                     | 36.2 ms: 1.23x faster                                                       |
| coroutines               | 16.0 ms                                                     | 13.1 ms: 1.23x faster                                                       |
| scimark_sor              | 106 ms                                                      | 87.1 ms: 1.22x faster                                                       |
| sympy_sum                | 107 ms                                                      | 88.2 ms: 1.21x faster                                                       |
| sqlite_synth             | 1.91 us                                                     | 1.58 us: 1.21x faster                                                       |
| dulwich_log              | 50.5 ms                                                     | 41.8 ms: 1.21x faster                                                       |
| chameleon                | 5.79 ms                                                     | 4.80 ms: 1.20x faster                                                       |
| docutils                 | 1.92 sec                                                    | 1.60 sec: 1.20x faster                                                      |
| regex_dna                | 136 ms                                                      | 114 ms: 1.19x faster                                                        |
| scimark_lu               | 85.8 ms                                                     | 72.0 ms: 1.19x faster                                                       |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.29 ms: 1.19x faster                                                       |
| nbody                    | 71.3 ms                                                     | 59.9 ms: 1.19x faster                                                       |
| regex_compile            | 106 ms                                                      | 90.9 ms: 1.17x faster                                                       |
| sqlglot_normalize        | 205 ms                                                      | 176 ms: 1.16x faster                                                        |
| sympy_str                | 194 ms                                                      | 167 ms: 1.16x faster                                                        |
| pprint_safe_repr         | 592 ms                                                      | 510 ms: 1.16x faster                                                        |
| sympy_integrate          | 15.3 ms                                                     | 13.3 ms: 1.15x faster                                                       |
| pprint_pformat           | 1.22 sec                                                    | 1.06 sec: 1.15x faster                                                      |
| hexiom                   | 5.74 ms                                                     | 5.01 ms: 1.15x faster                                                       |
| deepcopy                 | 255 us                                                      | 223 us: 1.14x faster                                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 34.9 ms: 1.14x faster                                                       |
| bench_thread_pool        | 958 us                                                      | 840 us: 1.14x faster                                                        |
| deepcopy_reduce          | 2.20 us                                                     | 1.99 us: 1.11x faster                                                       |
| 2to3                     | 246 ms                                                      | 223 ms: 1.10x faster                                                        |
| sympy_expand             | 314 ms                                                      | 288 ms: 1.09x faster                                                        |
| nqueens                  | 66.6 ms                                                     | 61.4 ms: 1.09x faster                                                       |
| create_gc_cycles         | 800 us                                                      | 742 us: 1.08x faster                                                        |
| unpickle                 | 9.09 us                                                     | 8.50 us: 1.07x faster                                                       |
| regex_v8                 | 15.4 ms                                                     | 14.5 ms: 1.07x faster                                                       |
| regex_effbot             | 1.66 ms                                                     | 1.56 ms: 1.06x faster                                                       |
| logging_format           | 6.76 us                                                     | 6.38 us: 1.06x faster                                                       |
| xml_etree_parse          | 96.8 ms                                                     | 91.8 ms: 1.06x faster                                                       |
| scimark_fft              | 187 ms                                                      | 179 ms: 1.05x faster                                                        |
| xml_etree_generate       | 55.5 ms                                                     | 53.1 ms: 1.05x faster                                                       |
| logging_simple           | 6.22 us                                                     | 5.96 us: 1.04x faster                                                       |
| json                     | 3.14 ms                                                     | 3.01 ms: 1.04x faster                                                       |
| xml_etree_iterparse      | 65.0 ms                                                     | 62.5 ms: 1.04x faster                                                       |
| meteor_contest           | 75.9 ms                                                     | 73.3 ms: 1.04x faster                                                       |
| json_loads               | 14.0 us                                                     | 13.7 us: 1.02x faster                                                       |
| pathlib                  | 75.7 ms                                                     | 76.1 ms: 1.01x slower                                                       |
| pidigits                 | 149 ms                                                      | 150 ms: 1.01x slower                                                        |
| pickle_dict              | 17.2 us                                                     | 17.5 us: 1.02x slower                                                       |
| fannkuch                 | 256 ms                                                      | 261 ms: 1.02x slower                                                        |
| unpickle_list            | 2.71 us                                                     | 2.78 us: 1.02x slower                                                       |
| pickle_list              | 2.75 us                                                     | 2.88 us: 1.05x slower                                                       |
| pickle                   | 6.85 us                                                     | 7.19 us: 1.05x slower                                                       |
| gc_traversal             | 1.41 ms                                                     | 1.50 ms: 1.07x slower                                                       |
| async_generators         | 222 ms                                                      | 242 ms: 1.09x slower                                                        |
| bench_mp_pool            | 62.0 ms                                                     | 69.9 ms: 1.13x slower                                                       |
| python_startup           | 20.6 ms                                                     | 24.0 ms: 1.16x slower                                                       |
| coverage                 | 39.0 ms                                                     | 45.8 ms: 1.18x slower                                                       |
| telco                    | 3.94 ms                                                     | 4.65 ms: 1.18x slower                                                       |
| python_startup_no_site   | 15.5 ms                                                     | 21.7 ms: 1.40x slower                                                       |
| unpack_sequence          | 39.6 ns                                                     | 58.3 ns: 1.47x slower                                                       |
| Geometric mean           | (ref)                                                       | 1.20x faster                                                                |
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f0df35e-JIT/bm-20240229-pythonperf1-amd64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.16x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: unknown