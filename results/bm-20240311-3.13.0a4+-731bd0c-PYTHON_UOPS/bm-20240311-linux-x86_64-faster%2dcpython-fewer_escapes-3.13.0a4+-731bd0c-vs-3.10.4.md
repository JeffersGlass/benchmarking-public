# Results vs. 3.10.4

- fork: faster-cpython
- ref: fewer_escapes
- machine: linux-x86_64
- commit hash: 731bd0c
- commit date: 2024-03-11
- overall geometric mean: 1.21x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.12x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 300 ms: 1.16x faster                                                      |
| chameleon      | 9.68 ms                                                | 7.20 ms: 1.34x faster                                                     |
| docutils       | 3.30 sec                                               | 2.90 sec: 1.14x faster                                                    |
| html5lib       | 88.9 ms                                                | 70.6 ms: 1.26x faster                                                     |
| tornado_http   | 136 ms                                                 | 104 ms: 1.31x faster                                                      |
| Geometric mean | (ref)                                                  | 1.24x faster                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 460 ms: 1.58x faster                                                      |
| async_tree_memoization  | 870 ms                                                 | 595 ms: 1.46x faster                                                      |
| async_tree_io           | 1.77 sec                                               | 1.22 sec: 1.44x faster                                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 739 ms: 1.38x faster                                                      |
| Geometric mean          | (ref)                                                  | 1.46x faster                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 125 ms: 1.23x faster                                                      |
| float          | 117 ms                                                 | 97.0 ms: 1.21x faster                                                     |
| pidigits       | 191 ms                                                 | 191 ms: 1.00x slower                                                      |
| Geometric mean | (ref)                                                  | 1.14x faster                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.6 ms: 1.09x faster                                                     |
| regex_compile  | 188 ms                                                 | 178 ms: 1.06x faster                                                      |
| regex_effbot   | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                     |
| regex_dna      | 227 ms                                                 | 225 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                  | 1.05x faster                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 310 us: 1.56x faster                                                      |
| json_dumps           | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                     |
| xml_etree_process    | 79.1 ms                                                | 63.6 ms: 1.24x faster                                                     |
| tomli_loads          | 3.14 sec                                               | 2.53 sec: 1.24x faster                                                    |
| unpickle_pure_python | 331 us                                                 | 285 us: 1.16x faster                                                      |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                                     |
| xml_etree_generate   | 99.4 ms                                                | 92.7 ms: 1.07x faster                                                     |
| xml_etree_parse      | 168 ms                                                 | 162 ms: 1.04x faster                                                      |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                                     |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                                     |
| xml_etree_iterparse  | 115 ms                                                 | 113 ms: 1.02x faster                                                      |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                     |
| unpickle             | 14.4 us                                                | 16.1 us: 1.12x slower                                                     |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                     |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                              |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                     |
| python_startup_no_site | 5.93 ms                                                | 8.98 ms: 1.51x slower                                                     |
| Geometric mean         | (ref)                                                  | 1.04x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| django_template | 48.2 ms                                                | 35.3 ms: 1.36x faster                                                     |
| mako            | 16.3 ms                                                | 13.3 ms: 1.23x faster                                                     |
| genshi_text     | 31.8 ms                                                | 28.3 ms: 1.13x faster                                                     |
| genshi_xml      | 66.0 ms                                                | 65.0 ms: 1.02x faster                                                     |
| Geometric mean  | (ref)                                                  | 1.18x faster                                                              |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.67x faster                                                      |
| generators               | 80.1 ms                                                | 30.4 ms: 2.63x faster                                                     |
| deltablue                | 7.91 ms                                                | 3.91 ms: 2.02x faster                                                     |
| asyncio_tcp              | 922 ms                                                 | 506 ms: 1.82x faster                                                      |
| logging_silent           | 190 ns                                                 | 105 ns: 1.80x faster                                                      |
| pylint                   | 551 ms                                                 | 334 ms: 1.65x faster                                                      |
| async_tree_none          | 728 ms                                                 | 460 ms: 1.58x faster                                                      |
| pickle_pure_python       | 484 us                                                 | 310 us: 1.56x faster                                                      |
| coroutines               | 35.1 ms                                                | 23.3 ms: 1.51x faster                                                     |
| sqlglot_parse            | 2.17 ms                                                | 1.45 ms: 1.49x faster                                                     |
| chaos                    | 115 ms                                                 | 77.7 ms: 1.49x faster                                                     |
| richards_super           | 94.7 ms                                                | 64.4 ms: 1.47x faster                                                     |
| async_tree_memoization   | 870 ms                                                 | 595 ms: 1.46x faster                                                      |
| async_tree_io            | 1.77 sec                                               | 1.22 sec: 1.44x faster                                                    |
| scimark_sor              | 220 ms                                                 | 152 ms: 1.44x faster                                                      |
| sqlglot_transpile        | 2.57 ms                                                | 1.80 ms: 1.43x faster                                                     |
| crypto_pyaes             | 128 ms                                                 | 89.6 ms: 1.43x faster                                                     |
| raytrace                 | 507 ms                                                 | 356 ms: 1.42x faster                                                      |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                                     |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                                    |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 739 ms: 1.38x faster                                                      |
| django_template          | 48.2 ms                                                | 35.3 ms: 1.36x faster                                                     |
| richards                 | 79.3 ms                                                | 58.2 ms: 1.36x faster                                                     |
| deepcopy_memo            | 58.5 us                                                | 43.3 us: 1.35x faster                                                     |
| chameleon                | 9.68 ms                                                | 7.20 ms: 1.34x faster                                                     |
| json_dumps               | 14.2 ms                                                | 10.7 ms: 1.33x faster                                                     |
| scimark_monte_carlo      | 118 ms                                                 | 89.4 ms: 1.32x faster                                                     |
| logging_simple           | 8.30 us                                                | 6.29 us: 1.32x faster                                                     |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                     |
| go                       | 240 ms                                                 | 182 ms: 1.32x faster                                                      |
| thrift                   | 1.07 ms                                                | 817 us: 1.31x faster                                                      |
| tornado_http             | 136 ms                                                 | 104 ms: 1.31x faster                                                      |
| comprehensions           | 28.8 us                                                | 22.1 us: 1.30x faster                                                     |
| logging_format           | 9.09 us                                                | 7.00 us: 1.30x faster                                                     |
| deepcopy                 | 479 us                                                 | 371 us: 1.29x faster                                                      |
| html5lib                 | 88.9 ms                                                | 70.6 ms: 1.26x faster                                                     |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                      |
| xml_etree_process        | 79.1 ms                                                | 63.6 ms: 1.24x faster                                                     |
| tomli_loads              | 3.14 sec                                               | 2.53 sec: 1.24x faster                                                    |
| mako                     | 16.3 ms                                                | 13.3 ms: 1.23x faster                                                     |
| nbody                    | 154 ms                                                 | 125 ms: 1.23x faster                                                      |
| djangocms                | 38.4 us                                                | 31.5 us: 1.22x faster                                                     |
| float                    | 117 ms                                                 | 97.0 ms: 1.21x faster                                                     |
| pyflate                  | 716 ms                                                 | 597 ms: 1.20x faster                                                      |
| sympy_integrate          | 25.8 ms                                                | 21.8 ms: 1.19x faster                                                     |
| aiohttp                  | 1.44 ms                                                | 1.22 ms: 1.18x faster                                                     |
| sympy_sum                | 196 ms                                                 | 169 ms: 1.17x faster                                                      |
| dask                     | 441 ms                                                 | 379 ms: 1.16x faster                                                      |
| gunicorn                 | 1.53 ms                                                | 1.32 ms: 1.16x faster                                                     |
| 2to3                     | 348 ms                                                 | 300 ms: 1.16x faster                                                      |
| unpickle_pure_python     | 331 us                                                 | 285 us: 1.16x faster                                                      |
| dulwich_log              | 84.3 ms                                                | 72.9 ms: 1.16x faster                                                     |
| pycparser                | 1.58 sec                                               | 1.37 sec: 1.15x faster                                                    |
| docutils                 | 3.30 sec                                               | 2.90 sec: 1.14x faster                                                    |
| spectral_norm            | 170 ms                                                 | 150 ms: 1.13x faster                                                      |
| sympy_str                | 346 ms                                                 | 306 ms: 1.13x faster                                                      |
| bench_thread_pool        | 986 us                                                 | 875 us: 1.13x faster                                                      |
| genshi_text              | 31.8 ms                                                | 28.3 ms: 1.13x faster                                                     |
| sqlglot_optimize         | 69.2 ms                                                | 61.6 ms: 1.12x faster                                                     |
| pprint_safe_repr         | 1.02 sec                                               | 913 ms: 1.11x faster                                                      |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                                     |
| hexiom                   | 10.4 ms                                                | 9.40 ms: 1.11x faster                                                     |
| pprint_pformat           | 2.10 sec                                               | 1.91 sec: 1.10x faster                                                    |
| sympy_expand             | 566 ms                                                 | 516 ms: 1.10x faster                                                      |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.92 ms: 1.09x faster                                                     |
| regex_v8                 | 27.8 ms                                                | 25.6 ms: 1.09x faster                                                     |
| scimark_lu               | 176 ms                                                 | 163 ms: 1.08x faster                                                      |
| json                     | 5.69 ms                                                | 5.29 ms: 1.08x faster                                                     |
| xml_etree_generate       | 99.4 ms                                                | 92.7 ms: 1.07x faster                                                     |
| fannkuch                 | 532 ms                                                 | 497 ms: 1.07x faster                                                      |
| scimark_fft              | 466 ms                                                 | 436 ms: 1.07x faster                                                      |
| regex_compile            | 188 ms                                                 | 178 ms: 1.06x faster                                                      |
| pathlib                  | 20.5 ms                                                | 19.3 ms: 1.06x faster                                                     |
| create_gc_cycles         | 1.62 ms                                                | 1.53 ms: 1.06x faster                                                     |
| xml_etree_parse          | 168 ms                                                 | 162 ms: 1.04x faster                                                      |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                                     |
| regex_effbot             | 3.63 ms                                                | 3.52 ms: 1.03x faster                                                     |
| mdp                      | 2.85 sec                                               | 2.76 sec: 1.03x faster                                                    |
| pickle_list              | 5.08 us                                                | 4.97 us: 1.02x faster                                                     |
| xml_etree_iterparse      | 115 ms                                                 | 113 ms: 1.02x faster                                                      |
| sqlite_synth             | 3.02 us                                                | 2.98 us: 1.02x faster                                                     |
| genshi_xml               | 66.0 ms                                                | 65.0 ms: 1.02x faster                                                     |
| nqueens                  | 106 ms                                                 | 105 ms: 1.01x faster                                                      |
| regex_dna                | 227 ms                                                 | 225 ms: 1.01x faster                                                      |
| pidigits                 | 191 ms                                                 | 191 ms: 1.00x slower                                                      |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                                      |
| meteor_contest           | 120 ms                                                 | 121 ms: 1.01x slower                                                      |
| gc_traversal             | 3.62 ms                                                | 3.81 ms: 1.05x slower                                                     |
| async_generators         | 444 ms                                                 | 473 ms: 1.07x slower                                                      |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                     |
| unpickle                 | 14.4 us                                                | 16.1 us: 1.12x slower                                                     |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                     |
| telco                    | 7.27 ms                                                | 8.84 ms: 1.22x slower                                                     |
| coverage                 | 79.4 ms                                                | 98.0 ms: 1.23x slower                                                     |
| python_startup_no_site   | 5.93 ms                                                | 8.98 ms: 1.51x slower                                                     |
| Geometric mean           | (ref)                                                  | 1.21x faster                                                              |

Benchmark hidden because not significant (3): unpack_sequence, bench_mp_pool, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240311-3.13.0a4+-731bd0c-PYTHON_UOPS/bm-20240311-linux-x86_64-faster%2dcpython-fewer_escapes-3.13.0a4+-731bd0c.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.14x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.12x


# Memory

- memory change: 1.08x