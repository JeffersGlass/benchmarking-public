# Results vs. base

- fork: python
- ref: a768e12f094a9b14a9a1
- machine: windows-amd64
- commit hash: a768e12
- commit date: 2024-01-27
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 210 ms                                                                                                                 | 222 ms: 1.06x slower                                                                                                               |
| chameleon      | 4.81 ms                                                                                                                | 5.01 ms: 1.04x slower                                                                                                              |
| docutils       | 1.56 sec                                                                                                               | 1.60 sec: 1.03x slower                                                                                                             |
| tornado_http   | 85.8 ms                                                                                                                | 86.8 ms: 1.01x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|-------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 465 ms                                                                                                                 | 457 ms: 1.02x faster                                                                                                               |
| async_tree_none_tg      | 279 ms                                                                                                                 | 283 ms: 1.01x slower                                                                                                               |
| async_tree_io_tg        | 769 ms                                                                                                                 | 783 ms: 1.02x slower                                                                                                               |
| Geometric mean          | (ref)                                                                                                                  | 1.00x slower                                                                                                                       |

Benchmark hidden because not significant (5): async_tree_memoization_tg, async_tree_io, async_tree_memoization, async_tree_cpu_io_mixed_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| float          | 53.5 ms                                                                                                                | 57.2 ms: 1.07x slower                                                                                                              |
| nbody          | 72.3 ms                                                                                                                | 83.1 ms: 1.15x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.07x slower                                                                                                                       |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_v8       | 17.1 ms                                                                                                                | 14.8 ms: 1.16x faster                                                                                                              |
| regex_effbot   | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| regex_dna      | 118 ms                                                                                                                 | 121 ms: 1.02x slower                                                                                                               |
| regex_compile  | 76.9 ms                                                                                                                | 85.2 ms: 1.11x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.01x faster                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pickle_pure_python   | 185 us                                                                                                                 | 182 us: 1.02x faster                                                                                                               |
| xml_etree_parse      | 94.1 ms                                                                                                                | 92.7 ms: 1.02x faster                                                                                                              |
| pickle               | 7.25 us                                                                                                                | 7.20 us: 1.01x faster                                                                                                              |
| json_dumps           | 5.63 ms                                                                                                                | 5.66 ms: 1.00x slower                                                                                                              |
| pickle_dict          | 18.6 us                                                                                                                | 18.8 us: 1.01x slower                                                                                                              |
| json_loads           | 13.5 us                                                                                                                | 13.7 us: 1.01x slower                                                                                                              |
| xml_etree_process    | 37.0 ms                                                                                                                | 38.2 ms: 1.03x slower                                                                                                              |
| unpickle_list        | 2.75 us                                                                                                                | 2.85 us: 1.04x slower                                                                                                              |
| xml_etree_iterparse  | 65.5 ms                                                                                                                | 68.0 ms: 1.04x slower                                                                                                              |
| xml_etree_generate   | 53.9 ms                                                                                                                | 56.2 ms: 1.04x slower                                                                                                              |
| unpickle_pure_python | 130 us                                                                                                                 | 137 us: 1.05x slower                                                                                                               |
| Geometric mean       | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (3): unpickle, tomli_loads, pickle_list

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup_no_site, python_startup

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.65 ms                                                                                                                | 7.38 ms: 1.11x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                | results/bm-20240127-3.13.0a3+-a768e12/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json | results/bm-20240127-3.13.0a3+-a768e12-PYTHON_UOPS/bm-20240127-pythonperf1-amd64-python-a768e12f094a9b14a9a1-3.13.0a3+-a768e12.json |
|--------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| json                     | 3.39 ms                                                                                                                | 2.93 ms: 1.16x faster                                                                                                              |
| regex_v8                 | 17.1 ms                                                                                                                | 14.8 ms: 1.16x faster                                                                                                              |
| richards                 | 28.0 ms                                                                                                                | 26.8 ms: 1.04x faster                                                                                                              |
| asyncio_tcp              | 491 ms                                                                                                                 | 478 ms: 1.03x faster                                                                                                               |
| logging_silent           | 55.5 ns                                                                                                                | 54.1 ns: 1.03x faster                                                                                                              |
| coroutines               | 13.4 ms                                                                                                                | 13.1 ms: 1.03x faster                                                                                                              |
| richards_super           | 31.0 ms                                                                                                                | 30.4 ms: 1.02x faster                                                                                                              |
| async_tree_cpu_io_mixed  | 465 ms                                                                                                                 | 457 ms: 1.02x faster                                                                                                               |
| pickle_pure_python       | 185 us                                                                                                                 | 182 us: 1.02x faster                                                                                                               |
| async_generators         | 235 ms                                                                                                                 | 231 ms: 1.02x faster                                                                                                               |
| xml_etree_parse          | 94.1 ms                                                                                                                | 92.7 ms: 1.02x faster                                                                                                              |
| create_gc_cycles         | 760 us                                                                                                                 | 750 us: 1.01x faster                                                                                                               |
| generators               | 21.3 ms                                                                                                                | 21.0 ms: 1.01x faster                                                                                                              |
| pathlib                  | 81.0 ms                                                                                                                | 80.2 ms: 1.01x faster                                                                                                              |
| regex_effbot             | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                              |
| pickle                   | 7.25 us                                                                                                                | 7.20 us: 1.01x faster                                                                                                              |
| json_dumps               | 5.63 ms                                                                                                                | 5.66 ms: 1.00x slower                                                                                                              |
| bench_mp_pool            | 67.9 ms                                                                                                                | 68.4 ms: 1.01x slower                                                                                                              |
| telco                    | 4.71 ms                                                                                                                | 4.75 ms: 1.01x slower                                                                                                              |
| logging_simple           | 6.16 us                                                                                                                | 6.22 us: 1.01x slower                                                                                                              |
| pickle_dict              | 18.6 us                                                                                                                | 18.8 us: 1.01x slower                                                                                                              |
| deepcopy                 | 226 us                                                                                                                 | 229 us: 1.01x slower                                                                                                               |
| json_loads               | 13.5 us                                                                                                                | 13.7 us: 1.01x slower                                                                                                              |
| tornado_http             | 85.8 ms                                                                                                                | 86.8 ms: 1.01x slower                                                                                                              |
| dask                     | 259 ms                                                                                                                 | 263 ms: 1.01x slower                                                                                                               |
| sqlglot_parse            | 778 us                                                                                                                 | 789 us: 1.01x slower                                                                                                               |
| async_tree_none_tg       | 279 ms                                                                                                                 | 283 ms: 1.01x slower                                                                                                               |
| scimark_sor              | 77.4 ms                                                                                                                | 78.7 ms: 1.02x slower                                                                                                              |
| async_tree_io_tg         | 769 ms                                                                                                                 | 783 ms: 1.02x slower                                                                                                               |
| deepcopy_reduce          | 1.97 us                                                                                                                | 2.01 us: 1.02x slower                                                                                                              |
| regex_dna                | 118 ms                                                                                                                 | 121 ms: 1.02x slower                                                                                                               |
| docutils                 | 1.56 sec                                                                                                               | 1.60 sec: 1.03x slower                                                                                                             |
| raytrace                 | 166 ms                                                                                                                 | 170 ms: 1.03x slower                                                                                                               |
| pprint_safe_repr         | 512 ms                                                                                                                 | 528 ms: 1.03x slower                                                                                                               |
| sympy_expand             | 276 ms                                                                                                                 | 284 ms: 1.03x slower                                                                                                               |
| bench_thread_pool        | 861 us                                                                                                                 | 888 us: 1.03x slower                                                                                                               |
| mypy2                    | 419 ms                                                                                                                 | 432 ms: 1.03x slower                                                                                                               |
| xml_etree_process        | 37.0 ms                                                                                                                | 38.2 ms: 1.03x slower                                                                                                              |
| typing_runtime_protocols | 73.1 us                                                                                                                | 75.6 us: 1.03x slower                                                                                                              |
| sqlglot_transpile        | 981 us                                                                                                                 | 1.01 ms: 1.03x slower                                                                                                              |
| deepcopy_memo            | 22.6 us                                                                                                                | 23.4 us: 1.04x slower                                                                                                              |
| unpickle_list            | 2.75 us                                                                                                                | 2.85 us: 1.04x slower                                                                                                              |
| xml_etree_iterparse      | 65.5 ms                                                                                                                | 68.0 ms: 1.04x slower                                                                                                              |
| chameleon                | 4.81 ms                                                                                                                | 5.01 ms: 1.04x slower                                                                                                              |
| xml_etree_generate       | 53.9 ms                                                                                                                | 56.2 ms: 1.04x slower                                                                                                              |
| logging_format           | 6.46 us                                                                                                                | 6.73 us: 1.04x slower                                                                                                              |
| pprint_pformat           | 1.04 sec                                                                                                               | 1.09 sec: 1.05x slower                                                                                                             |
| unpickle_pure_python     | 130 us                                                                                                                 | 137 us: 1.05x slower                                                                                                               |
| meteor_contest           | 73.7 ms                                                                                                                | 77.5 ms: 1.05x slower                                                                                                              |
| dulwich_log              | 41.4 ms                                                                                                                | 43.7 ms: 1.05x slower                                                                                                              |
| nqueens                  | 60.2 ms                                                                                                                | 63.5 ms: 1.06x slower                                                                                                              |
| sqlglot_normalize        | 179 ms                                                                                                                 | 189 ms: 1.06x slower                                                                                                               |
| 2to3                     | 210 ms                                                                                                                 | 222 ms: 1.06x slower                                                                                                               |
| sympy_str                | 161 ms                                                                                                                 | 170 ms: 1.06x slower                                                                                                               |
| go                       | 85.5 ms                                                                                                                | 91.5 ms: 1.07x slower                                                                                                              |
| float                    | 53.5 ms                                                                                                                | 57.2 ms: 1.07x slower                                                                                                              |
| sqlglot_optimize         | 33.2 ms                                                                                                                | 35.7 ms: 1.07x slower                                                                                                              |
| sympy_integrate          | 12.4 ms                                                                                                                | 13.3 ms: 1.08x slower                                                                                                              |
| mdp                      | 1.42 sec                                                                                                               | 1.53 sec: 1.08x slower                                                                                                             |
| sympy_sum                | 83.1 ms                                                                                                                | 89.6 ms: 1.08x slower                                                                                                              |
| scimark_lu               | 53.8 ms                                                                                                                | 58.8 ms: 1.09x slower                                                                                                              |
| regex_compile            | 76.9 ms                                                                                                                | 85.2 ms: 1.11x slower                                                                                                              |
| pyflate                  | 293 ms                                                                                                                 | 325 ms: 1.11x slower                                                                                                               |
| mako                     | 6.65 ms                                                                                                                | 7.38 ms: 1.11x slower                                                                                                              |
| unpack_sequence          | 37.6 ns                                                                                                                | 42.1 ns: 1.12x slower                                                                                                              |
| chaos                    | 39.6 ms                                                                                                                | 44.4 ms: 1.12x slower                                                                                                              |
| fannkuch                 | 235 ms                                                                                                                 | 266 ms: 1.13x slower                                                                                                               |
| crypto_pyaes             | 42.3 ms                                                                                                                | 48.6 ms: 1.15x slower                                                                                                              |
| nbody                    | 72.3 ms                                                                                                                | 83.1 ms: 1.15x slower                                                                                                              |
| scimark_fft              | 177 ms                                                                                                                 | 205 ms: 1.16x slower                                                                                                               |
| scimark_monte_carlo      | 41.0 ms                                                                                                                | 47.7 ms: 1.16x slower                                                                                                              |
| comprehensions           | 10.9 us                                                                                                                | 13.0 us: 1.19x slower                                                                                                              |
| hexiom                   | 3.84 ms                                                                                                                | 4.80 ms: 1.25x slower                                                                                                              |
| scimark_sparse_mat_mult  | 2.45 ms                                                                                                                | 3.07 ms: 1.25x slower                                                                                                              |
| deltablue                | 2.01 ms                                                                                                                | 2.59 ms: 1.29x slower                                                                                                              |
| spectral_norm            | 61.8 ms                                                                                                                | 80.9 ms: 1.31x slower                                                                                                              |
| Geometric mean           | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmark hidden because not significant (16): asyncio_tcp_ssl, unpickle, async_tree_memoization_tg, tomli_loads, async_tree_io, gc_traversal, sqlite_synth, coverage, pickle_list, async_tree_memoization, pidigits, python_startup_no_site, async_tree_cpu_io_mixed_tg, python_startup, async_tree_none, pycparser


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown