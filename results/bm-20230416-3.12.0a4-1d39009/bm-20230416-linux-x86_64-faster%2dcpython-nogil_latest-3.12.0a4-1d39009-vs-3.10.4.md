
# Results vs. 3.10.4

- fork: faster-cpython
- ref: nogil_latest
- machine: linux-x86_64
- commit hash: 1d39009
- commit date: 2023-04-16
- overall geometric mean: 1.26x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.21x faster
- Memory change: 1.44x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 290 ms: 1.20x faster                                                    |
| chameleon      | 9.68 ms                                                | 7.81 ms: 1.24x faster                                                   |
| docutils       | 3.30 sec                                               | 3.15 sec: 1.05x faster                                                  |
| html5lib       | 88.9 ms                                                | 69.2 ms: 1.28x faster                                                   |
| Geometric mean | (ref)                                                  | 1.19x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 616 ms: 2.87x faster                                                    |
| async_tree_none         | 728 ms                                                 | 311 ms: 2.34x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 381 ms: 2.28x faster                                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 534 ms: 1.90x faster                                                    |
| Geometric mean          | (ref)                                                  | 2.32x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| float          | 117 ms                                                 | 65.9 ms: 1.78x faster                                                   |
| nbody          | 154 ms                                                 | 107 ms: 1.43x faster                                                    |
| pidigits       | 191 ms                                                 | 186 ms: 1.03x faster                                                    |
| Geometric mean | (ref)                                                  | 1.38x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                   |
| regex_compile  | 188 ms                                                 | 152 ms: 1.24x faster                                                    |
| regex_dna      | 227 ms                                                 | 205 ms: 1.10x faster                                                    |
| regex_effbot   | 3.63 ms                                                | 3.46 ms: 1.05x faster                                                   |
| Geometric mean | (ref)                                                  | 1.17x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 321 us: 1.51x faster                                                    |
| unpickle_pure_python | 331 us                                                 | 229 us: 1.44x faster                                                    |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                   |
| xml_etree_process    | 79.1 ms                                                | 61.3 ms: 1.29x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 137 ms: 1.22x faster                                                    |
| xml_etree_generate   | 99.4 ms                                                | 83.7 ms: 1.19x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.33 us: 1.17x faster                                                   |
| json_loads           | 31.2 us                                                | 28.0 us: 1.11x faster                                                   |
| pickle               | 10.7 us                                                | 10.3 us: 1.04x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 114 ms: 1.02x faster                                                    |
| pickle_dict          | 29.6 us                                                | 30.0 us: 1.01x slower                                                   |
| unpickle             | 14.4 us                                                | 15.5 us: 1.08x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                            |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.18 ms: 1.59x faster                                                   |
| python_startup_no_site | 5.93 ms                                                | 6.59 ms: 1.11x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.20x faster                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| genshi_text     | 31.8 ms                                                | 24.4 ms: 1.31x faster                                                   |
| django_template | 48.2 ms                                                | 37.4 ms: 1.29x faster                                                   |
| genshi_xml      | 66.0 ms                                                | 52.0 ms: 1.27x faster                                                   |
| mako            | 16.3 ms                                                | 13.2 ms: 1.23x faster                                                   |
| Geometric mean  | (ref)                                                  | 1.27x faster                                                            |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20230416-linux-x86_64-faster%2dcpython-nogil_latest-3.12.0a4-1d39009 |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 616 ms: 2.87x faster                                                    |
| async_tree_none         | 728 ms                                                 | 311 ms: 2.34x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 381 ms: 2.28x faster                                                    |
| deltablue               | 7.91 ms                                                | 3.91 ms: 2.02x faster                                                   |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 534 ms: 1.90x faster                                                    |
| logging_silent          | 190 ns                                                 | 104 ns: 1.83x faster                                                    |
| scimark_sor             | 220 ms                                                 | 123 ms: 1.79x faster                                                    |
| float                   | 117 ms                                                 | 65.9 ms: 1.78x faster                                                   |
| asyncio_tcp             | 922 ms                                                 | 525 ms: 1.76x faster                                                    |
| go                      | 240 ms                                                 | 146 ms: 1.64x faster                                                    |
| richards                | 79.3 ms                                                | 48.4 ms: 1.64x faster                                                   |
| python_startup          | 14.6 ms                                                | 9.18 ms: 1.59x faster                                                   |
| crypto_pyaes            | 128 ms                                                 | 81.8 ms: 1.56x faster                                                   |
| scimark_monte_carlo     | 118 ms                                                 | 76.4 ms: 1.55x faster                                                   |
| chaos                   | 115 ms                                                 | 74.6 ms: 1.55x faster                                                   |
| pyflate                 | 716 ms                                                 | 470 ms: 1.53x faster                                                    |
| spectral_norm           | 170 ms                                                 | 112 ms: 1.51x faster                                                    |
| pickle_pure_python      | 484 us                                                 | 321 us: 1.51x faster                                                    |
| hexiom                  | 10.4 ms                                                | 6.89 ms: 1.51x faster                                                   |
| raytrace                | 507 ms                                                 | 346 ms: 1.47x faster                                                    |
| deepcopy_memo           | 58.5 us                                                | 40.1 us: 1.46x faster                                                   |
| unpickle_pure_python    | 331 us                                                 | 229 us: 1.44x faster                                                    |
| nbody                   | 154 ms                                                 | 107 ms: 1.43x faster                                                    |
| scimark_lu              | 176 ms                                                 | 128 ms: 1.38x faster                                                    |
| pycparser               | 1.58 sec                                               | 1.15 sec: 1.37x faster                                                  |
| json_dumps              | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                   |
| pprint_safe_repr        | 1.02 sec                                               | 765 ms: 1.33x faster                                                    |
| pprint_pformat          | 2.10 sec                                               | 1.58 sec: 1.33x faster                                                  |
| regex_v8                | 27.8 ms                                                | 21.1 ms: 1.32x faster                                                   |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.94 ms: 1.31x faster                                                   |
| coroutines              | 35.1 ms                                                | 26.8 ms: 1.31x faster                                                   |
| genshi_text             | 31.8 ms                                                | 24.4 ms: 1.31x faster                                                   |
| xml_etree_process       | 79.1 ms                                                | 61.3 ms: 1.29x faster                                                   |
| django_template         | 48.2 ms                                                | 37.4 ms: 1.29x faster                                                   |
| html5lib                | 88.9 ms                                                | 69.2 ms: 1.28x faster                                                   |
| deepcopy                | 479 us                                                 | 375 us: 1.28x faster                                                    |
| genshi_xml              | 66.0 ms                                                | 52.0 ms: 1.27x faster                                                   |
| thrift                  | 1.07 ms                                                | 851 us: 1.26x faster                                                    |
| sqlglot_normalize       | 143 ms                                                 | 115 ms: 1.25x faster                                                    |
| chameleon               | 9.68 ms                                                | 7.81 ms: 1.24x faster                                                   |
| regex_compile           | 188 ms                                                 | 152 ms: 1.24x faster                                                    |
| dulwich_log             | 84.3 ms                                                | 68.1 ms: 1.24x faster                                                   |
| nqueens                 | 106 ms                                                 | 85.8 ms: 1.23x faster                                                   |
| mako                    | 16.3 ms                                                | 13.2 ms: 1.23x faster                                                   |
| sqlglot_transpile       | 2.57 ms                                                | 2.10 ms: 1.23x faster                                                   |
| xml_etree_parse         | 168 ms                                                 | 137 ms: 1.22x faster                                                    |
| fannkuch                | 532 ms                                                 | 436 ms: 1.22x faster                                                    |
| deepcopy_reduce         | 4.17 us                                                | 3.42 us: 1.22x faster                                                   |
| scimark_fft             | 466 ms                                                 | 383 ms: 1.22x faster                                                    |
| sqlglot_parse           | 2.17 ms                                                | 1.79 ms: 1.21x faster                                                   |
| sqlglot_optimize        | 69.2 ms                                                | 57.1 ms: 1.21x faster                                                   |
| 2to3                    | 348 ms                                                 | 290 ms: 1.20x faster                                                    |
| xml_etree_generate      | 99.4 ms                                                | 83.7 ms: 1.19x faster                                                   |
| logging_format          | 9.09 us                                                | 7.66 us: 1.19x faster                                                   |
| logging_simple          | 8.30 us                                                | 7.00 us: 1.19x faster                                                   |
| async_generators        | 444 ms                                                 | 377 ms: 1.18x faster                                                    |
| pickle_list             | 5.08 us                                                | 4.33 us: 1.17x faster                                                   |
| sqlite_synth            | 3.02 us                                                | 2.62 us: 1.15x faster                                                   |
| sympy_integrate         | 25.8 ms                                                | 22.8 ms: 1.13x faster                                                   |
| json                    | 5.69 ms                                                | 5.06 ms: 1.12x faster                                                   |
| pathlib                 | 20.5 ms                                                | 18.2 ms: 1.12x faster                                                   |
| json_loads              | 31.2 us                                                | 28.0 us: 1.11x faster                                                   |
| regex_dna               | 227 ms                                                 | 205 ms: 1.10x faster                                                    |
| comprehensions          | 28.8 us                                                | 26.3 us: 1.09x faster                                                   |
| sympy_expand            | 566 ms                                                 | 537 ms: 1.05x faster                                                    |
| sympy_str               | 346 ms                                                 | 329 ms: 1.05x faster                                                    |
| telco                   | 7.27 ms                                                | 6.92 ms: 1.05x faster                                                   |
| regex_effbot            | 3.63 ms                                                | 3.46 ms: 1.05x faster                                                   |
| docutils                | 3.30 sec                                               | 3.15 sec: 1.05x faster                                                  |
| pickle                  | 10.7 us                                                | 10.3 us: 1.04x faster                                                   |
| unpack_sequence         | 60.0 ns                                                | 58.1 ns: 1.03x faster                                                   |
| pidigits                | 191 ms                                                 | 186 ms: 1.03x faster                                                    |
| mdp                     | 2.85 sec                                               | 2.79 sec: 1.02x faster                                                  |
| sympy_sum               | 196 ms                                                 | 192 ms: 1.02x faster                                                    |
| create_gc_cycles        | 1.62 ms                                                | 1.59 ms: 1.02x faster                                                   |
| xml_etree_iterparse     | 115 ms                                                 | 114 ms: 1.02x faster                                                    |
| generators              | 80.1 ms                                                | 78.8 ms: 1.02x faster                                                   |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                                   |
| gc_traversal            | 3.62 ms                                                | 3.67 ms: 1.01x slower                                                   |
| pickle_dict             | 29.6 us                                                | 30.0 us: 1.01x slower                                                   |
| meteor_contest          | 120 ms                                                 | 124 ms: 1.04x slower                                                    |
| unpickle                | 14.4 us                                                | 15.5 us: 1.08x slower                                                   |
| python_startup_no_site  | 5.93 ms                                                | 6.59 ms: 1.11x slower                                                   |
| coverage                | 79.4 ms                                                | 109 ms: 1.37x slower                                                    |
| bench_thread_pool       | 986 us                                                 | 1.64 ms: 1.67x slower                                                   |
| Geometric mean          | (ref)                                                  | 1.26x faster                                                            |

Benchmark hidden because not significant (2): djangocms, unpickle_list
Ignored benchmarks (14) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, asyncio_websockets, dask, flaskblogging, gunicorn, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.23x
- 95% likely to have a speedup of 1.22x
- 99% likely to have a speedup of 1.21x


# Memory

- memory change: 1.44x