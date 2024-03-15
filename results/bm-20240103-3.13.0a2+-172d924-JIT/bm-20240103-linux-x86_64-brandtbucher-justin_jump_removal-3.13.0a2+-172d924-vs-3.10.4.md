
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_jump_removal
- machine: linux-x86_64
- commit hash: 172d924
- commit date: 2024-01-03
- overall geometric mean: 1.31x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 274 ms: 1.27x faster                                                        |
| chameleon      | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                       |
| docutils       | 3.30 sec                                               | 2.65 sec: 1.24x faster                                                      |
| tornado_http   | 136 ms                                                 | 96.6 ms: 1.41x faster                                                       |
| Geometric mean | (ref)                                                  | 1.33x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 441 ms: 1.65x faster                                                        |
| async_tree_memoization  | 870 ms                                                 | 570 ms: 1.53x faster                                                        |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                      |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 720 ms: 1.41x faster                                                        |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.8 ms: 1.60x faster                                                       |
| float          | 117 ms                                                 | 84.3 ms: 1.39x faster                                                       |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                  | 1.31x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 139 ms: 1.35x faster                                                        |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                       |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                  | 1.11x faster                                                                |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.62x faster                                                        |
| unpickle_pure_python | 331 us                                                 | 226 us: 1.46x faster                                                        |
| tomli_loads          | 3.14 sec                                               | 2.16 sec: 1.45x faster                                                      |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                       |
| xml_etree_process    | 79.1 ms                                                | 59.1 ms: 1.34x faster                                                       |
| xml_etree_generate   | 99.4 ms                                                | 86.9 ms: 1.14x faster                                                       |
| json_loads           | 31.2 us                                                | 28.6 us: 1.09x faster                                                       |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                        |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                        |
| pickle_list          | 5.08 us                                                | 5.03 us: 1.01x faster                                                       |
| unpickle_list        | 5.20 us                                                | 5.37 us: 1.03x slower                                                       |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                       |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                       |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                       |
| python_startup_no_site | 5.93 ms                                                | 8.86 ms: 1.49x slower                                                       |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                       |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.89x faster                                                        |
| generators               | 80.1 ms                                                | 29.4 ms: 2.73x faster                                                       |
| deltablue                | 7.91 ms                                                | 3.91 ms: 2.03x faster                                                       |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                        |
| richards_super           | 94.7 ms                                                | 52.0 ms: 1.82x faster                                                       |
| raytrace                 | 507 ms                                                 | 280 ms: 1.81x faster                                                        |
| logging_silent           | 190 ns                                                 | 106 ns: 1.78x faster                                                        |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                                        |
| richards                 | 79.3 ms                                                | 45.6 ms: 1.74x faster                                                       |
| chaos                    | 115 ms                                                 | 66.8 ms: 1.73x faster                                                       |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.69x faster                                                       |
| async_tree_none          | 728 ms                                                 | 441 ms: 1.65x faster                                                        |
| crypto_pyaes             | 128 ms                                                 | 77.6 ms: 1.65x faster                                                       |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.62x faster                                                        |
| go                       | 240 ms                                                 | 149 ms: 1.61x faster                                                        |
| nbody                    | 154 ms                                                 | 95.8 ms: 1.60x faster                                                       |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.60x faster                                                       |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                       |
| scimark_monte_carlo      | 118 ms                                                 | 74.4 ms: 1.59x faster                                                       |
| comprehensions           | 28.8 us                                                | 18.3 us: 1.57x faster                                                       |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                                        |
| async_tree_memoization   | 870 ms                                                 | 570 ms: 1.53x faster                                                        |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                      |
| deepcopy_memo            | 58.5 us                                                | 39.2 us: 1.49x faster                                                       |
| unpickle_pure_python     | 331 us                                                 | 226 us: 1.46x faster                                                        |
| tomli_loads              | 3.14 sec                                               | 2.16 sec: 1.45x faster                                                      |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                      |
| pyflate                  | 716 ms                                                 | 502 ms: 1.43x faster                                                        |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                       |
| logging_format           | 9.09 us                                                | 6.42 us: 1.42x faster                                                       |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 720 ms: 1.41x faster                                                        |
| tornado_http             | 136 ms                                                 | 96.6 ms: 1.41x faster                                                       |
| logging_simple           | 8.30 us                                                | 5.92 us: 1.40x faster                                                       |
| float                    | 117 ms                                                 | 84.3 ms: 1.39x faster                                                       |
| chameleon                | 9.68 ms                                                | 7.00 ms: 1.38x faster                                                       |
| hexiom                   | 10.4 ms                                                | 7.58 ms: 1.37x faster                                                       |
| deepcopy                 | 479 us                                                 | 351 us: 1.37x faster                                                        |
| regex_compile            | 188 ms                                                 | 139 ms: 1.35x faster                                                        |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                                      |
| mako                     | 16.3 ms                                                | 12.1 ms: 1.35x faster                                                       |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                       |
| xml_etree_process        | 79.1 ms                                                | 59.1 ms: 1.34x faster                                                       |
| deepcopy_reduce          | 4.17 us                                                | 3.12 us: 1.34x faster                                                       |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                        |
| spectral_norm            | 170 ms                                                 | 131 ms: 1.30x faster                                                        |
| pprint_safe_repr         | 1.02 sec                                               | 788 ms: 1.29x faster                                                        |
| pprint_pformat           | 2.10 sec                                               | 1.65 sec: 1.28x faster                                                      |
| 2to3                     | 348 ms                                                 | 274 ms: 1.27x faster                                                        |
| scimark_fft              | 466 ms                                                 | 367 ms: 1.27x faster                                                        |
| dulwich_log              | 84.3 ms                                                | 66.9 ms: 1.26x faster                                                       |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.14 ms: 1.26x faster                                                       |
| sqlglot_optimize         | 69.2 ms                                                | 55.4 ms: 1.25x faster                                                       |
| fannkuch                 | 532 ms                                                 | 426 ms: 1.25x faster                                                        |
| docutils                 | 3.30 sec                                               | 2.65 sec: 1.24x faster                                                      |
| sympy_sum                | 196 ms                                                 | 158 ms: 1.24x faster                                                        |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                       |
| sympy_str                | 346 ms                                                 | 283 ms: 1.22x faster                                                        |
| unpack_sequence          | 60.0 ns                                                | 49.7 ns: 1.21x faster                                                       |
| dask                     | 441 ms                                                 | 365 ms: 1.21x faster                                                        |
| sympy_expand             | 566 ms                                                 | 474 ms: 1.19x faster                                                        |
| nqueens                  | 106 ms                                                 | 89.4 ms: 1.18x faster                                                       |
| bench_thread_pool        | 986 us                                                 | 843 us: 1.17x faster                                                        |
| xml_etree_generate       | 99.4 ms                                                | 86.9 ms: 1.14x faster                                                       |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                       |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                       |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                                      |
| json_loads               | 31.2 us                                                | 28.6 us: 1.09x faster                                                       |
| json                     | 5.69 ms                                                | 5.23 ms: 1.09x faster                                                       |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                       |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                                        |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.07x faster                                                       |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                        |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                        |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                        |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                        |
| asyncio_websockets       | 559 ms                                                 | 553 ms: 1.01x faster                                                        |
| pickle_list              | 5.08 us                                                | 5.03 us: 1.01x faster                                                       |
| async_generators         | 444 ms                                                 | 452 ms: 1.02x slower                                                        |
| unpickle_list            | 5.20 us                                                | 5.37 us: 1.03x slower                                                       |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                                       |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                       |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                       |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                       |
| telco                    | 7.27 ms                                                | 8.60 ms: 1.18x slower                                                       |
| coverage                 | 79.4 ms                                                | 94.6 ms: 1.19x slower                                                       |
| python_startup_no_site   | 5.93 ms                                                | 8.86 ms: 1.49x slower                                                       |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                                |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240103-3.13.0a2+-172d924-JIT/bm-20240103-linux-x86_64-brandtbucher-justin_jump_removal-3.13.0a2+-172d924.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x