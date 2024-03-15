
# Results vs. 3.10.4

- fork: python
- ref: v3.12.1
- machine: linux-x86_64
- commit hash: 2305ca5
- commit date: 2023-12-07
- overall geometric mean: 1.31x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.23x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 274 ms: 1.27x faster                                   |
| chameleon      | 9.68 ms                                                | 7.24 ms: 1.34x faster                                  |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                 |
| tornado_http   | 136 ms                                                 | 99.4 ms: 1.37x faster                                  |
| Geometric mean | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 475 ms: 1.53x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 582 ms: 1.49x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 725 ms: 1.40x faster                                   |
| Geometric mean          | (ref)                                                  | 1.48x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.2 ms: 1.65x faster                                  |
| float          | 117 ms                                                 | 84.6 ms: 1.38x faster                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.32x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 145 ms: 1.30x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.8 ms: 1.22x faster                                  |
| regex_dna      | 227 ms                                                 | 205 ms: 1.10x faster                                   |
| Geometric mean | (ref)                                                  | 1.15x faster                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 322 us: 1.50x faster                                   |
| unpickle_pure_python | 331 us                                                 | 231 us: 1.43x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.29 sec: 1.37x faster                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 61.2 ms: 1.29x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 88.2 ms: 1.13x faster                                  |
| json_loads           | 31.2 us                                                | 28.0 us: 1.11x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                   |
| unpickle_list        | 5.20 us                                                | 4.99 us: 1.04x faster                                  |
| pickle_list          | 5.08 us                                                | 4.93 us: 1.03x faster                                  |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                  |
| unpickle             | 14.4 us                                                | 15.7 us: 1.09x slower                                  |
| pickle_dict          | 29.6 us                                                | 33.1 us: 1.12x slower                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.44 ms: 1.54x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.81 ms: 1.15x slower                                  |
| Geometric mean         | (ref)                                                  | 1.16x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.3 ms: 1.45x faster                                  |
| django_template | 48.2 ms                                                | 34.7 ms: 1.39x faster                                  |
| Geometric mean  | (ref)                                                  | 1.42x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 121 us: 4.50x faster                                   |
| generators               | 80.1 ms                                                | 31.7 ms: 2.53x faster                                  |
| deltablue                | 7.91 ms                                                | 3.76 ms: 2.10x faster                                  |
| logging_silent           | 190 ns                                                 | 104 ns: 1.83x faster                                   |
| richards_super           | 94.7 ms                                                | 52.0 ms: 1.82x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 510 ms: 1.81x faster                                   |
| richards                 | 79.3 ms                                                | 45.8 ms: 1.73x faster                                  |
| chaos                    | 115 ms                                                 | 66.8 ms: 1.73x faster                                  |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                   |
| scimark_sor              | 220 ms                                                 | 132 ms: 1.66x faster                                   |
| nbody                    | 154 ms                                                 | 93.2 ms: 1.65x faster                                  |
| raytrace                 | 507 ms                                                 | 308 ms: 1.65x faster                                   |
| scimark_monte_carlo      | 118 ms                                                 | 74.3 ms: 1.59x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.38 ms: 1.58x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.60 ms: 1.57x faster                                  |
| pyflate                  | 716 ms                                                 | 460 ms: 1.56x faster                                   |
| python_startup           | 14.6 ms                                                | 9.44 ms: 1.54x faster                                  |
| async_tree_none          | 728 ms                                                 | 475 ms: 1.53x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 83.5 ms: 1.53x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.70 ms: 1.51x faster                                  |
| coroutines               | 35.1 ms                                                | 23.3 ms: 1.50x faster                                  |
| pickle_pure_python       | 484 us                                                 | 322 us: 1.50x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 582 ms: 1.49x faster                                   |
| scimark_lu               | 176 ms                                                 | 118 ms: 1.49x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 39.2 us: 1.49x faster                                  |
| spectral_norm            | 170 ms                                                 | 116 ms: 1.46x faster                                   |
| mako                     | 16.3 ms                                                | 11.3 ms: 1.45x faster                                  |
| unpickle_pure_python     | 331 us                                                 | 231 us: 1.43x faster                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 725 ms: 1.40x faster                                   |
| django_template          | 48.2 ms                                                | 34.7 ms: 1.39x faster                                  |
| float                    | 117 ms                                                 | 84.6 ms: 1.38x faster                                  |
| comprehensions           | 28.8 us                                                | 20.9 us: 1.38x faster                                  |
| tomli_loads              | 3.14 sec                                               | 2.29 sec: 1.37x faster                                 |
| tornado_http             | 136 ms                                                 | 99.4 ms: 1.37x faster                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.56 sec: 1.35x faster                                 |
| pycparser                | 1.58 sec                                               | 1.17 sec: 1.35x faster                                 |
| chameleon                | 9.68 ms                                                | 7.24 ms: 1.34x faster                                  |
| pprint_safe_repr         | 1.02 sec                                               | 764 ms: 1.33x faster                                   |
| deepcopy                 | 479 us                                                 | 366 us: 1.31x faster                                   |
| fannkuch                 | 532 ms                                                 | 409 ms: 1.30x faster                                   |
| regex_compile            | 188 ms                                                 | 145 ms: 1.30x faster                                   |
| sqlglot_normalize        | 143 ms                                                 | 110 ms: 1.29x faster                                   |
| xml_etree_process        | 79.1 ms                                                | 61.2 ms: 1.29x faster                                  |
| mypy2                    | 894 ms                                                 | 696 ms: 1.28x faster                                   |
| logging_simple           | 8.30 us                                                | 6.47 us: 1.28x faster                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.27 us: 1.28x faster                                  |
| 2to3                     | 348 ms                                                 | 274 ms: 1.27x faster                                   |
| sqlglot_optimize         | 69.2 ms                                                | 54.7 ms: 1.26x faster                                  |
| logging_format           | 9.09 us                                                | 7.21 us: 1.26x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.14 ms: 1.26x faster                                  |
| nqueens                  | 106 ms                                                 | 84.2 ms: 1.26x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.8 ms: 1.24x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| scimark_fft              | 466 ms                                                 | 376 ms: 1.24x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.23 ms: 1.24x faster                                  |
| dulwich_log              | 84.3 ms                                                | 68.4 ms: 1.23x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.24 ms: 1.23x faster                                  |
| regex_v8                 | 27.8 ms                                                | 22.8 ms: 1.22x faster                                  |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                 |
| sympy_sum                | 196 ms                                                 | 164 ms: 1.20x faster                                   |
| dask                     | 441 ms                                                 | 370 ms: 1.19x faster                                   |
| sympy_expand             | 566 ms                                                 | 477 ms: 1.19x faster                                   |
| bench_thread_pool        | 986 us                                                 | 836 us: 1.18x faster                                   |
| sqlalchemy_declarative   | 172 ms                                                 | 146 ms: 1.18x faster                                   |
| sympy_str                | 346 ms                                                 | 294 ms: 1.17x faster                                   |
| unpack_sequence          | 60.0 ns                                                | 53.0 ns: 1.13x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 88.2 ms: 1.13x faster                                  |
| json_loads               | 31.2 us                                                | 28.0 us: 1.11x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                  |
| regex_dna                | 227 ms                                                 | 205 ms: 1.10x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                   |
| json                     | 5.69 ms                                                | 5.20 ms: 1.09x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                 |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.06x faster                                  |
| coverage                 | 79.4 ms                                                | 75.2 ms: 1.06x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                   |
| unpickle_list            | 5.20 us                                                | 4.99 us: 1.04x faster                                  |
| pickle_list              | 5.08 us                                                | 4.93 us: 1.03x faster                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                   |
| async_generators         | 444 ms                                                 | 456 ms: 1.03x slower                                   |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                  |
| gc_traversal             | 3.62 ms                                                | 3.93 ms: 1.08x slower                                  |
| unpickle                 | 14.4 us                                                | 15.7 us: 1.09x slower                                  |
| pickle_dict              | 29.6 us                                                | 33.1 us: 1.12x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.81 ms: 1.15x slower                                  |
| Geometric mean           | (ref)                                                  | 1.31x faster                                           |

Benchmark hidden because not significant (3): regex_effbot, telco, bench_mp_pool
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20231207-3.12.1-2305ca5/bm-20231207-linux-x86_64-python-v3.12.1-3.12.1-2305ca5.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.23x


# Memory

- memory change: 1.10x