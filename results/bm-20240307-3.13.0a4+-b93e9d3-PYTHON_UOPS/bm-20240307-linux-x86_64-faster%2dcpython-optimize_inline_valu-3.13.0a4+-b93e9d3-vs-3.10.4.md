# Results vs. 3.10.4

- fork: faster-cpython
- ref: optimize_inline_valu
- machine: linux-x86_64
- commit hash: b93e9d3
- commit date: 2024-03-07
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.18x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 290 ms: 1.20x faster                                                             |
| chameleon      | 9.68 ms                                                | 6.93 ms: 1.40x faster                                                            |
| docutils       | 3.30 sec                                               | 2.83 sec: 1.17x faster                                                           |
| html5lib       | 88.9 ms                                                | 68.8 ms: 1.29x faster                                                            |
| tornado_http   | 136 ms                                                 | 97.5 ms: 1.40x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 444 ms: 1.64x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 572 ms: 1.52x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 718 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.51x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| float          | 117 ms                                                 | 93.3 ms: 1.25x faster                                                            |
| nbody          | 154 ms                                                 | 122 ms: 1.25x faster                                                             |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                             |
| Geometric mean | (ref)                                                  | 1.17x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 160 ms: 1.18x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                            |
| regex_effbot   | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                            |
| regex_dna      | 227 ms                                                 | 221 ms: 1.03x faster                                                             |
| Geometric mean | (ref)                                                  | 1.09x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.58x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                            |
| xml_etree_process    | 79.1 ms                                                | 60.2 ms: 1.31x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.48 sec: 1.27x faster                                                           |
| unpickle_pure_python | 331 us                                                 | 262 us: 1.26x faster                                                             |
| xml_etree_generate   | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                            |
| json_loads           | 31.2 us                                                | 27.8 us: 1.12x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.86 us: 1.07x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                            |
| pickle_dict          | 29.6 us                                                | 34.3 us: 1.16x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.12x faster                                                                     |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.79 ms: 1.48x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| django_template | 48.2 ms                                                | 34.0 ms: 1.42x faster                                                            |
| mako            | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                            |
| genshi_text     | 31.8 ms                                                | 25.1 ms: 1.27x faster                                                            |
| genshi_xml      | 66.0 ms                                                | 57.4 ms: 1.15x faster                                                            |
| Geometric mean  | (ref)                                                  | 1.30x faster                                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3 |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 114 us: 4.78x faster                                                             |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                                            |
| deltablue                | 7.91 ms                                                | 3.78 ms: 2.10x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                             |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                                             |
| richards_super           | 94.7 ms                                                | 53.8 ms: 1.76x faster                                                            |
| pylint                   | 551 ms                                                 | 321 ms: 1.72x faster                                                             |
| richards                 | 79.3 ms                                                | 47.3 ms: 1.68x faster                                                            |
| async_tree_none          | 728 ms                                                 | 444 ms: 1.64x faster                                                             |
| coroutines               | 35.1 ms                                                | 21.8 ms: 1.61x faster                                                            |
| sqlglot_parse            | 2.17 ms                                                | 1.35 ms: 1.61x faster                                                            |
| chaos                    | 115 ms                                                 | 72.3 ms: 1.60x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.58x faster                                                             |
| crypto_pyaes             | 128 ms                                                 | 83.1 ms: 1.54x faster                                                            |
| raytrace                 | 507 ms                                                 | 330 ms: 1.53x faster                                                             |
| sqlglot_transpile        | 2.57 ms                                                | 1.68 ms: 1.53x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 572 ms: 1.52x faster                                                             |
| spectral_norm            | 170 ms                                                 | 114 ms: 1.48x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                           |
| scimark_sor              | 220 ms                                                 | 151 ms: 1.46x faster                                                             |
| logging_format           | 9.09 us                                                | 6.26 us: 1.45x faster                                                            |
| logging_simple           | 8.30 us                                                | 5.73 us: 1.45x faster                                                            |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| django_template          | 48.2 ms                                                | 34.0 ms: 1.42x faster                                                            |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 718 ms: 1.41x faster                                                             |
| deepcopy_memo            | 58.5 us                                                | 41.8 us: 1.40x faster                                                            |
| tornado_http             | 136 ms                                                 | 97.5 ms: 1.40x faster                                                            |
| chameleon                | 9.68 ms                                                | 6.93 ms: 1.40x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 85.7 ms: 1.38x faster                                                            |
| go                       | 240 ms                                                 | 175 ms: 1.38x faster                                                             |
| mako                     | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                            |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.2 us: 1.36x faster                                                            |
| thrift                   | 1.07 ms                                                | 793 us: 1.35x faster                                                             |
| deepcopy_reduce          | 4.17 us                                                | 3.10 us: 1.34x faster                                                            |
| deepcopy                 | 479 us                                                 | 362 us: 1.32x faster                                                             |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                             |
| xml_etree_process        | 79.1 ms                                                | 60.2 ms: 1.31x faster                                                            |
| html5lib                 | 88.9 ms                                                | 68.8 ms: 1.29x faster                                                            |
| pprint_safe_repr         | 1.02 sec                                               | 801 ms: 1.27x faster                                                             |
| genshi_text              | 31.8 ms                                                | 25.1 ms: 1.27x faster                                                            |
| pprint_pformat           | 2.10 sec                                               | 1.66 sec: 1.27x faster                                                           |
| tomli_loads              | 3.14 sec                                               | 2.48 sec: 1.27x faster                                                           |
| unpickle_pure_python     | 331 us                                                 | 262 us: 1.26x faster                                                             |
| pyflate                  | 716 ms                                                 | 571 ms: 1.26x faster                                                             |
| float                    | 117 ms                                                 | 93.3 ms: 1.25x faster                                                            |
| nbody                    | 154 ms                                                 | 122 ms: 1.25x faster                                                             |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                            |
| sqlglot_optimize         | 69.2 ms                                                | 55.9 ms: 1.24x faster                                                            |
| sympy_sum                | 196 ms                                                 | 159 ms: 1.23x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.1 ms: 1.22x faster                                                            |
| aiohttp                  | 1.44 ms                                                | 1.18 ms: 1.22x faster                                                            |
| 2to3                     | 348 ms                                                 | 290 ms: 1.20x faster                                                             |
| gunicorn                 | 1.53 ms                                                | 1.28 ms: 1.20x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.32 sec: 1.20x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.78 ms: 1.18x faster                                                            |
| sympy_str                | 346 ms                                                 | 292 ms: 1.18x faster                                                             |
| regex_compile            | 188 ms                                                 | 160 ms: 1.18x faster                                                             |
| djangocms                | 38.4 us                                                | 32.9 us: 1.17x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.83 sec: 1.17x faster                                                           |
| sympy_expand             | 566 ms                                                 | 490 ms: 1.16x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 857 us: 1.15x faster                                                             |
| genshi_xml               | 66.0 ms                                                | 57.4 ms: 1.15x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 88.3 ms: 1.13x faster                                                            |
| regex_v8                 | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                            |
| json_loads               | 31.2 us                                                | 27.8 us: 1.12x faster                                                            |
| fannkuch                 | 532 ms                                                 | 481 ms: 1.11x faster                                                             |
| scimark_lu               | 176 ms                                                 | 160 ms: 1.10x faster                                                             |
| scimark_fft              | 466 ms                                                 | 426 ms: 1.09x faster                                                             |
| json                     | 5.69 ms                                                | 5.21 ms: 1.09x faster                                                            |
| nqueens                  | 106 ms                                                 | 98.1 ms: 1.08x faster                                                            |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                                           |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                             |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.02 ms: 1.07x faster                                                            |
| unpickle_list            | 5.20 us                                                | 4.86 us: 1.07x faster                                                            |
| pathlib                  | 20.5 ms                                                | 19.3 ms: 1.06x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 57.7 ns: 1.04x faster                                                            |
| regex_effbot             | 3.63 ms                                                | 3.49 ms: 1.04x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.93 us: 1.03x faster                                                            |
| meteor_contest           | 120 ms                                                 | 116 ms: 1.03x faster                                                             |
| regex_dna                | 227 ms                                                 | 221 ms: 1.03x faster                                                             |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                             |
| gc_traversal             | 3.62 ms                                                | 3.71 ms: 1.02x slower                                                            |
| async_generators         | 444 ms                                                 | 463 ms: 1.04x slower                                                             |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                            |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                            |
| pickle_dict              | 29.6 us                                                | 34.3 us: 1.16x slower                                                            |
| telco                    | 7.27 ms                                                | 8.51 ms: 1.17x slower                                                            |
| coverage                 | 79.4 ms                                                | 96.5 ms: 1.22x slower                                                            |
| dask                     | 441 ms                                                 | 536 ms: 1.22x slower                                                             |
| python_startup_no_site   | 5.93 ms                                                | 8.79 ms: 1.48x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.26x faster                                                                     |

Benchmark hidden because not significant (3): mypy2, pickle_list, bench_mp_pool
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240307-3.13.0a4+-b93e9d3-PYTHON_UOPS/bm-20240307-linux-x86_64-faster%2dcpython-optimize_inline_valu-3.13.0a4+-b93e9d3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.21x
- 95% likely to have a speedup of 1.20x
- 99% likely to have a speedup of 1.18x


# Memory

- memory change: 1.08x