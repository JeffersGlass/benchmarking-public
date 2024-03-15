
# Results vs. 3.10.4

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: linux-x86_64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.31x faster
- Memory change: 1.08x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 249 ms: 1.40x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.51 ms: 1.49x faster                                                 |
| docutils       | 3.30 sec                                               | 2.52 sec: 1.31x faster                                                |
| html5lib       | 88.9 ms                                                | 59.9 ms: 1.48x faster                                                 |
| tornado_http   | 136 ms                                                 | 93.7 ms: 1.46x faster                                                 |
| Geometric mean | (ref)                                                  | 1.43x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 1.02 sec                                               | 730 ms: 1.39x faster                                                  |
| async_tree_none         | 728 ms                                                 | 529 ms: 1.38x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.33 sec: 1.33x faster                                                |
| async_tree_memoization  | 870 ms                                                 | 656 ms: 1.33x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| float          | 117 ms                                                 | 71.4 ms: 1.64x faster                                                 |
| nbody          | 154 ms                                                 | 96.6 ms: 1.59x faster                                                 |
| pidigits       | 191 ms                                                 | 198 ms: 1.04x slower                                                  |
| Geometric mean | (ref)                                                  | 1.36x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 127 ms: 1.48x faster                                                  |
| regex_v8       | 27.8 ms                                                | 21.4 ms: 1.30x faster                                                 |
| regex_dna      | 227 ms                                                 | 201 ms: 1.13x faster                                                  |
| regex_effbot   | 3.63 ms                                                | 3.37 ms: 1.08x faster                                                 |
| Geometric mean | (ref)                                                  | 1.24x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 285 us: 1.70x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 202 us: 1.64x faster                                                  |
| json_dumps           | 14.2 ms                                                | 9.36 ms: 1.51x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 53.4 ms: 1.48x faster                                                 |
| json_loads           | 31.2 us                                                | 23.5 us: 1.33x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 76.0 ms: 1.31x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.19 us: 1.21x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 145 ms: 1.16x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 101 ms: 1.15x faster                                                  |
| unpickle             | 14.4 us                                                | 13.2 us: 1.09x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.91 us: 1.06x faster                                                 |
| pickle               | 10.7 us                                                | 10.1 us: 1.05x faster                                                 |
| pickle_dict          | 29.6 us                                                | 31.1 us: 1.05x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.26x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.42 ms: 1.73x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 5.93 ms: 1.00x faster                                                 |
| Geometric mean         | (ref)                                                  | 1.32x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.64 ms: 1.69x faster                                                 |
| genshi_text     | 31.8 ms                                                | 21.5 ms: 1.48x faster                                                 |
| django_template | 48.2 ms                                                | 33.0 ms: 1.46x faster                                                 |
| genshi_xml      | 66.0 ms                                                | 50.0 ms: 1.32x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.48x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-linux-x86_64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.30 ms: 2.40x faster                                                 |
| scimark_sor             | 220 ms                                                 | 106 ms: 2.08x faster                                                  |
| logging_silent          | 190 ns                                                 | 91.6 ns: 2.07x faster                                                 |
| richards                | 79.3 ms                                                | 42.4 ms: 1.87x faster                                                 |
| raytrace                | 507 ms                                                 | 282 ms: 1.79x faster                                                  |
| spectral_norm           | 170 ms                                                 | 95.2 ms: 1.78x faster                                                 |
| go                      | 240 ms                                                 | 135 ms: 1.78x faster                                                  |
| scimark_monte_carlo     | 118 ms                                                 | 66.6 ms: 1.77x faster                                                 |
| pyflate                 | 716 ms                                                 | 407 ms: 1.76x faster                                                  |
| python_startup          | 14.6 ms                                                | 8.42 ms: 1.73x faster                                                 |
| chaos                   | 115 ms                                                 | 67.1 ms: 1.72x faster                                                 |
| crypto_pyaes            | 128 ms                                                 | 74.8 ms: 1.71x faster                                                 |
| hexiom                  | 10.4 ms                                                | 6.11 ms: 1.70x faster                                                 |
| deepcopy_memo           | 58.5 us                                                | 34.4 us: 1.70x faster                                                 |
| pickle_pure_python      | 484 us                                                 | 285 us: 1.70x faster                                                  |
| mako                    | 16.3 ms                                                | 9.64 ms: 1.69x faster                                                 |
| float                   | 117 ms                                                 | 71.4 ms: 1.64x faster                                                 |
| unpickle_pure_python    | 331 us                                                 | 202 us: 1.64x faster                                                  |
| scimark_lu              | 176 ms                                                 | 108 ms: 1.62x faster                                                  |
| sqlglot_parse           | 2.17 ms                                                | 1.34 ms: 1.62x faster                                                 |
| nbody                   | 154 ms                                                 | 96.6 ms: 1.59x faster                                                 |
| sqlglot_transpile       | 2.57 ms                                                | 1.63 ms: 1.58x faster                                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.13 ms: 1.57x faster                                                 |
| pprint_safe_repr        | 1.02 sec                                               | 665 ms: 1.53x faster                                                  |
| pprint_pformat          | 2.10 sec                                               | 1.38 sec: 1.53x faster                                                |
| json_dumps              | 14.2 ms                                                | 9.36 ms: 1.51x faster                                                 |
| scimark_fft             | 466 ms                                                 | 312 ms: 1.49x faster                                                  |
| chameleon               | 9.68 ms                                                | 6.51 ms: 1.49x faster                                                 |
| genshi_text             | 31.8 ms                                                | 21.5 ms: 1.48x faster                                                 |
| html5lib                | 88.9 ms                                                | 59.9 ms: 1.48x faster                                                 |
| xml_etree_process       | 79.1 ms                                                | 53.4 ms: 1.48x faster                                                 |
| regex_compile           | 188 ms                                                 | 127 ms: 1.48x faster                                                  |
| django_template         | 48.2 ms                                                | 33.0 ms: 1.46x faster                                                 |
| tornado_http            | 136 ms                                                 | 93.7 ms: 1.46x faster                                                 |
| deepcopy                | 479 us                                                 | 333 us: 1.44x faster                                                  |
| fannkuch                | 532 ms                                                 | 370 ms: 1.44x faster                                                  |
| thrift                  | 1.07 ms                                                | 746 us: 1.44x faster                                                  |
| deepcopy_reduce         | 4.17 us                                                | 2.91 us: 1.44x faster                                                 |
| aiohttp                 | 1.44 ms                                                | 1.00 ms: 1.43x faster                                                 |
| logging_simple          | 8.30 us                                                | 5.80 us: 1.43x faster                                                 |
| gunicorn                | 1.53 ms                                                | 1.07 ms: 1.43x faster                                                 |
| logging_format          | 9.09 us                                                | 6.38 us: 1.42x faster                                                 |
| coroutines              | 35.1 ms                                                | 24.7 ms: 1.42x faster                                                 |
| pycparser               | 1.58 sec                                               | 1.12 sec: 1.41x faster                                                |
| 2to3                    | 348 ms                                                 | 249 ms: 1.40x faster                                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 730 ms: 1.39x faster                                                  |
| async_tree_none         | 728 ms                                                 | 529 ms: 1.38x faster                                                  |
| sqlglot_normalize       | 143 ms                                                 | 104 ms: 1.37x faster                                                  |
| unpack_sequence         | 60.0 ns                                                | 44.1 ns: 1.36x faster                                                 |
| dulwich_log             | 84.3 ms                                                | 62.4 ms: 1.35x faster                                                 |
| sqlglot_optimize        | 69.2 ms                                                | 51.2 ms: 1.35x faster                                                 |
| comprehensions          | 28.8 us                                                | 21.3 us: 1.35x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.33 sec: 1.33x faster                                                |
| json_loads              | 31.2 us                                                | 23.5 us: 1.33x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 656 ms: 1.33x faster                                                  |
| genshi_xml              | 66.0 ms                                                | 50.0 ms: 1.32x faster                                                 |
| nqueens                 | 106 ms                                                 | 80.7 ms: 1.31x faster                                                 |
| docutils                | 3.30 sec                                               | 2.52 sec: 1.31x faster                                                |
| xml_etree_generate      | 99.4 ms                                                | 76.0 ms: 1.31x faster                                                 |
| regex_v8                | 27.8 ms                                                | 21.4 ms: 1.30x faster                                                 |
| async_generators        | 444 ms                                                 | 349 ms: 1.27x faster                                                  |
| bench_thread_pool       | 986 us                                                 | 780 us: 1.26x faster                                                  |
| sympy_integrate         | 25.8 ms                                                | 20.4 ms: 1.26x faster                                                 |
| json                    | 5.69 ms                                                | 4.55 ms: 1.25x faster                                                 |
| sympy_expand            | 566 ms                                                 | 455 ms: 1.24x faster                                                  |
| dask                    | 441 ms                                                 | 360 ms: 1.22x faster                                                  |
| sympy_str               | 346 ms                                                 | 283 ms: 1.22x faster                                                  |
| pickle_list             | 5.08 us                                                | 4.19 us: 1.21x faster                                                 |
| pylint                  | 551 ms                                                 | 458 ms: 1.20x faster                                                  |
| sympy_sum               | 196 ms                                                 | 164 ms: 1.20x faster                                                  |
| djangocms               | 38.4 us                                                | 32.5 us: 1.18x faster                                                 |
| xml_etree_parse         | 168 ms                                                 | 145 ms: 1.16x faster                                                  |
| sqlite_synth            | 3.02 us                                                | 2.62 us: 1.15x faster                                                 |
| meteor_contest          | 120 ms                                                 | 104 ms: 1.15x faster                                                  |
| xml_etree_iterparse     | 115 ms                                                 | 101 ms: 1.15x faster                                                  |
| mdp                     | 2.85 sec                                               | 2.48 sec: 1.15x faster                                                |
| pathlib                 | 20.5 ms                                                | 17.9 ms: 1.14x faster                                                 |
| regex_dna               | 227 ms                                                 | 201 ms: 1.13x faster                                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                 |
| telco                   | 7.27 ms                                                | 6.55 ms: 1.11x faster                                                 |
| unpickle                | 14.4 us                                                | 13.2 us: 1.09x faster                                                 |
| generators              | 80.1 ms                                                | 74.1 ms: 1.08x faster                                                 |
| regex_effbot            | 3.63 ms                                                | 3.37 ms: 1.08x faster                                                 |
| unpickle_list           | 5.20 us                                                | 4.91 us: 1.06x faster                                                 |
| pickle                  | 10.7 us                                                | 10.1 us: 1.05x faster                                                 |
| asyncio_tcp             | 922 ms                                                 | 890 ms: 1.04x faster                                                  |
| gc_traversal            | 3.62 ms                                                | 3.55 ms: 1.02x faster                                                 |
| python_startup_no_site  | 5.93 ms                                                | 5.93 ms: 1.00x faster                                                 |
| pidigits                | 191 ms                                                 | 198 ms: 1.04x slower                                                  |
| pickle_dict             | 29.6 us                                                | 31.1 us: 1.05x slower                                                 |
| coverage                | 79.4 ms                                                | 102 ms: 1.28x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.37x faster                                                          |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.34x
- 95% likely to have a speedup of 1.33x
- 99% likely to have a speedup of 1.31x


# Memory

- memory change: 1.08x