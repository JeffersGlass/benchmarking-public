
# Results vs. 3.10.4

- fork: faster_cpython
- ref: nogil
- machine: linux-x86_64
- commit hash: 258cab1
- commit date: 2022-12-21
- overall geometric mean: 1.07x faster \*
- HPT reliability: 99.94%
- HPT 99th percentile: 1.02x faster
- Memory change: 1.47x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 382 ms: 1.10x slower                                         |
| chameleon      | 9.68 ms                                                | 8.20 ms: 1.18x faster                                        |
| docutils       | 3.30 sec                                               | 5.20 sec: 1.58x slower                                       |
| html5lib       | 88.9 ms                                                | 81.7 ms: 1.09x faster                                        |
| tornado_http   | 136 ms                                                 | 124 ms: 1.10x faster                                         |
| Geometric mean | (ref)                                                  | 1.04x slower                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 829 ms: 2.13x faster                                         |
| async_tree_none         | 728 ms                                                 | 372 ms: 1.96x faster                                         |
| async_tree_memoization  | 870 ms                                                 | 460 ms: 1.89x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 614 ms: 1.66x faster                                         |
| Geometric mean          | (ref)                                                  | 1.90x faster                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| float          | 117 ms                                                 | 104 ms: 1.12x faster                                         |
| pidigits       | 191 ms                                                 | 186 ms: 1.03x faster                                         |
| nbody          | 154 ms                                                 | 172 ms: 1.12x slower                                         |
| Geometric mean | (ref)                                                  | 1.01x faster                                                 |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| regex_v8       | 27.8 ms                                                | 24.1 ms: 1.15x faster                                        |
| regex_effbot   | 3.63 ms                                                | 3.35 ms: 1.08x faster                                        |
| regex_dna      | 227 ms                                                 | 218 ms: 1.04x faster                                         |
| regex_compile  | 188 ms                                                 | 186 ms: 1.01x faster                                         |
| Geometric mean | (ref)                                                  | 1.07x faster                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 346 us: 1.40x faster                                         |
| unpickle_pure_python | 331 us                                                 | 262 us: 1.26x faster                                         |
| pickle_list          | 5.08 us                                                | 4.17 us: 1.22x faster                                        |
| xml_etree_iterparse  | 115 ms                                                 | 95.5 ms: 1.21x faster                                        |
| pickle_dict          | 29.6 us                                                | 25.3 us: 1.17x faster                                        |
| xml_etree_generate   | 99.4 ms                                                | 87.8 ms: 1.13x faster                                        |
| xml_etree_parse      | 168 ms                                                 | 149 ms: 1.13x faster                                         |
| xml_etree_process    | 79.1 ms                                                | 71.4 ms: 1.11x faster                                        |
| pickle               | 10.7 us                                                | 10.0 us: 1.06x faster                                        |
| json_dumps           | 14.2 ms                                                | 13.4 ms: 1.06x faster                                        |
| json_loads           | 31.2 us                                                | 32.5 us: 1.04x slower                                        |
| unpickle_list        | 5.20 us                                                | 5.80 us: 1.12x slower                                        |
| unpickle             | 14.4 us                                                | 18.6 us: 1.29x slower                                        |
| Geometric mean       | (ref)                                                  | 1.09x faster                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 9.41 ms: 1.55x faster                                        |
| python_startup_no_site | 5.93 ms                                                | 5.91 ms: 1.00x faster                                        |
| Geometric mean         | (ref)                                                  | 1.25x faster                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| django_template | 48.2 ms                                                | 42.6 ms: 1.13x faster                                        |
| mako            | 16.3 ms                                                | 16.4 ms: 1.01x slower                                        |
| genshi_xml      | 66.0 ms                                                | 73.6 ms: 1.11x slower                                        |
| genshi_text     | 31.8 ms                                                | 52.1 ms: 1.64x slower                                        |
| Geometric mean  | (ref)                                                  | 1.13x slower                                                 |

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 829 ms: 2.13x faster                                         |
| richards                | 79.3 ms                                                | 39.3 ms: 2.01x faster                                        |
| logging_silent          | 190 ns                                                 | 96.0 ns: 1.98x faster                                        |
| async_tree_none         | 728 ms                                                 | 372 ms: 1.96x faster                                         |
| async_tree_memoization  | 870 ms                                                 | 460 ms: 1.89x faster                                         |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 614 ms: 1.66x faster                                         |
| python_startup          | 14.6 ms                                                | 9.41 ms: 1.55x faster                                        |
| scimark_sor             | 220 ms                                                 | 144 ms: 1.52x faster                                         |
| go                      | 240 ms                                                 | 159 ms: 1.51x faster                                         |
| pprint_pformat          | 2.10 sec                                               | 1.40 sec: 1.50x faster                                       |
| deltablue               | 7.91 ms                                                | 5.41 ms: 1.46x faster                                        |
| deepcopy_memo           | 58.5 us                                                | 40.1 us: 1.46x faster                                        |
| pickle_pure_python      | 484 us                                                 | 346 us: 1.40x faster                                         |
| hexiom                  | 10.4 ms                                                | 7.74 ms: 1.34x faster                                        |
| unpickle_pure_python    | 331 us                                                 | 262 us: 1.26x faster                                         |
| deepcopy                | 479 us                                                 | 393 us: 1.22x faster                                         |
| raytrace                | 507 ms                                                 | 416 ms: 1.22x faster                                         |
| pickle_list             | 5.08 us                                                | 4.17 us: 1.22x faster                                        |
| xml_etree_iterparse     | 115 ms                                                 | 95.5 ms: 1.21x faster                                        |
| logging_simple          | 8.30 us                                                | 6.95 us: 1.19x faster                                        |
| spectral_norm           | 170 ms                                                 | 143 ms: 1.19x faster                                         |
| logging_format          | 9.09 us                                                | 7.69 us: 1.18x faster                                        |
| chameleon               | 9.68 ms                                                | 8.20 ms: 1.18x faster                                        |
| scimark_lu              | 176 ms                                                 | 149 ms: 1.18x faster                                         |
| scimark_monte_carlo     | 118 ms                                                 | 101 ms: 1.17x faster                                         |
| pickle_dict             | 29.6 us                                                | 25.3 us: 1.17x faster                                        |
| pycparser               | 1.58 sec                                               | 1.35 sec: 1.17x faster                                       |
| regex_v8                | 27.8 ms                                                | 24.1 ms: 1.15x faster                                        |
| deepcopy_reduce         | 4.17 us                                                | 3.63 us: 1.15x faster                                        |
| unpack_sequence         | 60.0 ns                                                | 52.4 ns: 1.14x faster                                        |
| chaos                   | 115 ms                                                 | 102 ms: 1.13x faster                                         |
| xml_etree_generate      | 99.4 ms                                                | 87.8 ms: 1.13x faster                                        |
| django_template         | 48.2 ms                                                | 42.6 ms: 1.13x faster                                        |
| xml_etree_parse         | 168 ms                                                 | 149 ms: 1.13x faster                                         |
| pyflate                 | 716 ms                                                 | 636 ms: 1.13x faster                                         |
| float                   | 117 ms                                                 | 104 ms: 1.12x faster                                         |
| xml_etree_process       | 79.1 ms                                                | 71.4 ms: 1.11x faster                                        |
| tornado_http            | 136 ms                                                 | 124 ms: 1.10x faster                                         |
| dulwich_log             | 84.3 ms                                                | 77.0 ms: 1.09x faster                                        |
| html5lib                | 88.9 ms                                                | 81.7 ms: 1.09x faster                                        |
| fannkuch                | 532 ms                                                 | 490 ms: 1.09x faster                                         |
| regex_effbot            | 3.63 ms                                                | 3.35 ms: 1.08x faster                                        |
| scimark_fft             | 466 ms                                                 | 430 ms: 1.08x faster                                         |
| thrift                  | 1.07 ms                                                | 992 us: 1.08x faster                                         |
| sympy_expand            | 566 ms                                                 | 531 ms: 1.07x faster                                         |
| pickle                  | 10.7 us                                                | 10.0 us: 1.06x faster                                        |
| scimark_sparse_mat_mult | 6.47 ms                                                | 6.09 ms: 1.06x faster                                        |
| json                    | 5.69 ms                                                | 5.37 ms: 1.06x faster                                        |
| json_dumps              | 14.2 ms                                                | 13.4 ms: 1.06x faster                                        |
| crypto_pyaes            | 128 ms                                                 | 122 ms: 1.05x faster                                         |
| regex_dna               | 227 ms                                                 | 218 ms: 1.04x faster                                         |
| sympy_str               | 346 ms                                                 | 335 ms: 1.03x faster                                         |
| pidigits                | 191 ms                                                 | 186 ms: 1.03x faster                                         |
| sympy_integrate         | 25.8 ms                                                | 25.4 ms: 1.02x faster                                        |
| telco                   | 7.27 ms                                                | 7.15 ms: 1.02x faster                                        |
| regex_compile           | 188 ms                                                 | 186 ms: 1.01x faster                                         |
| bench_mp_pool           | 24.0 ms                                                | 23.8 ms: 1.01x faster                                        |
| python_startup_no_site  | 5.93 ms                                                | 5.91 ms: 1.00x faster                                        |
| mako                    | 16.3 ms                                                | 16.4 ms: 1.01x slower                                        |
| pathlib                 | 20.5 ms                                                | 20.6 ms: 1.01x slower                                        |
| sqlglot_normalize       | 143 ms                                                 | 144 ms: 1.01x slower                                         |
| generators              | 80.1 ms                                                | 81.6 ms: 1.02x slower                                        |
| nqueens                 | 106 ms                                                 | 109 ms: 1.03x slower                                         |
| json_loads              | 31.2 us                                                | 32.5 us: 1.04x slower                                        |
| djangocms               | 38.4 us                                                | 40.5 us: 1.05x slower                                        |
| meteor_contest          | 120 ms                                                 | 127 ms: 1.06x slower                                         |
| sqlite_synth            | 3.02 us                                                | 3.24 us: 1.07x slower                                        |
| sympy_sum               | 196 ms                                                 | 212 ms: 1.08x slower                                         |
| mdp                     | 2.85 sec                                               | 3.10 sec: 1.09x slower                                       |
| 2to3                    | 348 ms                                                 | 382 ms: 1.10x slower                                         |
| genshi_xml              | 66.0 ms                                                | 73.6 ms: 1.11x slower                                        |
| unpickle_list           | 5.20 us                                                | 5.80 us: 1.12x slower                                        |
| nbody                   | 154 ms                                                 | 172 ms: 1.12x slower                                         |
| pylint                  | 551 ms                                                 | 626 ms: 1.14x slower                                         |
| bench_thread_pool       | 986 us                                                 | 1.19 ms: 1.20x slower                                        |
| unpickle                | 14.4 us                                                | 18.6 us: 1.29x slower                                        |
| async_generators        | 444 ms                                                 | 626 ms: 1.41x slower                                         |
| flaskblogging           | 8.58 ms                                                | 12.1 ms: 1.42x slower                                        |
| docutils                | 3.30 sec                                               | 5.20 sec: 1.58x slower                                       |
| genshi_text             | 31.8 ms                                                | 52.1 ms: 1.64x slower                                        |
| coroutines              | 35.1 ms                                                | 72.5 ms: 2.07x slower                                        |
| coverage                | 79.4 ms                                                | 553 ms: 6.96x slower                                         |
| Geometric mean          | (ref)                                                  | 1.07x faster                                                 |

Benchmark hidden because not significant (5): sqlglot_transpile, gunicorn, aiohttp, sqlglot_optimize, sqlglot_parse
Ignored benchmarks (14) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, comprehensions, create_gc_cycles, dask, gc_traversal, mypy2, pprint_safe_repr, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20221221-3.9.10-258cab1/bm-20221221-linux-x86_64-faster_cpython-nogil-3.9.10-258cab1.json: mypy


# HPT report

- Reliability score: 99.94% likely to be faster
- 90% likely to have a speedup of 1.04x
- 95% likely to have a speedup of 1.03x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 1.47x