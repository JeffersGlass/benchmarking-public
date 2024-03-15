
# Results vs. 3.10.4

- fork: faster-cpython
- ref: guarantee_forward_pr
- machine: linux-x86_64
- commit hash: 1501bca
- commit date: 2024-01-08
- overall geometric mean: 1.27x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.20x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| chameleon      | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                            |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                           |
| tornado_http   | 136 ms                                                 | 97.3 ms: 1.40x faster                                                            |
| Geometric mean | (ref)                                                  | 1.29x faster                                                                     |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 448 ms: 1.63x faster                                                             |
| async_tree_memoization  | 870 ms                                                 | 578 ms: 1.51x faster                                                             |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                           |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| Geometric mean          | (ref)                                                  | 1.50x faster                                                                     |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 115 ms: 1.33x faster                                                             |
| float          | 117 ms                                                 | 92.7 ms: 1.26x faster                                                            |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| Geometric mean | (ref)                                                  | 1.20x faster                                                                     |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                            |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| regex_effbot   | 3.63 ms                                                | 3.57 ms: 1.02x faster                                                            |
| Geometric mean | (ref)                                                  | 1.10x faster                                                                     |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 303 us: 1.60x faster                                                             |
| unpickle_pure_python | 331 us                                                 | 237 us: 1.40x faster                                                             |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.34x faster                                                            |
| tomli_loads          | 3.14 sec                                               | 2.36 sec: 1.33x faster                                                           |
| xml_etree_process    | 79.1 ms                                                | 61.3 ms: 1.29x faster                                                            |
| xml_etree_generate   | 99.4 ms                                                | 90.3 ms: 1.10x faster                                                            |
| json_loads           | 31.2 us                                                | 28.5 us: 1.10x faster                                                            |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| unpickle_list        | 5.20 us                                                | 4.92 us: 1.06x faster                                                            |
| xml_etree_iterparse  | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| pickle_list          | 5.08 us                                                | 4.86 us: 1.05x faster                                                            |
| unpickle             | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| pickle_dict          | 29.6 us                                                | 35.7 us: 1.21x slower                                                            |
| Geometric mean       | (ref)                                                  | 1.13x faster                                                                     |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.0 ms: 1.45x faster                                                            |
| python_startup_no_site | 5.93 ms                                                | 8.68 ms: 1.46x slower                                                            |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                                     |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.8 ms: 1.18x faster                                                            |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.68x faster                                                             |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                                            |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                             |
| logging_silent           | 190 ns                                                 | 103 ns: 1.84x faster                                                             |
| richards_super           | 94.7 ms                                                | 55.6 ms: 1.70x faster                                                            |
| deltablue                | 7.91 ms                                                | 4.71 ms: 1.68x faster                                                            |
| raytrace                 | 507 ms                                                 | 302 ms: 1.68x faster                                                             |
| scimark_sor              | 220 ms                                                 | 133 ms: 1.65x faster                                                             |
| sqlglot_parse            | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                            |
| async_tree_none          | 728 ms                                                 | 448 ms: 1.63x faster                                                             |
| richards                 | 79.3 ms                                                | 49.1 ms: 1.61x faster                                                            |
| pickle_pure_python       | 484 us                                                 | 303 us: 1.60x faster                                                             |
| coroutines               | 35.1 ms                                                | 22.1 ms: 1.59x faster                                                            |
| chaos                    | 115 ms                                                 | 73.2 ms: 1.58x faster                                                            |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                            |
| crypto_pyaes             | 128 ms                                                 | 83.2 ms: 1.54x faster                                                            |
| go                       | 240 ms                                                 | 158 ms: 1.52x faster                                                             |
| unpack_sequence          | 60.0 ns                                                | 39.7 ns: 1.51x faster                                                            |
| async_tree_memoization   | 870 ms                                                 | 578 ms: 1.51x faster                                                             |
| scimark_lu               | 176 ms                                                 | 117 ms: 1.50x faster                                                             |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                           |
| python_startup           | 14.6 ms                                                | 10.0 ms: 1.45x faster                                                            |
| scimark_monte_carlo      | 118 ms                                                 | 81.8 ms: 1.44x faster                                                            |
| deepcopy_memo            | 58.5 us                                                | 40.8 us: 1.43x faster                                                            |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                           |
| pyflate                  | 716 ms                                                 | 506 ms: 1.42x faster                                                             |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 721 ms: 1.41x faster                                                             |
| tornado_http             | 136 ms                                                 | 97.3 ms: 1.40x faster                                                            |
| unpickle_pure_python     | 331 us                                                 | 237 us: 1.40x faster                                                             |
| logging_simple           | 8.30 us                                                | 6.08 us: 1.37x faster                                                            |
| comprehensions           | 28.8 us                                                | 21.2 us: 1.36x faster                                                            |
| deepcopy                 | 479 us                                                 | 356 us: 1.34x faster                                                             |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.34x faster                                                            |
| nbody                    | 154 ms                                                 | 115 ms: 1.33x faster                                                             |
| logging_format           | 9.09 us                                                | 6.83 us: 1.33x faster                                                            |
| tomli_loads              | 3.14 sec                                               | 2.36 sec: 1.33x faster                                                           |
| chameleon                | 9.68 ms                                                | 7.32 ms: 1.32x faster                                                            |
| deepcopy_reduce          | 4.17 us                                                | 3.16 us: 1.32x faster                                                            |
| xml_etree_process        | 79.1 ms                                                | 61.3 ms: 1.29x faster                                                            |
| pycparser                | 1.58 sec                                               | 1.24 sec: 1.27x faster                                                           |
| float                    | 117 ms                                                 | 92.7 ms: 1.26x faster                                                            |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                                             |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                                             |
| pprint_safe_repr         | 1.02 sec                                               | 818 ms: 1.24x faster                                                             |
| pprint_pformat           | 2.10 sec                                               | 1.70 sec: 1.24x faster                                                           |
| hexiom                   | 10.4 ms                                                | 8.42 ms: 1.23x faster                                                            |
| 2to3                     | 348 ms                                                 | 283 ms: 1.23x faster                                                             |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                             |
| dulwich_log              | 84.3 ms                                                | 69.2 ms: 1.22x faster                                                            |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                            |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                                           |
| sqlglot_optimize         | 69.2 ms                                                | 57.6 ms: 1.20x faster                                                            |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                                             |
| fannkuch                 | 532 ms                                                 | 444 ms: 1.20x faster                                                             |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                                             |
| mako                     | 16.3 ms                                                | 13.8 ms: 1.18x faster                                                            |
| spectral_norm            | 170 ms                                                 | 146 ms: 1.17x faster                                                             |
| bench_thread_pool        | 986 us                                                 | 848 us: 1.16x faster                                                             |
| sympy_expand             | 566 ms                                                 | 490 ms: 1.15x faster                                                             |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                            |
| nqueens                  | 106 ms                                                 | 94.5 ms: 1.12x faster                                                            |
| create_gc_cycles         | 1.62 ms                                                | 1.47 ms: 1.10x faster                                                            |
| xml_etree_generate       | 99.4 ms                                                | 90.3 ms: 1.10x faster                                                            |
| json_loads               | 31.2 us                                                | 28.5 us: 1.10x faster                                                            |
| pathlib                  | 20.5 ms                                                | 18.9 ms: 1.08x faster                                                            |
| json                     | 5.69 ms                                                | 5.27 ms: 1.08x faster                                                            |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 6.03 ms: 1.07x faster                                                            |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                             |
| mdp                      | 2.85 sec                                               | 2.69 sec: 1.06x faster                                                           |
| unpickle_list            | 5.20 us                                                | 4.92 us: 1.06x faster                                                            |
| xml_etree_iterparse      | 115 ms                                                 | 110 ms: 1.05x faster                                                             |
| pickle_list              | 5.08 us                                                | 4.86 us: 1.05x faster                                                            |
| sqlite_synth             | 3.02 us                                                | 2.90 us: 1.04x faster                                                            |
| meteor_contest           | 120 ms                                                 | 115 ms: 1.04x faster                                                             |
| scimark_fft              | 466 ms                                                 | 449 ms: 1.04x faster                                                             |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                             |
| regex_effbot             | 3.63 ms                                                | 3.57 ms: 1.02x faster                                                            |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                             |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                             |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                                             |
| unpickle                 | 14.4 us                                                | 14.9 us: 1.03x slower                                                            |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                            |
| gc_traversal             | 3.62 ms                                                | 4.29 ms: 1.19x slower                                                            |
| coverage                 | 79.4 ms                                                | 94.9 ms: 1.19x slower                                                            |
| telco                    | 7.27 ms                                                | 8.75 ms: 1.20x slower                                                            |
| pickle_dict              | 29.6 us                                                | 35.7 us: 1.21x slower                                                            |
| python_startup_no_site   | 5.93 ms                                                | 8.68 ms: 1.46x slower                                                            |
| Geometric mean           | (ref)                                                  | 1.27x faster                                                                     |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240108-3.13.0a2+-1501bca-PYTHON_UOPS/bm-20240108-linux-x86_64-faster%2dcpython-guarantee_forward_pr-3.13.0a2+-1501bca.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.22x
- 95% likely to have a speedup of 1.21x
- 99% likely to have a speedup of 1.20x


# Memory

- memory change: 1.06x