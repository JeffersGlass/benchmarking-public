
# Results vs. 3.11.0

- fork: python
- ref: v3.11.4
- machine: linux-x86_64
- commit hash: d2340ef
- commit date: 2023-06-06
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 258 ms: 1.02x faster                                   |
| chameleon      | 6.70 ms                                                | 6.58 ms: 1.02x faster                                  |
| docutils       | 2.66 sec                                               | 2.57 sec: 1.04x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.6 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 738 ms: 1.01x faster                                   |
| async_tree_none         | 528 ms                                                 | 523 ms: 1.01x faster                                   |
| Geometric mean          | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 78.9 ms                                                | 77.1 ms: 1.02x faster                                  |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| nbody          | 96.0 ms                                                | 99.4 ms: 1.04x slower                                  |
| Geometric mean | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| regex_v8       | 22.9 ms                                                | 22.2 ms: 1.03x faster                                  |
| regex_dna      | 205 ms                                                 | 200 ms: 1.02x faster                                   |
| regex_effbot   | 3.51 ms                                                | 3.45 ms: 1.02x faster                                  |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 4.59 us                                                | 4.01 us: 1.14x faster                                  |
| pickle               | 11.0 us                                                | 9.76 us: 1.13x faster                                  |
| pickle_dict          | 34.6 us                                                | 30.7 us: 1.13x faster                                  |
| json_loads           | 29.2 us                                                | 26.2 us: 1.11x faster                                  |
| pickle_pure_python   | 320 us                                                 | 302 us: 1.06x faster                                   |
| unpickle             | 13.8 us                                                | 13.1 us: 1.06x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 76.5 ms: 1.06x faster                                  |
| json_dumps           | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                   |
| xml_etree_process    | 56.9 ms                                                | 53.9 ms: 1.05x faster                                  |
| tomli_loads          | 2.30 sec                                               | 2.19 sec: 1.05x faster                                 |
| unpickle_list        | 5.21 us                                                | 5.02 us: 1.04x faster                                  |
| xml_etree_iterparse  | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| xml_etree_parse      | 164 ms                                                 | 160 ms: 1.03x faster                                   |
| Geometric mean       | (ref)                                                  | 1.07x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.53 ms: 1.00x faster                                  |
| python_startup_no_site | 6.01 ms                                                | 6.01 ms: 1.00x faster                                  |
| Geometric mean         | (ref)                                                  | 1.00x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.80 ms: 1.09x faster                                  |
| genshi_xml      | 53.4 ms                                                | 51.8 ms: 1.03x faster                                  |
| django_template | 33.5 ms                                                | 33.0 ms: 1.02x faster                                  |
| genshi_text     | 22.5 ms                                                | 22.4 ms: 1.01x faster                                  |
| Geometric mean  | (ref)                                                  | 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230606-linux-x86_64-python-v3.11.4-3.11.4-d2340ef |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list              | 4.59 us                                                | 4.01 us: 1.14x faster                                  |
| pickle                   | 11.0 us                                                | 9.76 us: 1.13x faster                                  |
| pickle_dict              | 34.6 us                                                | 30.7 us: 1.13x faster                                  |
| spectral_norm            | 108 ms                                                 | 97.1 ms: 1.11x faster                                  |
| json_loads               | 29.2 us                                                | 26.2 us: 1.11x faster                                  |
| deepcopy_memo            | 40.2 us                                                | 36.5 us: 1.10x faster                                  |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.58 ms: 1.10x faster                                  |
| deepcopy_reduce          | 3.22 us                                                | 2.94 us: 1.09x faster                                  |
| mako                     | 10.7 ms                                                | 9.80 ms: 1.09x faster                                  |
| json                     | 5.24 ms                                                | 4.85 ms: 1.08x faster                                  |
| logging_silent           | 111 ns                                                 | 103 ns: 1.08x faster                                   |
| pprint_pformat           | 1.55 sec                                               | 1.45 sec: 1.07x faster                                 |
| deepcopy                 | 365 us                                                 | 341 us: 1.07x faster                                   |
| mdp                      | 2.77 sec                                               | 2.60 sec: 1.07x faster                                 |
| scimark_lu               | 116 ms                                                 | 109 ms: 1.07x faster                                   |
| go                       | 149 ms                                                 | 140 ms: 1.06x faster                                   |
| scimark_fft              | 345 ms                                                 | 326 ms: 1.06x faster                                   |
| hexiom                   | 6.89 ms                                                | 6.50 ms: 1.06x faster                                  |
| pickle_pure_python       | 320 us                                                 | 302 us: 1.06x faster                                   |
| unpickle                 | 13.8 us                                                | 13.1 us: 1.06x faster                                  |
| xml_etree_generate       | 81.1 ms                                                | 76.5 ms: 1.06x faster                                  |
| json_dumps               | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| deltablue                | 3.92 ms                                                | 3.71 ms: 1.06x faster                                  |
| nqueens                  | 87.9 ms                                                | 83.1 ms: 1.06x faster                                  |
| pprint_safe_repr         | 747 ms                                                 | 707 ms: 1.06x faster                                   |
| unpickle_pure_python     | 242 us                                                 | 229 us: 1.06x faster                                   |
| xml_etree_process        | 56.9 ms                                                | 53.9 ms: 1.05x faster                                  |
| tomli_loads              | 2.30 sec                                               | 2.19 sec: 1.05x faster                                 |
| typing_runtime_protocols | 520 us                                                 | 495 us: 1.05x faster                                   |
| sqlglot_transpile        | 1.75 ms                                                | 1.67 ms: 1.05x faster                                  |
| raytrace                 | 309 ms                                                 | 294 ms: 1.05x faster                                   |
| comprehensions           | 23.6 us                                                | 22.6 us: 1.05x faster                                  |
| sqlglot_parse            | 1.43 ms                                                | 1.37 ms: 1.05x faster                                  |
| scimark_monte_carlo      | 70.7 ms                                                | 67.7 ms: 1.04x faster                                  |
| coroutines               | 27.0 ms                                                | 25.9 ms: 1.04x faster                                  |
| sqlglot_optimize         | 55.3 ms                                                | 53.0 ms: 1.04x faster                                  |
| sqlglot_normalize        | 113 ms                                                 | 108 ms: 1.04x faster                                   |
| regex_compile            | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| unpickle_list            | 5.21 us                                                | 5.02 us: 1.04x faster                                  |
| docutils                 | 2.66 sec                                               | 2.57 sec: 1.04x faster                                 |
| xml_etree_iterparse      | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| logging_format           | 6.81 us                                                | 6.58 us: 1.04x faster                                  |
| async_generators         | 374 ms                                                 | 361 ms: 1.04x faster                                   |
| telco                    | 6.86 ms                                                | 6.62 ms: 1.04x faster                                  |
| scimark_sor              | 121 ms                                                 | 118 ms: 1.03x faster                                   |
| genshi_xml               | 53.4 ms                                                | 51.8 ms: 1.03x faster                                  |
| pathlib                  | 18.5 ms                                                | 18.0 ms: 1.03x faster                                  |
| richards_super           | 61.9 ms                                                | 60.0 ms: 1.03x faster                                  |
| sympy_expand             | 484 ms                                                 | 470 ms: 1.03x faster                                   |
| regex_v8                 | 22.9 ms                                                | 22.2 ms: 1.03x faster                                  |
| pylint                   | 476 ms                                                 | 462 ms: 1.03x faster                                   |
| pyflate                  | 434 ms                                                 | 421 ms: 1.03x faster                                   |
| meteor_contest           | 109 ms                                                 | 106 ms: 1.03x faster                                   |
| crypto_pyaes             | 76.7 ms                                                | 74.6 ms: 1.03x faster                                  |
| fannkuch                 | 405 ms                                                 | 394 ms: 1.03x faster                                   |
| sympy_integrate          | 21.5 ms                                                | 20.9 ms: 1.03x faster                                  |
| sqlite_synth             | 2.57 us                                                | 2.51 us: 1.03x faster                                  |
| sqlalchemy_imperative    | 18.3 ms                                                | 17.9 ms: 1.03x faster                                  |
| xml_etree_parse          | 164 ms                                                 | 160 ms: 1.03x faster                                   |
| sympy_str                | 297 ms                                                 | 290 ms: 1.03x faster                                   |
| richards                 | 49.8 ms                                                | 48.5 ms: 1.03x faster                                  |
| 2to3                     | 264 ms                                                 | 258 ms: 1.02x faster                                   |
| float                    | 78.9 ms                                                | 77.1 ms: 1.02x faster                                  |
| pidigits                 | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| gunicorn                 | 1.20 ms                                                | 1.17 ms: 1.02x faster                                  |
| chaos                    | 71.9 ms                                                | 70.2 ms: 1.02x faster                                  |
| bench_thread_pool        | 834 us                                                 | 816 us: 1.02x faster                                   |
| regex_dna                | 205 ms                                                 | 200 ms: 1.02x faster                                   |
| logging_simple           | 6.22 us                                                | 6.09 us: 1.02x faster                                  |
| aiohttp                  | 1.12 ms                                                | 1.09 ms: 1.02x faster                                  |
| chameleon                | 6.70 ms                                                | 6.58 ms: 1.02x faster                                  |
| sympy_sum                | 169 ms                                                 | 166 ms: 1.02x faster                                   |
| thrift                   | 784 us                                                 | 771 us: 1.02x faster                                   |
| regex_effbot             | 3.51 ms                                                | 3.45 ms: 1.02x faster                                  |
| generators               | 74.9 ms                                                | 73.7 ms: 1.02x faster                                  |
| flaskblogging            | 7.28 ms                                                | 7.17 ms: 1.02x faster                                  |
| tornado_http             | 98.1 ms                                                | 96.6 ms: 1.02x faster                                  |
| django_template          | 33.5 ms                                                | 33.0 ms: 1.02x faster                                  |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 738 ms: 1.01x faster                                   |
| dask                     | 365 ms                                                 | 360 ms: 1.01x faster                                   |
| sqlalchemy_declarative   | 140 ms                                                 | 139 ms: 1.01x faster                                   |
| async_tree_none          | 528 ms                                                 | 523 ms: 1.01x faster                                   |
| genshi_text              | 22.5 ms                                                | 22.4 ms: 1.01x faster                                  |
| python_startup           | 8.56 ms                                                | 8.53 ms: 1.00x faster                                  |
| python_startup_no_site   | 6.01 ms                                                | 6.01 ms: 1.00x faster                                  |
| gc_traversal             | 4.01 ms                                                | 4.04 ms: 1.01x slower                                  |
| asyncio_tcp_ssl          | 3.11 sec                                               | 3.15 sec: 1.01x slower                                 |
| dulwich_log              | 64.6 ms                                                | 65.5 ms: 1.01x slower                                  |
| nbody                    | 96.0 ms                                                | 99.4 ms: 1.04x slower                                  |
| create_gc_cycles         | 1.43 ms                                                | 1.49 ms: 1.04x slower                                  |
| asyncio_tcp              | 875 ms                                                 | 922 ms: 1.05x slower                                   |
| Geometric mean           | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (7): djangocms, html5lib, pycparser, async_tree_memoization, bench_mp_pool, unpack_sequence, async_tree_io
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x