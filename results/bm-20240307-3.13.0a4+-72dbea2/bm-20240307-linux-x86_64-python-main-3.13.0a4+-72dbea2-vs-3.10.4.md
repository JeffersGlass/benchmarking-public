# Results vs. 3.10.4

- fork: python
- ref: main
- machine: linux-x86_64
- commit hash: 72dbea2
- commit date: 2024-03-07
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                   |
| chameleon      | 9.68 ms                                                | 6.92 ms: 1.40x faster                                  |
| docutils       | 3.30 sec                                               | 2.63 sec: 1.25x faster                                 |
| html5lib       | 88.9 ms                                                | 66.1 ms: 1.35x faster                                  |
| tornado_http   | 136 ms                                                 | 95.1 ms: 1.43x faster                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 430 ms: 1.69x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 554 ms: 1.57x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 92.0 ms: 1.67x faster                                  |
| float          | 117 ms                                                 | 80.4 ms: 1.46x faster                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.43x faster                                   |
| regex_v8       | 27.8 ms                                                | 25.2 ms: 1.10x faster                                  |
| regex_dna      | 227 ms                                                 | 217 ms: 1.04x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.54 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 296 us: 1.64x faster                                   |
| unpickle_pure_python | 331 us                                                 | 214 us: 1.55x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.16 sec: 1.46x faster                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 57.8 ms: 1.37x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 84.4 ms: 1.18x faster                                  |
| json_loads           | 31.2 us                                                | 28.0 us: 1.11x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                   |
| unpickle_list        | 5.20 us                                                | 5.02 us: 1.04x faster                                  |
| pickle_list          | 5.08 us                                                | 5.10 us: 1.00x slower                                  |
| unpickle             | 14.4 us                                                | 14.6 us: 1.01x slower                                  |
| pickle               | 10.7 us                                                | 11.5 us: 1.08x slower                                  |
| pickle_dict          | 29.6 us                                                | 35.9 us: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 8.72 ms: 1.47x slower                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.1 ms: 1.47x faster                                  |
| django_template | 48.2 ms                                                | 33.8 ms: 1.42x faster                                  |
| genshi_text     | 31.8 ms                                                | 23.0 ms: 1.38x faster                                  |
| genshi_xml      | 66.0 ms                                                | 50.7 ms: 1.30x faster                                  |
| Geometric mean  | (ref)                                                  | 1.39x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.94x faster                                   |
| generators               | 80.1 ms                                                | 29.9 ms: 2.68x faster                                  |
| deltablue                | 7.91 ms                                                | 3.15 ms: 2.51x faster                                  |
| raytrace                 | 507 ms                                                 | 262 ms: 1.94x faster                                   |
| chaos                    | 115 ms                                                 | 59.6 ms: 1.94x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.91x faster                                   |
| logging_silent           | 190 ns                                                 | 100 ns: 1.90x faster                                   |
| scimark_sor              | 220 ms                                                 | 116 ms: 1.89x faster                                   |
| richards_super           | 94.7 ms                                                | 50.7 ms: 1.87x faster                                  |
| comprehensions           | 28.8 us                                                | 15.8 us: 1.82x faster                                  |
| pylint                   | 551 ms                                                 | 306 ms: 1.80x faster                                   |
| scimark_monte_carlo      | 118 ms                                                 | 65.9 ms: 1.79x faster                                  |
| crypto_pyaes             | 128 ms                                                 | 71.7 ms: 1.78x faster                                  |
| richards                 | 79.3 ms                                                | 44.5 ms: 1.78x faster                                  |
| go                       | 240 ms                                                 | 136 ms: 1.76x faster                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.04 ms: 1.72x faster                                  |
| async_tree_none          | 728 ms                                                 | 430 ms: 1.69x faster                                   |
| nbody                    | 154 ms                                                 | 92.0 ms: 1.67x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                  |
| pickle_pure_python       | 484 us                                                 | 296 us: 1.64x faster                                   |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.60x faster                                  |
| pyflate                  | 716 ms                                                 | 455 ms: 1.58x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 554 ms: 1.57x faster                                   |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.57x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 214 us: 1.55x faster                                   |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.55x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 38.2 us: 1.53x faster                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                 |
| logging_simple           | 8.30 us                                                | 5.58 us: 1.49x faster                                  |
| logging_format           | 9.09 us                                                | 6.15 us: 1.48x faster                                  |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                  |
| tomli_loads              | 3.14 sec                                               | 2.16 sec: 1.46x faster                                 |
| float                    | 117 ms                                                 | 80.4 ms: 1.46x faster                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                  |
| regex_compile            | 188 ms                                                 | 131 ms: 1.43x faster                                   |
| tornado_http             | 136 ms                                                 | 95.1 ms: 1.43x faster                                  |
| django_template          | 48.2 ms                                                | 33.8 ms: 1.42x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.49 sec: 1.41x faster                                 |
| pprint_safe_repr         | 1.02 sec                                               | 725 ms: 1.40x faster                                   |
| chameleon                | 9.68 ms                                                | 6.92 ms: 1.40x faster                                  |
| deepcopy                 | 479 us                                                 | 344 us: 1.39x faster                                   |
| thrift                   | 1.07 ms                                                | 771 us: 1.39x faster                                   |
| genshi_text              | 31.8 ms                                                | 23.0 ms: 1.38x faster                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.03 us: 1.38x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 104 ms: 1.37x faster                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 57.8 ms: 1.37x faster                                  |
| fannkuch                 | 532 ms                                                 | 391 ms: 1.36x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.78 ms: 1.35x faster                                  |
| html5lib                 | 88.9 ms                                                | 66.1 ms: 1.35x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 44.7 ns: 1.34x faster                                  |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                   |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                   |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                 |
| nqueens                  | 106 ms                                                 | 80.1 ms: 1.32x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 52.9 ms: 1.31x faster                                  |
| sympy_str                | 346 ms                                                 | 265 ms: 1.30x faster                                   |
| genshi_xml               | 66.0 ms                                                | 50.7 ms: 1.30x faster                                  |
| dulwich_log              | 84.3 ms                                                | 65.4 ms: 1.29x faster                                  |
| scimark_fft              | 466 ms                                                 | 364 ms: 1.28x faster                                   |
| aiohttp                  | 1.44 ms                                                | 1.14 ms: 1.27x faster                                  |
| sympy_expand             | 566 ms                                                 | 450 ms: 1.26x faster                                   |
| docutils                 | 3.30 sec                                               | 2.63 sec: 1.25x faster                                 |
| gunicorn                 | 1.53 ms                                                | 1.25 ms: 1.23x faster                                  |
| bench_thread_pool        | 986 us                                                 | 823 us: 1.20x faster                                   |
| djangocms                | 38.4 us                                                | 32.2 us: 1.19x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 84.4 ms: 1.18x faster                                  |
| mdp                      | 2.85 sec                                               | 2.49 sec: 1.14x faster                                 |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.2 ms: 1.12x faster                                  |
| json_loads               | 31.2 us                                                | 28.0 us: 1.11x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                   |
| json                     | 5.69 ms                                                | 5.13 ms: 1.11x faster                                  |
| regex_v8                 | 27.8 ms                                                | 25.2 ms: 1.10x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                   |
| sqlite_synth             | 3.02 us                                                | 2.87 us: 1.05x faster                                  |
| regex_dna                | 227 ms                                                 | 217 ms: 1.04x faster                                   |
| unpickle_list            | 5.20 us                                                | 5.02 us: 1.04x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.54 ms: 1.02x faster                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                   |
| pickle_list              | 5.08 us                                                | 5.10 us: 1.00x slower                                  |
| gc_traversal             | 3.62 ms                                                | 3.67 ms: 1.01x slower                                  |
| unpickle                 | 14.4 us                                                | 14.6 us: 1.01x slower                                  |
| pickle                   | 10.7 us                                                | 11.5 us: 1.08x slower                                  |
| telco                    | 7.27 ms                                                | 8.28 ms: 1.14x slower                                  |
| dask                     | 441 ms                                                 | 519 ms: 1.18x slower                                   |
| coverage                 | 79.4 ms                                                | 95.7 ms: 1.20x slower                                  |
| pickle_dict              | 29.6 us                                                | 35.9 us: 1.21x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.72 ms: 1.47x slower                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                           |

Benchmark hidden because not significant (3): mypy2, async_generators, bench_mp_pool
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240307-3.13.0a4+-72dbea2/bm-20240307-linux-x86_64-python-main-3.13.0a4+-72dbea2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.31x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.07x