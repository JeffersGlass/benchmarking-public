# Results vs. base

- fork: python
- ref: 52eade22237eef1f3843
- machine: windows-amd64
- commit hash: 52eade2
- commit date: 2024-01-20
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 213 ms                                                                                                                 | 218 ms: 1.02x slower                                                                                                               |
| chameleon      | 4.90 ms                                                                                                                | 5.01 ms: 1.02x slower                                                                                                              |
| docutils       | 1.53 sec                                                                                                               | 1.59 sec: 1.03x slower                                                                                                             |
| tornado_http   | 86.2 ms                                                                                                                | 87.4 ms: 1.01x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.02x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_none_tg         | 272 ms                                                                                                                 | 276 ms: 1.01x slower                                                                                                               |
| async_tree_io              | 716 ms                                                                                                                 | 726 ms: 1.01x slower                                                                                                               |
| async_tree_cpu_io_mixed_tg | 465 ms                                                                                                                 | 473 ms: 1.02x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 446 ms                                                                                                                 | 459 ms: 1.03x slower                                                                                                               |
| Geometric mean             | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (4): async_tree_io_tg, async_tree_memoization, async_tree_memoization_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 147 ms                                                                                                                 | 148 ms: 1.01x slower                                                                                                               |
| float          | 51.3 ms                                                                                                                | 55.8 ms: 1.09x slower                                                                                                              |
| nbody          | 72.8 ms                                                                                                                | 80.2 ms: 1.10x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.07x slower                                                                                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 1.56 ms                                                                                                                | 1.60 ms: 1.02x slower                                                                                                              |
| regex_dna      | 117 ms                                                                                                                 | 122 ms: 1.04x slower                                                                                                               |
| regex_v8       | 14.5 ms                                                                                                                | 15.3 ms: 1.05x slower                                                                                                              |
| regex_compile  | 78.0 ms                                                                                                                | 84.7 ms: 1.09x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.05x slower                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| unpickle             | 8.73 us                                                                                                                | 8.30 us: 1.05x faster                                                                                                              |
| json_loads           | 13.6 us                                                                                                                | 13.5 us: 1.01x faster                                                                                                              |
| pickle_dict          | 18.3 us                                                                                                                | 18.4 us: 1.01x slower                                                                                                              |
| tomli_loads          | 1.42 sec                                                                                                               | 1.43 sec: 1.01x slower                                                                                                             |
| pickle_pure_python   | 180 us                                                                                                                 | 181 us: 1.01x slower                                                                                                               |
| xml_etree_parse      | 92.9 ms                                                                                                                | 94.2 ms: 1.01x slower                                                                                                              |
| pickle               | 7.18 us                                                                                                                | 7.29 us: 1.01x slower                                                                                                              |
| xml_etree_generate   | 54.3 ms                                                                                                                | 55.6 ms: 1.03x slower                                                                                                              |
| xml_etree_process    | 36.8 ms                                                                                                                | 37.8 ms: 1.03x slower                                                                                                              |
| unpickle_list        | 2.69 us                                                                                                                | 2.80 us: 1.04x slower                                                                                                              |
| unpickle_pure_python | 128 us                                                                                                                 | 135 us: 1.05x slower                                                                                                               |
| xml_etree_iterparse  | 63.5 ms                                                                                                                | 68.9 ms: 1.09x slower                                                                                                              |
| pickle_list          | 2.82 us                                                                                                                | 3.18 us: 1.13x slower                                                                                                              |
| Geometric mean       | (ref)                                                                                                                  | 1.02x slower                                                                                                                       |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.48 ms                                                                                                                | 7.60 ms: 1.17x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                  | results/bm-20240120-3.13.0a3+-52eade2/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json | results/bm-20240120-3.13.0a3+-52eade2-PYTHON_UOPS/bm-20240120-pythonperf1-amd64-python-52eade22237eef1f3843-3.13.0a3+-52eade2.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 1.82 sec                                                                                                               | 1.68 sec: 1.08x faster                                                                                                             |
| unpickle                   | 8.73 us                                                                                                                | 8.30 us: 1.05x faster                                                                                                              |
| scimark_sor                | 80.2 ms                                                                                                                | 76.7 ms: 1.05x faster                                                                                                              |
| unpack_sequence            | 39.8 ns                                                                                                                | 38.1 ns: 1.04x faster                                                                                                              |
| async_generators           | 235 ms                                                                                                                 | 230 ms: 1.02x faster                                                                                                               |
| richards_super             | 31.2 ms                                                                                                                | 30.6 ms: 1.02x faster                                                                                                              |
| coverage                   | 46.2 ms                                                                                                                | 45.3 ms: 1.02x faster                                                                                                              |
| deepcopy                   | 224 us                                                                                                                 | 221 us: 1.02x faster                                                                                                               |
| telco                      | 4.80 ms                                                                                                                | 4.74 ms: 1.01x faster                                                                                                              |
| richards                   | 27.5 ms                                                                                                                | 27.2 ms: 1.01x faster                                                                                                              |
| generators                 | 21.9 ms                                                                                                                | 21.6 ms: 1.01x faster                                                                                                              |
| json_loads                 | 13.6 us                                                                                                                | 13.5 us: 1.01x faster                                                                                                              |
| sympy_expand               | 273 ms                                                                                                                 | 274 ms: 1.00x slower                                                                                                               |
| pickle_dict                | 18.3 us                                                                                                                | 18.4 us: 1.01x slower                                                                                                              |
| tomli_loads                | 1.42 sec                                                                                                               | 1.43 sec: 1.01x slower                                                                                                             |
| gc_traversal               | 1.49 ms                                                                                                                | 1.50 ms: 1.01x slower                                                                                                              |
| sqlglot_transpile          | 999 us                                                                                                                 | 1.01 ms: 1.01x slower                                                                                                              |
| pidigits                   | 147 ms                                                                                                                 | 148 ms: 1.01x slower                                                                                                               |
| bench_mp_pool              | 66.7 ms                                                                                                                | 67.3 ms: 1.01x slower                                                                                                              |
| pickle_pure_python         | 180 us                                                                                                                 | 181 us: 1.01x slower                                                                                                               |
| logging_format             | 6.50 us                                                                                                                | 6.57 us: 1.01x slower                                                                                                              |
| logging_simple             | 6.08 us                                                                                                                | 6.15 us: 1.01x slower                                                                                                              |
| dask                       | 253 ms                                                                                                                 | 256 ms: 1.01x slower                                                                                                               |
| logging_silent             | 55.0 ns                                                                                                                | 55.7 ns: 1.01x slower                                                                                                              |
| async_tree_none_tg         | 272 ms                                                                                                                 | 276 ms: 1.01x slower                                                                                                               |
| xml_etree_parse            | 92.9 ms                                                                                                                | 94.2 ms: 1.01x slower                                                                                                              |
| tornado_http               | 86.2 ms                                                                                                                | 87.4 ms: 1.01x slower                                                                                                              |
| async_tree_io              | 716 ms                                                                                                                 | 726 ms: 1.01x slower                                                                                                               |
| pickle                     | 7.18 us                                                                                                                | 7.29 us: 1.01x slower                                                                                                              |
| deepcopy_reduce            | 1.94 us                                                                                                                | 1.97 us: 1.02x slower                                                                                                              |
| async_tree_cpu_io_mixed_tg | 465 ms                                                                                                                 | 473 ms: 1.02x slower                                                                                                               |
| create_gc_cycles           | 715 us                                                                                                                 | 728 us: 1.02x slower                                                                                                               |
| sqlglot_normalize          | 178 ms                                                                                                                 | 181 ms: 1.02x slower                                                                                                               |
| 2to3                       | 213 ms                                                                                                                 | 218 ms: 1.02x slower                                                                                                               |
| chameleon                  | 4.90 ms                                                                                                                | 5.01 ms: 1.02x slower                                                                                                              |
| mypy2                      | 413 ms                                                                                                                 | 422 ms: 1.02x slower                                                                                                               |
| dulwich_log                | 41.4 ms                                                                                                                | 42.3 ms: 1.02x slower                                                                                                              |
| regex_effbot               | 1.56 ms                                                                                                                | 1.60 ms: 1.02x slower                                                                                                              |
| xml_etree_generate         | 54.3 ms                                                                                                                | 55.6 ms: 1.03x slower                                                                                                              |
| typing_runtime_protocols   | 71.9 us                                                                                                                | 73.7 us: 1.03x slower                                                                                                              |
| mdp                        | 1.34 sec                                                                                                               | 1.37 sec: 1.03x slower                                                                                                             |
| sqlglot_optimize           | 33.9 ms                                                                                                                | 34.8 ms: 1.03x slower                                                                                                              |
| xml_etree_process          | 36.8 ms                                                                                                                | 37.8 ms: 1.03x slower                                                                                                              |
| raytrace                   | 169 ms                                                                                                                 | 174 ms: 1.03x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 446 ms                                                                                                                 | 459 ms: 1.03x slower                                                                                                               |
| docutils                   | 1.53 sec                                                                                                               | 1.59 sec: 1.03x slower                                                                                                             |
| sympy_str                  | 159 ms                                                                                                                 | 165 ms: 1.04x slower                                                                                                               |
| unpickle_list              | 2.69 us                                                                                                                | 2.80 us: 1.04x slower                                                                                                              |
| scimark_lu                 | 55.7 ms                                                                                                                | 58.0 ms: 1.04x slower                                                                                                              |
| regex_dna                  | 117 ms                                                                                                                 | 122 ms: 1.04x slower                                                                                                               |
| meteor_contest             | 71.5 ms                                                                                                                | 75.1 ms: 1.05x slower                                                                                                              |
| unpickle_pure_python       | 128 us                                                                                                                 | 135 us: 1.05x slower                                                                                                               |
| regex_v8                   | 14.5 ms                                                                                                                | 15.3 ms: 1.05x slower                                                                                                              |
| sympy_integrate            | 12.3 ms                                                                                                                | 13.1 ms: 1.06x slower                                                                                                              |
| sympy_sum                  | 82.4 ms                                                                                                                | 87.6 ms: 1.06x slower                                                                                                              |
| go                         | 86.0 ms                                                                                                                | 92.0 ms: 1.07x slower                                                                                                              |
| pprint_safe_repr           | 493 ms                                                                                                                 | 528 ms: 1.07x slower                                                                                                               |
| pprint_pformat             | 1.01 sec                                                                                                               | 1.09 sec: 1.08x slower                                                                                                             |
| xml_etree_iterparse        | 63.5 ms                                                                                                                | 68.9 ms: 1.09x slower                                                                                                              |
| regex_compile              | 78.0 ms                                                                                                                | 84.7 ms: 1.09x slower                                                                                                              |
| float                      | 51.3 ms                                                                                                                | 55.8 ms: 1.09x slower                                                                                                              |
| nqueens                    | 58.9 ms                                                                                                                | 64.0 ms: 1.09x slower                                                                                                              |
| crypto_pyaes               | 43.1 ms                                                                                                                | 47.1 ms: 1.09x slower                                                                                                              |
| chaos                      | 40.1 ms                                                                                                                | 43.9 ms: 1.09x slower                                                                                                              |
| nbody                      | 72.8 ms                                                                                                                | 80.2 ms: 1.10x slower                                                                                                              |
| json                       | 2.88 ms                                                                                                                | 3.19 ms: 1.11x slower                                                                                                              |
| fannkuch                   | 244 ms                                                                                                                 | 271 ms: 1.11x slower                                                                                                               |
| pickle_list                | 2.82 us                                                                                                                | 3.18 us: 1.13x slower                                                                                                              |
| pyflate                    | 287 ms                                                                                                                 | 325 ms: 1.13x slower                                                                                                               |
| scimark_monte_carlo        | 40.9 ms                                                                                                                | 47.1 ms: 1.15x slower                                                                                                              |
| mako                       | 6.48 ms                                                                                                                | 7.60 ms: 1.17x slower                                                                                                              |
| scimark_fft                | 179 ms                                                                                                                 | 211 ms: 1.17x slower                                                                                                               |
| comprehensions             | 10.6 us                                                                                                                | 13.0 us: 1.22x slower                                                                                                              |
| scimark_sparse_mat_mult    | 2.48 ms                                                                                                                | 3.06 ms: 1.24x slower                                                                                                              |
| hexiom                     | 3.87 ms                                                                                                                | 4.87 ms: 1.26x slower                                                                                                              |
| deltablue                  | 2.03 ms                                                                                                                | 2.70 ms: 1.33x slower                                                                                                              |
| spectral_norm              | 60.4 ms                                                                                                                | 84.3 ms: 1.39x slower                                                                                                              |
| Geometric mean             | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmark hidden because not significant (15): pycparser, asyncio_tcp, async_tree_io_tg, coroutines, sqlglot_parse, json_dumps, deepcopy_memo, sqlite_synth, bench_thread_pool, python_startup, pathlib, python_startup_no_site, async_tree_memoization, async_tree_memoization_tg, async_tree_none


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown