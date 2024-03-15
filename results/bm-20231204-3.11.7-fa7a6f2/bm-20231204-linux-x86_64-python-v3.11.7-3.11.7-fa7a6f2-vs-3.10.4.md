
# Results vs. 3.10.4

- fork: python
- ref: v3.11.7
- machine: linux-x86_64
- commit hash: fa7a6f2
- commit date: 2023-12-04
- overall geometric mean: 1.28x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 261 ms: 1.33x faster                                   |
| chameleon      | 9.68 ms                                                | 7.03 ms: 1.38x faster                                  |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| html5lib       | 88.9 ms                                                | 64.7 ms: 1.37x faster                                  |
| tornado_http   | 136 ms                                                 | 96.6 ms: 1.41x faster                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 533 ms: 1.37x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 750 ms: 1.36x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.31 sec: 1.35x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 650 ms: 1.34x faster                                   |
| Geometric mean          | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.5 ms: 1.64x faster                                  |
| float          | 117 ms                                                 | 79.1 ms: 1.48x faster                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.9 ms: 1.21x faster                                  |
| regex_dna      | 227 ms                                                 | 209 ms: 1.08x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.43 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.18x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 317 us: 1.53x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 56.6 ms: 1.40x faster                                  |
| unpickle_pure_python | 331 us                                                 | 239 us: 1.38x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.31 sec: 1.36x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 81.0 ms: 1.23x faster                                  |
| json_loads           | 31.2 us                                                | 25.8 us: 1.21x faster                                  |
| pickle_list          | 5.08 us                                                | 4.69 us: 1.08x faster                                  |
| json_dumps           | 14.2 ms                                                | 13.2 ms: 1.07x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| xml_etree_parse      | 168 ms                                                 | 163 ms: 1.03x faster                                   |
| unpickle             | 14.4 us                                                | 14.1 us: 1.02x faster                                  |
| pickle               | 10.7 us                                                | 11.0 us: 1.03x slower                                  |
| pickle_dict          | 29.6 us                                                | 36.1 us: 1.22x slower                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                           |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.59 ms: 1.70x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.04 ms: 1.02x slower                                  |
| Geometric mean         | (ref)                                                  | 1.29x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.1 ms: 1.47x faster                                  |
| django_template | 48.2 ms                                                | 34.0 ms: 1.42x faster                                  |
| genshi_text     | 31.8 ms                                                | 23.1 ms: 1.38x faster                                  |
| genshi_xml      | 66.0 ms                                                | 53.6 ms: 1.23x faster                                  |
| Geometric mean  | (ref)                                                  | 1.37x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.79 ms: 2.09x faster                                  |
| logging_silent           | 190 ns                                                 | 106 ns: 1.79x faster                                   |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                   |
| python_startup           | 14.6 ms                                                | 8.59 ms: 1.70x faster                                  |
| pyflate                  | 716 ms                                                 | 424 ms: 1.69x faster                                   |
| go                       | 240 ms                                                 | 143 ms: 1.68x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 76.3 ms: 1.67x faster                                  |
| richards                 | 79.3 ms                                                | 47.6 ms: 1.66x faster                                  |
| raytrace                 | 507 ms                                                 | 306 ms: 1.66x faster                                   |
| nbody                    | 154 ms                                                 | 93.5 ms: 1.64x faster                                  |
| chaos                    | 115 ms                                                 | 70.8 ms: 1.63x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 72.8 ms: 1.62x faster                                  |
| richards_super           | 94.7 ms                                                | 59.5 ms: 1.59x faster                                  |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.58x faster                                   |
| hexiom                   | 10.4 ms                                                | 6.77 ms: 1.53x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.42 ms: 1.53x faster                                  |
| pickle_pure_python       | 484 us                                                 | 317 us: 1.53x faster                                   |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.52x faster                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.72 ms: 1.50x faster                                  |
| float                    | 117 ms                                                 | 79.1 ms: 1.48x faster                                  |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 39.8 us: 1.47x faster                                  |
| django_template          | 48.2 ms                                                | 34.0 ms: 1.42x faster                                  |
| tornado_http             | 136 ms                                                 | 96.6 ms: 1.41x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 56.6 ms: 1.40x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.52 sec: 1.38x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 735 ms: 1.38x faster                                   |
| pycparser                | 1.58 sec                                               | 1.14 sec: 1.38x faster                                 |
| unpickle_pure_python     | 331 us                                                 | 239 us: 1.38x faster                                   |
| genshi_text              | 31.8 ms                                                | 23.1 ms: 1.38x faster                                  |
| chameleon                | 9.68 ms                                                | 7.03 ms: 1.38x faster                                  |
| regex_compile            | 188 ms                                                 | 137 ms: 1.37x faster                                   |
| html5lib                 | 88.9 ms                                                | 64.7 ms: 1.37x faster                                  |
| async_tree_none          | 728 ms                                                 | 533 ms: 1.37x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.31 sec: 1.36x faster                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 750 ms: 1.36x faster                                   |
| deepcopy                 | 479 us                                                 | 355 us: 1.35x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.31 sec: 1.35x faster                                 |
| scimark_fft              | 466 ms                                                 | 345 ms: 1.35x faster                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.10 us: 1.35x faster                                  |
| logging_format           | 9.09 us                                                | 6.76 us: 1.35x faster                                  |
| thrift                   | 1.07 ms                                                | 797 us: 1.34x faster                                   |
| logging_simple           | 8.30 us                                                | 6.18 us: 1.34x faster                                  |
| async_tree_memoization   | 870 ms                                                 | 650 ms: 1.34x faster                                   |
| 2to3                     | 348 ms                                                 | 261 ms: 1.33x faster                                   |
| fannkuch                 | 532 ms                                                 | 400 ms: 1.33x faster                                   |
| coroutines               | 35.1 ms                                                | 26.4 ms: 1.33x faster                                  |
| mypy2                    | 894 ms                                                 | 679 ms: 1.32x faster                                   |
| aiohttp                  | 1.44 ms                                                | 1.10 ms: 1.31x faster                                  |
| dulwich_log              | 84.3 ms                                                | 64.5 ms: 1.31x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.17 ms: 1.31x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 17.9 ms: 1.30x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.06 ms: 1.28x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 112 ms: 1.27x faster                                   |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| sqlglot_optimize         | 69.2 ms                                                | 55.0 ms: 1.26x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 47.9 ns: 1.25x faster                                  |
| sqlalchemy_declarative   | 172 ms                                                 | 138 ms: 1.25x faster                                   |
| comprehensions           | 28.8 us                                                | 23.1 us: 1.25x faster                                  |
| nqueens                  | 106 ms                                                 | 85.2 ms: 1.24x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| genshi_xml               | 66.0 ms                                                | 53.6 ms: 1.23x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 81.0 ms: 1.23x faster                                  |
| async_generators         | 444 ms                                                 | 362 ms: 1.22x faster                                   |
| dask                     | 441 ms                                                 | 362 ms: 1.22x faster                                   |
| regex_v8                 | 27.8 ms                                                | 22.9 ms: 1.21x faster                                  |
| json_loads               | 31.2 us                                                | 25.8 us: 1.21x faster                                  |
| flaskblogging            | 8.58 ms                                                | 7.18 ms: 1.19x faster                                  |
| pylint                   | 551 ms                                                 | 462 ms: 1.19x faster                                   |
| sympy_sum                | 196 ms                                                 | 165 ms: 1.19x faster                                   |
| bench_thread_pool        | 986 us                                                 | 831 us: 1.19x faster                                   |
| djangocms                | 38.4 us                                                | 32.4 us: 1.19x faster                                  |
| sympy_str                | 346 ms                                                 | 295 ms: 1.17x faster                                   |
| sqlite_synth             | 3.02 us                                                | 2.58 us: 1.17x faster                                  |
| json                     | 5.69 ms                                                | 4.94 ms: 1.15x faster                                  |
| sympy_expand             | 566 ms                                                 | 495 ms: 1.14x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.45 ms: 1.12x faster                                  |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                  |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                   |
| regex_dna                | 227 ms                                                 | 209 ms: 1.08x faster                                   |
| pickle_list              | 5.08 us                                                | 4.69 us: 1.08x faster                                  |
| json_dumps               | 14.2 ms                                                | 13.2 ms: 1.07x faster                                  |
| telco                    | 7.27 ms                                                | 6.79 ms: 1.07x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                   |
| typing_runtime_protocols | 544 us                                                 | 512 us: 1.06x faster                                   |
| generators               | 80.1 ms                                                | 75.5 ms: 1.06x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.43 ms: 1.06x faster                                  |
| mdp                      | 2.85 sec                                               | 2.71 sec: 1.05x faster                                 |
| asyncio_tcp              | 922 ms                                                 | 880 ms: 1.05x faster                                   |
| xml_etree_parse          | 168 ms                                                 | 163 ms: 1.03x faster                                   |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| unpickle                 | 14.4 us                                                | 14.1 us: 1.02x faster                                  |
| asyncio_websockets       | 559 ms                                                 | 550 ms: 1.02x faster                                   |
| python_startup_no_site   | 5.93 ms                                                | 6.04 ms: 1.02x slower                                  |
| gc_traversal             | 3.62 ms                                                | 3.74 ms: 1.03x slower                                  |
| pickle                   | 10.7 us                                                | 11.0 us: 1.03x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.10 sec: 1.21x slower                                 |
| pickle_dict              | 29.6 us                                                | 36.1 us: 1.22x slower                                  |
| Geometric mean           | (ref)                                                  | 1.28x faster                                           |

Benchmark hidden because not significant (3): bench_mp_pool, coverage, unpickle_list
Ignored benchmarks (4) of results/bm-20231204-3.11.7-fa7a6f2/bm-20231204-linux-x86_64-python-v3.11.7-3.11.7-fa7a6f2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.07x