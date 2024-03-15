# Results vs. 3.10.4

- fork: python
- ref: 8c094c3095feb4de2efe
- machine: linux-x86_64
- commit hash: 8c094c3
- commit date: 2024-03-13
- overall geometric mean: 1.29x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 282 ms: 1.23x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| docutils       | 3.30 sec                                               | 2.77 sec: 1.19x faster                                                 |
| html5lib       | 88.9 ms                                                | 65.7 ms: 1.35x faster                                                  |
| tornado_http   | 136 ms                                                 | 98.7 ms: 1.38x faster                                                  |
| Geometric mean | (ref)                                                  | 1.31x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 449 ms: 1.62x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.22 sec: 1.45x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.4 ms: 1.66x faster                                                  |
| float          | 117 ms                                                 | 79.8 ms: 1.47x faster                                                  |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.4 ms: 1.09x faster                                                  |
| regex_dna      | 227 ms                                                 | 238 ms: 1.05x slower                                                   |
| regex_effbot   | 3.63 ms                                                | 3.82 ms: 1.05x slower                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.60x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.08 sec: 1.51x faster                                                 |
| unpickle_pure_python | 331 us                                                 | 239 us: 1.38x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 86.8 ms: 1.14x faster                                                  |
| json_loads           | 31.2 us                                                | 27.9 us: 1.12x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.93 us: 1.05x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.05x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.31 us: 1.05x slower                                                  |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                                  |
| pickle               | 10.7 us                                                | 12.0 us: 1.12x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.4 us: 1.20x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.28x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|-----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                  |
| django_template | 48.2 ms                                                | 34.4 ms: 1.40x faster                                                  |
| genshi_text     | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                  |
| genshi_xml      | 66.0 ms                                                | 54.9 ms: 1.20x faster                                                  |
| Geometric mean  | (ref)                                                  | 1.35x faster                                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.93x faster                                                   |
| generators               | 80.1 ms                                                | 29.7 ms: 2.69x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.44 ms: 2.30x faster                                                  |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 503 ms: 1.83x faster                                                   |
| richards_super           | 94.7 ms                                                | 52.2 ms: 1.82x faster                                                  |
| chaos                    | 115 ms                                                 | 64.1 ms: 1.80x faster                                                  |
| raytrace                 | 507 ms                                                 | 294 ms: 1.73x faster                                                   |
| richards                 | 79.3 ms                                                | 46.5 ms: 1.71x faster                                                  |
| pylint                   | 551 ms                                                 | 324 ms: 1.70x faster                                                   |
| scimark_sor              | 220 ms                                                 | 130 ms: 1.70x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 75.6 ms: 1.69x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 70.1 ms: 1.69x faster                                                  |
| nbody                    | 154 ms                                                 | 92.4 ms: 1.66x faster                                                  |
| comprehensions           | 28.8 us                                                | 17.3 us: 1.66x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.31 ms: 1.65x faster                                                  |
| async_tree_none          | 728 ms                                                 | 449 ms: 1.62x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.60x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                  |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.54x faster                                                  |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.52x faster                                                  |
| go                       | 240 ms                                                 | 158 ms: 1.52x faster                                                   |
| tomli_loads              | 3.14 sec                                               | 2.08 sec: 1.51x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 577 ms: 1.51x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 39.5 us: 1.48x faster                                                  |
| float                    | 117 ms                                                 | 79.8 ms: 1.47x faster                                                  |
| hexiom                   | 10.4 ms                                                | 7.09 ms: 1.47x faster                                                  |
| pyflate                  | 716 ms                                                 | 490 ms: 1.46x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.22 sec: 1.45x faster                                                 |
| spectral_norm            | 170 ms                                                 | 118 ms: 1.44x faster                                                   |
| logging_simple           | 8.30 us                                                | 5.86 us: 1.42x faster                                                  |
| logging_format           | 9.09 us                                                | 6.46 us: 1.41x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 724 ms: 1.40x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.90 ms: 1.40x faster                                                  |
| django_template          | 48.2 ms                                                | 34.4 ms: 1.40x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.85 sec: 1.39x faster                                                 |
| unpickle_pure_python     | 331 us                                                 | 239 us: 1.38x faster                                                   |
| tornado_http             | 136 ms                                                 | 98.7 ms: 1.38x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| scimark_fft              | 466 ms                                                 | 343 ms: 1.36x faster                                                   |
| deepcopy                 | 479 us                                                 | 354 us: 1.36x faster                                                   |
| html5lib                 | 88.9 ms                                                | 65.7 ms: 1.35x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                                  |
| fannkuch                 | 532 ms                                                 | 395 ms: 1.35x faster                                                   |
| scimark_lu               | 176 ms                                                 | 132 ms: 1.33x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.58 sec: 1.33x faster                                                 |
| thrift                   | 1.07 ms                                                | 811 us: 1.32x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 59.9 ms: 1.32x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.91 ms: 1.32x faster                                                  |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 779 ms: 1.31x faster                                                   |
| genshi_text              | 31.8 ms                                                | 24.7 ms: 1.29x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.25 sec: 1.26x faster                                                 |
| 2to3                     | 348 ms                                                 | 282 ms: 1.23x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 56.6 ms: 1.22x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 21.2 ms: 1.22x faster                                                  |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                                   |
| genshi_xml               | 66.0 ms                                                | 54.9 ms: 1.20x faster                                                  |
| sympy_str                | 346 ms                                                 | 288 ms: 1.20x faster                                                   |
| aiohttp                  | 1.44 ms                                                | 1.20 ms: 1.20x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 70.5 ms: 1.20x faster                                                  |
| djangocms                | 38.4 us                                                | 32.2 us: 1.19x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.77 sec: 1.19x faster                                                 |
| gunicorn                 | 1.53 ms                                                | 1.30 ms: 1.18x faster                                                  |
| dask                     | 441 ms                                                 | 374 ms: 1.18x faster                                                   |
| nqueens                  | 106 ms                                                 | 90.5 ms: 1.17x faster                                                  |
| sympy_expand             | 566 ms                                                 | 487 ms: 1.16x faster                                                   |
| python_startup           | 14.6 ms                                                | 12.6 ms: 1.16x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 86.8 ms: 1.14x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 862 us: 1.14x faster                                                   |
| json_loads               | 31.2 us                                                | 27.9 us: 1.12x faster                                                  |
| json                     | 5.69 ms                                                | 5.16 ms: 1.10x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.4 ms: 1.09x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                                  |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.07x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.83 us: 1.07x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.93 us: 1.05x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.05x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.75 sec: 1.04x faster                                                 |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 563 ms: 1.01x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.31 us: 1.05x slower                                                  |
| regex_dna                | 227 ms                                                 | 238 ms: 1.05x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                                  |
| regex_effbot             | 3.63 ms                                                | 3.82 ms: 1.05x slower                                                  |
| async_generators         | 444 ms                                                 | 469 ms: 1.06x slower                                                   |
| gc_traversal             | 3.62 ms                                                | 3.95 ms: 1.09x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 26.4 ms: 1.10x slower                                                  |
| pickle                   | 10.7 us                                                | 12.0 us: 1.12x slower                                                  |
| telco                    | 7.27 ms                                                | 8.42 ms: 1.16x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.4 us: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 97.6 ms: 1.23x slower                                                  |
| unpack_sequence          | 60.0 ns                                                | 90.6 ns: 1.51x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 11.2 ms: 1.88x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                           |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240313-3.13.0a5+-8c094c3-JIT/bm-20240313-linux-x86_64-python-8c094c3095feb4de2efe-3.13.0a5+-8c094c3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.24x
- 95% likely to have a speedup of 1.23x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.33x