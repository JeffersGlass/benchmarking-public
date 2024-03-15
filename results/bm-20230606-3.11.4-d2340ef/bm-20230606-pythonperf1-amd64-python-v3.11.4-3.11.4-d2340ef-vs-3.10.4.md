
# Results vs. 3.10.4

- fork: python
- ref: v3.11.4
- machine: windows-amd64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 221 ms: 1.11x faster                                        |
| chameleon      | 5.79 ms                                                     | 5.44 ms: 1.06x faster                                       |
| docutils       | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                      |
| html5lib       | 51.0 ms                                                     | 39.4 ms: 1.29x faster                                       |
| tornado_http   | 108 ms                                                      | 103 ms: 1.05x faster                                        |
| Geometric mean | (ref)                                                       | 1.13x faster                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 813 ms: 1.36x faster                                        |
| async_tree_memoization  | 526 ms                                                      | 392 ms: 1.34x faster                                        |
| async_tree_none         | 435 ms                                                      | 334 ms: 1.30x faster                                        |
| async_tree_cpu_io_mixed | 638 ms                                                      | 522 ms: 1.22x faster                                        |
| Geometric mean          | (ref)                                                       | 1.31x faster                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| float          | 61.7 ms                                                     | 56.7 ms: 1.09x faster                                       |
| nbody          | 71.3 ms                                                     | 70.4 ms: 1.01x faster                                       |
| pidigits       | 149 ms                                                      | 151 ms: 1.01x slower                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 92.8 ms: 1.14x faster                                       |
| regex_dna      | 136 ms                                                      | 120 ms: 1.14x faster                                        |
| regex_v8       | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                       |
| regex_effbot   | 1.66 ms                                                     | 1.52 ms: 1.09x faster                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| pickle_pure_python   | 270 us                                                      | 201 us: 1.34x faster                                        |
| unpickle_pure_python | 183 us                                                      | 153 us: 1.20x faster                                        |
| xml_etree_process    | 44.5 ms                                                     | 37.9 ms: 1.17x faster                                       |
| tomli_loads          | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                      |
| json_dumps           | 9.16 ms                                                     | 7.92 ms: 1.16x faster                                       |
| unpickle             | 9.09 us                                                     | 8.15 us: 1.12x faster                                       |
| json_loads           | 14.0 us                                                     | 13.3 us: 1.06x faster                                       |
| xml_etree_generate   | 55.5 ms                                                     | 53.8 ms: 1.03x faster                                       |
| pickle               | 6.85 us                                                     | 6.74 us: 1.02x faster                                       |
| pickle_dict          | 17.2 us                                                     | 18.8 us: 1.09x slower                                       |
| Geometric mean       | (ref)                                                       | 1.08x faster                                                |

