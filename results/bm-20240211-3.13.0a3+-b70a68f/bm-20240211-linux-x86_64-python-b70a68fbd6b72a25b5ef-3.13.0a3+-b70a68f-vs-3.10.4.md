
# Results vs. 3.10.4

- fork: python
- ref: b70a68fbd6b72a25b5ef
- machine: linux-x86_64
- commit hash: b70a68f
- commit date: 2024-02-11
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                  |
| docutils       | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.6 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 430 ms: 1.69x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 90.0 ms: 1.71x faster                                                  |
| float          | 117 ms                                                 | 81.3 ms: 1.44x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.36x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| regex_dna      | 227 ms                                                 | 223 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.12x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 217 us: 1.52x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.13 sec: 1.48x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 159 ms: 1.06x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.25 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| unpickle             | 14.4 us                                                | 16.0 us: 1.11x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.3 us: 1.19x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.15x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.76 ms: 1.48x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.94x faster                                                   |
| generators               | 80.1 ms                                                | 29.2 ms: 2.74x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.16 ms: 2.50x faster                                                  |
| logging_silent           | 190 ns                                                 | 94.2 ns: 2.01x faster                                                  |
| raytrace                 | 507 ms                                                 | 256 ms: 1.98x faster                                                   |
| chaos                    | 115 ms                                                 | 58.8 ms: 1.96x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 70.7 ms: 1.81x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 65.7 ms: 1.80x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.3 ms: 1.78x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.76x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.25 ms: 1.74x faster                                                  |
| go                       | 240 ms                                                 | 139 ms: 1.73x faster                                                   |
| hexiom                   | 10.4 ms                                                | 6.05 ms: 1.72x faster                                                  |
| scimark_sor              | 220 ms                                                 | 128 ms: 1.71x faster                                                   |
| nbody                    | 154 ms                                                 | 90.0 ms: 1.71x faster                                                  |
| async_tree_none          | 728 ms                                                 | 430 ms: 1.69x faster                                                   |
| richards                 | 79.3 ms                                                | 46.9 ms: 1.69x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.59x faster                                                  |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.57x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 557 ms: 1.56x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.9 us: 1.54x faster                                                  |
| pyflate                  | 716 ms                                                 | 470 ms: 1.52x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 217 us: 1.52x faster                                                   |
| spectral_norm            | 170 ms                                                 | 112 ms: 1.52x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.62 us: 1.48x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.13 sec: 1.48x faster                                                 |
| logging_format           | 9.09 us                                                | 6.19 us: 1.47x faster                                                  |
| regex_compile            | 188 ms                                                 | 129 ms: 1.46x faster                                                   |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 703 ms: 1.45x faster                                                   |
| tornado_http             | 136 ms                                                 | 94.6 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                 |
| float                    | 117 ms                                                 | 81.3 ms: 1.44x faster                                                  |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.48 sec: 1.42x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 721 ms: 1.41x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.89 ms: 1.41x faster                                                  |
| deepcopy                 | 479 us                                                 | 344 us: 1.39x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.36x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 58.3 ms: 1.36x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.35x faster                                                 |
| fannkuch                 | 532 ms                                                 | 395 ms: 1.34x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.83 ms: 1.34x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                   |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.33x faster                                                   |
| 2to3                     | 348 ms                                                 | 263 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.32x faster                                                  |
| nqueens                  | 106 ms                                                 | 81.4 ms: 1.30x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.0 ms: 1.30x faster                                                  |
| sympy_str                | 346 ms                                                 | 268 ms: 1.29x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.29x faster                                                  |
| scimark_fft              | 466 ms                                                 | 363 ms: 1.28x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.61 sec: 1.26x faster                                                 |
| sympy_expand             | 566 ms                                                 | 454 ms: 1.25x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 48.8 ns: 1.23x faster                                                  |
| dask                     | 441 ms                                                 | 362 ms: 1.22x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 818 us: 1.21x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.6 ms: 1.16x faster                                                  |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                                  |
| json                     | 5.69 ms                                                | 5.07 ms: 1.12x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                  |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.58 sec: 1.10x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.08x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.79 us: 1.08x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.7 ms: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 159 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.98 us: 1.04x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| regex_dna                | 227 ms                                                 | 223 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| async_generators         | 444 ms                                                 | 449 ms: 1.01x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.25 us: 1.03x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.76 ms: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                  |
| unpickle                 | 14.4 us                                                | 16.0 us: 1.11x slower                                                  |
| telco                    | 7.27 ms                                                | 8.35 ms: 1.15x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.3 us: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.3 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.76 ms: 1.48x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.36x faster                                                           |

Benchmark hidden because not significant (3): mypy2, bench_mp_pool, regex_effbot
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240211-3.13.0a3+-b70a68f/bm-20240211-linux-x86_64-python-b70a68fbd6b72a25b5ef-3.13.0a3+-b70a68f.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.06x