
# Results vs. 3.11.0

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.04x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.02x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 259 ms: 1.02x faster                                   |
| chameleon      | 6.70 ms                                                | 6.61 ms: 1.01x faster                                  |
| docutils       | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| tornado_http   | 98.1 ms                                                | 96.7 ms: 1.01x faster                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 749 ms                                                 | 740 ms: 1.01x faster                                   |
| async_tree_io           | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| Geometric mean          | (ref)                                                  | 1.00x faster                                           |

Benchmark hidden because not significant (2): async_tree_none, async_tree_memoization

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 78.9 ms                                                | 77.0 ms: 1.02x faster                                  |
| pidigits       | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.25 ms: 1.08x faster                                  |
| regex_v8       | 22.9 ms                                                | 21.8 ms: 1.05x faster                                  |
| regex_compile  | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| regex_dna      | 205 ms                                                 | 201 ms: 1.02x faster                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| json_loads           | 29.2 us                                                | 25.9 us: 1.13x faster                                  |
| pickle_dict          | 34.6 us                                                | 31.0 us: 1.12x faster                                  |
| pickle_list          | 4.59 us                                                | 4.12 us: 1.11x faster                                  |
| pickle               | 11.0 us                                                | 10.0 us: 1.10x faster                                  |
| xml_etree_generate   | 81.1 ms                                                | 76.2 ms: 1.06x faster                                  |
| xml_etree_process    | 56.9 ms                                                | 53.8 ms: 1.06x faster                                  |
| unpickle_pure_python | 242 us                                                 | 229 us: 1.06x faster                                   |
| json_dumps           | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| pickle_pure_python   | 320 us                                                 | 306 us: 1.05x faster                                   |
| unpickle_list        | 5.21 us                                                | 5.00 us: 1.04x faster                                  |
| unpickle             | 13.8 us                                                | 13.3 us: 1.04x faster                                  |
| tomli_loads          | 2.30 sec                                               | 2.22 sec: 1.04x faster                                 |
| xml_etree_parse      | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| xml_etree_iterparse  | 108 ms                                                 | 105 ms: 1.03x faster                                   |
| Geometric mean       | (ref)                                                  | 1.06x faster                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup         | 8.56 ms                                                | 8.56 ms: 1.00x slower                                  |
| python_startup_no_site | 6.01 ms                                                | 6.04 ms: 1.00x slower                                  |
| Geometric mean         | (ref)                                                  | 1.00x slower                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 10.7 ms                                                | 9.99 ms: 1.07x faster                                  |
| django_template | 33.5 ms                                                | 32.6 ms: 1.03x faster                                  |
| genshi_xml      | 53.4 ms                                                | 52.8 ms: 1.01x faster                                  |
| genshi_text     | 22.5 ms                                                | 22.3 ms: 1.01x faster                                  |
| Geometric mean  | (ref)                                                  | 1.03x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| logging_silent           | 111 ns                                                 | 98.6 ns: 1.13x faster                                  |
| json_loads               | 29.2 us                                                | 25.9 us: 1.13x faster                                  |
| pickle_dict              | 34.6 us                                                | 31.0 us: 1.12x faster                                  |
| pickle_list              | 4.59 us                                                | 4.12 us: 1.11x faster                                  |
| gc_traversal             | 4.01 ms                                                | 3.64 ms: 1.10x faster                                  |
| pickle                   | 11.0 us                                                | 10.0 us: 1.10x faster                                  |
| json                     | 5.24 ms                                                | 4.83 ms: 1.09x faster                                  |
| scimark_lu               | 116 ms                                                 | 107 ms: 1.08x faster                                   |
| hexiom                   | 6.89 ms                                                | 6.39 ms: 1.08x faster                                  |
| deepcopy_memo            | 40.2 us                                                | 37.2 us: 1.08x faster                                  |
| regex_effbot             | 3.51 ms                                                | 3.25 ms: 1.08x faster                                  |
| deepcopy_reduce          | 3.22 us                                                | 2.99 us: 1.08x faster                                  |
| pprint_pformat           | 1.55 sec                                               | 1.45 sec: 1.07x faster                                 |
| mdp                      | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| pprint_safe_repr         | 747 ms                                                 | 700 ms: 1.07x faster                                   |
| mako                     | 10.7 ms                                                | 9.99 ms: 1.07x faster                                  |
| scimark_sparse_mat_mult  | 5.03 ms                                                | 4.72 ms: 1.07x faster                                  |
| xml_etree_generate       | 81.1 ms                                                | 76.2 ms: 1.06x faster                                  |
| deltablue                | 3.92 ms                                                | 3.69 ms: 1.06x faster                                  |
| coroutines               | 27.0 ms                                                | 25.4 ms: 1.06x faster                                  |
| richards_super           | 61.9 ms                                                | 58.3 ms: 1.06x faster                                  |
| fannkuch                 | 405 ms                                                 | 383 ms: 1.06x faster                                   |
| richards                 | 49.8 ms                                                | 47.1 ms: 1.06x faster                                  |
| xml_etree_process        | 56.9 ms                                                | 53.8 ms: 1.06x faster                                  |
| unpickle_pure_python     | 242 us                                                 | 229 us: 1.06x faster                                   |
| json_dumps               | 13.3 ms                                                | 12.6 ms: 1.06x faster                                  |
| go                       | 149 ms                                                 | 141 ms: 1.06x faster                                   |
| typing_runtime_protocols | 520 us                                                 | 493 us: 1.05x faster                                   |
| regex_v8                 | 22.9 ms                                                | 21.8 ms: 1.05x faster                                  |
| scimark_fft              | 345 ms                                                 | 329 ms: 1.05x faster                                   |
| logging_simple           | 6.22 us                                                | 5.93 us: 1.05x faster                                  |
| chaos                    | 71.9 ms                                                | 68.5 ms: 1.05x faster                                  |
| pickle_pure_python       | 320 us                                                 | 306 us: 1.05x faster                                   |
| pycparser                | 1.19 sec                                               | 1.13 sec: 1.05x faster                                 |
| sqlglot_transpile        | 1.75 ms                                                | 1.67 ms: 1.05x faster                                  |
| raytrace                 | 309 ms                                                 | 295 ms: 1.04x faster                                   |
| nqueens                  | 87.9 ms                                                | 84.2 ms: 1.04x faster                                  |
| sqlglot_optimize         | 55.3 ms                                                | 53.0 ms: 1.04x faster                                  |
| unpickle_list            | 5.21 us                                                | 5.00 us: 1.04x faster                                  |
| sqlglot_parse            | 1.43 ms                                                | 1.37 ms: 1.04x faster                                  |
| comprehensions           | 23.6 us                                                | 22.7 us: 1.04x faster                                  |
| deepcopy                 | 365 us                                                 | 351 us: 1.04x faster                                   |
| spectral_norm            | 108 ms                                                 | 104 ms: 1.04x faster                                   |
| unpickle                 | 13.8 us                                                | 13.3 us: 1.04x faster                                  |
| sqlglot_normalize        | 113 ms                                                 | 108 ms: 1.04x faster                                   |
| logging_format           | 6.81 us                                                | 6.55 us: 1.04x faster                                  |
| meteor_contest           | 109 ms                                                 | 105 ms: 1.04x faster                                   |
| telco                    | 6.86 ms                                                | 6.60 ms: 1.04x faster                                  |
| pylint                   | 476 ms                                                 | 458 ms: 1.04x faster                                   |
| crypto_pyaes             | 76.7 ms                                                | 73.9 ms: 1.04x faster                                  |
| regex_compile            | 141 ms                                                 | 136 ms: 1.04x faster                                   |
| pyflate                  | 434 ms                                                 | 419 ms: 1.04x faster                                   |
| tomli_loads              | 2.30 sec                                               | 2.22 sec: 1.04x faster                                 |
| async_generators         | 374 ms                                                 | 361 ms: 1.04x faster                                   |
| scimark_sor              | 121 ms                                                 | 117 ms: 1.03x faster                                   |
| xml_etree_parse          | 164 ms                                                 | 159 ms: 1.03x faster                                   |
| django_template          | 33.5 ms                                                | 32.6 ms: 1.03x faster                                  |
| scimark_monte_carlo      | 70.7 ms                                                | 68.8 ms: 1.03x faster                                  |
| docutils                 | 2.66 sec                                               | 2.59 sec: 1.03x faster                                 |
| thrift                   | 784 us                                                 | 763 us: 1.03x faster                                   |
| xml_etree_iterparse      | 108 ms                                                 | 105 ms: 1.03x faster                                   |
| sqlalchemy_imperative    | 18.3 ms                                                | 17.9 ms: 1.03x faster                                  |
| pathlib                  | 18.5 ms                                                | 18.1 ms: 1.03x faster                                  |
| float                    | 78.9 ms                                                | 77.0 ms: 1.02x faster                                  |
| pidigits                 | 194 ms                                                 | 190 ms: 1.02x faster                                   |
| sympy_str                | 297 ms                                                 | 291 ms: 1.02x faster                                   |
| 2to3                     | 264 ms                                                 | 259 ms: 1.02x faster                                   |
| bench_thread_pool        | 834 us                                                 | 818 us: 1.02x faster                                   |
| flaskblogging            | 7.28 ms                                                | 7.14 ms: 1.02x faster                                  |
| sqlite_synth             | 2.57 us                                                | 2.52 us: 1.02x faster                                  |
| djangocms                | 33.5 us                                                | 32.9 us: 1.02x faster                                  |
| sympy_integrate          | 21.5 ms                                                | 21.1 ms: 1.02x faster                                  |
| regex_dna                | 205 ms                                                 | 201 ms: 1.02x faster                                   |
| sympy_expand             | 484 ms                                                 | 476 ms: 1.02x faster                                   |
| generators               | 74.9 ms                                                | 73.8 ms: 1.01x faster                                  |
| tornado_http             | 98.1 ms                                                | 96.7 ms: 1.01x faster                                  |
| dask                     | 365 ms                                                 | 360 ms: 1.01x faster                                   |
| chameleon                | 6.70 ms                                                | 6.61 ms: 1.01x faster                                  |
| asyncio_tcp              | 875 ms                                                 | 864 ms: 1.01x faster                                   |
| genshi_xml               | 53.4 ms                                                | 52.8 ms: 1.01x faster                                  |
| async_tree_cpu_io_mixed  | 749 ms                                                 | 740 ms: 1.01x faster                                   |
| genshi_text              | 22.5 ms                                                | 22.3 ms: 1.01x faster                                  |
| dulwich_log              | 64.6 ms                                                | 63.8 ms: 1.01x faster                                  |
| aiohttp                  | 1.12 ms                                                | 1.10 ms: 1.01x faster                                  |
| sympy_sum                | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| gunicorn                 | 1.20 ms                                                | 1.19 ms: 1.00x faster                                  |
| python_startup           | 8.56 ms                                                | 8.56 ms: 1.00x slower                                  |
| python_startup_no_site   | 6.01 ms                                                | 6.04 ms: 1.00x slower                                  |
| unpack_sequence          | 43.5 ns                                                | 43.9 ns: 1.01x slower                                  |
| async_tree_io            | 1.29 sec                                               | 1.30 sec: 1.01x slower                                 |
| asyncio_tcp_ssl          | 3.11 sec                                               | 3.18 sec: 1.02x slower                                 |
| create_gc_cycles         | 1.43 ms                                                | 1.48 ms: 1.04x slower                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                           |

Benchmark hidden because not significant (6): html5lib, sqlalchemy_declarative, async_tree_none, nbody, bench_mp_pool, async_tree_memoization
Ignored benchmarks (7) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.02x