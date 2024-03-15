# Results vs. base

- fork: python
- ref: b905fad83819ec9102ec
- machine: linux-x86_64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: 1.04x

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 291 ms                                                                                                                  | 299 ms: 1.03x slower                                                                                                        |
| chameleon      | 7.28 ms                                                                                                                 | 7.69 ms: 1.06x slower                                                                                                       |
| docutils       | 2.85 sec                                                                                                                | 2.89 sec: 1.01x slower                                                                                                      |
| tornado_http   | 121 ms                                                                                                                  | 124 ms: 1.03x slower                                                                                                        |
| Geometric mean | (ref)                                                                                                                   | 1.03x slower                                                                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed    | 693 ms                                                                                                                  | 700 ms: 1.01x slower                                                                                                        |
| async_tree_memoization     | 541 ms                                                                                                                  | 550 ms: 1.02x slower                                                                                                        |
| async_tree_io              | 1.06 sec                                                                                                                | 1.08 sec: 1.02x slower                                                                                                      |
| async_tree_cpu_io_mixed_tg | 697 ms                                                                                                                  | 710 ms: 1.02x slower                                                                                                        |
| async_tree_none            | 428 ms                                                                                                                  | 438 ms: 1.02x slower                                                                                                        |
| async_tree_io_tg           | 1.06 sec                                                                                                                | 1.08 sec: 1.02x slower                                                                                                      |
| async_tree_memoization_tg  | 543 ms                                                                                                                  | 558 ms: 1.03x slower                                                                                                        |
| async_tree_none_tg         | 429 ms                                                                                                                  | 442 ms: 1.03x slower                                                                                                        |
| Geometric mean             | (ref)                                                                                                                   | 1.02x slower                                                                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| float          | 79.6 ms                                                                                                                 | 81.7 ms: 1.03x slower                                                                                                       |
| nbody          | 85.6 ms                                                                                                                 | 107 ms: 1.25x slower                                                                                                        |
| Geometric mean | (ref)                                                                                                                   | 1.09x slower                                                                                                                |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 3.67 ms                                                                                                                 | 3.46 ms: 1.06x faster                                                                                                       |
| regex_v8       | 25.8 ms                                                                                                                 | 24.4 ms: 1.06x faster                                                                                                       |
| regex_dna      | 238 ms                                                                                                                  | 232 ms: 1.02x faster                                                                                                        |
| regex_compile  | 139 ms                                                                                                                  | 147 ms: 1.06x slower                                                                                                        |
| Geometric mean | (ref)                                                                                                                   | 1.02x faster                                                                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 15.4 us                                                                                                                 | 14.8 us: 1.04x faster                                                                                                       |
| xml_etree_iterparse  | 109 ms                                                                                                                  | 106 ms: 1.03x faster                                                                                                        |
| unpickle_list        | 4.89 us                                                                                                                 | 4.77 us: 1.02x faster                                                                                                       |
| xml_etree_parse      | 148 ms                                                                                                                  | 147 ms: 1.01x faster                                                                                                        |
| json_loads           | 24.9 us                                                                                                                 | 25.1 us: 1.01x slower                                                                                                       |
| xml_etree_process    | 58.8 ms                                                                                                                 | 59.6 ms: 1.01x slower                                                                                                       |
| pickle_pure_python   | 303 us                                                                                                                  | 308 us: 1.02x slower                                                                                                        |
| xml_etree_generate   | 84.4 ms                                                                                                                 | 86.6 ms: 1.03x slower                                                                                                       |
| json_dumps           | 10.5 ms                                                                                                                 | 10.8 ms: 1.03x slower                                                                                                       |
| pickle_list          | 4.45 us                                                                                                                 | 4.62 us: 1.04x slower                                                                                                       |
| pickle               | 10.1 us                                                                                                                 | 10.6 us: 1.05x slower                                                                                                       |
| tomli_loads          | 2.23 sec                                                                                                                | 2.35 sec: 1.05x slower                                                                                                      |
| pickle_dict          | 30.8 us                                                                                                                 | 32.8 us: 1.06x slower                                                                                                       |
| unpickle_pure_python | 209 us                                                                                                                  | 232 us: 1.11x slower                                                                                                        |
| Geometric mean       | (ref)                                                                                                                   | 1.02x slower                                                                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|------------------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| python_startup_no_site | 11.0 ms                                                                                                                 | 11.1 ms: 1.00x slower                                                                                                       |
| Geometric mean         | (ref)                                                                                                                   | 1.00x slower                                                                                                                |

Benchmark hidden because not significant (1): python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|-----------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| mako      | 10.4 ms                                                                                                                 | 12.0 ms: 1.15x slower                                                                                                       |

