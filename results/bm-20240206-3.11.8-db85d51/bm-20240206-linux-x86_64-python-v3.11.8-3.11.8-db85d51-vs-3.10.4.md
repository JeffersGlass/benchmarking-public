
# Results vs. 3.10.4

- fork: python
- ref: v3.11.8
- machine: linux-x86_64
- commit hash: db85d51
- commit date: 2024-02-06
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 259 ms: 1.34x faster                                   |
| chameleon      | 9.68 ms                                                | 6.92 ms: 1.40x faster                                  |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| html5lib       | 88.9 ms                                                | 64.1 ms: 1.39x faster                                  |
| tornado_http   | 136 ms                                                 | 96.1 ms: 1.42x faster                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 529 ms: 1.38x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 744 ms: 1.37x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 646 ms: 1.35x faster                                   |
| Geometric mean          | (ref)                                                  | 1.36x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.5 ms: 1.61x faster                                  |
| float          | 117 ms                                                 | 77.8 ms: 1.51x faster                                  |
| pidigits       | 191 ms                                                 | 195 ms: 1.02x slower                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.8 ms: 1.22x faster                                  |
| regex_dna      | 227 ms                                                 | 208 ms: 1.09x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.45 ms: 1.05x faster                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 311 us: 1.56x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 56.1 ms: 1.41x faster                                  |
| unpickle_pure_python | 331 us                                                 | 235 us: 1.40x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.33 sec: 1.35x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 80.3 ms: 1.24x faster                                  |
| json_loads           | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 107 ms: 1.08x faster                                   |
| pickle_list          | 5.08 us                                                | 4.73 us: 1.07x faster                                  |
| unpickle             | 14.4 us                                                | 13.4 us: 1.07x faster                                  |
| json_dumps           | 14.2 ms                                                | 13.3 ms: 1.06x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 165 ms: 1.02x faster                                   |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                  |
| pickle_dict          | 29.6 us                                                | 35.8 us: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.00 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 10.8 ms: 1.51x faster                                  |
| django_template | 48.2 ms                                                | 33.0 ms: 1.46x faster                                  |
| genshi_text     | 31.8 ms                                                | 22.2 ms: 1.44x faster                                  |
| genshi_xml      | 66.0 ms                                                | 52.8 ms: 1.25x faster                                  |
| Geometric mean  | (ref)                                                  | 1.41x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.72 ms: 2.12x faster                                  |
| logging_silent           | 190 ns                                                 | 102 ns: 1.87x faster                                   |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.82x faster                                   |
| richards                 | 79.3 ms                                                | 46.4 ms: 1.71x faster                                  |
| python_startup           | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| pyflate                  | 716 ms                                                 | 422 ms: 1.70x faster                                   |
| raytrace                 | 507 ms                                                 | 299 ms: 1.69x faster                                   |
| go                       | 240 ms                                                 | 142 ms: 1.69x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 76.0 ms: 1.68x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 70.6 ms: 1.67x faster                                  |
| richards_super           | 94.7 ms                                                | 58.1 ms: 1.63x faster                                  |
| chaos                    | 115 ms                                                 | 71.1 ms: 1.62x faster                                  |
| nbody                    | 154 ms                                                 | 95.5 ms: 1.61x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.58 ms: 1.58x faster                                  |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.58x faster                                   |
| pickle_pure_python       | 484 us                                                 | 311 us: 1.56x faster                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.40 ms: 1.55x faster                                  |
| scimark_lu               | 176 ms                                                 | 115 ms: 1.53x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 38.8 us: 1.51x faster                                  |
| float                    | 117 ms                                                 | 77.8 ms: 1.51x faster                                  |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.71 ms: 1.50x faster                                  |
| django_template          | 48.2 ms                                                | 33.0 ms: 1.46x faster                                  |
| genshi_text              | 31.8 ms                                                | 22.2 ms: 1.44x faster                                  |
| tornado_http             | 136 ms                                                 | 96.1 ms: 1.42x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 56.1 ms: 1.41x faster                                  |
| unpickle_pure_python     | 331 us                                                 | 235 us: 1.40x faster                                   |
| chameleon                | 9.68 ms                                                | 6.92 ms: 1.40x faster                                  |
| pycparser                | 1.58 sec                                               | 1.14 sec: 1.39x faster                                 |
| pprint_pformat           | 2.10 sec                                               | 1.52 sec: 1.39x faster                                 |
| html5lib                 | 88.9 ms                                                | 64.1 ms: 1.39x faster                                  |
| pprint_safe_repr         | 1.02 sec                                               | 736 ms: 1.38x faster                                   |
| async_tree_none          | 728 ms                                                 | 529 ms: 1.38x faster                                   |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                   |
| regex_compile            | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| logging_format           | 9.09 us                                                | 6.63 us: 1.37x faster                                  |
| thrift                   | 1.07 ms                                                | 783 us: 1.37x faster                                   |
| logging_simple           | 8.30 us                                                | 6.07 us: 1.37x faster                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 744 ms: 1.37x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| tomli_loads              | 3.14 sec                                               | 2.33 sec: 1.35x faster                                 |
| deepcopy_reduce          | 4.17 us                                                | 3.09 us: 1.35x faster                                  |
| async_tree_memoization   | 870 ms                                                 | 646 ms: 1.35x faster                                   |
| 2to3                     | 348 ms                                                 | 259 ms: 1.34x faster                                   |
| scimark_fft              | 466 ms                                                 | 349 ms: 1.34x faster                                   |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                   |
| coroutines               | 35.1 ms                                                | 26.4 ms: 1.33x faster                                  |
| mypy2                    | 894 ms                                                 | 678 ms: 1.32x faster                                   |
| aiohttp                  | 1.44 ms                                                | 1.09 ms: 1.31x faster                                  |
| dulwich_log              | 84.3 ms                                                | 64.3 ms: 1.31x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.17 ms: 1.31x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 17.9 ms: 1.30x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.00 ms: 1.29x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 46.5 ns: 1.29x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 111 ms: 1.28x faster                                   |
| comprehensions           | 28.8 us                                                | 22.6 us: 1.27x faster                                  |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| sqlglot_optimize         | 69.2 ms                                                | 54.5 ms: 1.27x faster                                  |
| genshi_xml               | 66.0 ms                                                | 52.8 ms: 1.25x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 80.3 ms: 1.24x faster                                  |
| async_generators         | 444 ms                                                 | 361 ms: 1.23x faster                                   |
| sqlalchemy_declarative   | 172 ms                                                 | 140 ms: 1.23x faster                                   |
| nqueens                  | 106 ms                                                 | 86.5 ms: 1.22x faster                                  |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                   |
| regex_v8                 | 27.8 ms                                                | 22.8 ms: 1.22x faster                                  |
| bench_thread_pool        | 986 us                                                 | 824 us: 1.20x faster                                   |
| pylint                   | 551 ms                                                 | 462 ms: 1.19x faster                                   |
| json_loads               | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| flaskblogging            | 8.58 ms                                                | 7.23 ms: 1.19x faster                                  |
| sympy_sum                | 196 ms                                                 | 166 ms: 1.18x faster                                   |
| sympy_str                | 346 ms                                                 | 292 ms: 1.18x faster                                   |
| json                     | 5.69 ms                                                | 4.84 ms: 1.18x faster                                  |
| sqlite_synth             | 3.02 us                                                | 2.58 us: 1.17x faster                                  |
| djangocms                | 38.4 us                                                | 32.9 us: 1.17x faster                                  |
| sympy_expand             | 566 ms                                                 | 488 ms: 1.16x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.44 ms: 1.12x faster                                  |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                  |
| regex_dna                | 227 ms                                                 | 208 ms: 1.09x faster                                   |
| xml_etree_iterparse      | 115 ms                                                 | 107 ms: 1.08x faster                                   |
| pickle_list              | 5.08 us                                                | 4.73 us: 1.07x faster                                  |
| unpickle                 | 14.4 us                                                | 13.4 us: 1.07x faster                                  |
| json_dumps               | 14.2 ms                                                | 13.3 ms: 1.06x faster                                  |
| telco                    | 7.27 ms                                                | 6.83 ms: 1.06x faster                                  |
| typing_runtime_protocols | 544 us                                                 | 514 us: 1.06x faster                                   |
| generators               | 80.1 ms                                                | 75.9 ms: 1.06x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.45 ms: 1.05x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 165 ms: 1.02x faster                                   |
| asyncio_websockets       | 559 ms                                                 | 550 ms: 1.02x faster                                   |
| asyncio_tcp              | 922 ms                                                 | 909 ms: 1.01x faster                                   |
| mdp                      | 2.85 sec                                               | 2.82 sec: 1.01x faster                                 |
| coverage                 | 79.4 ms                                                | 78.9 ms: 1.01x faster                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.00 ms: 1.01x slower                                  |
| pidigits                 | 191 ms                                                 | 195 ms: 1.02x slower                                   |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                  |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                  |
| pickle_dict              | 29.6 us                                                | 35.8 us: 1.21x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.12 sec: 1.21x slower                                 |
| Geometric mean           | (ref)                                                  | 1.29x faster                                           |

Benchmark hidden because not significant (2): unpickle_list, bench_mp_pool
Ignored benchmarks (4) of results/bm-20240206-3.11.8-db85d51/bm-20240206-linux-x86_64-python-v3.11.8-3.11.8-db85d51.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.27x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.08x