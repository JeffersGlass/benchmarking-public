# Results vs. 3.10.4

- fork: faster-cpython
- ref: replicate_fast_local
- machine: linux-x86_64
- commit hash: 5208402
- commit date: 2024-03-12
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.13x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 301 ms: 1.16x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.08 ms: 1.37x faster                                                            |
| docutils       | 3.30 sec                                               | 2.89 sec: 1.14x faster                                                           |
| html5lib       | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                            |
| tornado_http   | 136 ms                                                 | 104 ms: 1.32x faster                                                             |
| Geometric mean | (ref)                                                  | 1.24x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 461 ms: 1.58x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 592 ms: 1.47x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.24 sec: 1.43x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 742 ms: 1.37x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.46x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 124 ms: 1.24x faster                                                             |
| float          | 117 ms                                                 | 94.6 ms: 1.24x faster                                                            |
| pidigits       | 191 ms                                                 | 192 ms: 1.00x slower                                                             |
| Geometric mean | (ref)                                                  | 1.15x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                            |
| regex_compile  | 188 ms                                                 | 179 ms: 1.05x faster                                                             |
| regex_dna      | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| regex_effbot   | 3.63 ms                                                | 3.71 ms: 1.02x slower                                                            |
| Geometric mean | (ref)                                                  | 1.04x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 311 us: 1.56x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 63.5 ms: 1.25x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 277 us: 1.19x faster                                                             |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 92.7 ms: 1.07x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 161 ms: 1.04x faster                                                             |
| unpickle_list        | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| pickle_list          | 5.08 us                                                | 5.06 us: 1.00x faster                                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| unpickle             | 14.4 us                                                | 16.0 us: 1.11x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.99 ms: 1.52x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 48.2 ms                                                | 35.0 ms: 1.38x faster                                                            |
| mako            | 16.3 ms                                                | 12.8 ms: 1.28x faster                                                            |
| genshi_text     | 31.8 ms                                                | 26.9 ms: 1.18x faster                                                            |
| genshi_xml      | 66.0 ms                                                | 63.2 ms: 1.04x faster                                                            |
| Geometric mean  | (ref)                                                  | 1.21x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 115 us: 4.74x faster                                                             |
| generators               | 80.1 ms                                                | 30.3 ms: 2.64x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.90 ms: 2.03x faster                                                            |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                             |
| asyncio_tcp              | 922 ms                                                 | 507 ms: 1.82x faster                                                             |
| pylint                   | 551 ms                                                 | 333 ms: 1.65x faster                                                             |
| async_tree_none          | 728 ms                                                 | 461 ms: 1.58x faster                                                             |
| pickle_pure_python       | 484 us                                                 | 311 us: 1.56x faster                                                             |
| richards_super           | 94.7 ms                                                | 62.7 ms: 1.51x faster                                                            |
| chaos                    | 115 ms                                                 | 76.6 ms: 1.51x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.45 ms: 1.50x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 85.8 ms: 1.49x faster                                                            |
| raytrace                 | 507 ms                                                 | 343 ms: 1.48x faster                                                             |
| async_tree_memoization   | 870 ms                                                 | 592 ms: 1.47x faster                                                             |
| sqlglot_transpile        | 2.57 ms                                                | 1.79 ms: 1.44x faster                                                            |
| async_tree_io            | 1.77 sec                                               | 1.24 sec: 1.43x faster                                                           |
| scimark_sor              | 220 ms                                                 | 154 ms: 1.43x faster                                                             |
| coroutines               | 35.1 ms                                                | 24.7 ms: 1.42x faster                                                            |
| richards                 | 79.3 ms                                                | 56.1 ms: 1.41x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 41.5 us: 1.41x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.86 sec: 1.38x faster                                                           |
| django_template          | 48.2 ms                                                | 35.0 ms: 1.38x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 742 ms: 1.37x faster                                                             |
| chameleon                | 9.68 ms                                                | 7.08 ms: 1.37x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.3 us: 1.35x faster                                                            |
| go                       | 240 ms                                                 | 178 ms: 1.35x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.11 us: 1.34x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 88.3 ms: 1.34x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                            |
| deepcopy                 | 479 us                                                 | 362 us: 1.32x faster                                                             |
| thrift                   | 1.07 ms                                                | 813 us: 1.32x faster                                                             |
| tornado_http             | 136 ms                                                 | 104 ms: 1.32x faster                                                             |
| logging_simple           | 8.30 us                                                | 6.34 us: 1.31x faster                                                            |
| logging_format           | 9.09 us                                                | 7.07 us: 1.28x faster                                                            |
| mako                     | 16.3 ms                                                | 12.8 ms: 1.28x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                                             |
| xml_etree_process        | 79.1 ms                                                | 63.5 ms: 1.25x faster                                                            |
| html5lib                 | 88.9 ms                                                | 71.7 ms: 1.24x faster                                                            |
| nbody                    | 154 ms                                                 | 124 ms: 1.24x faster                                                             |
| float                    | 117 ms                                                 | 94.6 ms: 1.24x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.55 sec: 1.23x faster                                                           |
| djangocms                | 38.4 us                                                | 31.4 us: 1.22x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.30 sec: 1.21x faster                                                           |
| pyflate                  | 716 ms                                                 | 594 ms: 1.21x faster                                                             |
| spectral_norm            | 170 ms                                                 | 142 ms: 1.20x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 21.6 ms: 1.19x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 277 us: 1.19x faster                                                             |
| genshi_text              | 31.8 ms                                                | 26.9 ms: 1.18x faster                                                            |
| aiohttp                  | 1.44 ms                                                | 1.22 ms: 1.18x faster                                                            |
| sympy_sum                | 196 ms                                                 | 167 ms: 1.18x faster                                                             |
| dask                     | 441 ms                                                 | 377 ms: 1.17x faster                                                             |
| gunicorn                 | 1.53 ms                                                | 1.32 ms: 1.16x faster                                                            |
| 2to3                     | 348 ms                                                 | 301 ms: 1.16x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 885 ms: 1.15x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 73.7 ms: 1.14x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.89 sec: 1.14x faster                                                           |
| pprint_pformat           | 2.10 sec                                               | 1.85 sec: 1.14x faster                                                           |
| sympy_str                | 346 ms                                                 | 304 ms: 1.14x faster                                                             |
| sqlglot_optimize         | 69.2 ms                                                | 61.2 ms: 1.13x faster                                                            |
| bench_thread_pool        | 986 us                                                 | 874 us: 1.13x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                            |
| hexiom                   | 10.4 ms                                                | 9.23 ms: 1.13x faster                                                            |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                                            |
| scimark_lu               | 176 ms                                                 | 160 ms: 1.10x faster                                                             |
| sympy_expand             | 566 ms                                                 | 517 ms: 1.09x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.91 ms: 1.09x faster                                                            |
| json                     | 5.69 ms                                                | 5.24 ms: 1.09x faster                                                            |
| fannkuch                 | 532 ms                                                 | 490 ms: 1.08x faster                                                             |
| xml_etree_generate       | 99.4 ms                                                | 92.7 ms: 1.07x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.70 sec: 1.06x faster                                                           |
| regex_compile            | 188 ms                                                 | 179 ms: 1.05x faster                                                             |
| create_gc_cycles         | 1.62 ms                                                | 1.54 ms: 1.05x faster                                                            |
| pathlib                  | 20.5 ms                                                | 19.4 ms: 1.05x faster                                                            |
| genshi_xml               | 66.0 ms                                                | 63.2 ms: 1.04x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 161 ms: 1.04x faster                                                             |
| nqueens                  | 106 ms                                                 | 101 ms: 1.04x faster                                                             |
| unpickle_list            | 5.20 us                                                | 5.06 us: 1.03x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                                             |
| regex_dna                | 227 ms                                                 | 221 ms: 1.02x faster                                                             |
| sqlite_synth             | 3.02 us                                                | 2.96 us: 1.02x faster                                                            |
| scimark_fft              | 466 ms                                                 | 459 ms: 1.02x faster                                                             |
| meteor_contest           | 120 ms                                                 | 119 ms: 1.01x faster                                                             |
| pickle_list              | 5.08 us                                                | 5.06 us: 1.00x faster                                                            |
| pidigits                 | 191 ms                                                 | 192 ms: 1.00x slower                                                             |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                                             |
| regex_effbot             | 3.63 ms                                                | 3.71 ms: 1.02x slower                                                            |
| unpack_sequence          | 60.0 ns                                                | 62.0 ns: 1.03x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 3.79 ms: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| async_generators         | 444 ms                                                 | 484 ms: 1.09x slower                                                             |
| unpickle                 | 14.4 us                                                | 16.0 us: 1.11x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                            |
| telco                    | 7.27 ms                                                | 8.79 ms: 1.21x slower                                                            |
| coverage                 | 79.4 ms                                                | 99.2 ms: 1.25x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.99 ms: 1.52x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.22x faster                                                                     |

Benchmark hidden because not significant (2): bench_mp_pool, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240312-3.13.0a4+-5208402-PYTHON_UOPS/bm-20240312-linux-x86_64-faster%2dcpython-replicate_fast_local-3.13.0a4+-5208402.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.13x


# Memory

- memory change: 1.08x