All benchmarks:
===============

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf2-x86_64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:-----------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------:|
| unpack_sequence            | 48.8 ns                                                                                                                 | 45.9 ns: 1.06x faster                                                                                                       |
| regex_effbot               | 3.67 ms                                                                                                                 | 3.46 ms: 1.06x faster                                                                                                       |
| regex_v8                   | 25.8 ms                                                                                                                 | 24.4 ms: 1.06x faster                                                                                                       |
| create_gc_cycles           | 1.61 ms                                                                                                                 | 1.54 ms: 1.05x faster                                                                                                       |
| unpickle                   | 15.4 us                                                                                                                 | 14.8 us: 1.04x faster                                                                                                       |
| xml_etree_iterparse        | 109 ms                                                                                                                  | 106 ms: 1.03x faster                                                                                                        |
| unpickle_list              | 4.89 us                                                                                                                 | 4.77 us: 1.02x faster                                                                                                       |
| regex_dna                  | 238 ms                                                                                                                  | 232 ms: 1.02x faster                                                                                                        |
| richards                   | 51.6 ms                                                                                                                 | 50.8 ms: 1.02x faster                                                                                                       |
| xml_etree_parse            | 148 ms                                                                                                                  | 147 ms: 1.01x faster                                                                                                        |
| richards_super             | 57.6 ms                                                                                                                 | 56.9 ms: 1.01x faster                                                                                                       |
| python_startup_no_site     | 11.0 ms                                                                                                                 | 11.1 ms: 1.00x slower                                                                                                       |
| deepcopy_reduce            | 3.32 us                                                                                                                 | 3.33 us: 1.00x slower                                                                                                       |
| logging_silent             | 94.1 ns                                                                                                                 | 94.9 ns: 1.01x slower                                                                                                       |
| json_loads                 | 24.9 us                                                                                                                 | 25.1 us: 1.01x slower                                                                                                       |
| async_tree_cpu_io_mixed    | 693 ms                                                                                                                  | 700 ms: 1.01x slower                                                                                                        |
| deepcopy_memo              | 37.2 us                                                                                                                 | 37.6 us: 1.01x slower                                                                                                       |
| asyncio_tcp_ssl            | 1.57 sec                                                                                                                | 1.59 sec: 1.01x slower                                                                                                      |
| xml_etree_process          | 58.8 ms                                                                                                                 | 59.6 ms: 1.01x slower                                                                                                       |
| docutils                   | 2.85 sec                                                                                                                | 2.89 sec: 1.01x slower                                                                                                      |
| go                         | 166 ms                                                                                                                  | 169 ms: 1.01x slower                                                                                                        |
| asyncio_tcp                | 366 ms                                                                                                                  | 372 ms: 1.01x slower                                                                                                        |
| json                       | 5.16 ms                                                                                                                 | 5.24 ms: 1.02x slower                                                                                                       |
| async_tree_memoization     | 541 ms                                                                                                                  | 550 ms: 1.02x slower                                                                                                        |
| async_tree_io              | 1.06 sec                                                                                                                | 1.08 sec: 1.02x slower                                                                                                      |
| logging_simple             | 6.59 us                                                                                                                 | 6.70 us: 1.02x slower                                                                                                       |
| pycparser                  | 1.26 sec                                                                                                                | 1.28 sec: 1.02x slower                                                                                                      |
| async_tree_cpu_io_mixed_tg | 697 ms                                                                                                                  | 710 ms: 1.02x slower                                                                                                        |
| typing_runtime_protocols   | 117 us                                                                                                                  | 119 us: 1.02x slower                                                                                                        |
| pickle_pure_python         | 303 us                                                                                                                  | 308 us: 1.02x slower                                                                                                        |
| sqlglot_parse              | 1.38 ms                                                                                                                 | 1.41 ms: 1.02x slower                                                                                                       |
| dask                       | 397 ms                                                                                                                  | 406 ms: 1.02x slower                                                                                                        |
| sympy_expand               | 494 ms                                                                                                                  | 505 ms: 1.02x slower                                                                                                        |
| async_tree_none            | 428 ms                                                                                                                  | 438 ms: 1.02x slower                                                                                                        |
| dulwich_log                | 67.2 ms                                                                                                                 | 68.7 ms: 1.02x slower                                                                                                       |
| pathlib                    | 18.7 ms                                                                                                                 | 19.1 ms: 1.02x slower                                                                                                       |
| async_tree_io_tg           | 1.06 sec                                                                                                                | 1.08 sec: 1.02x slower                                                                                                      |
| sqlglot_normalize          | 116 ms                                                                                                                  | 119 ms: 1.02x slower                                                                                                        |
| scimark_sor                | 141 ms                                                                                                                  | 144 ms: 1.02x slower                                                                                                        |
| float                      | 79.6 ms                                                                                                                 | 81.7 ms: 1.03x slower                                                                                                       |
| scimark_lu                 | 98.6 ms                                                                                                                 | 101 ms: 1.03x slower                                                                                                        |
| xml_etree_generate         | 84.4 ms                                                                                                                 | 86.6 ms: 1.03x slower                                                                                                       |
| tornado_http               | 121 ms                                                                                                                  | 124 ms: 1.03x slower                                                                                                        |
| async_tree_memoization_tg  | 543 ms                                                                                                                  | 558 ms: 1.03x slower                                                                                                        |
| sqlglot_transpile          | 1.79 ms                                                                                                                 | 1.84 ms: 1.03x slower                                                                                                       |
| deepcopy                   | 367 us                                                                                                                  | 378 us: 1.03x slower                                                                                                        |
| json_dumps                 | 10.5 ms                                                                                                                 | 10.8 ms: 1.03x slower                                                                                                       |
| 2to3                       | 291 ms                                                                                                                  | 299 ms: 1.03x slower                                                                                                        |
| async_tree_none_tg         | 429 ms                                                                                                                  | 442 ms: 1.03x slower                                                                                                        |
| coroutines                 | 21.8 ms                                                                                                                 | 22.5 ms: 1.03x slower                                                                                                       |
| mdp                        | 2.49 sec                                                                                                                | 2.58 sec: 1.04x slower                                                                                                      |
| pyflate                    | 502 ms                                                                                                                  | 520 ms: 1.04x slower                                                                                                        |
| pickle_list                | 4.45 us                                                                                                                 | 4.62 us: 1.04x slower                                                                                                       |
| sympy_str                  | 289 ms                                                                                                                  | 300 ms: 1.04x slower                                                                                                        |
| gc_traversal               | 3.51 ms                                                                                                                 | 3.65 ms: 1.04x slower                                                                                                       |
| telco                      | 8.02 ms                                                                                                                 | 8.34 ms: 1.04x slower                                                                                                       |
| async_generators           | 360 ms                                                                                                                  | 374 ms: 1.04x slower                                                                                                        |
| sympy_integrate            | 23.2 ms                                                                                                                 | 24.2 ms: 1.05x slower                                                                                                       |
| logging_format             | 7.23 us                                                                                                                 | 7.58 us: 1.05x slower                                                                                                       |
| pickle                     | 10.1 us                                                                                                                 | 10.6 us: 1.05x slower                                                                                                       |
| tomli_loads                | 2.23 sec                                                                                                                | 2.35 sec: 1.05x slower                                                                                                      |
| generators                 | 33.8 ms                                                                                                                 | 35.6 ms: 1.05x slower                                                                                                       |
| sympy_sum                  | 151 ms                                                                                                                  | 159 ms: 1.05x slower                                                                                                        |
| sqlglot_optimize           | 58.4 ms                                                                                                                 | 61.5 ms: 1.05x slower                                                                                                       |
| chameleon                  | 7.28 ms                                                                                                                 | 7.69 ms: 1.06x slower                                                                                                       |
| meteor_contest             | 127 ms                                                                                                                  | 134 ms: 1.06x slower                                                                                                        |
| regex_compile              | 139 ms                                                                                                                  | 147 ms: 1.06x slower                                                                                                        |
| pickle_dict                | 30.8 us                                                                                                                 | 32.8 us: 1.06x slower                                                                                                       |
| pprint_safe_repr           | 805 ms                                                                                                                  | 865 ms: 1.07x slower                                                                                                        |
| fannkuch                   | 385 ms                                                                                                                  | 415 ms: 1.08x slower                                                                                                        |
| pprint_pformat             | 1.66 sec                                                                                                                | 1.79 sec: 1.08x slower                                                                                                      |
| raytrace                   | 258 ms                                                                                                                  | 281 ms: 1.09x slower                                                                                                        |
| bench_mp_pool              | 4.56 ms                                                                                                                 | 5.02 ms: 1.10x slower                                                                                                       |
| coverage                   | 78.7 ms                                                                                                                 | 86.7 ms: 1.10x slower                                                                                                       |
| nqueens                    | 87.5 ms                                                                                                                 | 96.9 ms: 1.11x slower                                                                                                       |
| unpickle_pure_python       | 209 us                                                                                                                  | 232 us: 1.11x slower                                                                                                        |
| deltablue                  | 3.58 ms                                                                                                                 | 4.03 ms: 1.13x slower                                                                                                       |
| mako                       | 10.4 ms                                                                                                                 | 12.0 ms: 1.15x slower                                                                                                       |
| crypto_pyaes               | 69.8 ms                                                                                                                 | 81.5 ms: 1.17x slower                                                                                                       |
| scimark_monte_carlo        | 65.6 ms                                                                                                                 | 79.0 ms: 1.20x slower                                                                                                       |
| chaos                      | 59.0 ms                                                                                                                 | 71.6 ms: 1.21x slower                                                                                                       |
| scimark_fft                | 298 ms                                                                                                                  | 365 ms: 1.22x slower                                                                                                        |
| nbody                      | 85.6 ms                                                                                                                 | 107 ms: 1.25x slower                                                                                                        |
| hexiom                     | 6.31 ms                                                                                                                 | 7.86 ms: 1.25x slower                                                                                                       |
| scimark_sparse_mat_mult    | 4.12 ms                                                                                                                 | 5.14 ms: 1.25x slower                                                                                                       |
| spectral_norm              | 92.6 ms                                                                                                                 | 116 ms: 1.25x slower                                                                                                        |
| comprehensions             | 16.4 us                                                                                                                 | 20.7 us: 1.26x slower                                                                                                       |
| Geometric mean             | (ref)                                                                                                                   | 1.04x slower                                                                                                                |

Benchmark hidden because not significant (6): pidigits, asyncio_websockets, python_startup, sqlite_synth, bench_thread_pool, mypy2


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: 1.04x