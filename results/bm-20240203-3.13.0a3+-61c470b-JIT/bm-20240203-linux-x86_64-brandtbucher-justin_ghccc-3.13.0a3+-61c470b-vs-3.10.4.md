
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_ghccc
- machine: linux-x86_64
- commit hash: 61c470b
- commit date: 2024-02-03
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 275 ms: 1.27x faster                                                 |
| chameleon      | 9.68 ms                                                | 7.04 ms: 1.38x faster                                                |
| docutils       | 3.30 sec                                               | 2.65 sec: 1.24x faster                                               |
| tornado_http   | 136 ms                                                 | 97.6 ms: 1.40x faster                                                |
| Geometric mean | (ref)                                                  | 1.32x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 565 ms: 1.54x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                               |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 711 ms: 1.43x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.2 ms: 1.74x faster                                                |
| float          | 117 ms                                                 | 81.7 ms: 1.43x faster                                                |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.36x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 140 ms: 1.35x faster                                                 |
| regex_v8       | 27.8 ms                                                | 25.6 ms: 1.08x faster                                                |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| Geometric mean | (ref)                                                  | 1.11x faster                                                         |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 300 us: 1.62x faster                                                 |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                               |
| unpickle_pure_python | 331 us                                                 | 226 us: 1.47x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 58.4 ms: 1.36x faster                                                |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                |
| xml_etree_generate   | 99.4 ms                                                | 86.4 ms: 1.15x faster                                                |
| json_loads           | 31.2 us                                                | 28.4 us: 1.10x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.08x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                                |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                                |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                |
| python_startup_no_site | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 112 us: 4.86x faster                                                 |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                |
| deltablue                | 7.91 ms                                                | 3.78 ms: 2.09x faster                                                |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                 |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                 |
| richards_super           | 94.7 ms                                                | 52.0 ms: 1.82x faster                                                |
| raytrace                 | 507 ms                                                 | 281 ms: 1.80x faster                                                 |
| crypto_pyaes             | 128 ms                                                 | 72.5 ms: 1.76x faster                                                |
| nbody                    | 154 ms                                                 | 88.2 ms: 1.74x faster                                                |
| richards                 | 79.3 ms                                                | 46.2 ms: 1.72x faster                                                |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.69x faster                                                |
| chaos                    | 115 ms                                                 | 68.4 ms: 1.69x faster                                                |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                 |
| scimark_sor              | 220 ms                                                 | 133 ms: 1.66x faster                                                 |
| scimark_monte_carlo      | 118 ms                                                 | 73.2 ms: 1.62x faster                                                |
| pickle_pure_python       | 484 us                                                 | 300 us: 1.62x faster                                                 |
| go                       | 240 ms                                                 | 150 ms: 1.60x faster                                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.56x faster                                                 |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                                |
| comprehensions           | 28.8 us                                                | 18.6 us: 1.54x faster                                                |
| async_tree_memoization   | 870 ms                                                 | 565 ms: 1.54x faster                                                 |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                               |
| deepcopy_memo            | 58.5 us                                                | 39.5 us: 1.48x faster                                                |
| pyflate                  | 716 ms                                                 | 484 ms: 1.48x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                               |
| unpickle_pure_python     | 331 us                                                 | 226 us: 1.47x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                |
| float                    | 117 ms                                                 | 81.7 ms: 1.43x faster                                                |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                               |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 711 ms: 1.43x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.88 us: 1.41x faster                                                |
| logging_format           | 9.09 us                                                | 6.49 us: 1.40x faster                                                |
| tornado_http             | 136 ms                                                 | 97.6 ms: 1.40x faster                                                |
| chameleon                | 9.68 ms                                                | 7.04 ms: 1.38x faster                                                |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                 |
| mako                     | 16.3 ms                                                | 11.9 ms: 1.37x faster                                                |
| xml_etree_process        | 79.1 ms                                                | 58.4 ms: 1.36x faster                                                |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                |
| regex_compile            | 188 ms                                                 | 140 ms: 1.35x faster                                                 |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                                |
| spectral_norm            | 170 ms                                                 | 126 ms: 1.35x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.81 ms: 1.34x faster                                                |
| scimark_fft              | 466 ms                                                 | 349 ms: 1.33x faster                                                 |
| hexiom                   | 10.4 ms                                                | 7.81 ms: 1.33x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 109 ms: 1.31x faster                                                 |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.30x faster                                               |
| fannkuch                 | 532 ms                                                 | 414 ms: 1.29x faster                                                 |
| unpack_sequence          | 60.0 ns                                                | 47.2 ns: 1.27x faster                                                |
| 2to3                     | 348 ms                                                 | 275 ms: 1.27x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 812 ms: 1.25x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.69 sec: 1.25x faster                                               |
| docutils                 | 3.30 sec                                               | 2.65 sec: 1.24x faster                                               |
| sqlglot_optimize         | 69.2 ms                                                | 55.9 ms: 1.24x faster                                                |
| dulwich_log              | 84.3 ms                                                | 68.4 ms: 1.23x faster                                                |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                                |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                 |
| sympy_str                | 346 ms                                                 | 284 ms: 1.22x faster                                                 |
| nqueens                  | 106 ms                                                 | 87.0 ms: 1.22x faster                                                |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                 |
| bench_thread_pool        | 986 us                                                 | 840 us: 1.17x faster                                                 |
| sympy_expand             | 566 ms                                                 | 483 ms: 1.17x faster                                                 |
| xml_etree_generate       | 99.4 ms                                                | 86.4 ms: 1.15x faster                                                |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                                |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                |
| json_loads               | 31.2 us                                                | 28.4 us: 1.10x faster                                                |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.09x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                 |
| json                     | 5.69 ms                                                | 5.23 ms: 1.09x faster                                                |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.08x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 25.6 ms: 1.08x faster                                                |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                                |
| unpickle_list            | 5.20 us                                                | 4.98 us: 1.04x faster                                                |
| mdp                      | 2.85 sec                                               | 2.77 sec: 1.03x faster                                               |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                 |
| pickle_list              | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                 |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                 |
| gc_traversal             | 3.62 ms                                                | 3.59 ms: 1.01x faster                                                |
| async_generators         | 444 ms                                                 | 470 ms: 1.06x slower                                                 |
| unpickle                 | 14.4 us                                                | 15.5 us: 1.08x slower                                                |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                                |
| telco                    | 7.27 ms                                                | 8.44 ms: 1.16x slower                                                |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                |
| coverage                 | 79.4 ms                                                | 94.5 ms: 1.19x slower                                                |
| python_startup_no_site   | 5.93 ms                                                | 8.77 ms: 1.48x slower                                                |
| Geometric mean           | (ref)                                                  | 1.32x faster                                                         |

Benchmark hidden because not significant (3): mypy2, regex_effbot, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240203-3.13.0a3+-61c470b-JIT/bm-20240203-linux-x86_64-brandtbucher-justin_ghccc-3.13.0a3+-61c470b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.25x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.09x