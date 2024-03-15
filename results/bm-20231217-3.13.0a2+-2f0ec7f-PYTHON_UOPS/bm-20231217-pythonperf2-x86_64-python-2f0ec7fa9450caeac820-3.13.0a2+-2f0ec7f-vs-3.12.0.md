
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.08x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: 0.88x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| 2to3           | 285 ms                                                       | 308 ms: 1.08x slower                                                         |
| chameleon      | 7.23 ms                                                      | 7.85 ms: 1.09x slower                                                        |
| docutils       | 2.87 sec                                                     | 2.94 sec: 1.02x slower                                                       |
| tornado_http   | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| Geometric mean | (ref)                                                        | 1.06x slower                                                                 |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                         |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 557 ms: 1.02x slower                                                         |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 719 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| async_tree_memoization_tg  | 540 ms                                                       | 565 ms: 1.05x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.03x slower                                                                 |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| float          | 76.6 ms                                                      | 93.7 ms: 1.22x slower                                                        |
| nbody          | 88.0 ms                                                      | 112 ms: 1.27x slower                                                         |
| Geometric mean | (ref)                                                        | 1.16x slower                                                                 |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| regex_effbot   | 3.57 ms                                                      | 3.54 ms: 1.01x faster                                                        |
| regex_dna      | 239 ms                                                       | 245 ms: 1.03x slower                                                         |
| regex_v8       | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                        |
| regex_compile  | 144 ms                                                       | 168 ms: 1.17x slower                                                         |
| Geometric mean | (ref)                                                        | 1.07x slower                                                                 |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| pickle_dict          | 32.5 us                                                      | 31.6 us: 1.03x faster                                                        |
| pickle_pure_python   | 318 us                                                       | 312 us: 1.02x faster                                                         |
| unpickle             | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| pickle               | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| unpickle_list        | 4.66 us                                                      | 4.61 us: 1.01x faster                                                        |
| pickle_list          | 4.43 us                                                      | 4.47 us: 1.01x slower                                                        |
| xml_etree_parse      | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| xml_etree_process    | 58.4 ms                                                      | 60.9 ms: 1.04x slower                                                        |
| json_dumps           | 10.2 ms                                                      | 10.7 ms: 1.04x slower                                                        |
| json_loads           | 24.4 us                                                      | 25.4 us: 1.04x slower                                                        |
| xml_etree_generate   | 86.1 ms                                                      | 90.1 ms: 1.05x slower                                                        |
| xml_etree_iterparse  | 103 ms                                                       | 111 ms: 1.08x slower                                                         |
| unpickle_pure_python | 210 us                                                       | 228 us: 1.09x slower                                                         |
| tomli_loads          | 2.16 sec                                                     | 2.67 sec: 1.24x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.04x slower                                                                 |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| python_startup         | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| python_startup_no_site | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| Geometric mean         | (ref)                                                        | 1.18x slower                                                                 |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| mako      | 10.0 ms                                                      | 13.6 ms: 1.36x slower                                                        |

All benchmarks:
===============

