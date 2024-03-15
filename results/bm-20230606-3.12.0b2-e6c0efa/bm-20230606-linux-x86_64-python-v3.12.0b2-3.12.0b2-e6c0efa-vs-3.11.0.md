
# Results vs. 3.11.0

- fork: python
- ref: v3.12.0b2
- machine: linux-x86_64
- commit hash: e6c0efa
- commit date: 2023-06-06
- overall geometric mean: 1.06x faster \*
- HPT reliability: 98.80%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 269 ms: 1.02x slower                                       |
| docutils       | 2.66 sec                                               | 2.72 sec: 1.02x slower                                     |
| tornado_http   | 98.1 ms                                                | 99.3 ms: 1.01x slower                                      |
| Geometric mean | (ref)                                                  | 1.02x slower                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| async_tree_none         | 528 ms                                                 | 468 ms: 1.13x faster                                       |
| async_tree_memoization  | 639 ms                                                 | 570 ms: 1.12x faster                                       |
| async_tree_io           | 1.29 sec                                               | 1.15 sec: 1.11x faster                                     |
| async_tree_cpu_io_mixed | 749 ms                                                 | 708 ms: 1.06x faster                                       |
| Geometric mean          | (ref)                                                  | 1.11x faster                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| nbody          | 96.0 ms                                                | 89.7 ms: 1.07x faster                                      |
| pidigits       | 194 ms                                                 | 197 ms: 1.02x slower                                       |
| float          | 78.9 ms                                                | 80.3 ms: 1.02x slower                                      |
| Geometric mean | (ref)                                                  | 1.01x faster                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| regex_dna      | 205 ms                                                 | 202 ms: 1.01x faster                                       |
| regex_compile  | 141 ms                                                 | 145 ms: 1.02x slower                                       |
| regex_effbot   | 3.51 ms                                                | 3.83 ms: 1.09x slower                                      |
| Geometric mean | (ref)                                                  | 1.03x slower                                               |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| json_dumps           | 13.3 ms                                                | 9.69 ms: 1.38x faster                                      |
| json_loads           | 29.2 us                                                | 25.1 us: 1.16x faster                                      |
| unpickle_pure_python | 242 us                                                 | 217 us: 1.12x faster                                       |
| pickle_dict          | 34.6 us                                                | 31.3 us: 1.10x faster                                      |
| unpickle_list        | 5.21 us                                                | 4.90 us: 1.06x faster                                      |
| xml_etree_parse      | 164 ms                                                 | 156 ms: 1.05x faster                                       |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                       |
| tomli_loads          | 2.30 sec                                               | 2.24 sec: 1.03x faster                                     |
| pickle_pure_python   | 320 us                                                 | 314 us: 1.02x faster                                       |
| pickle               | 11.0 us                                                | 10.9 us: 1.01x faster                                      |
| pickle_list          | 4.59 us                                                | 4.75 us: 1.04x slower                                      |
| xml_etree_process    | 56.9 ms                                                | 59.1 ms: 1.04x slower                                      |
| xml_etree_generate   | 81.1 ms                                                | 85.6 ms: 1.06x slower                                      |
| unpickle             | 13.8 us                                                | 15.0 us: 1.08x slower                                      |
| Geometric mean       | (ref)                                                  | 1.05x faster                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 9.30 ms: 1.09x slower                                      |
| python_startup_no_site | 6.01 ms                                                | 6.76 ms: 1.12x slower                                      |
| Geometric mean         | (ref)                                                  | 1.11x slower                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------:|
| mako      | 10.7 ms                                                | 10.6 ms: 1.01x faster                                      |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.12.0b2-3.12.0b2-e6c0efa |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------:|
| typing_runtime_protocols | 520 us                                                 | 148 us: 3.51x faster                                       |
| generators               | 74.9 ms                                                | 31.6 ms: 2.37x faster                                      |
| asyncio_tcp_ssl          | 3.11 sec                                               | 1.80 sec: 1.73x faster                                     |
| asyncio_tcp              | 875 ms                                                 | 511 ms: 1.71x faster                                       |
| json_dumps               | 13.3 ms                                                | 9.69 ms: 1.38x faster                                      |
| richards_super           | 61.9 ms                                                | 48.9 ms: 1.27x faster                                      |
| coroutines               | 27.0 ms                                                | 22.1 ms: 1.22x faster                                      |
| json_loads               | 29.2 us                                                | 25.1 us: 1.16x faster                                      |
| richards                 | 49.8 ms                                                | 43.1 ms: 1.16x faster                                      |
| deltablue                | 3.92 ms                                                | 3.46 ms: 1.13x faster                                      |
| chaos                    | 71.9 ms                                                | 63.6 ms: 1.13x faster                                      |
| comprehensions           | 23.6 us                                                | 20.9 us: 1.13x faster                                      |
| async_tree_none          | 528 ms                                                 | 468 ms: 1.13x faster                                       |
| async_tree_memoization   | 639 ms                                                 | 570 ms: 1.12x faster                                       |
| unpickle_pure_python     | 242 us                                                 | 217 us: 1.12x faster                                       |
| async_tree_io            | 1.29 sec                                               | 1.15 sec: 1.11x faster                                     |
| hexiom                   | 6.89 ms                                                | 6.19 ms: 1.11x faster                                      |
| pickle_dict              | 34.6 us                                                | 31.3 us: 1.10x faster                                      |
| json                     | 5.24 ms                                                | 4.76 ms: 1.10x faster                                      |
| go                       | 149 ms                                                 | 136 ms: 1.10x faster                                       |
| mdp                      | 2.77 sec                                               | 2.55 sec: 1.09x faster                                     |
| logging_silent           | 111 ns                                                 | 103 ns: 1.08x faster                                       |
| nbody                    | 96.0 ms                                                | 89.7 ms: 1.07x faster                                      |
| nqueens                  | 87.9 ms                                                | 82.6 ms: 1.06x faster                                      |
| unpickle_list            | 5.21 us                                                | 4.90 us: 1.06x faster                                      |
| sqlglot_parse            | 1.43 ms                                                | 1.35 ms: 1.06x faster                                      |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 708 ms: 1.06x faster                                       |
| deepcopy_memo            | 40.2 us                                                | 38.1 us: 1.05x faster                                      |
| xml_etree_parse          | 164 ms                                                 | 156 ms: 1.05x faster                                       |
| sqlglot_transpile        | 1.75 ms                                                | 1.67 ms: 1.05x faster                                      |
| raytrace                 | 309 ms                                                 | 296 ms: 1.04x faster                                       |
| sqlglot_normalize        | 113 ms                                                 | 109 ms: 1.04x faster                                       |
| spectral_norm            | 108 ms                                                 | 104 ms: 1.04x faster                                       |
| xml_etree_iterparse      | 108 ms                                                 | 104 ms: 1.04x faster                                       |
| pprint_pformat           | 1.55 sec                                               | 1.51 sec: 1.03x faster                                     |
| meteor_contest           | 109 ms                                                 | 106 ms: 1.03x faster                                       |
| tomli_loads              | 2.30 sec                                               | 2.24 sec: 1.03x faster                                     |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.89 ms: 1.03x faster                                      |
| scimark_lu               | 116 ms                                                 | 113 ms: 1.03x faster                                       |
| sqlglot_optimize         | 55.3 ms                                                | 54.2 ms: 1.02x faster                                      |
| fannkuch                 | 405 ms                                                 | 398 ms: 1.02x faster                                       |
| pickle_pure_python       | 320 us                                                 | 314 us: 1.02x faster                                       |
| deepcopy                 | 365 us                                                 | 359 us: 1.02x faster                                       |
| pprint_safe_repr         | 747 ms                                                 | 735 ms: 1.02x faster                                       |
| pycparser                | 1.19 sec                                               | 1.17 sec: 1.01x faster                                     |
| regex_dna                | 205 ms                                                 | 202 ms: 1.01x faster                                       |
| scimark_sor              | 121 ms                                                 | 120 ms: 1.01x faster                                       |
| deepcopy_reduce          | 3.22 us                                                | 3.19 us: 1.01x faster                                      |
| mako                     | 10.7 ms                                                | 10.6 ms: 1.01x faster                                      |
| pickle                   | 11.0 us                                                | 10.9 us: 1.01x faster                                      |
| bench_thread_pool        | 834 us                                                 | 829 us: 1.01x faster                                       |
| scimark_monte_carlo      | 70.7 ms                                                | 71.3 ms: 1.01x slower                                      |
| tornado_http             | 98.1 ms                                                | 99.3 ms: 1.01x slower                                      |
| pathlib                  | 18.5 ms                                                | 18.8 ms: 1.02x slower                                      |
| pidigits                 | 194 ms                                                 | 197 ms: 1.02x slower                                       |
| crypto_pyaes             | 76.7 ms                                                | 78.0 ms: 1.02x slower                                      |
| 2to3                     | 264 ms                                                 | 269 ms: 1.02x slower                                       |
| float                    | 78.9 ms                                                | 80.3 ms: 1.02x slower                                      |
| logging_format           | 6.81 us                                                | 6.96 us: 1.02x slower                                      |
| docutils                 | 2.66 sec                                               | 2.72 sec: 1.02x slower                                     |
| regex_compile            | 141 ms                                                 | 145 ms: 1.02x slower                                       |
| sqlalchemy_imperative    | 18.3 ms                                                | 18.8 ms: 1.03x slower                                      |
| sqlalchemy_declarative   | 140 ms                                                 | 145 ms: 1.03x slower                                       |
| pyflate                  | 434 ms                                                 | 448 ms: 1.03x slower                                       |
| pickle_list              | 4.59 us                                                | 4.75 us: 1.04x slower                                      |
| scimark_fft              | 345 ms                                                 | 358 ms: 1.04x slower                                       |
| xml_etree_process        | 56.9 ms                                                | 59.1 ms: 1.04x slower                                      |
| xml_etree_generate       | 81.1 ms                                                | 85.6 ms: 1.06x slower                                      |
| create_gc_cycles         | 1.43 ms                                                | 1.52 ms: 1.06x slower                                      |
| dulwich_log              | 64.6 ms                                                | 68.4 ms: 1.06x slower                                      |
| gc_traversal             | 4.01 ms                                                | 4.25 ms: 1.06x slower                                      |
| sqlite_synth             | 2.57 us                                                | 2.73 us: 1.06x slower                                      |
| unpack_sequence          | 43.5 ns                                                | 46.7 ns: 1.07x slower                                      |
| unpickle                 | 13.8 us                                                | 15.0 us: 1.08x slower                                      |
| python_startup           | 8.56 ms                                                | 9.30 ms: 1.09x slower                                      |
| regex_effbot             | 3.51 ms                                                | 3.83 ms: 1.09x slower                                      |
| python_startup_no_site   | 6.01 ms                                                | 6.76 ms: 1.12x slower                                      |
| coverage                 | 78.8 ms                                                | 93.8 ms: 1.19x slower                                      |
| async_generators         | 374 ms                                                 | 450 ms: 1.20x slower                                       |
| dask                     | 365 ms                                                 | 536 ms: 1.47x slower                                       |
| Geometric mean           | (ref)                                                  | 1.06x faster                                               |

Benchmark hidden because not significant (4): telco, bench_mp_pool, regex_v8, logging_simple
Ignored benchmarks (21) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, chameleon, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, mypy2, pylint, sympy_expand, sympy_integrate, sympy_str, sympy_sum, thrift


# HPT report

- Reliability score: 98.80% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.09x