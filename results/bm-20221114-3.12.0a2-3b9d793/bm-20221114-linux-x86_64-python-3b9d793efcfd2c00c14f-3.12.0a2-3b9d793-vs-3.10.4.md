
# Results vs. 3.10.4

- fork: python
- ref: 3b9d793efcfd2c00c14f
- machine: linux-x86_64
- commit hash: 3b9d793
- commit date: 2022-11-14
- overall geometric mean: 1.38x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.32x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 245 ms: 1.42x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.30 ms: 1.54x faster                                                 |
| docutils       | 3.30 sec                                               | 2.50 sec: 1.32x faster                                                |
| html5lib       | 88.9 ms                                                | 58.9 ms: 1.51x faster                                                 |
| tornado_http   | 136 ms                                                 | 93.1 ms: 1.46x faster                                                 |
| Geometric mean | (ref)                                                  | 1.45x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 1.02 sec                                               | 730 ms: 1.39x faster                                                  |
| async_tree_none         | 728 ms                                                 | 527 ms: 1.38x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.32 sec: 1.34x faster                                                |
| async_tree_memoization  | 870 ms                                                 | 653 ms: 1.33x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.9 ms: 1.63x faster                                                 |
| float          | 117 ms                                                 | 72.0 ms: 1.63x faster                                                 |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.39x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 127 ms: 1.49x faster                                                  |
| regex_v8       | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                 |
| regex_dna      | 227 ms                                                 | 208 ms: 1.09x faster                                                  |
| regex_effbot   | 3.63 ms                                                | 3.47 ms: 1.05x faster                                                 |
| Geometric mean | (ref)                                                  | 1.22x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 283 us: 1.71x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 200 us: 1.66x faster                                                  |
| json_dumps           | 14.2 ms                                                | 9.66 ms: 1.47x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 53.9 ms: 1.47x faster                                                 |
| json_loads           | 31.2 us                                                | 23.9 us: 1.31x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 77.2 ms: 1.29x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.06 us: 1.25x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 149 ms: 1.13x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                                  |
| unpickle             | 14.4 us                                                | 12.9 us: 1.11x faster                                                 |
| pickle               | 10.7 us                                                | 9.88 us: 1.08x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.98 us: 1.04x faster                                                 |
| pickle_dict          | 29.6 us                                                | 30.8 us: 1.04x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.26x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.58 ms: 1.70x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 6.12 ms: 1.03x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.28x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.39 ms: 1.74x faster                                                 |
| genshi_text     | 31.8 ms                                                | 20.2 ms: 1.58x faster                                                 |
| django_template | 48.2 ms                                                | 32.8 ms: 1.47x faster                                                 |
| genshi_xml      | 66.0 ms                                                | 47.0 ms: 1.41x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.54x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221114-linux-x86_64-python-3b9d793efcfd2c00c14f-3.12.0a2-3b9d793 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.22 ms: 2.46x faster                                                 |
| scimark_sor             | 220 ms                                                 | 105 ms: 2.09x faster                                                  |
| logging_silent          | 190 ns                                                 | 93.4 ns: 2.03x faster                                                 |
| richards                | 79.3 ms                                                | 41.8 ms: 1.89x faster                                                 |
| raytrace                | 507 ms                                                 | 277 ms: 1.83x faster                                                  |
| spectral_norm           | 170 ms                                                 | 94.9 ms: 1.79x faster                                                 |
| go                      | 240 ms                                                 | 135 ms: 1.78x faster                                                  |
| pyflate                 | 716 ms                                                 | 402 ms: 1.78x faster                                                  |
| chaos                   | 115 ms                                                 | 65.8 ms: 1.75x faster                                                 |
| mako                    | 16.3 ms                                                | 9.39 ms: 1.74x faster                                                 |
| scimark_monte_carlo     | 118 ms                                                 | 68.0 ms: 1.74x faster                                                 |
| deepcopy_memo           | 58.5 us                                                | 33.6 us: 1.74x faster                                                 |
| hexiom                  | 10.4 ms                                                | 6.04 ms: 1.72x faster                                                 |
| crypto_pyaes            | 128 ms                                                 | 74.6 ms: 1.71x faster                                                 |
| pickle_pure_python      | 484 us                                                 | 283 us: 1.71x faster                                                  |
| python_startup          | 14.6 ms                                                | 8.58 ms: 1.70x faster                                                 |
| unpickle_pure_python    | 331 us                                                 | 200 us: 1.66x faster                                                  |
| nbody                   | 154 ms                                                 | 93.9 ms: 1.63x faster                                                 |
| sqlglot_parse           | 2.17 ms                                                | 1.33 ms: 1.63x faster                                                 |
| scimark_lu              | 176 ms                                                 | 108 ms: 1.63x faster                                                  |
| float                   | 117 ms                                                 | 72.0 ms: 1.63x faster                                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.00 ms: 1.62x faster                                                 |
| sqlglot_transpile       | 2.57 ms                                                | 1.62 ms: 1.59x faster                                                 |
| genshi_text             | 31.8 ms                                                | 20.2 ms: 1.58x faster                                                 |
| chameleon               | 9.68 ms                                                | 6.30 ms: 1.54x faster                                                 |
| pprint_pformat          | 2.10 sec                                               | 1.39 sec: 1.51x faster                                                |
| scimark_fft             | 466 ms                                                 | 309 ms: 1.51x faster                                                  |
| html5lib                | 88.9 ms                                                | 58.9 ms: 1.51x faster                                                 |
| pprint_safe_repr        | 1.02 sec                                               | 685 ms: 1.49x faster                                                  |
| regex_compile           | 188 ms                                                 | 127 ms: 1.49x faster                                                  |
| django_template         | 48.2 ms                                                | 32.8 ms: 1.47x faster                                                 |
| json_dumps              | 14.2 ms                                                | 9.66 ms: 1.47x faster                                                 |
| xml_etree_process       | 79.1 ms                                                | 53.9 ms: 1.47x faster                                                 |
| pycparser               | 1.58 sec                                               | 1.08 sec: 1.46x faster                                                |
| tornado_http            | 136 ms                                                 | 93.1 ms: 1.46x faster                                                 |
| deepcopy                | 479 us                                                 | 328 us: 1.46x faster                                                  |
| logging_simple          | 8.30 us                                                | 5.70 us: 1.46x faster                                                 |
| deepcopy_reduce         | 4.17 us                                                | 2.89 us: 1.44x faster                                                 |
| logging_format          | 9.09 us                                                | 6.30 us: 1.44x faster                                                 |
| fannkuch                | 532 ms                                                 | 369 ms: 1.44x faster                                                  |
| aiohttp                 | 1.44 ms                                                | 999 us: 1.44x faster                                                  |
| thrift                  | 1.07 ms                                                | 748 us: 1.43x faster                                                  |
| gunicorn                | 1.53 ms                                                | 1.08 ms: 1.42x faster                                                 |
| 2to3                    | 348 ms                                                 | 245 ms: 1.42x faster                                                  |
| coroutines              | 35.1 ms                                                | 24.7 ms: 1.42x faster                                                 |
| genshi_xml              | 66.0 ms                                                | 47.0 ms: 1.41x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 730 ms: 1.39x faster                                                  |
| async_tree_none         | 728 ms                                                 | 527 ms: 1.38x faster                                                  |
| dulwich_log             | 84.3 ms                                                | 61.8 ms: 1.36x faster                                                 |
| sqlglot_optimize        | 69.2 ms                                                | 51.0 ms: 1.36x faster                                                 |
| sqlglot_normalize       | 143 ms                                                 | 105 ms: 1.36x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.32 sec: 1.34x faster                                                |
| async_tree_memoization  | 870 ms                                                 | 653 ms: 1.33x faster                                                  |
| docutils                | 3.30 sec                                               | 2.50 sec: 1.32x faster                                                |
| regex_v8                | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                 |
| unpack_sequence         | 60.0 ns                                                | 45.7 ns: 1.31x faster                                                 |
| json_loads              | 31.2 us                                                | 23.9 us: 1.31x faster                                                 |
| nqueens                 | 106 ms                                                 | 81.1 ms: 1.30x faster                                                 |
| xml_etree_generate      | 99.4 ms                                                | 77.2 ms: 1.29x faster                                                 |
| sympy_integrate         | 25.8 ms                                                | 20.4 ms: 1.27x faster                                                 |
| bench_thread_pool       | 986 us                                                 | 780 us: 1.26x faster                                                  |
| async_generators        | 444 ms                                                 | 355 ms: 1.25x faster                                                  |
| pickle_list             | 5.08 us                                                | 4.06 us: 1.25x faster                                                 |
| sympy_expand            | 566 ms                                                 | 456 ms: 1.24x faster                                                  |
| comprehensions          | 28.8 us                                                | 23.4 us: 1.23x faster                                                 |
| sympy_str               | 346 ms                                                 | 282 ms: 1.23x faster                                                  |
| json                    | 5.69 ms                                                | 4.65 ms: 1.22x faster                                                 |
| dask                    | 441 ms                                                 | 360 ms: 1.22x faster                                                  |
| sympy_sum               | 196 ms                                                 | 165 ms: 1.19x faster                                                  |
| djangocms               | 38.4 us                                                | 32.5 us: 1.18x faster                                                 |
| meteor_contest          | 120 ms                                                 | 102 ms: 1.17x faster                                                  |
| sqlite_synth            | 3.02 us                                                | 2.60 us: 1.16x faster                                                 |
| pathlib                 | 20.5 ms                                                | 17.7 ms: 1.15x faster                                                 |
| mdp                     | 2.85 sec                                               | 2.48 sec: 1.15x faster                                                |
| telco                   | 7.27 ms                                                | 6.38 ms: 1.14x faster                                                 |
| xml_etree_parse         | 168 ms                                                 | 149 ms: 1.13x faster                                                  |
| xml_etree_iterparse     | 115 ms                                                 | 103 ms: 1.12x faster                                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                 |
| unpickle                | 14.4 us                                                | 12.9 us: 1.11x faster                                                 |
| regex_dna               | 227 ms                                                 | 208 ms: 1.09x faster                                                  |
| pickle                  | 10.7 us                                                | 9.88 us: 1.08x faster                                                 |
| regex_effbot            | 3.63 ms                                                | 3.47 ms: 1.05x faster                                                 |
| unpickle_list           | 5.20 us                                                | 4.98 us: 1.04x faster                                                 |
| asyncio_tcp             | 922 ms                                                 | 884 ms: 1.04x faster                                                  |
| generators              | 80.1 ms                                                | 77.4 ms: 1.03x faster                                                 |
| pidigits                | 191 ms                                                 | 189 ms: 1.01x faster                                                  |
| python_startup_no_site  | 5.93 ms                                                | 6.12 ms: 1.03x slower                                                 |
| pickle_dict             | 29.6 us                                                | 30.8 us: 1.04x slower                                                 |
| gc_traversal            | 3.62 ms                                                | 3.77 ms: 1.04x slower                                                 |
| coverage                | 79.4 ms                                                | 101 ms: 1.27x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.38x faster                                                          |

Benchmark hidden because not significant (1): bench_mp_pool
Ignored benchmarks (10) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.35x
- 95% likely to have a speedup of 1.34x
- 99% likely to have a speedup of 1.32x


# Memory

- memory change: 1.09x