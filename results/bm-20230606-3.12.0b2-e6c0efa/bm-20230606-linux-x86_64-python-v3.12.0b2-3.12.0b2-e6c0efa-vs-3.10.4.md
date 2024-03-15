
# Results vs. 3.10.4

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.35x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 269 ms: 1.30x faster                                       |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                     |
| tornado_http   | 136 ms                                                 | 99.3 ms: 1.37x faster                                      |
| Geometric mean | (ref)                                                  | 1.29x faster                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 468 ms: 1.56x faster                                       |
| async_tree_io           | 1.77 sec                                               | 1.15 sec: 1.53x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 570 ms: 1.53x faster                                       |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.44x faster                                       |
| Geometric mean          | (ref)                                                  | 1.51x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 154 ms                                                 | 89.7 ms: 1.71x faster                                      |
| float          | 117 ms                                                 | 80.3 ms: 1.46x faster                                      |
| pidigits       | 191 ms                                                 | 197 ms: 1.03x slower                                       |
| Geometric mean | (ref)                                                  | 1.34x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 145 ms: 1.30x faster                                       |
| regex_v8       | 27.8 ms                                                | 22.9 ms: 1.21x faster                                      |
| regex_dna      | 227 ms                                                 | 202 ms: 1.12x faster                                       |
| regex_effbot   | 3.63 ms                                                | 3.83 ms: 1.06x slower                                      |
| Geometric mean | (ref)                                                  | 1.14x faster                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 314 us: 1.54x faster                                       |
| unpickle_pure_python | 331 us                                                 | 217 us: 1.53x faster                                       |
| json_dumps           | 14.2 ms                                                | 9.69 ms: 1.46x faster                                      |
| tomli_loads          | 3.14 sec                                               | 2.24 sec: 1.40x faster                                     |
| xml_etree_process    | 79.1 ms                                                | 59.1 ms: 1.34x faster                                      |
| json_loads           | 31.2 us                                                | 25.1 us: 1.24x faster                                      |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                      |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                       |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                       |
| pickle_list          | 5.08 us                                                | 4.75 us: 1.07x faster                                      |
| unpickle_list        | 5.20 us                                                | 4.90 us: 1.06x faster                                      |
| pickle               | 10.7 us                                                | 10.9 us: 1.02x slower                                      |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                      |
| pickle_dict          | 29.6 us                                                | 31.3 us: 1.06x slower                                      |
| Geometric mean       | (ref)                                                  | 1.19x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.30 ms: 1.57x faster                                      |
| python_startup_no_site | 5.93 ms                                                | 6.76 ms: 1.14x slower                                      |
| Geometric mean         | (ref)                                                  | 1.17x faster                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.6 ms: 1.54x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 148 us: 3.68x faster                                       |
| generators               | 80.1 ms                                                | 31.6 ms: 2.54x faster                                      |
| deltablue                | 7.91 ms                                                | 3.46 ms: 2.29x faster                                      |
| richards_super           | 94.7 ms                                                | 48.9 ms: 1.94x faster                                      |
| logging_silent           | 190 ns                                                 | 103 ns: 1.85x faster                                       |
| richards                 | 79.3 ms                                                | 43.1 ms: 1.84x faster                                      |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.83x faster                                       |
| chaos                    | 115 ms                                                 | 63.6 ms: 1.82x faster                                      |
| asyncio_tcp              | 922 ms                                                 | 511 ms: 1.80x faster                                       |
| go                       | 240 ms                                                 | 136 ms: 1.77x faster                                       |
| raytrace                 | 507 ms                                                 | 296 ms: 1.71x faster                                       |
| nbody                    | 154 ms                                                 | 89.7 ms: 1.71x faster                                      |
| hexiom                   | 10.4 ms                                                | 6.19 ms: 1.68x faster                                      |
| scimark_monte_carlo      | 118 ms                                                 | 71.3 ms: 1.66x faster                                      |
| crypto_pyaes             | 128 ms                                                 | 78.0 ms: 1.64x faster                                      |
| spectral_norm            | 170 ms                                                 | 104 ms: 1.63x faster                                       |
| sqlglot_parse            | 2.17 ms                                                | 1.35 ms: 1.61x faster                                      |
| pyflate                  | 716 ms                                                 | 448 ms: 1.60x faster                                       |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                      |
| python_startup           | 14.6 ms                                                | 9.30 ms: 1.57x faster                                      |
| async_tree_none          | 728 ms                                                 | 468 ms: 1.56x faster                                       |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                       |
| mako                     | 16.3 ms                                                | 10.6 ms: 1.54x faster                                      |
| pickle_pure_python       | 484 us                                                 | 314 us: 1.54x faster                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                      |
| deepcopy_memo            | 58.5 us                                                | 38.1 us: 1.53x faster                                      |
| async_tree_io            | 1.77 sec                                               | 1.15 sec: 1.53x faster                                     |
| async_tree_memoization   | 870 ms                                                 | 570 ms: 1.53x faster                                       |
| unpickle_pure_python     | 331 us                                                 | 217 us: 1.53x faster                                       |
| json_dumps               | 14.2 ms                                                | 9.69 ms: 1.46x faster                                      |
| float                    | 117 ms                                                 | 80.3 ms: 1.46x faster                                      |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.44x faster                                       |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                     |
| tomli_loads              | 3.14 sec                                               | 2.24 sec: 1.40x faster                                     |
| pprint_pformat           | 2.10 sec                                               | 1.51 sec: 1.39x faster                                     |
| pprint_safe_repr         | 1.02 sec                                               | 735 ms: 1.38x faster                                       |
| comprehensions           | 28.8 us                                                | 20.9 us: 1.38x faster                                      |
| tornado_http             | 136 ms                                                 | 99.3 ms: 1.37x faster                                      |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.34x faster                                     |
| xml_etree_process        | 79.1 ms                                                | 59.1 ms: 1.34x faster                                      |
| fannkuch                 | 532 ms                                                 | 398 ms: 1.34x faster                                       |
| deepcopy                 | 479 us                                                 | 359 us: 1.33x faster                                       |
| logging_simple           | 8.30 us                                                | 6.24 us: 1.33x faster                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.89 ms: 1.32x faster                                      |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.19 us: 1.31x faster                                      |
| logging_format           | 9.09 us                                                | 6.96 us: 1.31x faster                                      |
| regex_compile            | 188 ms                                                 | 145 ms: 1.30x faster                                       |
| scimark_fft              | 466 ms                                                 | 358 ms: 1.30x faster                                       |
| 2to3                     | 348 ms                                                 | 269 ms: 1.30x faster                                       |
| unpack_sequence          | 60.0 ns                                                | 46.7 ns: 1.28x faster                                      |
| nqueens                  | 106 ms                                                 | 82.6 ms: 1.28x faster                                      |
| sqlglot_optimize         | 69.2 ms                                                | 54.2 ms: 1.28x faster                                      |
| json_loads               | 31.2 us                                                | 25.1 us: 1.24x faster                                      |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.8 ms: 1.24x faster                                      |
| dulwich_log              | 84.3 ms                                                | 68.4 ms: 1.23x faster                                      |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                     |
| regex_v8                 | 27.8 ms                                                | 22.9 ms: 1.21x faster                                      |
| json                     | 5.69 ms                                                | 4.76 ms: 1.19x faster                                      |
| bench_thread_pool        | 986 us                                                 | 829 us: 1.19x faster                                       |
| sqlalchemy_declarative   | 172 ms                                                 | 145 ms: 1.19x faster                                       |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                      |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                       |
| regex_dna                | 227 ms                                                 | 202 ms: 1.12x faster                                       |
| mdp                      | 2.85 sec                                               | 2.55 sec: 1.12x faster                                     |
| sqlite_synth             | 3.02 us                                                | 2.73 us: 1.11x faster                                      |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                       |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                      |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                       |
| pickle_list              | 5.08 us                                                | 4.75 us: 1.07x faster                                      |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.07x faster                                      |
| telco                    | 7.27 ms                                                | 6.83 ms: 1.06x faster                                      |
| unpickle_list            | 5.20 us                                                | 4.90 us: 1.06x faster                                      |
| async_generators         | 444 ms                                                 | 450 ms: 1.01x slower                                       |
| pickle                   | 10.7 us                                                | 10.9 us: 1.02x slower                                      |
| pidigits                 | 191 ms                                                 | 197 ms: 1.03x slower                                       |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                      |
| regex_effbot             | 3.63 ms                                                | 3.83 ms: 1.06x slower                                      |
| pickle_dict              | 29.6 us                                                | 31.3 us: 1.06x slower                                      |
| python_startup_no_site   | 5.93 ms                                                | 6.76 ms: 1.14x slower                                      |
| gc_traversal             | 3.62 ms                                                | 4.25 ms: 1.17x slower                                      |
| coverage                 | 79.4 ms                                                | 93.8 ms: 1.18x slower                                      |
| dask                     | 441 ms                                                 | 536 ms: 1.22x slower                                       |
| Geometric mean           | (ref)                                                  | 1.35x faster                                               |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (17) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.17x