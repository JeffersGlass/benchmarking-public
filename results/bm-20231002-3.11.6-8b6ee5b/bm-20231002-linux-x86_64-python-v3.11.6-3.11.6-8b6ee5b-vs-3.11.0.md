
# Results vs. 3.11.0

- fork: python
- ref: v3.11.6
- machine: linux-x86_64
- commit hash: 8b6ee5b
- commit date: 2023-10-02
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 257 ms: 1.03x faster                                   |
| chameleon      | 6.70 ms                                                | 6.61 ms: 1.01x faster                                  |
| docutils       | 2.66 sec                                               | 2.58 sec: 1.03x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.9 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_memoization  | 639 ms                                                 | 632 ms: 1.01x faster                                   |
| async_tree_none         | 528 ms                                                 | 522 ms: 1.01x faster                                   |
| async_tree_cpu_io_mixed | 749 ms                                                 | 742 ms: 1.01x faster                                   |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| Geometric mean          | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 78.9 ms                                                | 75.7 ms: 1.04x faster                                  |
| nbody          | 96.0 ms                                                | 92.6 ms: 1.04x faster                                  |
| pidigits       | 194 ms                                                 | 199 ms: 1.03x slower                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_v8       | 22.9 ms                                                | 21.9 ms: 1.04x faster                                  |
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| regex_dna      | 205 ms                                                 | 199 ms: 1.03x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.47 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 23.9 us: 1.22x faster                                  |
| pickle_dict          | 34.6 us                                                | 29.9 us: 1.16x faster                                  |
| pickle_list          | 4.59 us                                                | 4.05 us: 1.13x faster                                  |
| pickle               | 11.0 us                                                | 9.82 us: 1.12x faster                                  |
| xml_etree_process    | 56.9 ms                                                | 53.7 ms: 1.06x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 76.7 ms: 1.06x faster                                  |
| unpickle_pure_python | 242 us                                                 | 230 us: 1.05x faster                                   |
| json_dumps           | 13.3 ms                                                | 12.7 ms: 1.05x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 103 ms: 1.05x faster                                   |
| pickle_pure_python   | 320 us                                                 | 306 us: 1.05x faster                                   |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                  |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| unpickle_list        | 5.21 us                                                | 5.08 us: 1.03x faster                                  |
| tomli_loads          | 2.30 sec                                               | 2.25 sec: 1.02x faster                                 |
| Geometric mean       | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.50 ms: 1.01x faster                                  |
| python_startup_no_site | 6.01 ms                                                | 6.00 ms: 1.00x faster                                  |
| Geometric mean         | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.88 ms: 1.08x faster                                  |
| genshi_xml      | 53.4 ms                                                | 51.5 ms: 1.04x faster                                  |
| genshi_text     | 22.5 ms                                                | 21.9 ms: 1.03x faster                                  |
| django_template | 33.5 ms                                                | 33.1 ms: 1.01x faster                                  |
| Geometric mean  | (ref)                                                  | 1.04x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20231002-linux-x86_64-python-v3.11.6-3.11.6-8b6ee5b |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads               | 29.2 us                                                | 23.9 us: 1.22x faster                                  |
| pickle_dict              | 34.6 us                                                | 29.9 us: 1.16x faster                                  |
| json                     | 5.24 ms                                                | 4.59 ms: 1.14x faster                                  |
| pickle_list              | 4.59 us                                                | 4.05 us: 1.13x faster                                  |
| pickle                   | 11.0 us                                                | 9.82 us: 1.12x faster                                  |
| deepcopy_memo            | 40.2 us                                                | 36.3 us: 1.11x faster                                  |
| logging_silent           | 111 ns                                                 | 101 ns: 1.10x faster                                   |
| mako                     | 10.7 ms                                                | 9.88 ms: 1.08x faster                                  |
| deepcopy_reduce          | 3.22 us                                                | 2.98 us: 1.08x faster                                  |
| pprint_pformat           | 1.55 sec                                               | 1.45 sec: 1.07x faster                                 |
| deepcopy                 | 365 us                                                 | 342 us: 1.07x faster                                   |
| comprehensions           | 23.6 us                                                | 22.2 us: 1.06x faster                                  |
| pprint_safe_repr         | 747 ms                                                 | 703 ms: 1.06x faster                                   |
| go                       | 149 ms                                                 | 140 ms: 1.06x faster                                   |
| pycparser                | 1.19 sec                                               | 1.12 sec: 1.06x faster                                 |
| scimark_lu               | 116 ms                                                 | 110 ms: 1.06x faster                                   |
| hexiom                   | 6.89 ms                                                | 6.49 ms: 1.06x faster                                  |
| xml_etree_process        | 56.9 ms                                                | 53.7 ms: 1.06x faster                                  |
| xml_etree_generate       | 81.1 ms                                                | 76.7 ms: 1.06x faster                                  |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.76 ms: 1.06x faster                                  |
| unpickle_pure_python     | 242 us                                                 | 230 us: 1.05x faster                                   |
| typing_runtime_protocols | 520 us                                                 | 493 us: 1.05x faster                                   |
| pyflate                  | 434 ms                                                 | 412 ms: 1.05x faster                                   |
| raytrace                 | 309 ms                                                 | 293 ms: 1.05x faster                                   |
| async_generators         | 374 ms                                                 | 356 ms: 1.05x faster                                   |
| json_dumps               | 13.3 ms                                                | 12.7 ms: 1.05x faster                                  |
| logging_simple           | 6.22 us                                                | 5.93 us: 1.05x faster                                  |
| nqueens                  | 87.9 ms                                                | 83.7 ms: 1.05x faster                                  |
| richards_super           | 61.9 ms                                                | 59.0 ms: 1.05x faster                                  |
| fannkuch                 | 405 ms                                                 | 387 ms: 1.05x faster                                   |
| spectral_norm            | 108 ms                                                 | 103 ms: 1.05x faster                                   |
| xml_etree_iterparse      | 108 ms                                                 | 103 ms: 1.05x faster                                   |
| pickle_pure_python       | 320 us                                                 | 306 us: 1.05x faster                                   |
| chaos                    | 71.9 ms                                                | 68.8 ms: 1.04x faster                                  |
| sqlglot_normalize        | 113 ms                                                 | 108 ms: 1.04x faster                                   |
| logging_format           | 6.81 us                                                | 6.52 us: 1.04x faster                                  |
| sqlglot_optimize         | 55.3 ms                                                | 53.0 ms: 1.04x faster                                  |
| sqlglot_parse            | 1.43 ms                                                | 1.37 ms: 1.04x faster                                  |
| float                    | 78.9 ms                                                | 75.7 ms: 1.04x faster                                  |
| regex_v8                 | 22.9 ms                                                | 21.9 ms: 1.04x faster                                  |
| coroutines               | 27.0 ms                                                | 25.9 ms: 1.04x faster                                  |
| sqlglot_transpile        | 1.75 ms                                                | 1.68 ms: 1.04x faster                                  |
| regex_compile            | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| scimark_fft              | 345 ms                                                 | 332 ms: 1.04x faster                                   |
| unpickle                 | 13.8 us                                                | 13.3 us: 1.04x faster                                  |
| richards                 | 49.8 ms                                                | 47.9 ms: 1.04x faster                                  |
| xml_etree_parse          | 164 ms                                                 | 158 ms: 1.04x faster                                   |
| generators               | 74.9 ms                                                | 72.2 ms: 1.04x faster                                  |
| nbody                    | 96.0 ms                                                | 92.6 ms: 1.04x faster                                  |
| sqlalchemy_imperative    | 18.3 ms                                                | 17.7 ms: 1.04x faster                                  |
| genshi_xml               | 53.4 ms                                                | 51.5 ms: 1.04x faster                                  |
| meteor_contest           | 109 ms                                                 | 105 ms: 1.04x faster                                   |
| thrift                   | 784 us                                                 | 757 us: 1.04x faster                                   |
| flaskblogging            | 7.28 ms                                                | 7.04 ms: 1.03x faster                                  |
| sympy_str                | 297 ms                                                 | 287 ms: 1.03x faster                                   |
| scimark_monte_carlo      | 70.7 ms                                                | 68.5 ms: 1.03x faster                                  |
| docutils                 | 2.66 sec                                               | 2.58 sec: 1.03x faster                                 |
| sympy_integrate          | 21.5 ms                                                | 20.8 ms: 1.03x faster                                  |
| crypto_pyaes             | 76.7 ms                                                | 74.4 ms: 1.03x faster                                  |
| scimark_sor              | 121 ms                                                 | 118 ms: 1.03x faster                                   |
| regex_dna                | 205 ms                                                 | 199 ms: 1.03x faster                                   |
| telco                    | 6.86 ms                                                | 6.66 ms: 1.03x faster                                  |
| 2to3                     | 264 ms                                                 | 257 ms: 1.03x faster                                   |
| djangocms                | 33.5 us                                                | 32.6 us: 1.03x faster                                  |
| sqlite_synth             | 2.57 us                                                | 2.50 us: 1.03x faster                                  |
| sympy_expand             | 484 ms                                                 | 471 ms: 1.03x faster                                   |
| genshi_text              | 22.5 ms                                                | 21.9 ms: 1.03x faster                                  |
| unpickle_list            | 5.21 us                                                | 5.08 us: 1.03x faster                                  |
| tomli_loads              | 2.30 sec                                               | 2.25 sec: 1.02x faster                                 |
| gunicorn                 | 1.20 ms                                                | 1.17 ms: 1.02x faster                                  |
| sympy_sum                | 169 ms                                                 | 165 ms: 1.02x faster                                   |
| pathlib                  | 18.5 ms                                                | 18.2 ms: 1.02x faster                                  |
| dask                     | 365 ms                                                 | 358 ms: 1.02x faster                                   |
| aiohttp                  | 1.12 ms                                                | 1.10 ms: 1.02x faster                                  |
| bench_thread_pool        | 834 us                                                 | 821 us: 1.02x faster                                   |
| django_template          | 33.5 ms                                                | 33.1 ms: 1.01x faster                                  |
| chameleon                | 6.70 ms                                                | 6.61 ms: 1.01x faster                                  |
| sqlalchemy_declarative   | 140 ms                                                 | 139 ms: 1.01x faster                                   |
| unpack_sequence          | 43.5 ns                                                | 42.9 ns: 1.01x faster                                  |
| tornado_http             | 98.1 ms                                                | 96.9 ms: 1.01x faster                                  |
| async_tree_memoization   | 639 ms                                                 | 632 ms: 1.01x faster                                   |
| async_tree_none          | 528 ms                                                 | 522 ms: 1.01x faster                                   |
| regex_effbot             | 3.51 ms                                                | 3.47 ms: 1.01x faster                                  |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 742 ms: 1.01x faster                                   |
| python_startup           | 8.56 ms                                                | 8.50 ms: 1.01x faster                                  |
| python_startup_no_site   | 6.01 ms                                                | 6.00 ms: 1.00x faster                                  |
| asyncio_tcp_ssl          | 3.11 sec                                               | 3.14 sec: 1.01x slower                                 |
| async_tree_io            | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| mdp                      | 2.77 sec                                               | 2.81 sec: 1.01x slower                                 |
| pidigits                 | 194 ms                                                 | 199 ms: 1.03x slower                                   |
| create_gc_cycles         | 1.43 ms                                                | 1.47 ms: 1.03x slower                                  |
| gc_traversal             | 4.01 ms                                                | 4.25 ms: 1.06x slower                                  |
| asyncio_tcp              | 875 ms                                                 | 934 ms: 1.07x slower                                   |
| Geometric mean           | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (5): html5lib, pylint, dulwich_log, bench_mp_pool, deltablue
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x