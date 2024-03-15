# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: b6ae6da
- commit date: 2024-03-11
- overall geometric mean: 1.23x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.15x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 297 ms: 1.17x faster                                   |
| chameleon      | 9.68 ms                                                | 7.13 ms: 1.36x faster                                  |
| docutils       | 3.30 sec                                               | 2.86 sec: 1.15x faster                                 |
| html5lib       | 88.9 ms                                                | 69.5 ms: 1.28x faster                                  |
| tornado_http   | 136 ms                                                 | 103 ms: 1.32x faster                                   |
| Geometric mean | (ref)                                                  | 1.25x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 459 ms: 1.59x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 593 ms: 1.47x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.23 sec: 1.43x faster                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 743 ms: 1.37x faster                                   |
| Geometric mean          | (ref)                                                  | 1.46x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 120 ms: 1.28x faster                                   |
| float          | 117 ms                                                 | 93.0 ms: 1.26x faster                                  |
| pidigits       | 191 ms                                                 | 191 ms: 1.00x slower                                   |
| Geometric mean | (ref)                                                  | 1.17x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 25.1 ms: 1.11x faster                                  |
| regex_compile  | 188 ms                                                 | 174 ms: 1.08x faster                                   |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                   |
| Geometric mean | (ref)                                                  | 1.06x faster                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 310 us: 1.56x faster                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                  |
| tomli_loads          | 3.14 sec                                               | 2.43 sec: 1.29x faster                                 |
| xml_etree_process    | 79.1 ms                                                | 62.3 ms: 1.27x faster                                  |
| unpickle_pure_python | 331 us                                                 | 269 us: 1.23x faster                                   |
| json_loads           | 31.2 us                                                | 28.2 us: 1.11x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 90.8 ms: 1.09x faster                                  |
| unpickle_list        | 5.20 us                                                | 4.88 us: 1.07x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.05x faster                                   |
| pickle_list          | 5.08 us                                                | 4.90 us: 1.04x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 112 ms: 1.03x faster                                   |
| unpickle             | 14.4 us                                                | 15.3 us: 1.06x slower                                  |
| pickle_dict          | 29.6 us                                                | 32.9 us: 1.11x slower                                  |
| pickle               | 10.7 us                                                | 12.0 us: 1.13x slower                                  |
| Geometric mean       | (ref)                                                  | 1.12x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.4 ms: 1.40x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 9.01 ms: 1.52x slower                                  |
| Geometric mean         | (ref)                                                  | 1.04x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| django_template | 48.2 ms                                                | 35.3 ms: 1.36x faster                                  |
| mako            | 16.3 ms                                                | 12.7 ms: 1.28x faster                                  |
| genshi_text     | 31.8 ms                                                | 27.1 ms: 1.18x faster                                  |
| genshi_xml      | 66.0 ms                                                | 61.5 ms: 1.07x faster                                  |
| Geometric mean  | (ref)                                                  | 1.22x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 119 us: 4.57x faster                                   |
| generators               | 80.1 ms                                                | 30.0 ms: 2.67x faster                                  |
| deltablue                | 7.91 ms                                                | 3.82 ms: 2.07x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 507 ms: 1.82x faster                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                   |
| pylint                   | 551 ms                                                 | 331 ms: 1.66x faster                                   |
| async_tree_none          | 728 ms                                                 | 459 ms: 1.59x faster                                   |
| pickle_pure_python       | 484 us                                                 | 310 us: 1.56x faster                                   |
| coroutines               | 35.1 ms                                                | 22.5 ms: 1.56x faster                                  |
| chaos                    | 115 ms                                                 | 74.9 ms: 1.54x faster                                  |
| richards_super           | 94.7 ms                                                | 61.8 ms: 1.53x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.44 ms: 1.51x faster                                  |
| raytrace                 | 507 ms                                                 | 342 ms: 1.48x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 86.5 ms: 1.48x faster                                  |
| async_tree_memoization   | 870 ms                                                 | 593 ms: 1.47x faster                                   |
| scimark_sor              | 220 ms                                                 | 150 ms: 1.46x faster                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.78 ms: 1.44x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.23 sec: 1.43x faster                                 |
| scimark_monte_carlo      | 118 ms                                                 | 82.6 ms: 1.43x faster                                  |
| richards                 | 79.3 ms                                                | 55.6 ms: 1.43x faster                                  |
| python_startup           | 14.6 ms                                                | 10.4 ms: 1.40x faster                                  |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 42.3 us: 1.38x faster                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.86 sec: 1.38x faster                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 743 ms: 1.37x faster                                   |
| django_template          | 48.2 ms                                                | 35.3 ms: 1.36x faster                                  |
| go                       | 240 ms                                                 | 176 ms: 1.36x faster                                   |
| chameleon                | 9.68 ms                                                | 7.13 ms: 1.36x faster                                  |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                  |
| tornado_http             | 136 ms                                                 | 103 ms: 1.32x faster                                   |
| thrift                   | 1.07 ms                                                | 817 us: 1.31x faster                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.18 us: 1.31x faster                                  |
| logging_simple           | 8.30 us                                                | 6.33 us: 1.31x faster                                  |
| deepcopy                 | 479 us                                                 | 367 us: 1.31x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.43 sec: 1.29x faster                                 |
| logging_format           | 9.09 us                                                | 7.08 us: 1.28x faster                                  |
| mako                     | 16.3 ms                                                | 12.7 ms: 1.28x faster                                  |
| nbody                    | 154 ms                                                 | 120 ms: 1.28x faster                                   |
| html5lib                 | 88.9 ms                                                | 69.5 ms: 1.28x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 62.3 ms: 1.27x faster                                  |
| pyflate                  | 716 ms                                                 | 564 ms: 1.27x faster                                   |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                   |
| float                    | 117 ms                                                 | 93.0 ms: 1.26x faster                                  |
| unpickle_pure_python     | 331 us                                                 | 269 us: 1.23x faster                                   |
| pycparser                | 1.58 sec                                               | 1.29 sec: 1.22x faster                                 |
| spectral_norm            | 170 ms                                                 | 141 ms: 1.21x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 21.5 ms: 1.20x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.21 ms: 1.19x faster                                  |
| pprint_safe_repr         | 1.02 sec                                               | 860 ms: 1.18x faster                                   |
| hexiom                   | 10.4 ms                                                | 8.79 ms: 1.18x faster                                  |
| djangocms                | 38.4 us                                                | 32.6 us: 1.18x faster                                  |
| genshi_text              | 31.8 ms                                                | 27.1 ms: 1.18x faster                                  |
| sympy_sum                | 196 ms                                                 | 167 ms: 1.18x faster                                   |
| pprint_pformat           | 2.10 sec                                               | 1.79 sec: 1.17x faster                                 |
| 2to3                     | 348 ms                                                 | 297 ms: 1.17x faster                                   |
| dask                     | 441 ms                                                 | 378 ms: 1.17x faster                                   |
| gunicorn                 | 1.53 ms                                                | 1.31 ms: 1.17x faster                                  |
| dulwich_log              | 84.3 ms                                                | 73.1 ms: 1.15x faster                                  |
| docutils                 | 3.30 sec                                               | 2.86 sec: 1.15x faster                                 |
| sympy_str                | 346 ms                                                 | 303 ms: 1.14x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.69 ms: 1.14x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 61.0 ms: 1.13x faster                                  |
| bench_thread_pool        | 986 us                                                 | 872 us: 1.13x faster                                   |
| fannkuch                 | 532 ms                                                 | 472 ms: 1.13x faster                                   |
| scimark_lu               | 176 ms                                                 | 158 ms: 1.12x faster                                   |
| regex_v8                 | 27.8 ms                                                | 25.1 ms: 1.11x faster                                  |
| json_loads               | 31.2 us                                                | 28.2 us: 1.11x faster                                  |
| sympy_expand             | 566 ms                                                 | 512 ms: 1.10x faster                                   |
| xml_etree_generate       | 99.4 ms                                                | 90.8 ms: 1.09x faster                                  |
| json                     | 5.69 ms                                                | 5.24 ms: 1.09x faster                                  |
| regex_compile            | 188 ms                                                 | 174 ms: 1.08x faster                                   |
| genshi_xml               | 66.0 ms                                                | 61.5 ms: 1.07x faster                                  |
| scimark_fft              | 466 ms                                                 | 436 ms: 1.07x faster                                   |
| nqueens                  | 106 ms                                                 | 99.1 ms: 1.07x faster                                  |
| unpickle_list            | 5.20 us                                                | 4.88 us: 1.07x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.05x faster                                   |
| unpack_sequence          | 60.0 ns                                                | 57.0 ns: 1.05x faster                                  |
| pathlib                  | 20.5 ms                                                | 19.5 ms: 1.05x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.54 ms: 1.05x faster                                  |
| mdp                      | 2.85 sec                                               | 2.72 sec: 1.05x faster                                 |
| regex_dna                | 227 ms                                                 | 216 ms: 1.05x faster                                   |
| pickle_list              | 5.08 us                                                | 4.90 us: 1.04x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 112 ms: 1.03x faster                                   |
| meteor_contest           | 120 ms                                                 | 117 ms: 1.02x faster                                   |
| sqlite_synth             | 3.02 us                                                | 2.96 us: 1.02x faster                                  |
| pidigits                 | 191 ms                                                 | 191 ms: 1.00x slower                                   |
| asyncio_websockets       | 559 ms                                                 | 564 ms: 1.01x slower                                   |
| async_generators         | 444 ms                                                 | 469 ms: 1.06x slower                                   |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.06x slower                                  |
| gc_traversal             | 3.62 ms                                                | 3.94 ms: 1.09x slower                                  |
| pickle_dict              | 29.6 us                                                | 32.9 us: 1.11x slower                                  |
| pickle                   | 10.7 us                                                | 12.0 us: 1.13x slower                                  |
| telco                    | 7.27 ms                                                | 8.66 ms: 1.19x slower                                  |
| coverage                 | 79.4 ms                                                | 97.4 ms: 1.23x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 9.01 ms: 1.52x slower                                  |
| Geometric mean           | (ref)                                                  | 1.23x faster                                           |

Benchmark hidden because not significant (3): regex_effbot, bench_mp_pool, mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240311-3.13.0a4+-b6ae6da-PYTHON_UOPS/bm-20240311-linux-x86_64-python-main-3.13.0a4+-b6ae6da.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.17x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.15x


# Memory

- memory change: 1.08x