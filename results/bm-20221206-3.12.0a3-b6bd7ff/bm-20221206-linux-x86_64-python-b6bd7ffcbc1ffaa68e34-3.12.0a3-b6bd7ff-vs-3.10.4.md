
# Results vs. 3.10.4

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: linux-x86_64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.36x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.29x faster
- Memory change: 1.09x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 246 ms: 1.42x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.45 ms: 1.50x faster                                                 |
| docutils       | 3.30 sec                                               | 2.57 sec: 1.28x faster                                                |
| html5lib       | 88.9 ms                                                | 59.7 ms: 1.49x faster                                                 |
| Geometric mean | (ref)                                                  | 1.42x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 536 ms: 1.36x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.34 sec: 1.32x faster                                                |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 769 ms: 1.32x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 665 ms: 1.31x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.33x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.0 ms: 1.63x faster                                                 |
| float          | 117 ms                                                 | 73.2 ms: 1.60x faster                                                 |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                  |
| Geometric mean | (ref)                                                  | 1.38x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 129 ms: 1.46x faster                                                  |
| regex_v8       | 27.8 ms                                                | 22.3 ms: 1.24x faster                                                 |
| regex_dna      | 227 ms                                                 | 217 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.17x faster                                                          |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 282 us: 1.72x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 200 us: 1.65x faster                                                  |
| json_dumps           | 14.2 ms                                                | 9.52 ms: 1.49x faster                                                 |
| xml_etree_process    | 79.1 ms                                                | 53.7 ms: 1.47x faster                                                 |
| json_loads           | 31.2 us                                                | 23.8 us: 1.31x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 76.9 ms: 1.29x faster                                                 |
| pickle_list          | 5.08 us                                                | 3.95 us: 1.29x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 148 ms: 1.13x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                                  |
| unpickle             | 14.4 us                                                | 13.3 us: 1.08x faster                                                 |
| pickle               | 10.7 us                                                | 10.1 us: 1.05x faster                                                 |
| unpickle_list        | 5.20 us                                                | 4.97 us: 1.05x faster                                                 |
| pickle_dict          | 29.6 us                                                | 31.5 us: 1.07x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.25x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 8.52 ms: 1.71x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 6.07 ms: 1.02x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.29x faster                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 9.43 ms: 1.73x faster                                                 |
| genshi_text     | 31.8 ms                                                | 20.9 ms: 1.53x faster                                                 |
| django_template | 48.2 ms                                                | 33.0 ms: 1.46x faster                                                 |
| genshi_xml      | 66.0 ms                                                | 48.0 ms: 1.38x faster                                                 |
| Geometric mean  | (ref)                                                  | 1.52x faster                                                          |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221206-linux-x86_64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| deltablue               | 7.91 ms                                                | 3.22 ms: 2.46x faster                                                 |
| scimark_sor             | 220 ms                                                 | 105 ms: 2.09x faster                                                  |
| logging_silent          | 190 ns                                                 | 90.9 ns: 2.09x faster                                                 |
| richards                | 79.3 ms                                                | 42.0 ms: 1.89x faster                                                 |
| scimark_monte_carlo     | 118 ms                                                 | 65.4 ms: 1.81x faster                                                 |
| raytrace                | 507 ms                                                 | 281 ms: 1.81x faster                                                  |
| go                      | 240 ms                                                 | 136 ms: 1.77x faster                                                  |
| spectral_norm           | 170 ms                                                 | 96.0 ms: 1.77x faster                                                 |
| pyflate                 | 716 ms                                                 | 405 ms: 1.77x faster                                                  |
| mako                    | 16.3 ms                                                | 9.43 ms: 1.73x faster                                                 |
| chaos                   | 115 ms                                                 | 66.9 ms: 1.73x faster                                                 |
| pickle_pure_python      | 484 us                                                 | 282 us: 1.72x faster                                                  |
| python_startup          | 14.6 ms                                                | 8.52 ms: 1.71x faster                                                 |
| hexiom                  | 10.4 ms                                                | 6.08 ms: 1.71x faster                                                 |
| deepcopy_memo           | 58.5 us                                                | 34.2 us: 1.71x faster                                                 |
| crypto_pyaes            | 128 ms                                                 | 75.3 ms: 1.70x faster                                                 |
| scimark_lu              | 176 ms                                                 | 106 ms: 1.66x faster                                                  |
| unpickle_pure_python    | 331 us                                                 | 200 us: 1.65x faster                                                  |
| nbody                   | 154 ms                                                 | 94.0 ms: 1.63x faster                                                 |
| sqlglot_parse           | 2.17 ms                                                | 1.34 ms: 1.61x faster                                                 |
| float                   | 117 ms                                                 | 73.2 ms: 1.60x faster                                                 |
| sqlglot_transpile       | 2.57 ms                                                | 1.63 ms: 1.58x faster                                                 |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.20 ms: 1.54x faster                                                 |
| genshi_text             | 31.8 ms                                                | 20.9 ms: 1.53x faster                                                 |
| chameleon               | 9.68 ms                                                | 6.45 ms: 1.50x faster                                                 |
| html5lib                | 88.9 ms                                                | 59.7 ms: 1.49x faster                                                 |
| json_dumps              | 14.2 ms                                                | 9.52 ms: 1.49x faster                                                 |
| pprint_pformat          | 2.10 sec                                               | 1.41 sec: 1.49x faster                                                |
| pprint_safe_repr        | 1.02 sec                                               | 686 ms: 1.48x faster                                                  |
| scimark_fft             | 466 ms                                                 | 314 ms: 1.48x faster                                                  |
| xml_etree_process       | 79.1 ms                                                | 53.7 ms: 1.47x faster                                                 |
| regex_compile           | 188 ms                                                 | 129 ms: 1.46x faster                                                  |
| django_template         | 48.2 ms                                                | 33.0 ms: 1.46x faster                                                 |
| deepcopy                | 479 us                                                 | 332 us: 1.44x faster                                                  |
| pycparser               | 1.58 sec                                               | 1.09 sec: 1.44x faster                                                |
| thrift                  | 1.07 ms                                                | 751 us: 1.43x faster                                                  |
| logging_format          | 9.09 us                                                | 6.41 us: 1.42x faster                                                 |
| 2to3                    | 348 ms                                                 | 246 ms: 1.42x faster                                                  |
| logging_simple          | 8.30 us                                                | 5.88 us: 1.41x faster                                                 |
| coroutines              | 35.1 ms                                                | 25.0 ms: 1.41x faster                                                 |
| deepcopy_reduce         | 4.17 us                                                | 2.97 us: 1.40x faster                                                 |
| fannkuch                | 532 ms                                                 | 379 ms: 1.40x faster                                                  |
| unpack_sequence         | 60.0 ns                                                | 43.1 ns: 1.39x faster                                                 |
| genshi_xml              | 66.0 ms                                                | 48.0 ms: 1.38x faster                                                 |
| sqlglot_optimize        | 69.2 ms                                                | 50.6 ms: 1.37x faster                                                 |
| sqlglot_normalize       | 143 ms                                                 | 105 ms: 1.36x faster                                                  |
| async_tree_none         | 728 ms                                                 | 536 ms: 1.36x faster                                                  |
| dulwich_log             | 84.3 ms                                                | 62.5 ms: 1.35x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.34 sec: 1.32x faster                                                |
| nqueens                 | 106 ms                                                 | 80.1 ms: 1.32x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 769 ms: 1.32x faster                                                  |
| json_loads              | 31.2 us                                                | 23.8 us: 1.31x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 665 ms: 1.31x faster                                                  |
| xml_etree_generate      | 99.4 ms                                                | 76.9 ms: 1.29x faster                                                 |
| pickle_list             | 5.08 us                                                | 3.95 us: 1.29x faster                                                 |
| docutils                | 3.30 sec                                               | 2.57 sec: 1.28x faster                                                |
| bench_thread_pool       | 986 us                                                 | 778 us: 1.27x faster                                                  |
| sympy_integrate         | 25.8 ms                                                | 20.4 ms: 1.26x faster                                                 |
| async_generators        | 444 ms                                                 | 354 ms: 1.25x faster                                                  |
| regex_v8                | 27.8 ms                                                | 22.3 ms: 1.24x faster                                                 |
| sympy_expand            | 566 ms                                                 | 458 ms: 1.24x faster                                                  |
| dask                    | 441 ms                                                 | 360 ms: 1.22x faster                                                  |
| sympy_str               | 346 ms                                                 | 283 ms: 1.22x faster                                                  |
| comprehensions          | 28.8 us                                                | 23.5 us: 1.22x faster                                                 |
| json                    | 5.69 ms                                                | 4.67 ms: 1.22x faster                                                 |
| sympy_sum               | 196 ms                                                 | 164 ms: 1.20x faster                                                  |
| djangocms               | 38.4 us                                                | 32.6 us: 1.18x faster                                                 |
| sqlite_synth            | 3.02 us                                                | 2.58 us: 1.17x faster                                                 |
| meteor_contest          | 120 ms                                                 | 104 ms: 1.15x faster                                                  |
| mdp                     | 2.85 sec                                               | 2.50 sec: 1.14x faster                                                |
| xml_etree_parse         | 168 ms                                                 | 148 ms: 1.13x faster                                                  |
| create_gc_cycles        | 1.62 ms                                                | 1.44 ms: 1.13x faster                                                 |
| telco                   | 7.27 ms                                                | 6.46 ms: 1.13x faster                                                 |
| pathlib                 | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                 |
| xml_etree_iterparse     | 115 ms                                                 | 104 ms: 1.11x faster                                                  |
| unpickle                | 14.4 us                                                | 13.3 us: 1.08x faster                                                 |
| pickle                  | 10.7 us                                                | 10.1 us: 1.05x faster                                                 |
| unpickle_list           | 5.20 us                                                | 4.97 us: 1.05x faster                                                 |
| regex_dna               | 227 ms                                                 | 217 ms: 1.05x faster                                                  |
| asyncio_tcp             | 922 ms                                                 | 890 ms: 1.04x faster                                                  |
| generators              | 80.1 ms                                                | 79.1 ms: 1.01x faster                                                 |
| pidigits                | 191 ms                                                 | 189 ms: 1.01x faster                                                  |
| python_startup_no_site  | 5.93 ms                                                | 6.07 ms: 1.02x slower                                                 |
| gc_traversal            | 3.62 ms                                                | 3.81 ms: 1.05x slower                                                 |
| pickle_dict             | 29.6 us                                                | 31.5 us: 1.07x slower                                                 |
| coverage                | 79.4 ms                                                | 102 ms: 1.29x slower                                                  |
| Geometric mean          | (ref)                                                  | 1.36x faster                                                          |

Benchmark hidden because not significant (2): regex_effbot, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.32x
- 99% likely to have a speedup of 1.29x


# Memory

- memory change: 1.09x