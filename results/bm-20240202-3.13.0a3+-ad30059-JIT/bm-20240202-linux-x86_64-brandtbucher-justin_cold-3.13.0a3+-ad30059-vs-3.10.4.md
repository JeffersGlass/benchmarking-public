
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_cold
- machine: linux-x86_64
- commit hash: ad30059
- commit date: 2024-02-02
- overall geometric mean: 1.30x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.12x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                                |
| chameleon      | 9.68 ms                                                | 6.98 ms: 1.39x faster                                               |
| docutils       | 3.30 sec                                               | 2.66 sec: 1.24x faster                                              |
| tornado_http   | 136 ms                                                 | 97.6 ms: 1.40x faster                                               |
| Geometric mean | (ref)                                                  | 1.32x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 441 ms: 1.65x faster                                                |
| async_tree_memoization  | 870 ms                                                 | 566 ms: 1.54x faster                                                |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.49x faster                                              |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 713 ms: 1.43x faster                                                |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 106 ms: 1.45x faster                                                |
| float          | 117 ms                                                 | 86.5 ms: 1.35x faster                                               |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                                |
| Geometric mean | (ref)                                                  | 1.26x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                                |
| regex_v8       | 27.8 ms                                                | 24.9 ms: 1.11x faster                                               |
| regex_dna      | 227 ms                                                 | 222 ms: 1.02x faster                                                |
| Geometric mean | (ref)                                                  | 1.10x faster                                                        |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 295 us: 1.64x faster                                                |
| unpickle_pure_python | 331 us                                                 | 228 us: 1.45x faster                                                |
| tomli_loads          | 3.14 sec                                               | 2.22 sec: 1.42x faster                                              |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                               |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                               |
| xml_etree_generate   | 99.4 ms                                                | 86.6 ms: 1.15x faster                                               |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                               |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 109 ms: 1.06x faster                                                |
| unpickle_list        | 5.20 us                                                | 5.04 us: 1.03x faster                                               |
| pickle_list          | 5.08 us                                                | 5.20 us: 1.02x slower                                               |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                               |
| pickle               | 10.7 us                                                | 11.9 us: 1.11x slower                                               |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                               |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                               |
| python_startup_no_site | 5.93 ms                                                | 8.83 ms: 1.49x slower                                               |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|-----------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.7 ms: 1.29x faster                                               |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059 |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                |
| generators               | 80.1 ms                                                | 30.0 ms: 2.67x faster                                               |
| deltablue                | 7.91 ms                                                | 4.06 ms: 1.95x faster                                               |
| logging_silent           | 190 ns                                                 | 99.3 ns: 1.91x faster                                               |
| asyncio_tcp              | 922 ms                                                 | 496 ms: 1.86x faster                                                |
| richards_super           | 94.7 ms                                                | 51.3 ms: 1.85x faster                                               |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.83x faster                                                |
| raytrace                 | 507 ms                                                 | 283 ms: 1.79x faster                                                |
| richards                 | 79.3 ms                                                | 45.6 ms: 1.74x faster                                               |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                               |
| async_tree_none          | 728 ms                                                 | 441 ms: 1.65x faster                                                |
| pickle_pure_python       | 484 us                                                 | 295 us: 1.64x faster                                                |
| chaos                    | 115 ms                                                 | 70.4 ms: 1.64x faster                                               |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                               |
| crypto_pyaes             | 128 ms                                                 | 80.5 ms: 1.59x faster                                               |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.57x faster                                               |
| deepcopy_memo            | 58.5 us                                                | 37.4 us: 1.56x faster                                               |
| go                       | 240 ms                                                 | 154 ms: 1.56x faster                                                |
| async_tree_memoization   | 870 ms                                                 | 566 ms: 1.54x faster                                                |
| scimark_monte_carlo      | 118 ms                                                 | 76.9 ms: 1.54x faster                                               |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                                |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.49x faster                                              |
| comprehensions           | 28.8 us                                                | 19.7 us: 1.46x faster                                               |
| nbody                    | 154 ms                                                 | 106 ms: 1.45x faster                                                |
| unpickle_pure_python     | 331 us                                                 | 228 us: 1.45x faster                                                |
| logging_simple           | 8.30 us                                                | 5.77 us: 1.44x faster                                               |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                               |
| logging_format           | 9.09 us                                                | 6.36 us: 1.43x faster                                               |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 713 ms: 1.43x faster                                                |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                              |
| tomli_loads              | 3.14 sec                                               | 2.22 sec: 1.42x faster                                              |
| pyflate                  | 716 ms                                                 | 506 ms: 1.42x faster                                                |
| tornado_http             | 136 ms                                                 | 97.6 ms: 1.40x faster                                               |
| chameleon                | 9.68 ms                                                | 6.98 ms: 1.39x faster                                               |
| deepcopy                 | 479 us                                                 | 346 us: 1.38x faster                                                |
| deepcopy_reduce          | 4.17 us                                                | 3.03 us: 1.37x faster                                               |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                               |
| float                    | 117 ms                                                 | 86.5 ms: 1.35x faster                                               |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                               |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                              |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.30x faster                                                |
| mako                     | 16.3 ms                                                | 12.7 ms: 1.29x faster                                               |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                                |
| hexiom                   | 10.4 ms                                                | 8.28 ms: 1.26x faster                                               |
| unpack_sequence          | 60.0 ns                                                | 48.0 ns: 1.25x faster                                               |
| pprint_safe_repr         | 1.02 sec                                               | 814 ms: 1.25x faster                                                |
| fannkuch                 | 532 ms                                                 | 428 ms: 1.24x faster                                                |
| dulwich_log              | 84.3 ms                                                | 68.0 ms: 1.24x faster                                               |
| docutils                 | 3.30 sec                                               | 2.66 sec: 1.24x faster                                              |
| sqlglot_optimize         | 69.2 ms                                                | 55.9 ms: 1.24x faster                                               |
| pprint_pformat           | 2.10 sec                                               | 1.71 sec: 1.23x faster                                              |
| spectral_norm            | 170 ms                                                 | 139 ms: 1.22x faster                                                |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                               |
| scimark_fft              | 466 ms                                                 | 383 ms: 1.22x faster                                                |
| sympy_sum                | 196 ms                                                 | 162 ms: 1.21x faster                                                |
| sympy_str                | 346 ms                                                 | 288 ms: 1.20x faster                                                |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                |
| sympy_expand             | 566 ms                                                 | 482 ms: 1.17x faster                                                |
| bench_thread_pool        | 986 us                                                 | 845 us: 1.17x faster                                                |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.62 ms: 1.15x faster                                               |
| nqueens                  | 106 ms                                                 | 92.0 ms: 1.15x faster                                               |
| xml_etree_generate       | 99.4 ms                                                | 86.6 ms: 1.15x faster                                               |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                               |
| regex_v8                 | 27.8 ms                                                | 24.9 ms: 1.11x faster                                               |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                               |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.10x faster                                               |
| json                     | 5.69 ms                                                | 5.20 ms: 1.09x faster                                               |
| mdp                      | 2.85 sec                                               | 2.64 sec: 1.08x faster                                              |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                               |
| meteor_contest           | 120 ms                                                 | 111 ms: 1.08x faster                                                |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                |
| xml_etree_iterparse      | 115 ms                                                 | 109 ms: 1.06x faster                                                |
| unpickle_list            | 5.20 us                                                | 5.04 us: 1.03x faster                                               |
| regex_dna                | 227 ms                                                 | 222 ms: 1.02x faster                                                |
| pidigits                 | 191 ms                                                 | 188 ms: 1.01x faster                                                |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                |
| pickle_list              | 5.08 us                                                | 5.20 us: 1.02x slower                                               |
| gc_traversal             | 3.62 ms                                                | 3.81 ms: 1.05x slower                                               |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                               |
| async_generators         | 444 ms                                                 | 473 ms: 1.07x slower                                                |
| pickle                   | 10.7 us                                                | 11.9 us: 1.11x slower                                               |
| telco                    | 7.27 ms                                                | 8.49 ms: 1.17x slower                                               |
| coverage                 | 79.4 ms                                                | 93.8 ms: 1.18x slower                                               |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                               |
| python_startup_no_site   | 5.93 ms                                                | 8.83 ms: 1.49x slower                                               |
| Geometric mean           | (ref)                                                  | 1.30x faster                                                        |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240202-3.13.0a3+-ad30059-JIT/bm-20240202-linux-x86_64-brandtbucher-justin_cold-3.13.0a3+-ad30059.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.12x