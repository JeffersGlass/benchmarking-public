
# Results vs. 3.11.0

- fork: python
- ref: v3.10.4
- machine: linux-x86_64
- commit hash: 9d38120
- commit date: 2022-03-23
- overall geometric mean: 1.27x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x slower
- Memory change: 0.94x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 348 ms: 1.32x slower                                   |
| chameleon      | 6.70 ms                                                | 9.68 ms: 1.45x slower                                  |
| docutils       | 2.66 sec                                               | 3.30 sec: 1.24x slower                                 |
| html5lib       | 64.8 ms                                                | 88.9 ms: 1.37x slower                                  |
| tornado_http   | 98.1 ms                                                | 136 ms: 1.39x slower                                   |
| Geometric mean | (ref)                                                  | 1.35x slower                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 1.02 sec: 1.36x slower                                 |
| async_tree_memoization  | 639 ms                                                 | 870 ms: 1.36x slower                                   |
| async_tree_io           | 1.29 sec                                               | 1.77 sec: 1.37x slower                                 |
| async_tree_none         | 528 ms                                                 | 728 ms: 1.38x slower                                   |
| Geometric mean          | (ref)                                                  | 1.37x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 191 ms: 1.02x faster                                   |
| float          | 78.9 ms                                                | 117 ms: 1.48x slower                                   |
| nbody          | 96.0 ms                                                | 154 ms: 1.60x slower                                   |
| Geometric mean | (ref)                                                  | 1.33x slower                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.63 ms: 1.04x slower                                  |
| regex_dna      | 205 ms                                                 | 227 ms: 1.11x slower                                   |
| regex_v8       | 22.9 ms                                                | 27.8 ms: 1.21x slower                                  |
| regex_compile  | 141 ms                                                 | 188 ms: 1.33x slower                                   |
| Geometric mean | (ref)                                                  | 1.17x slower                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 29.6 us: 1.17x faster                                  |
| pickle               | 11.0 us                                                | 10.7 us: 1.03x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 168 ms: 1.02x slower                                   |
| unpickle             | 13.8 us                                                | 14.4 us: 1.04x slower                                  |
| json_dumps           | 13.3 ms                                                | 14.2 ms: 1.06x slower                                  |
| xml_etree_iterparse  | 108 ms                                                 | 115 ms: 1.07x slower                                   |
| json_loads           | 29.2 us                                                | 31.2 us: 1.07x slower                                  |
| pickle_list          | 4.59 us                                                | 5.08 us: 1.11x slower                                  |
| xml_etree_generate   | 81.1 ms                                                | 99.4 ms: 1.23x slower                                  |
| tomli_loads          | 2.30 sec                                               | 3.14 sec: 1.36x slower                                 |
| unpickle_pure_python | 242 us                                                 | 331 us: 1.37x slower                                   |
| xml_etree_process    | 56.9 ms                                                | 79.1 ms: 1.39x slower                                  |
| pickle_pure_python   | 320 us                                                 | 484 us: 1.51x slower                                   |
| Geometric mean       | (ref)                                                  | 1.13x slower                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.93 ms: 1.01x faster                                  |
| python_startup         | 8.56 ms                                                | 14.6 ms: 1.70x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 66.0 ms: 1.24x slower                                  |
| genshi_text     | 22.5 ms                                                | 31.8 ms: 1.41x slower                                  |
| django_template | 33.5 ms                                                | 48.2 ms: 1.44x slower                                  |
| mako            | 10.7 ms                                                | 16.3 ms: 1.53x slower                                  |
| Geometric mean  | (ref)                                                  | 1.40x slower                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| asyncio_tcp_ssl          | 3.11 sec                                               | 2.57 sec: 1.21x faster                                 |
| pickle_dict              | 34.6 us                                                | 29.6 us: 1.17x faster                                  |
| gc_traversal             | 4.01 ms                                                | 3.62 ms: 1.11x faster                                  |
| pickle                   | 11.0 us                                                | 10.7 us: 1.03x faster                                  |
| pidigits                 | 194 ms                                                 | 191 ms: 1.02x faster                                   |
| python_startup_no_site   | 6.01 ms                                                | 5.93 ms: 1.01x faster                                  |
| coverage                 | 78.8 ms                                                | 79.4 ms: 1.01x slower                                  |
| asyncio_websockets       | 550 ms                                                 | 559 ms: 1.02x slower                                   |
| xml_etree_parse          | 164 ms                                                 | 168 ms: 1.02x slower                                   |
| mdp                      | 2.77 sec                                               | 2.85 sec: 1.03x slower                                 |
| regex_effbot             | 3.51 ms                                                | 3.63 ms: 1.04x slower                                  |
| unpickle                 | 13.8 us                                                | 14.4 us: 1.04x slower                                  |
| typing_runtime_protocols | 520 us                                                 | 544 us: 1.05x slower                                   |
| asyncio_tcp              | 875 ms                                                 | 922 ms: 1.05x slower                                   |
| telco                    | 6.86 ms                                                | 7.27 ms: 1.06x slower                                  |
| json_dumps               | 13.3 ms                                                | 14.2 ms: 1.06x slower                                  |
| xml_etree_iterparse      | 108 ms                                                 | 115 ms: 1.07x slower                                   |
| json_loads               | 29.2 us                                                | 31.2 us: 1.07x slower                                  |
| generators               | 74.9 ms                                                | 80.1 ms: 1.07x slower                                  |
| json                     | 5.24 ms                                                | 5.69 ms: 1.09x slower                                  |
| meteor_contest           | 109 ms                                                 | 120 ms: 1.10x slower                                   |
| pathlib                  | 18.5 ms                                                | 20.5 ms: 1.10x slower                                  |
| pickle_list              | 4.59 us                                                | 5.08 us: 1.11x slower                                  |
| regex_dna                | 205 ms                                                 | 227 ms: 1.11x slower                                   |
| create_gc_cycles         | 1.43 ms                                                | 1.62 ms: 1.13x slower                                  |
| djangocms                | 33.5 us                                                | 38.4 us: 1.15x slower                                  |
| pylint                   | 476 ms                                                 | 551 ms: 1.16x slower                                   |
| sympy_str                | 297 ms                                                 | 346 ms: 1.16x slower                                   |
| sympy_sum                | 169 ms                                                 | 196 ms: 1.16x slower                                   |
| sympy_expand             | 484 ms                                                 | 566 ms: 1.17x slower                                   |
| sqlite_synth             | 2.57 us                                                | 3.02 us: 1.18x slower                                  |
| flaskblogging            | 7.28 ms                                                | 8.58 ms: 1.18x slower                                  |
| bench_thread_pool        | 834 us                                                 | 986 us: 1.18x slower                                   |
| async_generators         | 374 ms                                                 | 444 ms: 1.19x slower                                   |
| sympy_integrate          | 21.5 ms                                                | 25.8 ms: 1.20x slower                                  |
| nqueens                  | 87.9 ms                                                | 106 ms: 1.20x slower                                   |
| dask                     | 365 ms                                                 | 441 ms: 1.21x slower                                   |
| regex_v8                 | 22.9 ms                                                | 27.8 ms: 1.21x slower                                  |
| comprehensions           | 23.6 us                                                | 28.8 us: 1.22x slower                                  |
| sqlalchemy_declarative   | 140 ms                                                 | 172 ms: 1.23x slower                                   |
| xml_etree_generate       | 81.1 ms                                                | 99.4 ms: 1.23x slower                                  |
| genshi_xml               | 53.4 ms                                                | 66.0 ms: 1.24x slower                                  |
| docutils                 | 2.66 sec                                               | 3.30 sec: 1.24x slower                                 |
| sqlglot_optimize         | 55.3 ms                                                | 69.2 ms: 1.25x slower                                  |
| sqlglot_normalize        | 113 ms                                                 | 143 ms: 1.27x slower                                   |
| sqlalchemy_imperative    | 18.3 ms                                                | 23.3 ms: 1.27x slower                                  |
| gunicorn                 | 1.20 ms                                                | 1.53 ms: 1.28x slower                                  |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 6.47 ms: 1.29x slower                                  |
| aiohttp                  | 1.12 ms                                                | 1.44 ms: 1.29x slower                                  |
| deepcopy_reduce          | 3.22 us                                                | 4.17 us: 1.30x slower                                  |
| coroutines               | 27.0 ms                                                | 35.1 ms: 1.30x slower                                  |
| mypy2                    | 686 ms                                                 | 894 ms: 1.30x slower                                   |
| dulwich_log              | 64.6 ms                                                | 84.3 ms: 1.31x slower                                  |
| fannkuch                 | 405 ms                                                 | 532 ms: 1.31x slower                                   |
| deepcopy                 | 365 us                                                 | 479 us: 1.31x slower                                   |
| 2to3                     | 264 ms                                                 | 348 ms: 1.32x slower                                   |
| pycparser                | 1.19 sec                                               | 1.58 sec: 1.33x slower                                 |
| regex_compile            | 141 ms                                                 | 188 ms: 1.33x slower                                   |
| logging_format           | 6.81 us                                                | 9.09 us: 1.33x slower                                  |
| logging_simple           | 6.22 us                                                | 8.30 us: 1.33x slower                                  |
| scimark_fft              | 345 ms                                                 | 466 ms: 1.35x slower                                   |
| pprint_pformat           | 1.55 sec                                               | 2.10 sec: 1.35x slower                                 |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 1.02 sec: 1.36x slower                                 |
| async_tree_memoization   | 639 ms                                                 | 870 ms: 1.36x slower                                   |
| pprint_safe_repr         | 747 ms                                                 | 1.02 sec: 1.36x slower                                 |
| tomli_loads              | 2.30 sec                                               | 3.14 sec: 1.36x slower                                 |
| unpickle_pure_python     | 242 us                                                 | 331 us: 1.37x slower                                   |
| thrift                   | 784 us                                                 | 1.07 ms: 1.37x slower                                  |
| html5lib                 | 64.8 ms                                                | 88.9 ms: 1.37x slower                                  |
| async_tree_io            | 1.29 sec                                               | 1.77 sec: 1.37x slower                                 |
| async_tree_none          | 528 ms                                                 | 728 ms: 1.38x slower                                   |
| unpack_sequence          | 43.5 ns                                                | 60.0 ns: 1.38x slower                                  |
| xml_etree_process        | 56.9 ms                                                | 79.1 ms: 1.39x slower                                  |
| tornado_http             | 98.1 ms                                                | 136 ms: 1.39x slower                                   |
| genshi_text              | 22.5 ms                                                | 31.8 ms: 1.41x slower                                  |
| django_template          | 33.5 ms                                                | 48.2 ms: 1.44x slower                                  |
| chameleon                | 6.70 ms                                                | 9.68 ms: 1.45x slower                                  |
| deepcopy_memo            | 40.2 us                                                | 58.5 us: 1.46x slower                                  |
| sqlglot_transpile        | 1.75 ms                                                | 2.57 ms: 1.47x slower                                  |
| float                    | 78.9 ms                                                | 117 ms: 1.48x slower                                   |
| hexiom                   | 6.89 ms                                                | 10.4 ms: 1.51x slower                                  |
| scimark_lu               | 116 ms                                                 | 176 ms: 1.51x slower                                   |
| pickle_pure_python       | 320 us                                                 | 484 us: 1.51x slower                                   |
| sqlglot_parse            | 1.43 ms                                                | 2.17 ms: 1.51x slower                                  |
| richards_super           | 61.9 ms                                                | 94.7 ms: 1.53x slower                                  |
| mako                     | 10.7 ms                                                | 16.3 ms: 1.53x slower                                  |
| spectral_norm            | 108 ms                                                 | 170 ms: 1.57x slower                                   |
| richards                 | 49.8 ms                                                | 79.3 ms: 1.59x slower                                  |
| nbody                    | 96.0 ms                                                | 154 ms: 1.60x slower                                   |
| chaos                    | 71.9 ms                                                | 115 ms: 1.61x slower                                   |
| go                       | 149 ms                                                 | 240 ms: 1.62x slower                                   |
| raytrace                 | 309 ms                                                 | 507 ms: 1.64x slower                                   |
| pyflate                  | 434 ms                                                 | 716 ms: 1.65x slower                                   |
| crypto_pyaes             | 76.7 ms                                                | 128 ms: 1.67x slower                                   |
| scimark_monte_carlo      | 70.7 ms                                                | 118 ms: 1.67x slower                                   |
| python_startup           | 8.56 ms                                                | 14.6 ms: 1.70x slower                                  |
| logging_silent           | 111 ns                                                 | 190 ns: 1.71x slower                                   |
| scimark_sor              | 121 ms                                                 | 220 ms: 1.81x slower                                   |
| deltablue                | 3.92 ms                                                | 7.91 ms: 2.02x slower                                  |
| Geometric mean           | (ref)                                                  | 1.27x slower                                           |

Benchmark hidden because not significant (2): unpickle_list, bench_mp_pool
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.25x
- 95% likely to have a slowdown of 1.24x
- 99% likely to have a slowdown of 1.22x


# Memory

- memory change: 0.94x