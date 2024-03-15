# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 8c094c3
- commit date: 2024-03-13
- overall geometric mean: 1.22x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.14x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 298 ms: 1.17x faster                                   |
| chameleon      | 9.68 ms                                                | 6.87 ms: 1.41x faster                                  |
| docutils       | 3.30 sec                                               | 2.87 sec: 1.15x faster                                 |
| html5lib       | 88.9 ms                                                | 71.1 ms: 1.25x faster                                  |
| tornado_http   | 136 ms                                                 | 104 ms: 1.31x faster                                   |
| Geometric mean | (ref)                                                  | 1.25x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 463 ms: 1.57x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 594 ms: 1.46x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.25 sec: 1.42x faster                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 745 ms: 1.36x faster                                   |
| Geometric mean          | (ref)                                                  | 1.45x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 122 ms: 1.26x faster                                   |
| float          | 117 ms                                                 | 94.8 ms: 1.23x faster                                  |
| pidigits       | 191 ms                                                 | 192 ms: 1.00x slower                                   |
| Geometric mean | (ref)                                                  | 1.16x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.6 ms: 1.08x faster                                  |
| regex_compile  | 188 ms                                                 | 177 ms: 1.07x faster                                   |
| regex_dna      | 227 ms                                                 | 229 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.58x faster                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 62.2 ms: 1.27x faster                                  |
| tomli_loads          | 3.14 sec                                               | 2.51 sec: 1.25x faster                                 |
| unpickle_pure_python | 331 us                                                 | 274 us: 1.21x faster                                   |
| json_loads           | 31.2 us                                                | 28.3 us: 1.10x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 90.7 ms: 1.10x faster                                  |
| unpickle_list        | 5.20 us                                                | 4.91 us: 1.06x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 161 ms: 1.04x faster                                   |
| xml_etree_iterparse  | 115 ms                                                 | 111 ms: 1.04x faster                                   |
| pickle_list          | 5.08 us                                                | 4.97 us: 1.02x faster                                  |
| unpickle             | 14.4 us                                                | 15.1 us: 1.05x slower                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                  |
| pickle_dict          | 29.6 us                                                | 33.5 us: 1.13x slower                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 8.99 ms: 1.52x slower                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 48.2 ms                                                | 34.5 ms: 1.40x faster                                  |
| mako            | 16.3 ms                                                | 12.6 ms: 1.29x faster                                  |
| genshi_text     | 31.8 ms                                                | 27.3 ms: 1.16x faster                                  |
| genshi_xml      | 66.0 ms                                                | 63.1 ms: 1.05x faster                                  |
| Geometric mean  | (ref)                                                  | 1.22x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 116 us: 4.68x faster                                   |
| generators               | 80.1 ms                                                | 30.9 ms: 2.59x faster                                  |
| deltablue                | 7.91 ms                                                | 3.80 ms: 2.08x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 507 ms: 1.82x faster                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                   |
| pylint                   | 551 ms                                                 | 331 ms: 1.67x faster                                   |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.58x faster                                   |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.58x faster                                  |
| async_tree_none          | 728 ms                                                 | 463 ms: 1.57x faster                                   |
| scimark_sor              | 220 ms                                                 | 142 ms: 1.55x faster                                   |
| chaos                    | 115 ms                                                 | 75.3 ms: 1.53x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.44 ms: 1.50x faster                                  |
| richards_super           | 94.7 ms                                                | 63.4 ms: 1.50x faster                                  |
| raytrace                 | 507 ms                                                 | 345 ms: 1.47x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 594 ms: 1.46x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 87.7 ms: 1.46x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.79 ms: 1.44x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.25 sec: 1.42x faster                                 |
| chameleon                | 9.68 ms                                                | 6.87 ms: 1.41x faster                                  |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 41.9 us: 1.40x faster                                  |
| django_template          | 48.2 ms                                                | 34.5 ms: 1.40x faster                                  |
| richards                 | 79.3 ms                                                | 56.9 ms: 1.39x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 85.4 ms: 1.38x faster                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.86 sec: 1.38x faster                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 745 ms: 1.36x faster                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                  |
| comprehensions           | 28.8 us                                                | 21.4 us: 1.35x faster                                  |
| go                       | 240 ms                                                 | 178 ms: 1.35x faster                                   |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                  |
| deepcopy                 | 479 us                                                 | 364 us: 1.32x faster                                   |
| logging_simple           | 8.30 us                                                | 6.32 us: 1.31x faster                                  |
| tornado_http             | 136 ms                                                 | 104 ms: 1.31x faster                                   |
| thrift                   | 1.07 ms                                                | 829 us: 1.29x faster                                   |
| mako                     | 16.3 ms                                                | 12.6 ms: 1.29x faster                                  |
| logging_format           | 9.09 us                                                | 7.09 us: 1.28x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 62.2 ms: 1.27x faster                                  |
| nbody                    | 154 ms                                                 | 122 ms: 1.26x faster                                   |
| sqlglot_normalize        | 143 ms                                                 | 114 ms: 1.25x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.51 sec: 1.25x faster                                 |
| html5lib                 | 88.9 ms                                                | 71.1 ms: 1.25x faster                                  |
| float                    | 117 ms                                                 | 94.8 ms: 1.23x faster                                  |
| pyflate                  | 716 ms                                                 | 590 ms: 1.21x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 274 us: 1.21x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 21.7 ms: 1.19x faster                                  |
| spectral_norm            | 170 ms                                                 | 143 ms: 1.19x faster                                   |
| djangocms                | 38.4 us                                                | 32.4 us: 1.19x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.23 ms: 1.17x faster                                  |
| 2to3                     | 348 ms                                                 | 298 ms: 1.17x faster                                   |
| dask                     | 441 ms                                                 | 378 ms: 1.17x faster                                   |
| pycparser                | 1.58 sec                                               | 1.35 sec: 1.17x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 873 ms: 1.17x faster                                   |
| genshi_text              | 31.8 ms                                                | 27.3 ms: 1.16x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.32 ms: 1.16x faster                                  |
| sympy_sum                | 196 ms                                                 | 169 ms: 1.16x faster                                   |
| dulwich_log              | 84.3 ms                                                | 73.0 ms: 1.16x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.83 sec: 1.15x faster                                 |
| docutils                 | 3.30 sec                                               | 2.87 sec: 1.15x faster                                 |
| hexiom                   | 10.4 ms                                                | 9.14 ms: 1.14x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 61.2 ms: 1.13x faster                                  |
| bench_thread_pool        | 986 us                                                 | 876 us: 1.13x faster                                   |
| sympy_str                | 346 ms                                                 | 307 ms: 1.13x faster                                   |
| scimark_lu               | 176 ms                                                 | 158 ms: 1.12x faster                                   |
| unpack_sequence          | 60.0 ns                                                | 54.1 ns: 1.11x faster                                  |
| fannkuch                 | 532 ms                                                 | 481 ms: 1.10x faster                                   |
| json_loads               | 31.2 us                                                | 28.3 us: 1.10x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 90.7 ms: 1.10x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.92 ms: 1.09x faster                                  |
| json                     | 5.69 ms                                                | 5.22 ms: 1.09x faster                                  |
| sympy_expand             | 566 ms                                                 | 519 ms: 1.09x faster                                   |
| regex_v8                 | 27.8 ms                                                | 25.6 ms: 1.08x faster                                  |
| scimark_fft              | 466 ms                                                 | 432 ms: 1.08x faster                                   |
| regex_compile            | 188 ms                                                 | 177 ms: 1.07x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.06x faster                                  |
| unpickle_list            | 5.20 us                                                | 4.91 us: 1.06x faster                                  |
| pathlib                  | 20.5 ms                                                | 19.4 ms: 1.05x faster                                  |
| genshi_xml               | 66.0 ms                                                | 63.1 ms: 1.05x faster                                  |
| sqlite_synth             | 3.02 us                                                | 2.89 us: 1.05x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 161 ms: 1.04x faster                                   |
| xml_etree_iterparse      | 115 ms                                                 | 111 ms: 1.04x faster                                   |
| pickle_list              | 5.08 us                                                | 4.97 us: 1.02x faster                                  |
| nqueens                  | 106 ms                                                 | 104 ms: 1.01x faster                                   |
| mdp                      | 2.85 sec                                               | 2.83 sec: 1.01x faster                                 |
| meteor_contest           | 120 ms                                                 | 119 ms: 1.00x faster                                   |
| pidigits                 | 191 ms                                                 | 192 ms: 1.00x slower                                   |
| asyncio_websockets       | 559 ms                                                 | 564 ms: 1.01x slower                                   |
| regex_dna                | 227 ms                                                 | 229 ms: 1.01x slower                                   |
| unpickle                 | 14.4 us                                                | 15.1 us: 1.05x slower                                  |
| async_generators         | 444 ms                                                 | 472 ms: 1.06x slower                                   |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                  |
| gc_traversal             | 3.62 ms                                                | 4.05 ms: 1.12x slower                                  |
| pickle_dict              | 29.6 us                                                | 33.5 us: 1.13x slower                                  |
| telco                    | 7.27 ms                                                | 8.91 ms: 1.23x slower                                  |
| coverage                 | 79.4 ms                                                | 97.5 ms: 1.23x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.99 ms: 1.52x slower                                  |
| Geometric mean           | (ref)                                                  | 1.22x faster                                           |

Benchmark hidden because not significant (3): regex_effbot, bench_mp_pool, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240313-3.13.0a5+-8c094c3-PYTHON_UOPS/bm-20240313-linux-x86_64-python-main-3.13.0a5+-8c094c3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.15x
- 95% likely to have a speedup of 1.15x
- 99% likely to have a speedup of 1.14x


# Memory

- memory change: 1.08x