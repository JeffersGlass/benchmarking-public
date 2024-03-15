
# Results vs. 3.11.0

- fork: mdboom
- ref: RegCPython
- machine: linux-x86_64
- commit hash: 53f2d50
- commit date: 2022-07-20
- overall geometric mean: 1.14x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.10x slower
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 264 ms                                                 | 313 ms: 1.19x slower                                      |
| chameleon      | 6.70 ms                                                | 8.49 ms: 1.27x slower                                     |
| docutils       | 2.66 sec                                               | 3.10 sec: 1.16x slower                                    |
| html5lib       | 64.8 ms                                                | 76.8 ms: 1.19x slower                                     |
| tornado_http   | 98.1 ms                                                | 123 ms: 1.25x slower                                      |
| Geometric mean | (ref)                                                  | 1.21x slower                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_io           | 1.29 sec                                               | 1.61 sec: 1.25x slower                                    |
| async_tree_cpu_io_mixed | 749 ms                                                 | 970 ms: 1.29x slower                                      |
| async_tree_memoization  | 639 ms                                                 | 839 ms: 1.31x slower                                      |
| async_tree_none         | 528 ms                                                 | 724 ms: 1.37x slower                                      |
| Geometric mean          | (ref)                                                  | 1.31x slower                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 194 ms                                                 | 188 ms: 1.03x faster                                      |
| nbody          | 96.0 ms                                                | 101 ms: 1.05x slower                                      |
| float          | 78.9 ms                                                | 94.9 ms: 1.20x slower                                     |
| Geometric mean | (ref)                                                  | 1.07x slower                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_effbot   | 3.51 ms                                                | 3.31 ms: 1.06x faster                                     |
| regex_dna      | 205 ms                                                 | 216 ms: 1.05x slower                                      |
| regex_v8       | 22.9 ms                                                | 25.3 ms: 1.11x slower                                     |
| regex_compile  | 141 ms                                                 | 157 ms: 1.11x slower                                      |
| Geometric mean | (ref)                                                  | 1.05x slower                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_dict          | 34.6 us                                                | 27.2 us: 1.27x faster                                     |
| pickle               | 11.0 us                                                | 10.1 us: 1.09x faster                                     |
| unpickle_list        | 5.21 us                                                | 4.86 us: 1.07x faster                                     |
| xml_etree_parse      | 164 ms                                                 | 158 ms: 1.04x faster                                      |
| xml_etree_iterparse  | 108 ms                                                 | 106 ms: 1.02x faster                                      |
| json_loads           | 29.2 us                                                | 29.0 us: 1.01x faster                                     |
| pickle_list          | 4.59 us                                                | 4.65 us: 1.01x slower                                     |
| unpickle             | 13.8 us                                                | 14.3 us: 1.03x slower                                     |
| xml_etree_generate   | 81.1 ms                                                | 86.2 ms: 1.06x slower                                     |
| unpickle_pure_python | 242 us                                                 | 279 us: 1.15x slower                                      |
| xml_etree_process    | 56.9 ms                                                | 68.9 ms: 1.21x slower                                     |
| pickle_pure_python   | 320 us                                                 | 432 us: 1.35x slower                                      |
| Geometric mean       | (ref)                                                  | 1.02x slower                                              |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup_no_site | 6.01 ms                                                | 5.80 ms: 1.04x faster                                     |
| python_startup         | 8.56 ms                                                | 15.2 ms: 1.77x slower                                     |
| Geometric mean         | (ref)                                                  | 1.31x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| genshi_xml      | 53.4 ms                                                | 60.6 ms: 1.13x slower                                     |
| mako            | 10.7 ms                                                | 13.1 ms: 1.23x slower                                     |
| genshi_text     | 22.5 ms                                                | 29.0 ms: 1.29x slower                                     |
| django_template | 33.5 ms                                                | 48.4 ms: 1.44x slower                                     |
| Geometric mean  | (ref)                                                  | 1.27x slower                                              |

All benchmarks:
===============