Benchmark hidden because not significant (4): xml_etree_parse, xml_etree_iterparse, unpickle_list, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| python_startup_no_site | 15.5 ms                                                     | 17.5 ms: 1.13x slower                                       |
| Geometric mean         | (ref)                                                       | 1.06x slower                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| django_template | 28.9 ms                                                     | 24.5 ms: 1.18x faster                                       |
| mako            | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                       |
| genshi_text     | 19.8 ms                                                     | 17.8 ms: 1.11x faster                                       |
| genshi_xml      | 41.0 ms                                                     | 38.6 ms: 1.06x faster                                       |
| Geometric mean  | (ref)                                                       | 1.13x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-pythonperf1-amd64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
| deltablue                | 4.19 ms                                                     | 2.71 ms: 1.54x faster                                       |
| go                       | 139 ms                                                      | 100 ms: 1.38x faster                                        |
| scimark_sor              | 106 ms                                                      | 76.9 ms: 1.38x faster                                       |
| richards                 | 42.4 ms                                                     | 31.0 ms: 1.37x faster                                       |
| async_tree_io            | 1.11 sec                                                    | 813 ms: 1.36x faster                                        |
| scimark_lu               | 85.8 ms                                                     | 63.4 ms: 1.35x faster                                       |
| richards_super           | 52.2 ms                                                     | 38.6 ms: 1.35x faster                                       |
| async_tree_memoization   | 526 ms                                                      | 392 ms: 1.34x faster                                        |
| pickle_pure_python       | 270 us                                                      | 201 us: 1.34x faster                                        |
| pyflate                  | 409 ms                                                      | 310 ms: 1.32x faster                                        |
| raytrace                 | 273 ms                                                      | 208 ms: 1.32x faster                                        |
| logging_silent           | 94.6 ns                                                     | 72.1 ns: 1.31x faster                                       |
| async_tree_none          | 435 ms                                                      | 334 ms: 1.30x faster                                        |
| sqlglot_parse            | 1.22 ms                                                     | 936 us: 1.30x faster                                        |
| html5lib                 | 51.0 ms                                                     | 39.4 ms: 1.29x faster                                       |
| sqlglot_transpile        | 1.48 ms                                                     | 1.15 ms: 1.29x faster                                       |
| pycparser                | 930 ms                                                      | 726 ms: 1.28x faster                                        |
| thrift                   | 617 us                                                      | 486 us: 1.27x faster                                        |
| scimark_monte_carlo      | 57.3 ms                                                     | 45.1 ms: 1.27x faster                                       |
| chaos                    | 61.7 ms                                                     | 48.8 ms: 1.26x faster                                       |
| hexiom                   | 5.74 ms                                                     | 4.55 ms: 1.26x faster                                       |
| crypto_pyaes             | 62.5 ms                                                     | 49.7 ms: 1.26x faster                                       |
| sqlalchemy_declarative   | 103 ms                                                      | 82.7 ms: 1.25x faster                                       |
| async_tree_cpu_io_mixed  | 638 ms                                                      | 522 ms: 1.22x faster                                        |
| async_generators         | 222 ms                                                      | 184 ms: 1.20x faster                                        |
| unpickle_pure_python     | 183 us                                                      | 153 us: 1.20x faster                                        |
| django_template          | 28.9 ms                                                     | 24.5 ms: 1.18x faster                                       |
| mako                     | 9.03 ms                                                     | 7.67 ms: 1.18x faster                                       |
| xml_etree_process        | 44.5 ms                                                     | 37.9 ms: 1.17x faster                                       |
| tomli_loads              | 1.67 sec                                                    | 1.43 sec: 1.17x faster                                      |
| pprint_pformat           | 1.22 sec                                                    | 1.05 sec: 1.16x faster                                      |
| json_dumps               | 9.16 ms                                                     | 7.92 ms: 1.16x faster                                       |
| docutils                 | 1.92 sec                                                    | 1.66 sec: 1.16x faster                                      |
| pprint_safe_repr         | 592 ms                                                      | 513 ms: 1.15x faster                                        |
| regex_compile            | 106 ms                                                      | 92.8 ms: 1.14x faster                                       |
| regex_dna                | 136 ms                                                      | 120 ms: 1.14x faster                                        |
| sqlglot_optimize         | 39.8 ms                                                     | 35.2 ms: 1.13x faster                                       |
| deepcopy_memo            | 28.8 us                                                     | 25.6 us: 1.12x faster                                       |
| unpickle                 | 9.09 us                                                     | 8.15 us: 1.12x faster                                       |
| genshi_text              | 19.8 ms                                                     | 17.8 ms: 1.11x faster                                       |
| 2to3                     | 246 ms                                                      | 221 ms: 1.11x faster                                        |
| regex_v8                 | 15.4 ms                                                     | 13.9 ms: 1.11x faster                                       |
| sympy_integrate          | 15.3 ms                                                     | 13.9 ms: 1.10x faster                                       |
| sqlalchemy_imperative    | 11.4 ms                                                     | 10.4 ms: 1.09x faster                                       |
| regex_effbot             | 1.66 ms                                                     | 1.52 ms: 1.09x faster                                       |
| dask                     | 313 ms                                                      | 287 ms: 1.09x faster                                        |
| float                    | 61.7 ms                                                     | 56.7 ms: 1.09x faster                                       |
| dulwich_log              | 50.5 ms                                                     | 46.4 ms: 1.09x faster                                       |
| sqlite_synth             | 1.91 us                                                     | 1.76 us: 1.09x faster                                       |
| create_gc_cycles         | 800 us                                                      | 740 us: 1.08x faster                                        |
| coroutines               | 16.0 ms                                                     | 14.8 ms: 1.08x faster                                       |
| sqlglot_normalize        | 205 ms                                                      | 193 ms: 1.07x faster                                        |
| chameleon                | 5.79 ms                                                     | 5.44 ms: 1.06x faster                                       |
| genshi_xml               | 41.0 ms                                                     | 38.6 ms: 1.06x faster                                       |
| aiohttp                  | 995 us                                                      | 936 us: 1.06x faster                                        |
| json_loads               | 14.0 us                                                     | 13.3 us: 1.06x faster                                       |
| pylint                   | 350 ms                                                      | 331 ms: 1.06x faster                                        |
| comprehensions           | 16.5 us                                                     | 15.6 us: 1.06x faster                                       |
| deepcopy_reduce          | 2.20 us                                                     | 2.09 us: 1.05x faster                                       |
| sympy_expand             | 314 ms                                                      | 299 ms: 1.05x faster                                        |
| tornado_http             | 108 ms                                                      | 103 ms: 1.05x faster                                        |
| scimark_sparse_mat_mult  | 2.72 ms                                                     | 2.60 ms: 1.05x faster                                       |
| sympy_sum                | 107 ms                                                      | 103 ms: 1.04x faster                                        |
| sympy_str                | 194 ms                                                      | 187 ms: 1.04x faster                                        |
| deepcopy                 | 255 us                                                      | 246 us: 1.04x faster                                        |
| spectral_norm            | 77.3 ms                                                     | 74.7 ms: 1.03x faster                                       |
| xml_etree_generate       | 55.5 ms                                                     | 53.8 ms: 1.03x faster                                       |
| typing_runtime_protocols | 336 us                                                      | 326 us: 1.03x faster                                        |
| nqueens                  | 66.6 ms                                                     | 65.1 ms: 1.02x faster                                       |
| scimark_fft              | 187 ms                                                      | 184 ms: 1.02x faster                                        |
| pickle                   | 6.85 us                                                     | 6.74 us: 1.02x faster                                       |
| mdp                      | 1.78 sec                                                    | 1.76 sec: 1.01x faster                                      |
| nbody                    | 71.3 ms                                                     | 70.4 ms: 1.01x faster                                       |
| flaskblogging            | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                      |
| pidigits                 | 149 ms                                                      | 151 ms: 1.01x slower                                        |
| telco                    | 3.94 ms                                                     | 4.00 ms: 1.02x slower                                       |
| meteor_contest           | 75.9 ms                                                     | 77.4 ms: 1.02x slower                                       |
| pathlib                  | 75.7 ms                                                     | 77.5 ms: 1.02x slower                                       |
| fannkuch                 | 256 ms                                                      | 263 ms: 1.03x slower                                        |
| bench_mp_pool            | 62.0 ms                                                     | 66.1 ms: 1.06x slower                                       |
| generators               | 32.4 ms                                                     | 34.5 ms: 1.06x slower                                       |
| logging_format           | 6.76 us                                                     | 7.26 us: 1.07x slower                                       |
| gc_traversal             | 1.41 ms                                                     | 1.52 ms: 1.08x slower                                       |
| logging_simple           | 6.22 us                                                     | 6.71 us: 1.08x slower                                       |
| pickle_dict              | 17.2 us                                                     | 18.8 us: 1.09x slower                                       |
| json                     | 3.14 ms                                                     | 3.51 ms: 1.12x slower                                       |
| python_startup_no_site   | 15.5 ms                                                     | 17.5 ms: 1.13x slower                                       |
| asyncio_tcp_ssl          | 2.11 sec                                                    | 2.41 sec: 1.14x slower                                      |
| unpack_sequence          | 39.6 ns                                                     | 48.1 ns: 1.21x slower                                       |
| asyncio_tcp              | 732 ms                                                      | 932 ms: 1.27x slower                                        |
| coverage                 | 39.0 ms                                                     | 55.6 ms: 1.43x slower                                       |
| Geometric mean           | (ref)                                                       | 1.10x faster                                                |

Benchmark hidden because not significant (6): bench_thread_pool, xml_etree_parse, xml_etree_iterparse, python_startup, unpickle_list, pickle_list
Ignored benchmarks (1) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.07x
- 99% likely to have a speedup of 1.06x


# Memory

- memory change: unknown