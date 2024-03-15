
# Results vs. 3.10.4

- fork: mdboom
- ref: RegCPython
- machine: linux-x86_64
- commit hash: 53f2d50
- commit date: 2022-07-20
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.03x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 313 ms: 1.11x faster                                      |
| chameleon      | 9.68 ms                                                | 8.49 ms: 1.14x faster                                     |
| docutils       | 3.30 sec                                               | 3.10 sec: 1.06x faster                                    |
| html5lib       | 88.9 ms                                                | 76.8 ms: 1.16x faster                                     |
| tornado_http   | 136 ms                                                 | 123 ms: 1.11x faster                                      |
| Geometric mean | (ref)                                                  | 1.12x faster                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_io           | 1.77 sec                                               | 1.61 sec: 1.10x faster                                    |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 970 ms: 1.05x faster                                      |
| async_tree_memoization  | 870 ms                                                 | 839 ms: 1.04x faster                                      |
| Geometric mean          | (ref)                                                  | 1.05x faster                                              |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody          | 154 ms                                                 | 101 ms: 1.52x faster                                      |
| float          | 117 ms                                                 | 94.9 ms: 1.23x faster                                     |
| pidigits       | 191 ms                                                 | 188 ms: 1.01x faster                                      |
| Geometric mean | (ref)                                                  | 1.24x faster                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 157 ms: 1.20x faster                                      |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                     |
| regex_effbot   | 3.63 ms                                                | 3.31 ms: 1.10x faster                                     |
| regex_dna      | 227 ms                                                 | 216 ms: 1.05x faster                                      |
| Geometric mean | (ref)                                                  | 1.11x faster                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| unpickle_pure_python | 331 us                                                 | 279 us: 1.18x faster                                      |
| xml_etree_generate   | 99.4 ms                                                | 86.2 ms: 1.15x faster                                     |
| xml_etree_process    | 79.1 ms                                                | 68.9 ms: 1.15x faster                                     |
| pickle_pure_python   | 484 us                                                 | 432 us: 1.12x faster                                      |
| pickle_list          | 5.08 us                                                | 4.65 us: 1.09x faster                                     |
| pickle_dict          | 29.6 us                                                | 27.2 us: 1.09x faster                                     |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.08x faster                                      |
| json_loads           | 31.2 us                                                | 29.0 us: 1.08x faster                                     |
| unpickle_list        | 5.20 us                                                | 4.86 us: 1.07x faster                                     |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                      |
| json_dumps           | 14.2 ms                                                | 13.4 ms: 1.06x faster                                     |
| pickle               | 10.7 us                                                | 10.1 us: 1.06x faster                                     |
| Geometric mean       | (ref)                                                  | 1.09x faster                                              |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup_no_site | 5.93 ms                                                | 5.80 ms: 1.02x faster                                     |
| python_startup         | 14.6 ms                                                | 15.2 ms: 1.04x slower                                     |
| Geometric mean         | (ref)                                                  | 1.01x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako           | 16.3 ms                                                | 13.1 ms: 1.25x faster                                     |
| genshi_text    | 31.8 ms                                                | 29.0 ms: 1.10x faster                                     |
| genshi_xml     | 66.0 ms                                                | 60.6 ms: 1.09x faster                                     |
| Geometric mean | (ref)                                                  | 1.10x faster                                              |

Benchmark hidden because not significant (1): django_template

