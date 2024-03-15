
# Results vs. 3.10.4

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.33x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.27x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 259 ms: 1.35x faster                                   |
| chameleon      | 9.68 ms                                                | 6.61 ms: 1.47x faster                                  |
| docutils       | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| html5lib       | 88.9 ms                                                | 64.2 ms: 1.38x faster                                  |
| tornado_http   | 136 ms                                                 | 96.7 ms: 1.41x faster                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 526 ms: 1.39x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 740 ms: 1.37x faster                                   |
| async_tree_memoization  | 870 ms                                                 | 641 ms: 1.36x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| Geometric mean          | (ref)                                                  | 1.37x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.6 ms: 1.61x faster                                  |
| float          | 117 ms                                                 | 77.0 ms: 1.52x faster                                  |
| pidigits       | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| Geometric mean | (ref)                                                  | 1.35x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 136 ms: 1.38x faster                                   |
| regex_v8       | 27.8 ms                                                | 21.8 ms: 1.28x faster                                  |
| regex_dna      | 227 ms                                                 | 201 ms: 1.13x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.25 ms: 1.12x faster                                  |
| Geometric mean | (ref)                                                  | 1.22x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 306 us: 1.58x faster                                   |
| xml_etree_process    | 79.1 ms                                                | 53.8 ms: 1.47x faster                                  |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.45x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.22 sec: 1.41x faster                                 |
| xml_etree_generate   | 99.4 ms                                                | 76.2 ms: 1.30x faster                                  |
| pickle_list          | 5.08 us                                                | 4.12 us: 1.23x faster                                  |
| json_loads           | 31.2 us                                                | 25.9 us: 1.20x faster                                  |
| json_dumps           | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                   |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                  |
| pickle               | 10.7 us                                                | 10.0 us: 1.06x faster                                  |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                   |
| unpickle_list        | 5.20 us                                                | 5.00 us: 1.04x faster                                  |
| pickle_dict          | 29.6 us                                                | 31.0 us: 1.05x slower                                  |
| Geometric mean       | (ref)                                                  | 1.21x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.04 ms: 1.02x slower                                  |
| Geometric mean         | (ref)                                                  | 1.29x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.99 ms: 1.63x faster                                  |
| django_template | 48.2 ms                                                | 32.6 ms: 1.48x faster                                  |
| genshi_text     | 31.8 ms                                                | 22.3 ms: 1.43x faster                                  |
| genshi_xml      | 66.0 ms                                                | 52.8 ms: 1.25x faster                                  |
| Geometric mean  | (ref)                                                  | 1.44x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| deltablue                | 7.91 ms                                                | 3.69 ms: 2.14x faster                                  |
| logging_silent           | 190 ns                                                 | 98.6 ns: 1.92x faster                                  |
| scimark_sor              | 220 ms                                                 | 117 ms: 1.87x faster                                   |
| crypto_pyaes             | 128 ms                                                 | 73.9 ms: 1.73x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.8 ms: 1.72x faster                                  |
| raytrace                 | 507 ms                                                 | 295 ms: 1.72x faster                                   |
| pyflate                  | 716 ms                                                 | 419 ms: 1.71x faster                                   |
| go                       | 240 ms                                                 | 141 ms: 1.71x faster                                   |
| python_startup           | 14.6 ms                                                | 8.56 ms: 1.70x faster                                  |
| richards                 | 79.3 ms                                                | 47.1 ms: 1.68x faster                                  |
| chaos                    | 115 ms                                                 | 68.5 ms: 1.68x faster                                  |
| scimark_lu               | 176 ms                                                 | 107 ms: 1.64x faster                                   |
| spectral_norm            | 170 ms                                                 | 104 ms: 1.63x faster                                   |
| mako                     | 16.3 ms                                                | 9.99 ms: 1.63x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.39 ms: 1.63x faster                                  |
| richards_super           | 94.7 ms                                                | 58.3 ms: 1.63x faster                                  |
| nbody                    | 154 ms                                                 | 95.6 ms: 1.61x faster                                  |
| pickle_pure_python       | 484 us                                                 | 306 us: 1.58x faster                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.37 ms: 1.58x faster                                  |
| deepcopy_memo            | 58.5 us                                                | 37.2 us: 1.57x faster                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.67 ms: 1.54x faster                                  |
| float                    | 117 ms                                                 | 77.0 ms: 1.52x faster                                  |
| django_template          | 48.2 ms                                                | 32.6 ms: 1.48x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 53.8 ms: 1.47x faster                                  |
| chameleon                | 9.68 ms                                                | 6.61 ms: 1.47x faster                                  |
| pprint_safe_repr         | 1.02 sec                                               | 700 ms: 1.45x faster                                   |
| pprint_pformat           | 2.10 sec                                               | 1.45 sec: 1.45x faster                                 |
| unpickle_pure_python     | 331 us                                                 | 229 us: 1.45x faster                                   |
| genshi_text              | 31.8 ms                                                | 22.3 ms: 1.43x faster                                  |
| scimark_fft              | 466 ms                                                 | 329 ms: 1.42x faster                                   |
| tomli_loads              | 3.14 sec                                               | 2.22 sec: 1.41x faster                                 |
| tornado_http             | 136 ms                                                 | 96.7 ms: 1.41x faster                                  |
| thrift                   | 1.07 ms                                                | 763 us: 1.40x faster                                   |
| logging_simple           | 8.30 us                                                | 5.93 us: 1.40x faster                                  |
| deepcopy_reduce          | 4.17 us                                                | 2.99 us: 1.40x faster                                  |
| fannkuch                 | 532 ms                                                 | 383 ms: 1.39x faster                                   |
| pycparser                | 1.58 sec                                               | 1.13 sec: 1.39x faster                                 |
| logging_format           | 9.09 us                                                | 6.55 us: 1.39x faster                                  |
| async_tree_none          | 728 ms                                                 | 526 ms: 1.39x faster                                   |
| html5lib                 | 88.9 ms                                                | 64.2 ms: 1.38x faster                                  |
| regex_compile            | 188 ms                                                 | 136 ms: 1.38x faster                                   |
| coroutines               | 35.1 ms                                                | 25.4 ms: 1.38x faster                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 740 ms: 1.37x faster                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.72 ms: 1.37x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 43.9 ns: 1.37x faster                                  |
| deepcopy                 | 479 us                                                 | 351 us: 1.36x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 641 ms: 1.36x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.30 sec: 1.36x faster                                 |
| 2to3                     | 348 ms                                                 | 259 ms: 1.35x faster                                   |
| dulwich_log              | 84.3 ms                                                | 63.8 ms: 1.32x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.32x faster                                   |
| sqlalchemy_imperative    | 23.3 ms                                                | 17.9 ms: 1.31x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.10 ms: 1.31x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.0 ms: 1.30x faster                                  |
| xml_etree_generate       | 99.4 ms                                                | 76.2 ms: 1.30x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.19 ms: 1.28x faster                                  |
| regex_v8                 | 27.8 ms                                                | 21.8 ms: 1.28x faster                                  |
| docutils                 | 3.30 sec                                               | 2.59 sec: 1.27x faster                                 |
| comprehensions           | 28.8 us                                                | 22.7 us: 1.27x faster                                  |
| nqueens                  | 106 ms                                                 | 84.2 ms: 1.26x faster                                  |
| genshi_xml               | 66.0 ms                                                | 52.8 ms: 1.25x faster                                  |
| pickle_list              | 5.08 us                                                | 4.12 us: 1.23x faster                                  |
| sqlalchemy_declarative   | 172 ms                                                 | 140 ms: 1.23x faster                                   |
| async_generators         | 444 ms                                                 | 361 ms: 1.23x faster                                   |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.23x faster                                  |
| dask                     | 441 ms                                                 | 360 ms: 1.22x faster                                   |
| bench_thread_pool        | 986 us                                                 | 818 us: 1.21x faster                                   |
| json_loads               | 31.2 us                                                | 25.9 us: 1.20x faster                                  |
| pylint                   | 551 ms                                                 | 458 ms: 1.20x faster                                   |
| flaskblogging            | 8.58 ms                                                | 7.14 ms: 1.20x faster                                  |
| sqlite_synth             | 3.02 us                                                | 2.52 us: 1.20x faster                                  |
| sympy_str                | 346 ms                                                 | 291 ms: 1.19x faster                                   |
| sympy_expand             | 566 ms                                                 | 476 ms: 1.19x faster                                   |
| json                     | 5.69 ms                                                | 4.83 ms: 1.18x faster                                  |
| sympy_sum                | 196 ms                                                 | 167 ms: 1.17x faster                                   |
| djangocms                | 38.4 us                                                | 32.9 us: 1.17x faster                                  |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.1 ms: 1.13x faster                                  |
| regex_dna                | 227 ms                                                 | 201 ms: 1.13x faster                                   |
| json_dumps               | 14.2 ms                                                | 12.6 ms: 1.12x faster                                  |
| regex_effbot             | 3.63 ms                                                | 3.25 ms: 1.12x faster                                  |
| typing_runtime_protocols | 544 us                                                 | 493 us: 1.10x faster                                   |
| telco                    | 7.27 ms                                                | 6.60 ms: 1.10x faster                                  |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                 |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                  |
| generators               | 80.1 ms                                                | 73.8 ms: 1.09x faster                                  |
| unpickle                 | 14.4 us                                                | 13.3 us: 1.08x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 864 ms: 1.07x faster                                   |
| pickle                   | 10.7 us                                                | 10.0 us: 1.06x faster                                  |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                   |
| unpickle_list            | 5.20 us                                                | 5.00 us: 1.04x faster                                  |
| pidigits                 | 191 ms                                                 | 190 ms: 1.01x faster                                   |
| gc_traversal             | 3.62 ms                                                | 3.64 ms: 1.00x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.04 ms: 1.02x slower                                  |
| pickle_dict              | 29.6 us                                                | 31.0 us: 1.05x slower                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 3.18 sec: 1.24x slower                                 |
| Geometric mean           | (ref)                                                  | 1.33x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.30x
- 95% likely to have a speedup of 1.29x
- 99% likely to have a speedup of 1.27x


# Memory

- memory change: 1.09x