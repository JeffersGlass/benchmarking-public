
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_continue
- machine: linux-x86_64
- commit hash: 9e86002
- commit date: 2024-02-13
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.25x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 273 ms: 1.27x faster                                                    |
| chameleon      | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                   |
| docutils       | 3.30 sec                                               | 2.62 sec: 1.26x faster                                                  |
| tornado_http   | 136 ms                                                 | 96.7 ms: 1.41x faster                                                   |
| Geometric mean | (ref)                                                  | 1.34x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 563 ms: 1.55x faster                                                    |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.43x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.54x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 99.1 ms: 1.55x faster                                                   |
| float          | 117 ms                                                 | 84.2 ms: 1.39x faster                                                   |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| Geometric mean | (ref)                                                  | 1.30x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.38x faster                                                    |
| regex_v8       | 27.8 ms                                                | 25.6 ms: 1.09x faster                                                   |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                    |
| Geometric mean | (ref)                                                  | 1.11x faster                                                            |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 293 us: 1.65x faster                                                    |
| unpickle_pure_python | 331 us                                                 | 223 us: 1.48x faster                                                    |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.46x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 57.3 ms: 1.38x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                   |
| xml_etree_generate   | 99.4 ms                                                | 84.8 ms: 1.17x faster                                                   |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.07x faster                                                    |
| pickle_list          | 5.08 us                                                | 4.91 us: 1.03x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.04 us: 1.03x faster                                                   |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                   |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                   |
| pickle_dict          | 29.6 us                                                | 33.2 us: 1.12x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                   |
| python_startup_no_site | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 12.0 ms: 1.36x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002 |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 108 us: 5.03x faster                                                    |
| generators               | 80.1 ms                                                | 29.6 ms: 2.71x faster                                                   |
| deltablue                | 7.91 ms                                                | 3.33 ms: 2.38x faster                                                   |
| logging_silent           | 190 ns                                                 | 99.4 ns: 1.91x faster                                                   |
| richards_super           | 94.7 ms                                                | 50.6 ms: 1.87x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 492 ms: 1.87x faster                                                    |
| raytrace                 | 507 ms                                                 | 276 ms: 1.84x faster                                                    |
| richards                 | 79.3 ms                                                | 44.8 ms: 1.77x faster                                                   |
| scimark_sor              | 220 ms                                                 | 124 ms: 1.76x faster                                                    |
| sqlglot_parse            | 2.17 ms                                                | 1.27 ms: 1.70x faster                                                   |
| chaos                    | 115 ms                                                 | 67.8 ms: 1.70x faster                                                   |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                                    |
| pickle_pure_python       | 484 us                                                 | 293 us: 1.65x faster                                                    |
| go                       | 240 ms                                                 | 146 ms: 1.65x faster                                                    |
| crypto_pyaes             | 128 ms                                                 | 77.7 ms: 1.64x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 72.4 ms: 1.63x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.60 ms: 1.60x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.3 us: 1.57x faster                                                   |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                                    |
| nbody                    | 154 ms                                                 | 99.1 ms: 1.55x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 563 ms: 1.55x faster                                                    |
| comprehensions           | 28.8 us                                                | 18.7 us: 1.53x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 223 us: 1.48x faster                                                    |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.46x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.71 us: 1.45x faster                                                   |
| pyflate                  | 716 ms                                                 | 496 ms: 1.45x faster                                                    |
| chameleon                | 9.68 ms                                                | 6.74 ms: 1.44x faster                                                   |
| logging_format           | 9.09 us                                                | 6.34 us: 1.43x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.43x faster                                                    |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                  |
| tornado_http             | 136 ms                                                 | 96.7 ms: 1.41x faster                                                   |
| deepcopy                 | 479 us                                                 | 340 us: 1.41x faster                                                    |
| float                    | 117 ms                                                 | 84.2 ms: 1.39x faster                                                   |
| hexiom                   | 10.4 ms                                                | 7.52 ms: 1.38x faster                                                   |
| regex_compile            | 188 ms                                                 | 136 ms: 1.38x faster                                                    |
| xml_etree_process        | 79.1 ms                                                | 57.3 ms: 1.38x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.03 us: 1.38x faster                                                   |
| mako                     | 16.3 ms                                                | 12.0 ms: 1.36x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 752 ms: 1.35x faster                                                    |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.33x faster                                                    |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.31x faster                                                  |
| spectral_norm            | 170 ms                                                 | 131 ms: 1.30x faster                                                    |
| 2to3                     | 348 ms                                                 | 273 ms: 1.27x faster                                                    |
| fannkuch                 | 532 ms                                                 | 420 ms: 1.27x faster                                                    |
| sqlglot_optimize         | 69.2 ms                                                | 54.8 ms: 1.26x faster                                                   |
| scimark_fft              | 466 ms                                                 | 370 ms: 1.26x faster                                                    |
| docutils                 | 3.30 sec                                               | 2.62 sec: 1.26x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 67.3 ms: 1.25x faster                                                   |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                    |
| sympy_integrate          | 25.8 ms                                                | 20.7 ms: 1.25x faster                                                   |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                                    |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                                    |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.34 ms: 1.21x faster                                                   |
| nqueens                  | 106 ms                                                 | 87.8 ms: 1.21x faster                                                   |
| sympy_expand             | 566 ms                                                 | 471 ms: 1.20x faster                                                    |
| unpack_sequence          | 60.0 ns                                                | 50.2 ns: 1.20x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 836 us: 1.18x faster                                                    |
| xml_etree_generate       | 99.4 ms                                                | 84.8 ms: 1.17x faster                                                   |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                   |
| json                     | 5.69 ms                                                | 5.10 ms: 1.12x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.57 sec: 1.11x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                                   |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                    |
| sqlite_synth             | 3.02 us                                                | 2.78 us: 1.09x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 25.6 ms: 1.09x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.07x faster                                                    |
| gc_traversal             | 3.62 ms                                                | 3.47 ms: 1.05x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.91 us: 1.03x faster                                                   |
| unpickle_list            | 5.20 us                                                | 5.04 us: 1.03x faster                                                   |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                    |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                    |
| async_generators         | 444 ms                                                 | 461 ms: 1.04x slower                                                    |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                   |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                   |
| pickle_dict              | 29.6 us                                                | 33.2 us: 1.12x slower                                                   |
| telco                    | 7.27 ms                                                | 8.52 ms: 1.17x slower                                                   |
| coverage                 | 79.4 ms                                                | 94.0 ms: 1.18x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 8.83 ms: 1.49x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.33x faster                                                            |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240213-3.13.0a3+-9e86002-JIT/bm-20240213-linux-x86_64-brandtbucher-justin_continue-3.13.0a3+-9e86002.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.25x


# Memory

- memory change: 1.10x