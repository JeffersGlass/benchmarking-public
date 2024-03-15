
# Results vs. 3.12.0

- fork: mdboom
- ref: RegCPython
- machine: linux-x86_64
- commit hash: 53f2d50
- commit date: 2022-07-20
- overall geometric mean: 1.14x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x slower
- Memory change: 0.91x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 313 ms: 1.14x slower                                      |
| chameleon      | 7.41 ms                                                | 8.49 ms: 1.15x slower                                     |
| docutils       | 2.77 sec                                               | 3.10 sec: 1.12x slower                                    |
| tornado_http   | 103 ms                                                 | 123 ms: 1.20x slower                                      |
| Geometric mean | (ref)                                                  | 1.15x slower                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 970 ms: 1.34x slower                                      |
| async_tree_io           | 1.16 sec                                               | 1.61 sec: 1.39x slower                                    |
| async_tree_memoization  | 578 ms                                                 | 839 ms: 1.45x slower                                      |
| async_tree_none         | 472 ms                                                 | 724 ms: 1.53x slower                                      |
| Geometric mean          | (ref)                                                  | 1.43x slower                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 188 ms: 1.00x slower                                      |
| nbody          | 97.0 ms                                                | 101 ms: 1.04x slower                                      |
| float          | 84.7 ms                                                | 94.9 ms: 1.12x slower                                     |
| Geometric mean | (ref)                                                  | 1.05x slower                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.31 ms: 1.09x faster                                     |
| regex_dna      | 212 ms                                                 | 216 ms: 1.02x slower                                      |
| regex_compile  | 148 ms                                                 | 157 ms: 1.06x slower                                      |
| regex_v8       | 23.1 ms                                                | 25.3 ms: 1.10x slower                                     |
| Geometric mean | (ref)                                                  | 1.02x slower                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_dict          | 35.5 us                                                | 27.2 us: 1.31x faster                                     |
| pickle               | 11.6 us                                                | 10.1 us: 1.15x faster                                     |
| unpickle             | 15.9 us                                                | 14.3 us: 1.11x faster                                     |
| pickle_list          | 5.08 us                                                | 4.65 us: 1.09x faster                                     |
| unpickle_list        | 5.29 us                                                | 4.86 us: 1.09x faster                                     |
| xml_etree_generate   | 89.2 ms                                                | 86.2 ms: 1.03x faster                                     |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                      |
| json_loads           | 28.5 us                                                | 29.0 us: 1.02x slower                                     |
| xml_etree_process    | 61.7 ms                                                | 68.9 ms: 1.12x slower                                     |
| unpickle_pure_python | 230 us                                                 | 279 us: 1.21x slower                                      |
| json_dumps           | 10.4 ms                                                | 13.4 ms: 1.29x slower                                     |
| pickle_pure_python   | 324 us                                                 | 432 us: 1.33x slower                                      |
| Geometric mean       | (ref)                                                  | 1.01x slower                                              |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 5.80 ms: 1.20x faster                                     |
| python_startup         | 9.55 ms                                                | 15.2 ms: 1.59x slower                                     |
| Geometric mean         | (ref)                                                  | 1.15x slower                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-----------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| mako            | 11.9 ms                                                | 13.1 ms: 1.10x slower                                     |
| django_template | 34.6 ms                                                | 48.4 ms: 1.40x slower                                     |
| Geometric mean  | (ref)                                                  | 1.24x slower                                              |

