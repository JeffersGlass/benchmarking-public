
# Results vs. 3.10.4

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.32x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 258 ms: 1.35x faster                                   |
| chameleon      | 9.68 ms                                                | 6.58 ms: 1.47x faster                                  |
| docutils       | 3.30 sec                                               | 2.57 sec: 1.28x faster                                 |
| html5lib       | 88.9 ms                                                | 64.2 ms: 1.38x faster                                  |
| tornado_http   | 136 ms                                                 | 96.6 ms: 1.41x faster                                  |
| Geometric mean | (ref)                                                  | 1.38x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 523 ms: 1.39x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 738 ms: 1.38x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.29 sec: 1.37x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 638 ms: 1.36x faster                                   |
| Geometric mean          | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 99.4 ms: 1.55x faster                                  |
| float          | 117 ms                                                 | 77.1 ms: 1.52x faster                                  |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.39x faster                                   |
| regex_v8       | 27.8 ms                                                | 22.2 ms: 1.25x faster                                  |
| regex_dna      | 227 ms                                                 | 200 ms: 1.13x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.45 ms: 1.05x faster                                  |
| Geometric mean | (ref)                                                  | 1.20x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 302 us: 1.60x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 53.9 ms: 1.47x faster                                  |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.19 sec: 1.43x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 76.5 ms: 1.30x faster                                  |
| pickle_list          | 5.08 us                                                | 4.01 us: 1.27x faster                                  |
| json_loads           | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| json_dumps           | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| unpickle             | 14.4 us                                                | 13.1 us: 1.10x faster                                  |
| pickle               | 10.7 us                                                | 9.76 us: 1.09x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 160 ms: 1.05x faster                                   |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                  |
| pickle_dict          | 29.6 us                                                | 30.7 us: 1.04x slower                                  |
| Geometric mean       | (ref)                                                  | 1.21x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.53 ms: 1.71x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.01 ms: 1.01x slower                                  |
| Geometric mean         | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.80 ms: 1.67x faster                                  |
| django_template | 48.2 ms                                                | 33.0 ms: 1.46x faster                                  |
| genshi_text     | 31.8 ms                                                | 22.4 ms: 1.42x faster                                  |
| genshi_xml      | 66.0 ms                                                | 51.8 ms: 1.27x faster                                  |
| Geometric mean  | (ref)                                                  | 1.45x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.71 ms: 2.13x faster                                  |
| scimark_sor              | 220 ms                                                 | 118 ms: 1.87x faster                                   |
| logging_silent           | 190 ns                                                 | 103 ns: 1.85x faster                                   |
| spectral_norm            | 170 ms                                                 | 97.1 ms: 1.75x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 67.7 ms: 1.75x faster                                  |
| raytrace                 | 507 ms                                                 | 294 ms: 1.72x faster                                   |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 74.6 ms: 1.71x faster                                  |
| python_startup           | 14.6 ms                                                | 8.53 ms: 1.71x faster                                  |
| pyflate                  | 716 ms                                                 | 421 ms: 1.70x faster                                   |
| mako                     | 16.3 ms                                                | 9.80 ms: 1.67x faster                                  |
| chaos                    | 115 ms                                                 | 70.2 ms: 1.64x faster                                  |
| richards                 | 79.3 ms                                                | 48.5 ms: 1.63x faster                                  |
| scimark_lu               | 176 ms                                                 | 109 ms: 1.61x faster                                   |
| pickle_pure_python       | 484 us                                                 | 302 us: 1.60x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 36.5 us: 1.60x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.50 ms: 1.60x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.37 ms: 1.58x faster                                  |
| richards_super           | 94.7 ms                                                | 60.0 ms: 1.58x faster                                  |
| nbody                    | 154 ms                                                 | 99.4 ms: 1.55x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                  |
| float                    | 117 ms                                                 | 77.1 ms: 1.52x faster                                  |
| chameleon                | 9.68 ms                                                | 6.58 ms: 1.47x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 53.9 ms: 1.47x faster                                  |
| django_template          | 48.2 ms                                                | 33.0 ms: 1.46x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.45 sec: 1.45x faster                                 |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.44x faster                                   |
| pprint_safe_repr         | 1.02 sec                                               | 707 ms: 1.44x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.19 sec: 1.43x faster                                 |
| scimark_fft              | 466 ms                                                 | 326 ms: 1.43x faster                                   |
| genshi_text              | 31.8 ms                                                | 22.4 ms: 1.42x faster                                  |
| deepcopy_reduce          | 4.17 us                                                | 2.94 us: 1.42x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.58 ms: 1.41x faster                                  |
| tornado_http             | 136 ms                                                 | 96.6 ms: 1.41x faster                                  |
| deepcopy                 | 479 us                                                 | 341 us: 1.40x faster                                   |
| async_tree_none          | 728 ms                                                 | 523 ms: 1.39x faster                                   |
| thrift                   | 1.07 ms                                                | 771 us: 1.39x faster                                   |
| regex_compile            | 188 ms                                                 | 136 ms: 1.39x faster                                   |
| html5lib                 | 88.9 ms                                                | 64.2 ms: 1.38x faster                                  |
| logging_format           | 9.09 us                                                | 6.58 us: 1.38x faster                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 738 ms: 1.38x faster                                   |
| unpack_sequence          | 60.0 ns                                                | 43.6 ns: 1.38x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.29 sec: 1.37x faster                                 |
| logging_simple           | 8.30 us                                                | 6.09 us: 1.36x faster                                  |
| async_tree_memoization   | 870 ms                                                 | 638 ms: 1.36x faster                                   |
| coroutines               | 35.1 ms                                                | 25.9 ms: 1.36x faster                                  |
| 2to3                     | 348 ms                                                 | 258 ms: 1.35x faster                                   |
| fannkuch                 | 532 ms                                                 | 394 ms: 1.35x faster                                   |
| pycparser                | 1.58 sec                                               | 1.18 sec: 1.33x faster                                 |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                   |
| aiohttp                  | 1.44 ms                                                | 1.09 ms: 1.32x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.17 ms: 1.31x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 17.9 ms: 1.31x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.0 ms: 1.31x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 76.5 ms: 1.30x faster                                  |
| dulwich_log              | 84.3 ms                                                | 65.5 ms: 1.29x faster                                  |
| docutils                 | 3.30 sec                                               | 2.57 sec: 1.28x faster                                 |
| comprehensions           | 28.8 us                                                | 22.6 us: 1.27x faster                                  |
| genshi_xml               | 66.0 ms                                                | 51.8 ms: 1.27x faster                                  |
| nqueens                  | 106 ms                                                 | 83.1 ms: 1.27x faster                                  |
| pickle_list              | 5.08 us                                                | 4.01 us: 1.27x faster                                  |
| regex_v8                 | 27.8 ms                                                | 22.2 ms: 1.25x faster                                  |
| sqlalchemy_declarative   | 172 ms                                                 | 139 ms: 1.24x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 20.9 ms: 1.24x faster                                  |
| async_generators         | 444 ms                                                 | 361 ms: 1.23x faster                                   |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                   |
| bench_thread_pool        | 986 us                                                 | 816 us: 1.21x faster                                   |
| sqlite_synth             | 3.02 us                                                | 2.51 us: 1.21x faster                                  |
| sympy_expand             | 566 ms                                                 | 470 ms: 1.20x faster                                   |
| flaskblogging            | 8.58 ms                                                | 7.17 ms: 1.20x faster                                  |
| sympy_str                | 346 ms                                                 | 290 ms: 1.19x faster                                   |
| pylint                   | 551 ms                                                 | 462 ms: 1.19x faster                                   |
| json_loads               | 31.2 us                                                | 26.2 us: 1.19x faster                                  |
| sympy_sum                | 196 ms                                                 | 166 ms: 1.18x faster                                   |
| json                     | 5.69 ms                                                | 4.85 ms: 1.17x faster                                  |
| djangocms                | 38.4 us                                                | 33.0 us: 1.17x faster                                  |
| pathlib                  | 20.5 ms                                                | 18.0 ms: 1.14x faster                                  |
| regex_dna                | 227 ms                                                 | 200 ms: 1.13x faster                                   |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                   |
| json_dumps               | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| unpickle                 | 14.4 us                                                | 13.1 us: 1.10x faster                                  |
| typing_runtime_protocols | 544 us                                                 | 495 us: 1.10x faster                                   |
| telco                    | 7.27 ms                                                | 6.62 ms: 1.10x faster                                  |
| mdp                      | 2.85 sec                                               | 2.60 sec: 1.09x faster                                 |
| pickle                   | 10.7 us                                                | 9.76 us: 1.09x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                  |
| generators               | 80.1 ms                                                | 73.7 ms: 1.09x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.45 ms: 1.05x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 160 ms: 1.05x faster                                   |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                  |
| pidigits                 | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| python_startup_no_site   | 5.93 ms                                                | 6.01 ms: 1.01x slower                                  |
| pickle_dict              | 29.6 us                                                | 30.7 us: 1.04x slower                                  |
| gc_traversal             | 3.62 ms                                                | 4.04 ms: 1.12x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.15 sec: 1.22x slower                                 |
| Geometric mean           | (ref)                                                  | 1.32x faster                                           |

Benchmark hidden because not significant (2): bench_mp_pool, asyncio_tcp
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x