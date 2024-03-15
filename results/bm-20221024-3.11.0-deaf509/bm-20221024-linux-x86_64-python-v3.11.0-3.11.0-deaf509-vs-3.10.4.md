
# Results vs. 3.10.4

- fork: python
- ref: v3.11.0
- machine: linux-x86_64
- commit hash: deaf509
- commit date: 2022-10-24
- overall geometric mean: 1.27x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                   |
| chameleon      | 9.68 ms                                                | 6.70 ms: 1.45x faster                                  |
| docutils       | 3.30 sec                                               | 2.66 sec: 1.24x faster                                 |
| html5lib       | 88.9 ms                                                | 64.8 ms: 1.37x faster                                  |
| tornado_http   | 136 ms                                                 | 98.1 ms: 1.39x faster                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 528 ms: 1.38x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.29 sec: 1.37x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 639 ms: 1.36x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 749 ms: 1.36x faster                                   |
| Geometric mean          | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 96.0 ms: 1.60x faster                                  |
| float          | 117 ms                                                 | 78.9 ms: 1.48x faster                                  |
| pidigits       | 191 ms                                                 | 194 ms: 1.02x slower                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 141 ms: 1.33x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.9 ms: 1.21x faster                                  |
| regex_dna      | 227 ms                                                 | 205 ms: 1.11x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.51 ms: 1.04x faster                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 320 us: 1.51x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 56.9 ms: 1.39x faster                                  |
| unpickle_pure_python | 331 us                                                 | 242 us: 1.37x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.30 sec: 1.36x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 81.1 ms: 1.23x faster                                  |
| pickle_list          | 5.08 us                                                | 4.59 us: 1.11x faster                                  |
| json_loads           | 31.2 us                                                | 29.2 us: 1.07x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| json_dumps           | 14.2 ms                                                | 13.3 ms: 1.06x faster                                  |
| unpickle             | 14.4 us                                                | 13.8 us: 1.04x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 164 ms: 1.02x faster                                   |
| pickle               | 10.7 us                                                | 11.0 us: 1.03x slower                                  |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                  |
| Geometric mean       | (ref)                                                  | 1.13x faster                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.01 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.7 ms: 1.53x faster                                  |
| django_template | 48.2 ms                                                | 33.5 ms: 1.44x faster                                  |
| genshi_text     | 31.8 ms                                                | 22.5 ms: 1.41x faster                                  |
| genshi_xml      | 66.0 ms                                                | 53.4 ms: 1.24x faster                                  |
| Geometric mean  | (ref)                                                  | 1.40x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.92 ms: 2.02x faster                                  |
| scimark_sor              | 220 ms                                                 | 121 ms: 1.81x faster                                   |
| logging_silent           | 190 ns                                                 | 111 ns: 1.71x faster                                   |
| python_startup           | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 70.7 ms: 1.67x faster                                  |
| crypto_pyaes             | 128 ms                                                 | 76.7 ms: 1.67x faster                                  |
| pyflate                  | 716 ms                                                 | 434 ms: 1.65x faster                                   |
| raytrace                 | 507 ms                                                 | 309 ms: 1.64x faster                                   |
| go                       | 240 ms                                                 | 149 ms: 1.62x faster                                   |
| chaos                    | 115 ms                                                 | 71.9 ms: 1.61x faster                                  |
| nbody                    | 154 ms                                                 | 96.0 ms: 1.60x faster                                  |
| richards                 | 79.3 ms                                                | 49.8 ms: 1.59x faster                                  |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                   |
| mako                     | 16.3 ms                                                | 10.7 ms: 1.53x faster                                  |
| richards_super           | 94.7 ms                                                | 61.9 ms: 1.53x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.43 ms: 1.51x faster                                  |
| pickle_pure_python       | 484 us                                                 | 320 us: 1.51x faster                                   |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.51x faster                                   |
| hexiom                   | 10.4 ms                                                | 6.89 ms: 1.51x faster                                  |
| float                    | 117 ms                                                 | 78.9 ms: 1.48x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.75 ms: 1.47x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 40.2 us: 1.46x faster                                  |
| chameleon                | 9.68 ms                                                | 6.70 ms: 1.45x faster                                  |
| django_template          | 48.2 ms                                                | 33.5 ms: 1.44x faster                                  |
| genshi_text              | 31.8 ms                                                | 22.5 ms: 1.41x faster                                  |
| tornado_http             | 136 ms                                                 | 98.1 ms: 1.39x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 56.9 ms: 1.39x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 43.5 ns: 1.38x faster                                  |
| async_tree_none          | 728 ms                                                 | 528 ms: 1.38x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.29 sec: 1.37x faster                                 |
| html5lib                 | 88.9 ms                                                | 64.8 ms: 1.37x faster                                  |
| thrift                   | 1.07 ms                                                | 784 us: 1.37x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 242 us: 1.37x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.30 sec: 1.36x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 747 ms: 1.36x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 639 ms: 1.36x faster                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 749 ms: 1.36x faster                                   |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.35x faster                                 |
| scimark_fft              | 466 ms                                                 | 345 ms: 1.35x faster                                   |
| logging_simple           | 8.30 us                                                | 6.22 us: 1.33x faster                                  |
| logging_format           | 9.09 us                                                | 6.81 us: 1.33x faster                                  |
| regex_compile            | 188 ms                                                 | 141 ms: 1.33x faster                                   |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.33x faster                                 |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                   |
| deepcopy                 | 479 us                                                 | 365 us: 1.31x faster                                   |
| fannkuch                 | 532 ms                                                 | 405 ms: 1.31x faster                                   |
| dulwich_log              | 84.3 ms                                                | 64.6 ms: 1.31x faster                                  |
| mypy2                    | 894 ms                                                 | 686 ms: 1.30x faster                                   |
| coroutines               | 35.1 ms                                                | 27.0 ms: 1.30x faster                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.22 us: 1.30x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.12 ms: 1.29x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.03 ms: 1.29x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.20 ms: 1.28x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.3 ms: 1.27x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.27x faster                                   |
| sqlglot_optimize         | 69.2 ms                                                | 55.3 ms: 1.25x faster                                  |
| docutils                 | 3.30 sec                                               | 2.66 sec: 1.24x faster                                 |
| genshi_xml               | 66.0 ms                                                | 53.4 ms: 1.24x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 81.1 ms: 1.23x faster                                  |
| sqlalchemy_declarative   | 172 ms                                                 | 140 ms: 1.23x faster                                   |
| comprehensions           | 28.8 us                                                | 23.6 us: 1.22x faster                                  |
| regex_v8                 | 27.8 ms                                                | 22.9 ms: 1.21x faster                                  |
| dask                     | 441 ms                                                 | 365 ms: 1.21x faster                                   |
| nqueens                  | 106 ms                                                 | 87.9 ms: 1.20x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 21.5 ms: 1.20x faster                                  |
| async_generators         | 444 ms                                                 | 374 ms: 1.19x faster                                   |
| bench_thread_pool        | 986 us                                                 | 834 us: 1.18x faster                                   |
| flaskblogging            | 8.58 ms                                                | 7.28 ms: 1.18x faster                                  |
| sqlite_synth             | 3.02 us                                                | 2.57 us: 1.18x faster                                  |
| sympy_expand             | 566 ms                                                 | 484 ms: 1.17x faster                                   |
| sympy_sum                | 196 ms                                                 | 169 ms: 1.16x faster                                   |
| sympy_str                | 346 ms                                                 | 297 ms: 1.16x faster                                   |
| pylint                   | 551 ms                                                 | 476 ms: 1.16x faster                                   |
| djangocms                | 38.4 us                                                | 33.5 us: 1.15x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.43 ms: 1.13x faster                                  |
| regex_dna                | 227 ms                                                 | 205 ms: 1.11x faster                                   |
| pickle_list              | 5.08 us                                                | 4.59 us: 1.11x faster                                  |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.10x faster                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                   |
| json                     | 5.69 ms                                                | 5.24 ms: 1.09x faster                                  |
| generators               | 80.1 ms                                                | 74.9 ms: 1.07x faster                                  |
| json_loads               | 31.2 us                                                | 29.2 us: 1.07x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| json_dumps               | 14.2 ms                                                | 13.3 ms: 1.06x faster                                  |
| telco                    | 7.27 ms                                                | 6.86 ms: 1.06x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 875 ms: 1.05x faster                                   |
| typing_runtime_protocols | 544 us                                                 | 520 us: 1.05x faster                                   |
| unpickle                 | 14.4 us                                                | 13.8 us: 1.04x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.51 ms: 1.04x faster                                  |
| mdp                      | 2.85 sec                                               | 2.77 sec: 1.03x faster                                 |
| xml_etree_parse          | 168 ms                                                 | 164 ms: 1.02x faster                                   |
| asyncio_websockets       | 559 ms                                                 | 550 ms: 1.02x faster                                   |
| coverage                 | 79.4 ms                                                | 78.8 ms: 1.01x faster                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.01 ms: 1.01x slower                                  |
| pidigits                 | 191 ms                                                 | 194 ms: 1.02x slower                                   |
| pickle                   | 10.7 us                                                | 11.0 us: 1.03x slower                                  |
| gc_traversal             | 3.62 ms                                                | 4.01 ms: 1.11x slower                                  |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.11 sec: 1.21x slower                                 |
| Geometric mean           | (ref)                                                  | 1.27x faster                                           |

Benchmark hidden because not significant (2): bench_mp_pool, unpickle_list
Ignored benchmarks (4) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.07x