All benchmarks:
===============

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------:|
| pickle_dict             | 35.5 us                                                | 27.2 us: 1.31x faster                                     |
| python_startup_no_site  | 6.94 ms                                                | 5.80 ms: 1.20x faster                                     |
| scimark_sparse_mat_mult | 5.06 ms                                                | 4.29 ms: 1.18x faster                                     |
| pickle                  | 11.6 us                                                | 10.1 us: 1.15x faster                                     |
| scimark_fft             | 382 ms                                                 | 337 ms: 1.13x faster                                      |
| telco                   | 7.10 ms                                                | 6.27 ms: 1.13x faster                                     |
| fannkuch                | 417 ms                                                 | 369 ms: 1.13x faster                                      |
| unpickle                | 15.9 us                                                | 14.3 us: 1.11x faster                                     |
| pickle_list             | 5.08 us                                                | 4.65 us: 1.09x faster                                     |
| regex_effbot            | 3.61 ms                                                | 3.31 ms: 1.09x faster                                     |
| unpickle_list           | 5.29 us                                                | 4.86 us: 1.09x faster                                     |
| meteor_contest          | 112 ms                                                 | 108 ms: 1.04x faster                                      |
| xml_etree_generate      | 89.2 ms                                                | 86.2 ms: 1.03x faster                                     |
| unpack_sequence         | 54.0 ns                                                | 52.8 ns: 1.02x faster                                     |
| xml_etree_parse         | 159 ms                                                 | 158 ms: 1.01x faster                                      |
| pidigits                | 187 ms                                                 | 188 ms: 1.00x slower                                      |
| gc_traversal            | 3.79 ms                                                | 3.83 ms: 1.01x slower                                     |
| regex_dna               | 212 ms                                                 | 216 ms: 1.02x slower                                      |
| json_loads              | 28.5 us                                                | 29.0 us: 1.02x slower                                     |
| json                    | 5.26 ms                                                | 5.37 ms: 1.02x slower                                     |
| sqlite_synth            | 2.83 us                                                | 2.93 us: 1.03x slower                                     |
| pathlib                 | 19.3 ms                                                | 20.1 ms: 1.04x slower                                     |
| dulwich_log             | 68.5 ms                                                | 71.2 ms: 1.04x slower                                     |
| mdp                     | 2.63 sec                                               | 2.74 sec: 1.04x slower                                    |
| nbody                   | 97.0 ms                                                | 101 ms: 1.04x slower                                      |
| sympy_str               | 300 ms                                                 | 316 ms: 1.06x slower                                      |
| regex_compile           | 148 ms                                                 | 157 ms: 1.06x slower                                      |
| deepcopy_reduce         | 3.35 us                                                | 3.55 us: 1.06x slower                                     |
| nqueens                 | 83.3 ms                                                | 88.6 ms: 1.06x slower                                     |
| sqlalchemy_imperative   | 18.7 ms                                                | 19.9 ms: 1.06x slower                                     |
| async_generators        | 463 ms                                                 | 495 ms: 1.07x slower                                      |
| gunicorn                | 1.24 ms                                                | 1.33 ms: 1.07x slower                                     |
| sympy_integrate         | 21.4 ms                                                | 22.9 ms: 1.07x slower                                     |
| sympy_sum               | 169 ms                                                 | 181 ms: 1.07x slower                                      |
| spectral_norm           | 115 ms                                                 | 124 ms: 1.08x slower                                      |
| aiohttp                 | 1.15 ms                                                | 1.25 ms: 1.09x slower                                     |
| deepcopy                | 371 us                                                 | 404 us: 1.09x slower                                      |
| regex_v8                | 23.1 ms                                                | 25.3 ms: 1.10x slower                                     |
| mako                    | 11.9 ms                                                | 13.1 ms: 1.10x slower                                     |
| deepcopy_memo           | 40.7 us                                                | 45.1 us: 1.11x slower                                     |
| sympy_expand            | 478 ms                                                 | 533 ms: 1.11x slower                                      |
| sqlalchemy_declarative  | 147 ms                                                 | 164 ms: 1.12x slower                                      |
| xml_etree_process       | 61.7 ms                                                | 68.9 ms: 1.12x slower                                     |
| docutils                | 2.77 sec                                               | 3.10 sec: 1.12x slower                                    |
| float                   | 84.7 ms                                                | 94.9 ms: 1.12x slower                                     |
| bench_thread_pool       | 842 us                                                 | 947 us: 1.13x slower                                      |
| scimark_monte_carlo     | 75.1 ms                                                | 85.8 ms: 1.14x slower                                     |
| 2to3                    | 274 ms                                                 | 313 ms: 1.14x slower                                      |
| create_gc_cycles        | 1.48 ms                                                | 1.69 ms: 1.15x slower                                     |
| chameleon               | 7.41 ms                                                | 8.49 ms: 1.15x slower                                     |
| pycparser               | 1.18 sec                                               | 1.37 sec: 1.16x slower                                    |
| logging_format          | 7.23 us                                                | 8.42 us: 1.16x slower                                     |
| pprint_safe_repr        | 776 ms                                                 | 914 ms: 1.18x slower                                      |
| tornado_http            | 103 ms                                                 | 123 ms: 1.20x slower                                      |
| pprint_pformat          | 1.57 sec                                               | 1.88 sec: 1.20x slower                                    |
| pyflate                 | 482 ms                                                 | 580 ms: 1.20x slower                                      |
| sqlglot_optimize        | 54.8 ms                                                | 66.5 ms: 1.21x slower                                     |
| unpickle_pure_python    | 230 us                                                 | 279 us: 1.21x slower                                      |
| logging_simple          | 6.46 us                                                | 7.90 us: 1.22x slower                                     |
| coroutines              | 23.2 ms                                                | 28.6 ms: 1.24x slower                                     |
| sqlglot_normalize       | 110 ms                                                 | 139 ms: 1.26x slower                                      |
| json_dumps              | 10.4 ms                                                | 13.4 ms: 1.29x slower                                     |
| crypto_pyaes            | 81.9 ms                                                | 106 ms: 1.29x slower                                      |
| scimark_lu              | 118 ms                                                 | 153 ms: 1.30x slower                                      |
| hexiom                  | 6.41 ms                                                | 8.43 ms: 1.31x slower                                     |
| pickle_pure_python      | 324 us                                                 | 432 us: 1.33x slower                                      |
| async_tree_cpu_io_mixed | 726 ms                                                 | 970 ms: 1.34x slower                                      |
| chaos                   | 67.0 ms                                                | 91.1 ms: 1.36x slower                                     |
| scimark_sor             | 129 ms                                                 | 176 ms: 1.37x slower                                      |
| sqlglot_transpile       | 1.68 ms                                                | 2.31 ms: 1.37x slower                                     |
| async_tree_io           | 1.16 sec                                               | 1.61 sec: 1.39x slower                                    |
| django_template         | 34.6 ms                                                | 48.4 ms: 1.40x slower                                     |
| raytrace                | 312 ms                                                 | 440 ms: 1.41x slower                                      |
| sqlglot_parse           | 1.36 ms                                                | 1.93 ms: 1.42x slower                                     |
| async_tree_memoization  | 578 ms                                                 | 839 ms: 1.45x slower                                      |
| go                      | 139 ms                                                 | 203 ms: 1.45x slower                                      |
| richards                | 45.8 ms                                                | 67.6 ms: 1.47x slower                                     |
| async_tree_none         | 472 ms                                                 | 724 ms: 1.53x slower                                      |
| python_startup          | 9.55 ms                                                | 15.2 ms: 1.59x slower                                     |
| asyncio_tcp             | 491 ms                                                 | 885 ms: 1.80x slower                                      |
| generators              | 31.2 ms                                                | 56.3 ms: 1.80x slower                                     |
| logging_silent          | 104 ns                                                 | 194 ns: 1.85x slower                                      |
| deltablue               | 3.72 ms                                                | 7.24 ms: 1.95x slower                                     |
| Geometric mean          | (ref)                                                  | 1.14x slower                                              |

Benchmark hidden because not significant (2): xml_etree_iterparse, bench_mp_pool
Ignored benchmarks (13) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, asyncio_websockets, comprehensions, coverage, dask, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (8) of results/bm-20220720-3.10.1-53f2d50/bm-20220720-linux-x86_64-mdboom-RegCPython-3.10.1-53f2d50.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, mypy, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.10x
- 99% likely to have a slowdown of 1.08x


# Memory

- memory change: 0.91x