| Benchmark               | bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| generators              | 74.9 ms                                                | 56.3 ms: 1.33x faster                                     |
| pickle_dict             | 34.6 us                                                | 27.2 us: 1.27x faster                                     |
| scimark_sparse_mat_mult | 5.03 ms                                                | 4.29 ms: 1.17x faster                                     |
| fannkuch                | 405 ms                                                 | 369 ms: 1.10x faster                                      |
| telco                   | 6.86 ms                                                | 6.27 ms: 1.09x faster                                     |
| pickle                  | 11.0 us                                                | 10.1 us: 1.09x faster                                     |
| unpickle_list           | 5.21 us                                                | 4.86 us: 1.07x faster                                     |
| regex_effbot            | 3.51 ms                                                | 3.31 ms: 1.06x faster                                     |
| gc_traversal            | 4.01 ms                                                | 3.83 ms: 1.05x faster                                     |
| xml_etree_parse         | 164 ms                                                 | 158 ms: 1.04x faster                                      |
| python_startup_no_site  | 6.01 ms                                                | 5.80 ms: 1.04x faster                                     |
| pidigits                | 194 ms                                                 | 188 ms: 1.03x faster                                      |
| scimark_fft             | 345 ms                                                 | 337 ms: 1.02x faster                                      |
| xml_etree_iterparse     | 108 ms                                                 | 106 ms: 1.02x faster                                      |
| mdp                     | 2.77 sec                                               | 2.74 sec: 1.01x faster                                    |
| meteor_contest          | 109 ms                                                 | 108 ms: 1.01x faster                                      |
| json_loads              | 29.2 us                                                | 29.0 us: 1.01x faster                                     |
| nqueens                 | 87.9 ms                                                | 88.6 ms: 1.01x slower                                     |
| asyncio_tcp             | 875 ms                                                 | 885 ms: 1.01x slower                                      |
| pickle_list             | 4.59 us                                                | 4.65 us: 1.01x slower                                     |
| json                    | 5.24 ms                                                | 5.37 ms: 1.02x slower                                     |
| unpickle                | 13.8 us                                                | 14.3 us: 1.03x slower                                     |
| nbody                   | 96.0 ms                                                | 101 ms: 1.05x slower                                      |
| regex_dna               | 205 ms                                                 | 216 ms: 1.05x slower                                      |
| coroutines              | 27.0 ms                                                | 28.6 ms: 1.06x slower                                     |
| sympy_str               | 297 ms                                                 | 316 ms: 1.06x slower                                      |
| xml_etree_generate      | 81.1 ms                                                | 86.2 ms: 1.06x slower                                     |
| sympy_integrate         | 21.5 ms                                                | 22.9 ms: 1.07x slower                                     |
| sympy_sum               | 169 ms                                                 | 181 ms: 1.07x slower                                      |
| pylint                  | 476 ms                                                 | 512 ms: 1.08x slower                                      |
| djangocms               | 33.5 us                                                | 36.2 us: 1.08x slower                                     |
| pathlib                 | 18.5 ms                                                | 20.1 ms: 1.08x slower                                     |
| sqlalchemy_imperative   | 18.3 ms                                                | 19.9 ms: 1.09x slower                                     |
| sympy_expand            | 484 ms                                                 | 533 ms: 1.10x slower                                      |
| dulwich_log             | 64.6 ms                                                | 71.2 ms: 1.10x slower                                     |
| deepcopy_reduce         | 3.22 us                                                | 3.55 us: 1.10x slower                                     |
| deepcopy                | 365 us                                                 | 404 us: 1.11x slower                                      |
| flaskblogging           | 7.28 ms                                                | 8.07 ms: 1.11x slower                                     |
| regex_v8                | 22.9 ms                                                | 25.3 ms: 1.11x slower                                     |
| gunicorn                | 1.20 ms                                                | 1.33 ms: 1.11x slower                                     |
| regex_compile           | 141 ms                                                 | 157 ms: 1.11x slower                                      |
| aiohttp                 | 1.12 ms                                                | 1.25 ms: 1.12x slower                                     |
| deepcopy_memo           | 40.2 us                                                | 45.1 us: 1.12x slower                                     |
| genshi_xml              | 53.4 ms                                                | 60.6 ms: 1.13x slower                                     |
| bench_thread_pool       | 834 us                                                 | 947 us: 1.14x slower                                      |
| sqlite_synth            | 2.57 us                                                | 2.93 us: 1.14x slower                                     |
| spectral_norm           | 108 ms                                                 | 124 ms: 1.15x slower                                      |
| pycparser               | 1.19 sec                                               | 1.37 sec: 1.15x slower                                    |
| unpickle_pure_python    | 242 us                                                 | 279 us: 1.15x slower                                      |
| docutils                | 2.66 sec                                               | 3.10 sec: 1.16x slower                                    |
| sqlalchemy_declarative  | 140 ms                                                 | 164 ms: 1.17x slower                                      |
| create_gc_cycles        | 1.43 ms                                                | 1.69 ms: 1.18x slower                                     |
| html5lib                | 64.8 ms                                                | 76.8 ms: 1.19x slower                                     |
| 2to3                    | 264 ms                                                 | 313 ms: 1.19x slower                                      |
| float                   | 78.9 ms                                                | 94.9 ms: 1.20x slower                                     |
| sqlglot_optimize        | 55.3 ms                                                | 66.5 ms: 1.20x slower                                     |
| xml_etree_process       | 56.9 ms                                                | 68.9 ms: 1.21x slower                                     |
| pprint_pformat          | 1.55 sec                                               | 1.88 sec: 1.21x slower                                    |
| scimark_monte_carlo     | 70.7 ms                                                | 85.8 ms: 1.21x slower                                     |
| unpack_sequence         | 43.5 ns                                                | 52.8 ns: 1.21x slower                                     |
| hexiom                  | 6.89 ms                                                | 8.43 ms: 1.22x slower                                     |
| pprint_safe_repr        | 747 ms                                                 | 914 ms: 1.22x slower                                      |
| mako                    | 10.7 ms                                                | 13.1 ms: 1.23x slower                                     |
| logging_format          | 6.81 us                                                | 8.42 us: 1.24x slower                                     |
| sqlglot_normalize       | 113 ms                                                 | 139 ms: 1.24x slower                                      |
| async_tree_io           | 1.29 sec                                               | 1.61 sec: 1.25x slower                                    |
| tornado_http            | 98.1 ms                                                | 123 ms: 1.25x slower                                      |
| chameleon               | 6.70 ms                                                | 8.49 ms: 1.27x slower                                     |
| chaos                   | 71.9 ms                                                | 91.1 ms: 1.27x slower                                     |
| logging_simple          | 6.22 us                                                | 7.90 us: 1.27x slower                                     |
| genshi_text             | 22.5 ms                                                | 29.0 ms: 1.29x slower                                     |
| async_tree_cpu_io_mixed | 749 ms                                                 | 970 ms: 1.29x slower                                      |
| thrift                  | 784 us                                                 | 1.03 ms: 1.31x slower                                     |
| async_tree_memoization  | 639 ms                                                 | 839 ms: 1.31x slower                                      |
| scimark_lu              | 116 ms                                                 | 153 ms: 1.31x slower                                      |
| sqlglot_transpile       | 1.75 ms                                                | 2.31 ms: 1.32x slower                                     |
| async_generators        | 374 ms                                                 | 495 ms: 1.32x slower                                      |
| pyflate                 | 434 ms                                                 | 580 ms: 1.34x slower                                      |
| sqlglot_parse           | 1.43 ms                                                | 1.93 ms: 1.35x slower                                     |
| pickle_pure_python      | 320 us                                                 | 432 us: 1.35x slower                                      |
| richards                | 49.8 ms                                                | 67.6 ms: 1.36x slower                                     |
| go                      | 149 ms                                                 | 203 ms: 1.36x slower                                      |
| async_tree_none         | 528 ms                                                 | 724 ms: 1.37x slower                                      |
| crypto_pyaes            | 76.7 ms                                                | 106 ms: 1.38x slower                                      |
| raytrace                | 309 ms                                                 | 440 ms: 1.43x slower                                      |
| django_template         | 33.5 ms                                                | 48.4 ms: 1.44x slower                                     |
| scimark_sor             | 121 ms                                                 | 176 ms: 1.45x slower                                      |
| logging_silent          | 111 ns                                                 | 194 ns: 1.74x slower                                      |
| python_startup          | 8.56 ms                                                | 15.2 ms: 1.77x slower                                     |
| deltablue               | 3.92 ms                                                | 7.24 ms: 1.84x slower                                     |
| Geometric mean          | (ref)                                                  | 1.14x slower                                              |

Benchmark hidden because not significant (2): bench_mp_pool, json_dumps
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-linux-x86_64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, dask, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (1) of results/bm-20220720-3.10.1-53f2d50/bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50.json: mypy


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.11x
- 99% likely to have a slowdown of 1.10x


# Memory

- memory change: 0.96x