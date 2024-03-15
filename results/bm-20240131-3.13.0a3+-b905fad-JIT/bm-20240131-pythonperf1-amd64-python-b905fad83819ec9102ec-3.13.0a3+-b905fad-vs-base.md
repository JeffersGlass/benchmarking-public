# Results vs. base

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.01x slower
- HPT reliability: 72.95%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 216 ms                                                                                                                 | 222 ms: 1.03x slower                                                                                                       |
| chameleon      | 4.93 ms                                                                                                                | 4.72 ms: 1.05x faster                                                                                                      |
| docutils       | 1.59 sec                                                                                                               | 1.60 sec: 1.01x slower                                                                                                     |
| Geometric mean | (ref)                                                                                                                  | 1.00x faster                                                                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| async_tree_none_tg         | 283 ms                                                                                                                 | 273 ms: 1.04x faster                                                                                                       |
| async_tree_memoization_tg  | 368 ms                                                                                                                 | 358 ms: 1.03x faster                                                                                                       |
| async_tree_cpu_io_mixed_tg | 484 ms                                                                                                                 | 473 ms: 1.02x faster                                                                                                       |
| async_tree_cpu_io_mixed    | 473 ms                                                                                                                 | 462 ms: 1.02x faster                                                                                                       |
| async_tree_io_tg           | 787 ms                                                                                                                 | 770 ms: 1.02x faster                                                                                                       |
| async_tree_io              | 763 ms                                                                                                                 | 749 ms: 1.02x faster                                                                                                       |
| async_tree_memoization     | 356 ms                                                                                                                 | 350 ms: 1.02x faster                                                                                                       |
| Geometric mean             | (ref)                                                                                                                  | 1.02x faster                                                                                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody          | 72.0 ms                                                                                                                | 63.0 ms: 1.14x faster                                                                                                      |
| float          | 54.1 ms                                                                                                                | 52.0 ms: 1.04x faster                                                                                                      |
| pidigits       | 149 ms                                                                                                                 | 154 ms: 1.04x slower                                                                                                       |
| Geometric mean | (ref)                                                                                                                  | 1.05x faster                                                                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 1.59 ms                                                                                                                | 1.62 ms: 1.02x slower                                                                                                      |
| regex_compile  | 79.0 ms                                                                                                                | 81.6 ms: 1.03x slower                                                                                                      |
| regex_dna      | 117 ms                                                                                                                 | 125 ms: 1.07x slower                                                                                                       |
| regex_v8       | 14.6 ms                                                                                                                | 17.0 ms: 1.16x slower                                                                                                      |
| Geometric mean | (ref)                                                                                                                  | 1.07x slower                                                                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| tomli_loads          | 1.42 sec                                                                                                               | 1.28 sec: 1.11x faster                                                                                                     |
| pickle_dict          | 18.9 us                                                                                                                | 17.9 us: 1.06x faster                                                                                                      |
| xml_etree_process    | 37.6 ms                                                                                                                | 35.7 ms: 1.05x faster                                                                                                      |
| unpickle_pure_python | 133 us                                                                                                                 | 127 us: 1.05x faster                                                                                                       |
| pickle_pure_python   | 184 us                                                                                                                 | 177 us: 1.04x faster                                                                                                       |
| xml_etree_generate   | 53.9 ms                                                                                                                | 51.8 ms: 1.04x faster                                                                                                      |
| json_dumps           | 5.61 ms                                                                                                                | 5.51 ms: 1.02x faster                                                                                                      |
| xml_etree_parse      | 95.6 ms                                                                                                                | 94.0 ms: 1.02x faster                                                                                                      |
| json_loads           | 13.9 us                                                                                                                | 13.7 us: 1.01x faster                                                                                                      |
| pickle               | 7.15 us                                                                                                                | 7.21 us: 1.01x slower                                                                                                      |
| unpickle_list        | 2.72 us                                                                                                                | 2.77 us: 1.02x slower                                                                                                      |
| unpickle             | 8.45 us                                                                                                                | 9.00 us: 1.06x slower                                                                                                      |
| Geometric mean       | (ref)                                                                                                                  | 1.02x faster                                                                                                               |

