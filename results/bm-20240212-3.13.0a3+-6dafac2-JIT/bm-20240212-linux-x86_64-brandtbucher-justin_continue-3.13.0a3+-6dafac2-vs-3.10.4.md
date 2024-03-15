
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 6dafac2
- commit date: 2024-02-12
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 274 ms: 1.27x faster                                                    |
| chameleon      | 9.68 ms                                                | 6.93 ms: 1.40x faster                                                   |
| docutils       | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                  |
| tornado_http   | 136 ms                                                 | 96.7 ms: 1.41x faster                                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 440 ms: 1.66x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 565 ms: 1.54x faster                                                    |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 715 ms: 1.42x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.6 ms: 1.64x faster                                                   |
| float          | 117 ms                                                 | 82.8 ms: 1.42x faster                                                   |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| Geometric mean | (ref)                                                  | 1.33x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 137 ms: 1.38x faster                                                    |
| regex_v8       | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                   |
| regex_dna      | 227 ms                                                 | 226 ms: 1.00x faster                                                    |
| Geometric mean | (ref)                                                  | 1.10x faster                                                            |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 297 us: 1.63x faster                                                    |
| tomli_loads          | 3.14 sec                                               | 2.06 sec: 1.53x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 227 us: 1.46x faster                                                    |
| xml_etree_process    | 79.1 ms                                                | 57.5 ms: 1.38x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                   |
| xml_etree_generate   | 99.4 ms                                                | 85.5 ms: 1.16x faster                                                   |
| json_loads           | 31.2 us                                                | 27.8 us: 1.12x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                    |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.04 us: 1.03x faster                                                   |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                                   |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                   |
| pickle_dict          | 29.6 us                                                | 32.9 us: 1.11x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.42x faster                                                   |
| python_startup_no_site | 5.93 ms                                                | 8.88 ms: 1.50x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.8 ms: 1.39x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 5.01x faster                                                    |
| generators               | 80.1 ms                                                | 29.1 ms: 2.76x faster                                                   |
| deltablue                | 7.91 ms                                                | 3.32 ms: 2.38x faster                                                   |
| richards_super           | 94.7 ms                                                | 50.5 ms: 1.87x faster                                                   |
| logging_silent           | 190 ns                                                 | 101 ns: 1.87x faster                                                    |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                    |
| raytrace                 | 507 ms                                                 | 275 ms: 1.84x faster                                                    |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.78x faster                                                    |
| chaos                    | 115 ms                                                 | 65.5 ms: 1.76x faster                                                   |
| richards                 | 79.3 ms                                                | 45.3 ms: 1.75x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 75.8 ms: 1.69x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 71.2 ms: 1.66x faster                                                   |
| async_tree_none          | 728 ms                                                 | 440 ms: 1.66x faster                                                    |
| go                       | 240 ms                                                 | 145 ms: 1.65x faster                                                    |
| nbody                    | 154 ms                                                 | 93.6 ms: 1.64x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 297 us: 1.63x faster                                                    |
| comprehensions           | 28.8 us                                                | 17.8 us: 1.61x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                   |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                                    |
| deepcopy_memo            | 58.5 us                                                | 37.2 us: 1.57x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.54x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 39.0 ns: 1.54x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 565 ms: 1.54x faster                                                    |
| tomli_loads              | 3.14 sec                                               | 2.06 sec: 1.53x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.61 us: 1.48x faster                                                   |
| pyflate                  | 716 ms                                                 | 484 ms: 1.48x faster                                                    |
| logging_format           | 9.09 us                                                | 6.20 us: 1.46x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 227 us: 1.46x faster                                                    |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.42x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.42x faster                                                   |
| hexiom                   | 10.4 ms                                                | 7.31 ms: 1.42x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 715 ms: 1.42x faster                                                    |
| float                    | 117 ms                                                 | 82.8 ms: 1.42x faster                                                   |
| deepcopy                 | 479 us                                                 | 340 us: 1.41x faster                                                    |
| tornado_http             | 136 ms                                                 | 96.7 ms: 1.41x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.93 ms: 1.40x faster                                                   |
| mako                     | 16.3 ms                                                | 11.8 ms: 1.39x faster                                                   |
| regex_compile            | 188 ms                                                 | 137 ms: 1.38x faster                                                    |
| pprint_pformat           | 2.10 sec                                               | 1.53 sec: 1.38x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 57.5 ms: 1.38x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 744 ms: 1.37x faster                                                    |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                    |
| spectral_norm            | 170 ms                                                 | 130 ms: 1.31x faster                                                    |
| scimark_fft              | 466 ms                                                 | 357 ms: 1.31x faster                                                    |
| fannkuch                 | 532 ms                                                 | 410 ms: 1.30x faster                                                    |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                                  |
| 2to3                     | 348 ms                                                 | 274 ms: 1.27x faster                                                    |
| sqlglot_optimize         | 69.2 ms                                                | 55.2 ms: 1.25x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 20.7 ms: 1.25x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.64 sec: 1.25x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 67.6 ms: 1.25x faster                                                   |
| sympy_sum                | 196 ms                                                 | 158 ms: 1.24x faster                                                    |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.21 ms: 1.24x faster                                                   |
| nqueens                  | 106 ms                                                 | 86.0 ms: 1.23x faster                                                   |
| sympy_str                | 346 ms                                                 | 282 ms: 1.23x faster                                                    |
| dask                     | 441 ms                                                 | 365 ms: 1.21x faster                                                    |
| sympy_expand             | 566 ms                                                 | 473 ms: 1.20x faster                                                    |
| bench_thread_pool        | 986 us                                                 | 836 us: 1.18x faster                                                    |
| xml_etree_generate       | 99.4 ms                                                | 85.5 ms: 1.16x faster                                                   |
| json                     | 5.69 ms                                                | 5.03 ms: 1.13x faster                                                   |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                                    |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                   |
| json_loads               | 31.2 us                                                | 27.8 us: 1.12x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.78 us: 1.09x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                   |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                    |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.04 us: 1.03x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.78 sec: 1.02x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                    |
| regex_dna                | 227 ms                                                 | 226 ms: 1.00x faster                                                    |
| async_generators         | 444 ms                                                 | 462 ms: 1.04x slower                                                    |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                                   |
| gc_traversal             | 3.62 ms                                                | 3.85 ms: 1.06x slower                                                   |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                   |
| pickle_dict              | 29.6 us                                                | 32.9 us: 1.11x slower                                                   |
| telco                    | 7.27 ms                                                | 8.29 ms: 1.14x slower                                                   |
| coverage                 | 79.4 ms                                                | 98.9 ms: 1.24x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 8.88 ms: 1.50x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.33x faster                                                            |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240212-3.13.0a3+-6dafac2-JIT/bm-20240212-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-6dafac2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x