| Benchmark                  | bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-pythonperf2-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------------|:------------------------------------------------------------:|:----------------------------------------------------------------------------:|
| typing_runtime_protocols   | 152 us                                                       | 127 us: 1.19x faster                                                         |
| unpack_sequence            | 53.2 ns                                                      | 46.7 ns: 1.14x faster                                                        |
| generators                 | 37.4 ms                                                      | 33.8 ms: 1.11x faster                                                        |
| async_generators           | 390 ms                                                       | 375 ms: 1.04x faster                                                         |
| pickle_dict                | 32.5 us                                                      | 31.6 us: 1.03x faster                                                        |
| coroutines                 | 23.0 ms                                                      | 22.4 ms: 1.03x faster                                                        |
| pickle_pure_python         | 318 us                                                       | 312 us: 1.02x faster                                                         |
| unpickle                   | 14.8 us                                                      | 14.5 us: 1.02x faster                                                        |
| async_tree_none            | 452 ms                                                       | 444 ms: 1.02x faster                                                         |
| raytrace                   | 298 ms                                                       | 294 ms: 1.01x faster                                                         |
| pickle                     | 10.5 us                                                      | 10.4 us: 1.01x faster                                                        |
| unpickle_list              | 4.66 us                                                      | 4.61 us: 1.01x faster                                                        |
| regex_effbot               | 3.57 ms                                                      | 3.54 ms: 1.01x faster                                                        |
| asyncio_tcp_ssl            | 1.59 sec                                                     | 1.59 sec: 1.00x slower                                                       |
| deepcopy_reduce            | 3.37 us                                                      | 3.39 us: 1.01x slower                                                        |
| pickle_list                | 4.43 us                                                      | 4.47 us: 1.01x slower                                                        |
| logging_simple             | 6.71 us                                                      | 6.80 us: 1.01x slower                                                        |
| mdp                        | 2.57 sec                                                     | 2.61 sec: 1.02x slower                                                       |
| create_gc_cycles           | 1.59 ms                                                      | 1.62 ms: 1.02x slower                                                        |
| crypto_pyaes               | 80.3 ms                                                      | 82.1 ms: 1.02x slower                                                        |
| async_tree_cpu_io_mixed    | 696 ms                                                       | 711 ms: 1.02x slower                                                         |
| async_tree_memoization     | 544 ms                                                       | 557 ms: 1.02x slower                                                         |
| docutils                   | 2.87 sec                                                     | 2.94 sec: 1.02x slower                                                       |
| xml_etree_parse            | 144 ms                                                       | 147 ms: 1.02x slower                                                         |
| gc_traversal               | 3.48 ms                                                      | 3.56 ms: 1.02x slower                                                        |
| bench_thread_pool          | 950 us                                                       | 974 us: 1.03x slower                                                         |
| regex_dna                  | 239 ms                                                       | 245 ms: 1.03x slower                                                         |
| sqlglot_parse              | 1.38 ms                                                      | 1.42 ms: 1.03x slower                                                        |
| sqlglot_transpile          | 1.78 ms                                                      | 1.83 ms: 1.03x slower                                                        |
| async_tree_cpu_io_mixed_tg | 697 ms                                                       | 719 ms: 1.03x slower                                                         |
| async_tree_io_tg           | 1.05 sec                                                     | 1.09 sec: 1.03x slower                                                       |
| async_tree_none_tg         | 431 ms                                                       | 445 ms: 1.03x slower                                                         |
| tornado_http               | 121 ms                                                       | 125 ms: 1.03x slower                                                         |
| pathlib                    | 18.9 ms                                                      | 19.5 ms: 1.03x slower                                                        |
| json                       | 5.12 ms                                                      | 5.31 ms: 1.04x slower                                                        |
| logging_silent             | 94.4 ns                                                      | 97.9 ns: 1.04x slower                                                        |
| sympy_sum                  | 162 ms                                                       | 169 ms: 1.04x slower                                                         |
| xml_etree_process          | 58.4 ms                                                      | 60.9 ms: 1.04x slower                                                        |
| async_tree_io              | 1.04 sec                                                     | 1.09 sec: 1.04x slower                                                       |
| json_dumps                 | 10.2 ms                                                      | 10.7 ms: 1.04x slower                                                        |
| sympy_integrate            | 23.9 ms                                                      | 25.0 ms: 1.04x slower                                                        |
| json_loads                 | 24.4 us                                                      | 25.4 us: 1.04x slower                                                        |
| xml_etree_generate         | 86.1 ms                                                      | 90.1 ms: 1.05x slower                                                        |
| dask                       | 392 ms                                                       | 410 ms: 1.05x slower                                                         |
| deepcopy                   | 368 us                                                       | 386 us: 1.05x slower                                                         |
| async_tree_memoization_tg  | 540 ms                                                       | 565 ms: 1.05x slower                                                         |
| sqlglot_normalize          | 116 ms                                                       | 122 ms: 1.05x slower                                                         |
| comprehensions             | 21.9 us                                                      | 23.1 us: 1.06x slower                                                        |
| sympy_str                  | 302 ms                                                       | 325 ms: 1.08x slower                                                         |
| xml_etree_iterparse        | 103 ms                                                       | 111 ms: 1.08x slower                                                         |
| pycparser                  | 1.23 sec                                                     | 1.33 sec: 1.08x slower                                                       |
| meteor_contest             | 128 ms                                                       | 138 ms: 1.08x slower                                                         |
| regex_v8                   | 23.6 ms                                                      | 25.6 ms: 1.08x slower                                                        |
| 2to3                       | 285 ms                                                       | 308 ms: 1.08x slower                                                         |
| scimark_lu                 | 98.8 ms                                                      | 107 ms: 1.08x slower                                                         |
| python_startup             | 11.6 ms                                                      | 12.6 ms: 1.08x slower                                                        |
| mypy2                      | 830 ms                                                       | 900 ms: 1.08x slower                                                         |
| chameleon                  | 7.23 ms                                                      | 7.85 ms: 1.09x slower                                                        |
| unpickle_pure_python       | 210 us                                                       | 228 us: 1.09x slower                                                         |
| sqlglot_optimize           | 57.5 ms                                                      | 63.0 ms: 1.10x slower                                                        |
| deepcopy_memo              | 36.8 us                                                      | 40.4 us: 1.10x slower                                                        |
| dulwich_log                | 65.4 ms                                                      | 72.6 ms: 1.11x slower                                                        |
| pprint_safe_repr           | 807 ms                                                       | 904 ms: 1.12x slower                                                         |
| pprint_pformat             | 1.65 sec                                                     | 1.86 sec: 1.12x slower                                                       |
| sympy_expand               | 484 ms                                                       | 545 ms: 1.13x slower                                                         |
| chaos                      | 64.0 ms                                                      | 73.7 ms: 1.15x slower                                                        |
| nqueens                    | 89.9 ms                                                      | 104 ms: 1.15x slower                                                         |
| richards_super             | 51.3 ms                                                      | 59.9 ms: 1.17x slower                                                        |
| regex_compile              | 144 ms                                                       | 168 ms: 1.17x slower                                                         |
| telco                      | 6.96 ms                                                      | 8.21 ms: 1.18x slower                                                        |
| richards                   | 45.7 ms                                                      | 54.2 ms: 1.19x slower                                                        |
| go                         | 150 ms                                                       | 183 ms: 1.22x slower                                                         |
| float                      | 76.6 ms                                                      | 93.7 ms: 1.22x slower                                                        |
| scimark_monte_carlo        | 69.0 ms                                                      | 84.6 ms: 1.23x slower                                                        |
| tomli_loads                | 2.16 sec                                                     | 2.67 sec: 1.24x slower                                                       |
| coverage                   | 66.7 ms                                                      | 84.6 ms: 1.27x slower                                                        |
| nbody                      | 88.0 ms                                                      | 112 ms: 1.27x slower                                                         |
| fannkuch                   | 350 ms                                                       | 447 ms: 1.28x slower                                                         |
| python_startup_no_site     | 8.64 ms                                                      | 11.0 ms: 1.28x slower                                                        |
| pyflate                    | 439 ms                                                       | 569 ms: 1.30x slower                                                         |
| scimark_fft                | 301 ms                                                       | 396 ms: 1.31x slower                                                         |
| scimark_sor                | 109 ms                                                       | 148 ms: 1.36x slower                                                         |
| mako                       | 10.0 ms                                                      | 13.6 ms: 1.36x slower                                                        |
| scimark_sparse_mat_mult    | 4.21 ms                                                      | 6.01 ms: 1.43x slower                                                        |
| deltablue                  | 3.24 ms                                                      | 4.94 ms: 1.53x slower                                                        |
| hexiom                     | 5.96 ms                                                      | 9.23 ms: 1.55x slower                                                        |
| spectral_norm              | 91.6 ms                                                      | 150 ms: 1.64x slower                                                         |
| Geometric mean             | (ref)                                                        | 1.08x slower                                                                 |

Benchmark hidden because not significant (6): bench_mp_pool, asyncio_websockets, sqlite_synth, pidigits, asyncio_tcp, logging_format
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf2-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.04x
- 95% likely to have a slowdown of 1.04x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: 0.88x