Benchmark hidden because not significant (2): pickle_list, xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 20.5 ms                                                                                                                | 21.6 ms: 1.06x slower                                                                                                      |
| python_startup_no_site | 18.5 ms                                                                                                                | 19.6 ms: 1.06x slower                                                                                                      |
| Geometric mean         | (ref)                                                                                                                  | 1.06x slower                                                                                                               |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-JIT/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody                      | 72.0 ms                                                                                                                | 63.0 ms: 1.14x faster                                                                                                      |
| json                       | 3.26 ms                                                                                                                | 2.91 ms: 1.12x faster                                                                                                      |
| richards                   | 28.4 ms                                                                                                                | 25.4 ms: 1.12x faster                                                                                                      |
| tomli_loads                | 1.42 sec                                                                                                               | 1.28 sec: 1.11x faster                                                                                                     |
| richards_super             | 31.6 ms                                                                                                                | 28.5 ms: 1.11x faster                                                                                                      |
| generators                 | 21.8 ms                                                                                                                | 20.2 ms: 1.08x faster                                                                                                      |
| asyncio_tcp_ssl            | 1.87 sec                                                                                                               | 1.74 sec: 1.07x faster                                                                                                     |
| scimark_sor                | 81.5 ms                                                                                                                | 76.1 ms: 1.07x faster                                                                                                      |
| pickle_dict                | 18.9 us                                                                                                                | 17.9 us: 1.06x faster                                                                                                      |
| deepcopy_memo              | 23.0 us                                                                                                                | 21.8 us: 1.05x faster                                                                                                      |
| xml_etree_process          | 37.6 ms                                                                                                                | 35.7 ms: 1.05x faster                                                                                                      |
| unpickle_pure_python       | 133 us                                                                                                                 | 127 us: 1.05x faster                                                                                                       |
| chameleon                  | 4.93 ms                                                                                                                | 4.72 ms: 1.05x faster                                                                                                      |
| pickle_pure_python         | 184 us                                                                                                                 | 177 us: 1.04x faster                                                                                                       |
| xml_etree_generate         | 53.9 ms                                                                                                                | 51.8 ms: 1.04x faster                                                                                                      |
| float                      | 54.1 ms                                                                                                                | 52.0 ms: 1.04x faster                                                                                                      |
| async_tree_none_tg         | 283 ms                                                                                                                 | 273 ms: 1.04x faster                                                                                                       |
| pycparser                  | 710 ms                                                                                                                 | 688 ms: 1.03x faster                                                                                                       |
| logging_format             | 6.61 us                                                                                                                | 6.42 us: 1.03x faster                                                                                                      |
| logging_silent             | 54.8 ns                                                                                                                | 53.2 ns: 1.03x faster                                                                                                      |
| coverage                   | 48.0 ms                                                                                                                | 46.6 ms: 1.03x faster                                                                                                      |
| async_tree_memoization_tg  | 368 ms                                                                                                                 | 358 ms: 1.03x faster                                                                                                       |
| deepcopy_reduce            | 2.02 us                                                                                                                | 1.96 us: 1.03x faster                                                                                                      |
| async_tree_cpu_io_mixed_tg | 484 ms                                                                                                                 | 473 ms: 1.02x faster                                                                                                       |
| async_tree_cpu_io_mixed    | 473 ms                                                                                                                 | 462 ms: 1.02x faster                                                                                                       |
| sqlglot_parse              | 775 us                                                                                                                 | 757 us: 1.02x faster                                                                                                       |
| async_tree_io_tg           | 787 ms                                                                                                                 | 770 ms: 1.02x faster                                                                                                       |
| gc_traversal               | 1.54 ms                                                                                                                | 1.50 ms: 1.02x faster                                                                                                      |
| sqlite_synth               | 1.59 us                                                                                                                | 1.56 us: 1.02x faster                                                                                                      |
| asyncio_tcp                | 503 ms                                                                                                                 | 492 ms: 1.02x faster                                                                                                       |
| async_tree_io              | 763 ms                                                                                                                 | 749 ms: 1.02x faster                                                                                                       |
| typing_runtime_protocols   | 71.4 us                                                                                                                | 70.2 us: 1.02x faster                                                                                                      |
| json_dumps                 | 5.61 ms                                                                                                                | 5.51 ms: 1.02x faster                                                                                                      |
| xml_etree_parse            | 95.6 ms                                                                                                                | 94.0 ms: 1.02x faster                                                                                                      |
| async_tree_memoization     | 356 ms                                                                                                                 | 350 ms: 1.02x faster                                                                                                       |
| logging_simple             | 6.06 us                                                                                                                | 5.97 us: 1.01x faster                                                                                                      |
| json_loads                 | 13.9 us                                                                                                                | 13.7 us: 1.01x faster                                                                                                      |
| sqlglot_transpile          | 1.00 ms                                                                                                                | 990 us: 1.01x faster                                                                                                       |
| coroutines                 | 13.1 ms                                                                                                                | 12.9 ms: 1.01x faster                                                                                                      |
| dulwich_log                | 42.5 ms                                                                                                                | 42.0 ms: 1.01x faster                                                                                                      |
| deepcopy                   | 224 us                                                                                                                 | 222 us: 1.01x faster                                                                                                       |
| scimark_lu                 | 55.2 ms                                                                                                                | 55.5 ms: 1.01x slower                                                                                                      |
| docutils                   | 1.59 sec                                                                                                               | 1.60 sec: 1.01x slower                                                                                                     |
| pickle                     | 7.15 us                                                                                                                | 7.21 us: 1.01x slower                                                                                                      |
| fannkuch                   | 246 ms                                                                                                                 | 248 ms: 1.01x slower                                                                                                       |
| pprint_pformat             | 1.02 sec                                                                                                               | 1.03 sec: 1.02x slower                                                                                                     |
| deltablue                  | 2.06 ms                                                                                                                | 2.10 ms: 1.02x slower                                                                                                      |
| nqueens                    | 58.6 ms                                                                                                                | 59.5 ms: 1.02x slower                                                                                                      |
| unpack_sequence            | 39.0 ns                                                                                                                | 39.8 ns: 1.02x slower                                                                                                      |
| unpickle_list              | 2.72 us                                                                                                                | 2.77 us: 1.02x slower                                                                                                      |
| regex_effbot               | 1.59 ms                                                                                                                | 1.62 ms: 1.02x slower                                                                                                      |
| sqlglot_optimize           | 33.9 ms                                                                                                                | 34.6 ms: 1.02x slower                                                                                                      |
| sympy_expand               | 275 ms                                                                                                                 | 282 ms: 1.02x slower                                                                                                       |
| 2to3                       | 216 ms                                                                                                                 | 222 ms: 1.03x slower                                                                                                       |
| sqlglot_normalize          | 175 ms                                                                                                                 | 180 ms: 1.03x slower                                                                                                       |
| regex_compile              | 79.0 ms                                                                                                                | 81.6 ms: 1.03x slower                                                                                                      |
| mypy2                      | 421 ms                                                                                                                 | 436 ms: 1.03x slower                                                                                                       |
| pidigits                   | 149 ms                                                                                                                 | 154 ms: 1.04x slower                                                                                                       |
| raytrace                   | 163 ms                                                                                                                 | 170 ms: 1.04x slower                                                                                                       |
| crypto_pyaes               | 44.8 ms                                                                                                                | 46.8 ms: 1.04x slower                                                                                                      |
| async_generators           | 229 ms                                                                                                                 | 240 ms: 1.05x slower                                                                                                       |
| spectral_norm              | 62.2 ms                                                                                                                | 65.2 ms: 1.05x slower                                                                                                      |
| sympy_integrate            | 12.7 ms                                                                                                                | 13.4 ms: 1.05x slower                                                                                                      |
| python_startup             | 20.5 ms                                                                                                                | 21.6 ms: 1.06x slower                                                                                                      |
| sympy_sum                  | 85.1 ms                                                                                                                | 90.3 ms: 1.06x slower                                                                                                      |
| python_startup_no_site     | 18.5 ms                                                                                                                | 19.6 ms: 1.06x slower                                                                                                      |
| unpickle                   | 8.45 us                                                                                                                | 9.00 us: 1.06x slower                                                                                                      |
| regex_dna                  | 117 ms                                                                                                                 | 125 ms: 1.07x slower                                                                                                       |
| sympy_str                  | 159 ms                                                                                                                 | 169 ms: 1.07x slower                                                                                                       |
| chaos                      | 39.8 ms                                                                                                                | 42.4 ms: 1.07x slower                                                                                                      |
| scimark_sparse_mat_mult    | 2.54 ms                                                                                                                | 2.72 ms: 1.07x slower                                                                                                      |
| pyflate                    | 292 ms                                                                                                                 | 315 ms: 1.08x slower                                                                                                       |
| bench_mp_pool              | 67.7 ms                                                                                                                | 73.2 ms: 1.08x slower                                                                                                      |
| meteor_contest             | 72.8 ms                                                                                                                | 78.7 ms: 1.08x slower                                                                                                      |
| scimark_fft                | 180 ms                                                                                                                 | 197 ms: 1.10x slower                                                                                                       |
| comprehensions             | 10.5 us                                                                                                                | 11.6 us: 1.10x slower                                                                                                      |
| mdp                        | 1.41 sec                                                                                                               | 1.58 sec: 1.13x slower                                                                                                     |
| go                         | 85.7 ms                                                                                                                | 99.3 ms: 1.16x slower                                                                                                      |
| regex_v8                   | 14.6 ms                                                                                                                | 17.0 ms: 1.16x slower                                                                                                      |
| hexiom                     | 3.97 ms                                                                                                                | 5.27 ms: 1.33x slower                                                                                                      |
| scimark_monte_carlo        | 40.8 ms                                                                                                                | 58.0 ms: 1.42x slower                                                                                                      |
| Geometric mean             | (ref)                                                                                                                  | 1.01x slower                                                                                                               |

Benchmark hidden because not significant (11): async_tree_none, pickle_list, xml_etree_iterparse, create_gc_cycles, telco, pathlib, tornado_http, dask, mako, bench_thread_pool, pprint_safe_repr


# HPT report

- Reliability score: 72.95% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown