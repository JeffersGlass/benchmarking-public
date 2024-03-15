
# Results vs. 3.10.4

- fork: python
- ref: v3.12.2
- machine: linux-x86_64
- commit hash: 6abddd9
- commit date: 2024-02-06
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.10x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 272 ms: 1.28x faster                                   |
| chameleon      | 9.68 ms                                                | 7.26 ms: 1.33x faster                                  |
| docutils       | 3.30 sec                                               | 2.71 sec: 1.22x faster                                 |
| tornado_http   | 136 ms                                                 | 99.4 ms: 1.37x faster                                  |
| Geometric mean | (ref)                                                  | 1.30x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 474 ms: 1.54x faster                                   |
| async_tree_io           | 1.77 sec                                               | 1.15 sec: 1.53x faster                                 |
| async_tree_memoization  | 870 ms                                                 | 576 ms: 1.51x faster                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.5 ms: 1.62x faster                                  |
| float          | 117 ms                                                 | 84.1 ms: 1.39x faster                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.32x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 144 ms: 1.31x faster                                   |
| regex_v8       | 27.8 ms                                                | 23.0 ms: 1.21x faster                                  |
| regex_dna      | 227 ms                                                 | 214 ms: 1.06x faster                                   |
| regex_effbot   | 3.63 ms                                                | 3.89 ms: 1.07x slower                                  |
| Geometric mean | (ref)                                                  | 1.12x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 319 us: 1.52x faster                                   |
| unpickle_pure_python | 331 us                                                 | 228 us: 1.45x faster                                   |
| tomli_loads          | 3.14 sec                                               | 2.30 sec: 1.37x faster                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                  |
| xml_etree_process    | 79.1 ms                                                | 61.2 ms: 1.29x faster                                  |
| xml_etree_generate   | 99.4 ms                                                | 88.0 ms: 1.13x faster                                  |
| json_loads           | 31.2 us                                                | 28.1 us: 1.11x faster                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                   |
| pickle_list          | 5.08 us                                                | 4.89 us: 1.04x faster                                  |
| unpickle_list        | 5.20 us                                                | 5.36 us: 1.03x slower                                  |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                  |
| unpickle             | 14.4 us                                                | 15.3 us: 1.07x slower                                  |
| pickle_dict          | 29.6 us                                                | 33.4 us: 1.13x slower                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.45 ms: 1.54x faster                                  |
| python_startup_no_site | 5.93 ms                                                | 6.80 ms: 1.15x slower                                  |
| Geometric mean         | (ref)                                                  | 1.16x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.7 ms: 1.39x faster                                  |
| django_template | 48.2 ms                                                | 34.8 ms: 1.38x faster                                  |
| Geometric mean  | (ref)                                                  | 1.39x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 123 us: 4.44x faster                                   |
| generators               | 80.1 ms                                                | 32.3 ms: 2.48x faster                                  |
| deltablue                | 7.91 ms                                                | 3.64 ms: 2.17x faster                                  |
| richards_super           | 94.7 ms                                                | 50.4 ms: 1.88x faster                                  |
| asyncio_tcp              | 922 ms                                                 | 509 ms: 1.81x faster                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                   |
| richards                 | 79.3 ms                                                | 45.2 ms: 1.75x faster                                  |
| chaos                    | 115 ms                                                 | 66.3 ms: 1.74x faster                                  |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.70x faster                                   |
| go                       | 240 ms                                                 | 142 ms: 1.69x faster                                   |
| raytrace                 | 507 ms                                                 | 308 ms: 1.65x faster                                   |
| nbody                    | 154 ms                                                 | 94.5 ms: 1.62x faster                                  |
| hexiom                   | 10.4 ms                                                | 6.44 ms: 1.61x faster                                  |
| scimark_monte_carlo      | 118 ms                                                 | 73.9 ms: 1.60x faster                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.37 ms: 1.59x faster                                  |
| crypto_pyaes             | 128 ms                                                 | 80.9 ms: 1.58x faster                                  |
| python_startup           | 14.6 ms                                                | 9.45 ms: 1.54x faster                                  |
| async_tree_none          | 728 ms                                                 | 474 ms: 1.54x faster                                   |
| async_tree_io            | 1.77 sec                                               | 1.15 sec: 1.53x faster                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.69 ms: 1.53x faster                                  |
| pickle_pure_python       | 484 us                                                 | 319 us: 1.52x faster                                   |
| async_tree_memoization   | 870 ms                                                 | 576 ms: 1.51x faster                                   |
| pyflate                  | 716 ms                                                 | 477 ms: 1.50x faster                                   |
| coroutines               | 35.1 ms                                                | 23.5 ms: 1.49x faster                                  |
| spectral_norm            | 170 ms                                                 | 114 ms: 1.49x faster                                   |
| deepcopy_memo            | 58.5 us                                                | 39.7 us: 1.47x faster                                  |
| scimark_lu               | 176 ms                                                 | 120 ms: 1.46x faster                                   |
| unpickle_pure_python     | 331 us                                                 | 228 us: 1.45x faster                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                   |
| mako                     | 16.3 ms                                                | 11.7 ms: 1.39x faster                                  |
| float                    | 117 ms                                                 | 84.1 ms: 1.39x faster                                  |
| django_template          | 48.2 ms                                                | 34.8 ms: 1.38x faster                                  |
| tornado_http             | 136 ms                                                 | 99.4 ms: 1.37x faster                                  |
| tomli_loads              | 3.14 sec                                               | 2.30 sec: 1.37x faster                                 |
| comprehensions           | 28.8 us                                                | 21.0 us: 1.37x faster                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                  |
| pprint_pformat           | 2.10 sec                                               | 1.56 sec: 1.35x faster                                 |
| chameleon                | 9.68 ms                                                | 7.26 ms: 1.33x faster                                  |
| pprint_safe_repr         | 1.02 sec                                               | 765 ms: 1.33x faster                                   |
| deepcopy                 | 479 us                                                 | 364 us: 1.32x faster                                   |
| regex_compile            | 188 ms                                                 | 144 ms: 1.31x faster                                   |
| logging_simple           | 8.30 us                                                | 6.38 us: 1.30x faster                                  |
| xml_etree_process        | 79.1 ms                                                | 61.2 ms: 1.29x faster                                  |
| mypy2                    | 894 ms                                                 | 692 ms: 1.29x faster                                   |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.29x faster                                 |
| deepcopy_reduce          | 4.17 us                                                | 3.24 us: 1.29x faster                                  |
| sqlglot_normalize        | 143 ms                                                 | 112 ms: 1.28x faster                                   |
| 2to3                     | 348 ms                                                 | 272 ms: 1.28x faster                                   |
| logging_format           | 9.09 us                                                | 7.12 us: 1.28x faster                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.09 ms: 1.27x faster                                  |
| aiohttp                  | 1.44 ms                                                | 1.14 ms: 1.27x faster                                  |
| sqlalchemy_imperative    | 23.3 ms                                                | 18.4 ms: 1.27x faster                                  |
| fannkuch                 | 532 ms                                                 | 420 ms: 1.27x faster                                   |
| nqueens                  | 106 ms                                                 | 83.7 ms: 1.26x faster                                  |
| unpack_sequence          | 60.0 ns                                                | 47.6 ns: 1.26x faster                                  |
| sqlglot_optimize         | 69.2 ms                                                | 55.0 ms: 1.26x faster                                  |
| dulwich_log              | 84.3 ms                                                | 67.9 ms: 1.24x faster                                  |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                  |
| gunicorn                 | 1.53 ms                                                | 1.24 ms: 1.24x faster                                  |
| docutils                 | 3.30 sec                                               | 2.71 sec: 1.22x faster                                 |
| scimark_fft              | 466 ms                                                 | 383 ms: 1.22x faster                                   |
| regex_v8                 | 27.8 ms                                                | 23.0 ms: 1.21x faster                                  |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.20x faster                                   |
| dask                     | 441 ms                                                 | 368 ms: 1.20x faster                                   |
| sympy_expand             | 566 ms                                                 | 477 ms: 1.19x faster                                   |
| sqlalchemy_declarative   | 172 ms                                                 | 146 ms: 1.18x faster                                   |
| sympy_str                | 346 ms                                                 | 294 ms: 1.18x faster                                   |
| bench_thread_pool        | 986 us                                                 | 839 us: 1.18x faster                                   |
| xml_etree_generate       | 99.4 ms                                                | 88.0 ms: 1.13x faster                                  |
| json_loads               | 31.2 us                                                | 28.1 us: 1.11x faster                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                  |
| json                     | 5.69 ms                                                | 5.23 ms: 1.09x faster                                  |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                   |
| pathlib                  | 20.5 ms                                                | 18.8 ms: 1.09x faster                                  |
| coverage                 | 79.4 ms                                                | 73.3 ms: 1.08x faster                                  |
| meteor_contest           | 120 ms                                                 | 112 ms: 1.07x faster                                   |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                   |
| regex_dna                | 227 ms                                                 | 214 ms: 1.06x faster                                   |
| sqlite_synth             | 3.02 us                                                | 2.86 us: 1.06x faster                                  |
| pickle_list              | 5.08 us                                                | 4.89 us: 1.04x faster                                  |
| mdp                      | 2.85 sec                                               | 2.76 sec: 1.03x faster                                 |
| gc_traversal             | 3.62 ms                                                | 3.54 ms: 1.02x faster                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                   |
| telco                    | 7.27 ms                                                | 7.13 ms: 1.02x faster                                  |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                   |
| async_generators         | 444 ms                                                 | 453 ms: 1.02x slower                                   |
| unpickle_list            | 5.20 us                                                | 5.36 us: 1.03x slower                                  |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                  |
| unpickle                 | 14.4 us                                                | 15.3 us: 1.07x slower                                  |
| regex_effbot             | 3.63 ms                                                | 3.89 ms: 1.07x slower                                  |
| pickle_dict              | 29.6 us                                                | 33.4 us: 1.13x slower                                  |
| python_startup_no_site   | 5.93 ms                                                | 6.80 ms: 1.15x slower                                  |
| Geometric mean           | (ref)                                                  | 1.31x faster                                           |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (7) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift
Ignored benchmarks (4) of results/bm-20240206-3.12.2-6abddd9/bm-20240206-linux-x86_64-python-v3.12.2-3.12.2-6abddd9.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.26x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.10x