All benchmarks:
===============

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| nbody                   | 154 ms                                                 | 101 ms: 1.52x faster                                      |
| scimark_sparse_mat_mult | 6.47 ms                                                | 4.29 ms: 1.51x faster                                     |
| fannkuch                | 532 ms                                                 | 369 ms: 1.44x faster                                      |
| generators              | 80.1 ms                                                | 56.3 ms: 1.42x faster                                     |
| scimark_fft             | 466 ms                                                 | 337 ms: 1.38x faster                                      |
| scimark_monte_carlo     | 118 ms                                                 | 85.8 ms: 1.38x faster                                     |
| spectral_norm           | 170 ms                                                 | 124 ms: 1.37x faster                                      |
| deepcopy_memo           | 58.5 us                                                | 45.1 us: 1.30x faster                                     |
| chaos                   | 115 ms                                                 | 91.1 ms: 1.27x faster                                     |
| mako                    | 16.3 ms                                                | 13.1 ms: 1.25x faster                                     |
| scimark_sor             | 220 ms                                                 | 176 ms: 1.24x faster                                      |
| pyflate                 | 716 ms                                                 | 580 ms: 1.24x faster                                      |
| float                   | 117 ms                                                 | 94.9 ms: 1.23x faster                                     |
| hexiom                  | 10.4 ms                                                | 8.43 ms: 1.23x faster                                     |
| coroutines              | 35.1 ms                                                | 28.6 ms: 1.23x faster                                     |
| crypto_pyaes            | 128 ms                                                 | 106 ms: 1.21x faster                                      |
| regex_compile           | 188 ms                                                 | 157 ms: 1.20x faster                                      |
| nqueens                 | 106 ms                                                 | 88.6 ms: 1.19x faster                                     |
| deepcopy                | 479 us                                                 | 404 us: 1.19x faster                                      |
| dulwich_log             | 84.3 ms                                                | 71.2 ms: 1.18x faster                                     |
| go                      | 240 ms                                                 | 203 ms: 1.18x faster                                      |
| unpickle_pure_python    | 331 us                                                 | 279 us: 1.18x faster                                      |
| deepcopy_reduce         | 4.17 us                                                | 3.55 us: 1.18x faster                                     |
| sqlalchemy_imperative   | 23.3 ms                                                | 19.9 ms: 1.17x faster                                     |
| richards                | 79.3 ms                                                | 67.6 ms: 1.17x faster                                     |
| telco                   | 7.27 ms                                                | 6.27 ms: 1.16x faster                                     |
| html5lib                | 88.9 ms                                                | 76.8 ms: 1.16x faster                                     |
| gunicorn                | 1.53 ms                                                | 1.33 ms: 1.15x faster                                     |
| xml_etree_generate      | 99.4 ms                                                | 86.2 ms: 1.15x faster                                     |
| pycparser               | 1.58 sec                                               | 1.37 sec: 1.15x faster                                    |
| aiohttp                 | 1.44 ms                                                | 1.25 ms: 1.15x faster                                     |
| scimark_lu              | 176 ms                                                 | 153 ms: 1.15x faster                                      |
| raytrace                | 507 ms                                                 | 440 ms: 1.15x faster                                      |
| xml_etree_process       | 79.1 ms                                                | 68.9 ms: 1.15x faster                                     |
| chameleon               | 9.68 ms                                                | 8.49 ms: 1.14x faster                                     |
| unpack_sequence         | 60.0 ns                                                | 52.8 ns: 1.14x faster                                     |
| sqlglot_parse           | 2.17 ms                                                | 1.93 ms: 1.12x faster                                     |
| sympy_integrate         | 25.8 ms                                                | 22.9 ms: 1.12x faster                                     |
| pickle_pure_python      | 484 us                                                 | 432 us: 1.12x faster                                      |
| pprint_pformat          | 2.10 sec                                               | 1.88 sec: 1.12x faster                                    |
| sqlglot_transpile       | 2.57 ms                                                | 2.31 ms: 1.12x faster                                     |
| pprint_safe_repr        | 1.02 sec                                               | 914 ms: 1.11x faster                                      |
| 2to3                    | 348 ms                                                 | 313 ms: 1.11x faster                                      |
| tornado_http            | 136 ms                                                 | 123 ms: 1.11x faster                                      |
| meteor_contest          | 120 ms                                                 | 108 ms: 1.11x faster                                      |
| async_tree_io           | 1.77 sec                                               | 1.61 sec: 1.10x faster                                    |
| genshi_text             | 31.8 ms                                                | 29.0 ms: 1.10x faster                                     |
| regex_v8                | 27.8 ms                                                | 25.3 ms: 1.10x faster                                     |
| regex_effbot            | 3.63 ms                                                | 3.31 ms: 1.10x faster                                     |
| sympy_str               | 346 ms                                                 | 316 ms: 1.09x faster                                      |
| deltablue               | 7.91 ms                                                | 7.24 ms: 1.09x faster                                     |
| pickle_list             | 5.08 us                                                | 4.65 us: 1.09x faster                                     |
| genshi_xml              | 66.0 ms                                                | 60.6 ms: 1.09x faster                                     |
| pickle_dict             | 29.6 us                                                | 27.2 us: 1.09x faster                                     |
| xml_etree_iterparse     | 115 ms                                                 | 106 ms: 1.08x faster                                      |
| sympy_sum               | 196 ms                                                 | 181 ms: 1.08x faster                                      |
| logging_format          | 9.09 us                                                | 8.42 us: 1.08x faster                                     |
| pylint                  | 551 ms                                                 | 512 ms: 1.08x faster                                      |
| json_loads              | 31.2 us                                                | 29.0 us: 1.08x faster                                     |
| unpickle_list           | 5.20 us                                                | 4.86 us: 1.07x faster                                     |
| xml_etree_parse         | 168 ms                                                 | 158 ms: 1.07x faster                                      |
| docutils                | 3.30 sec                                               | 3.10 sec: 1.06x faster                                    |
| flaskblogging           | 8.58 ms                                                | 8.07 ms: 1.06x faster                                     |
| sympy_expand            | 566 ms                                                 | 533 ms: 1.06x faster                                      |
| djangocms               | 38.4 us                                                | 36.2 us: 1.06x faster                                     |
| json_dumps              | 14.2 ms                                                | 13.4 ms: 1.06x faster                                     |
| json                    | 5.69 ms                                                | 5.37 ms: 1.06x faster                                     |
| pickle                  | 10.7 us                                                | 10.1 us: 1.06x faster                                     |
| sqlalchemy_declarative  | 172 ms                                                 | 164 ms: 1.05x faster                                      |
| regex_dna               | 227 ms                                                 | 216 ms: 1.05x faster                                      |
| logging_simple          | 8.30 us                                                | 7.90 us: 1.05x faster                                     |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 970 ms: 1.05x faster                                      |
| asyncio_tcp             | 922 ms                                                 | 885 ms: 1.04x faster                                      |
| bench_thread_pool       | 986 us                                                 | 947 us: 1.04x faster                                      |
| thrift                  | 1.07 ms                                                | 1.03 ms: 1.04x faster                                     |
| mdp                     | 2.85 sec                                               | 2.74 sec: 1.04x faster                                    |
| sqlglot_optimize        | 69.2 ms                                                | 66.5 ms: 1.04x faster                                     |
| async_tree_memoization  | 870 ms                                                 | 839 ms: 1.04x faster                                      |
| sqlite_synth            | 3.02 us                                                | 2.93 us: 1.03x faster                                     |
| sqlglot_normalize       | 143 ms                                                 | 139 ms: 1.02x faster                                      |
| python_startup_no_site  | 5.93 ms                                                | 5.80 ms: 1.02x faster                                     |
| pathlib                 | 20.5 ms                                                | 20.1 ms: 1.02x faster                                     |
| pidigits                | 191 ms                                                 | 188 ms: 1.01x faster                                      |
| logging_silent          | 190 ns                                                 | 194 ns: 1.02x slower                                      |
| python_startup          | 14.6 ms                                                | 15.2 ms: 1.04x slower                                     |
| create_gc_cycles        | 1.62 ms                                                | 1.69 ms: 1.04x slower                                     |
| gc_traversal            | 3.62 ms                                                | 3.83 ms: 1.06x slower                                     |
| async_generators        | 444 ms                                                 | 495 ms: 1.11x slower                                      |
| Geometric mean          | (ref)                                                  | 1.12x faster                                              |

Benchmark hidden because not significant (4): async_tree_none, unpickle, bench_mp_pool, django_template
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, dask, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20220720-3.10.1-53f2d50/bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50.json: mypy


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.09x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.03x