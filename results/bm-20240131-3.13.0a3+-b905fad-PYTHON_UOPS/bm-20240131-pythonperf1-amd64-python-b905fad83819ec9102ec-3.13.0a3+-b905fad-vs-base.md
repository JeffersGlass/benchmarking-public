# Results vs. base

- fork: python
- ref: b905fad83819ec9102ec
- machine: windows-amd64
- commit hash: b905fad
- commit date: 2024-01-31
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 216 ms                                                                                                                 | 225 ms: 1.04x slower                                                                                                               |
| chameleon      | 4.93 ms                                                                                                                | 5.28 ms: 1.07x slower                                                                                                              |
| docutils       | 1.59 sec                                                                                                               | 1.63 sec: 1.02x slower                                                                                                             |
| tornado_http   | 86.3 ms                                                                                                                | 88.0 ms: 1.02x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|--------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io      | 763 ms                                                                                                                 | 754 ms: 1.01x faster                                                                                                               |
| async_tree_none_tg | 283 ms                                                                                                                 | 289 ms: 1.02x slower                                                                                                               |
| Geometric mean     | (ref)                                                                                                                  | 1.00x slower                                                                                                                       |

Benchmark hidden because not significant (6): async_tree_none, async_tree_memoization, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| float          | 54.1 ms                                                                                                                | 57.2 ms: 1.06x slower                                                                                                              |
| nbody          | 72.0 ms                                                                                                                | 83.0 ms: 1.15x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.07x slower                                                                                                                       |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_effbot   | 1.59 ms                                                                                                                | 1.63 ms: 1.03x slower                                                                                                              |
| regex_compile  | 79.0 ms                                                                                                                | 85.3 ms: 1.08x slower                                                                                                              |
| regex_dna      | 117 ms                                                                                                                 | 129 ms: 1.10x slower                                                                                                               |
| regex_v8       | 14.6 ms                                                                                                                | 18.5 ms: 1.27x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.11x slower                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| xml_etree_parse      | 95.6 ms                                                                                                                | 93.5 ms: 1.02x faster                                                                                                              |
| pickle_dict          | 18.9 us                                                                                                                | 18.7 us: 1.01x faster                                                                                                              |
| pickle               | 7.15 us                                                                                                                | 7.09 us: 1.01x faster                                                                                                              |
| json_loads           | 13.9 us                                                                                                                | 13.9 us: 1.01x slower                                                                                                              |
| xml_etree_process    | 37.6 ms                                                                                                                | 38.2 ms: 1.02x slower                                                                                                              |
| unpickle             | 8.45 us                                                                                                                | 8.60 us: 1.02x slower                                                                                                              |
| pickle_list          | 2.87 us                                                                                                                | 2.93 us: 1.02x slower                                                                                                              |
| json_dumps           | 5.61 ms                                                                                                                | 5.78 ms: 1.03x slower                                                                                                              |
| unpickle_list        | 2.72 us                                                                                                                | 2.82 us: 1.04x slower                                                                                                              |
| xml_etree_iterparse  | 65.0 ms                                                                                                                | 67.7 ms: 1.04x slower                                                                                                              |
| xml_etree_generate   | 53.9 ms                                                                                                                | 56.7 ms: 1.05x slower                                                                                                              |
| unpickle_pure_python | 133 us                                                                                                                 | 143 us: 1.08x slower                                                                                                               |
| Geometric mean       | (ref)                                                                                                                  | 1.02x slower                                                                                                                       |

Benchmark hidden because not significant (2): tomli_loads, pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark      | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| python_startup | 20.5 ms                                                                                                                | 20.8 ms: 1.01x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.00x slower                                                                                                                       |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.75 ms                                                                                                                | 7.44 ms: 1.10x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                | results/bm-20240131-3.13.0a3+-b905fad/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json | results/bm-20240131-3.13.0a3+-b905fad-PYTHON_UOPS/bm-20240131-pythonperf1-amd64-python-b905fad83819ec9102ec-3.13.0a3+-b905fad.json |
|--------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| json                     | 3.26 ms                                                                                                                | 2.95 ms: 1.10x faster                                                                                                              |
| asyncio_tcp              | 503 ms                                                                                                                 | 478 ms: 1.05x faster                                                                                                               |
| bench_thread_pool        | 877 us                                                                                                                 | 853 us: 1.03x faster                                                                                                               |
| xml_etree_parse          | 95.6 ms                                                                                                                | 93.5 ms: 1.02x faster                                                                                                              |
| async_tree_io            | 763 ms                                                                                                                 | 754 ms: 1.01x faster                                                                                                               |
| coverage                 | 48.0 ms                                                                                                                | 47.5 ms: 1.01x faster                                                                                                              |
| richards                 | 28.4 ms                                                                                                                | 28.1 ms: 1.01x faster                                                                                                              |
| pickle_dict              | 18.9 us                                                                                                                | 18.7 us: 1.01x faster                                                                                                              |
| pickle                   | 7.15 us                                                                                                                | 7.09 us: 1.01x faster                                                                                                              |
| deepcopy_reduce          | 2.02 us                                                                                                                | 2.01 us: 1.00x faster                                                                                                              |
| json_loads               | 13.9 us                                                                                                                | 13.9 us: 1.01x slower                                                                                                              |
| bench_mp_pool            | 67.7 ms                                                                                                                | 68.2 ms: 1.01x slower                                                                                                              |
| pathlib                  | 80.3 ms                                                                                                                | 81.0 ms: 1.01x slower                                                                                                              |
| sqlglot_transpile        | 1.00 ms                                                                                                                | 1.02 ms: 1.01x slower                                                                                                              |
| python_startup           | 20.5 ms                                                                                                                | 20.8 ms: 1.01x slower                                                                                                              |
| dask                     | 260 ms                                                                                                                 | 264 ms: 1.01x slower                                                                                                               |
| deepcopy_memo            | 23.0 us                                                                                                                | 23.3 us: 1.02x slower                                                                                                              |
| xml_etree_process        | 37.6 ms                                                                                                                | 38.2 ms: 1.02x slower                                                                                                              |
| scimark_sor              | 81.5 ms                                                                                                                | 83.0 ms: 1.02x slower                                                                                                              |
| unpickle                 | 8.45 us                                                                                                                | 8.60 us: 1.02x slower                                                                                                              |
| tornado_http             | 86.3 ms                                                                                                                | 88.0 ms: 1.02x slower                                                                                                              |
| async_tree_none_tg       | 283 ms                                                                                                                 | 289 ms: 1.02x slower                                                                                                               |
| pickle_list              | 2.87 us                                                                                                                | 2.93 us: 1.02x slower                                                                                                              |
| coroutines               | 13.1 ms                                                                                                                | 13.4 ms: 1.02x slower                                                                                                              |
| deepcopy                 | 224 us                                                                                                                 | 230 us: 1.02x slower                                                                                                               |
| async_generators         | 229 ms                                                                                                                 | 235 ms: 1.02x slower                                                                                                               |
| sympy_expand             | 275 ms                                                                                                                 | 282 ms: 1.02x slower                                                                                                               |
| mypy2                    | 421 ms                                                                                                                 | 432 ms: 1.02x slower                                                                                                               |
| dulwich_log              | 42.5 ms                                                                                                                | 43.6 ms: 1.02x slower                                                                                                              |
| docutils                 | 1.59 sec                                                                                                               | 1.63 sec: 1.02x slower                                                                                                             |
| telco                    | 4.61 ms                                                                                                                | 4.73 ms: 1.03x slower                                                                                                              |
| regex_effbot             | 1.59 ms                                                                                                                | 1.63 ms: 1.03x slower                                                                                                              |
| sqlglot_parse            | 775 us                                                                                                                 | 797 us: 1.03x slower                                                                                                               |
| json_dumps               | 5.61 ms                                                                                                                | 5.78 ms: 1.03x slower                                                                                                              |
| logging_simple           | 6.06 us                                                                                                                | 6.27 us: 1.03x slower                                                                                                              |
| mdp                      | 1.41 sec                                                                                                               | 1.46 sec: 1.04x slower                                                                                                             |
| sympy_sum                | 85.1 ms                                                                                                                | 88.2 ms: 1.04x slower                                                                                                              |
| sqlglot_optimize         | 33.9 ms                                                                                                                | 35.1 ms: 1.04x slower                                                                                                              |
| logging_silent           | 54.8 ns                                                                                                                | 56.8 ns: 1.04x slower                                                                                                              |
| typing_runtime_protocols | 71.4 us                                                                                                                | 74.2 us: 1.04x slower                                                                                                              |
| unpickle_list            | 2.72 us                                                                                                                | 2.82 us: 1.04x slower                                                                                                              |
| xml_etree_iterparse      | 65.0 ms                                                                                                                | 67.7 ms: 1.04x slower                                                                                                              |
| 2to3                     | 216 ms                                                                                                                 | 225 ms: 1.04x slower                                                                                                               |
| logging_format           | 6.61 us                                                                                                                | 6.92 us: 1.05x slower                                                                                                              |
| xml_etree_generate       | 53.9 ms                                                                                                                | 56.7 ms: 1.05x slower                                                                                                              |
| pprint_safe_repr         | 501 ms                                                                                                                 | 529 ms: 1.06x slower                                                                                                               |
| scimark_lu               | 55.2 ms                                                                                                                | 58.4 ms: 1.06x slower                                                                                                              |
| float                    | 54.1 ms                                                                                                                | 57.2 ms: 1.06x slower                                                                                                              |
| sympy_str                | 159 ms                                                                                                                 | 168 ms: 1.06x slower                                                                                                               |
| go                       | 85.7 ms                                                                                                                | 91.1 ms: 1.06x slower                                                                                                              |
| sympy_integrate          | 12.7 ms                                                                                                                | 13.5 ms: 1.06x slower                                                                                                              |
| sqlglot_normalize        | 175 ms                                                                                                                 | 187 ms: 1.07x slower                                                                                                               |
| pprint_pformat           | 1.02 sec                                                                                                               | 1.09 sec: 1.07x slower                                                                                                             |
| chameleon                | 4.93 ms                                                                                                                | 5.28 ms: 1.07x slower                                                                                                              |
| meteor_contest           | 72.8 ms                                                                                                                | 78.0 ms: 1.07x slower                                                                                                              |
| crypto_pyaes             | 44.8 ms                                                                                                                | 48.2 ms: 1.07x slower                                                                                                              |
| unpickle_pure_python     | 133 us                                                                                                                 | 143 us: 1.08x slower                                                                                                               |
| regex_compile            | 79.0 ms                                                                                                                | 85.3 ms: 1.08x slower                                                                                                              |
| raytrace                 | 163 ms                                                                                                                 | 176 ms: 1.08x slower                                                                                                               |
| nqueens                  | 58.6 ms                                                                                                                | 63.8 ms: 1.09x slower                                                                                                              |
| regex_dna                | 117 ms                                                                                                                 | 129 ms: 1.10x slower                                                                                                               |
| mako                     | 6.75 ms                                                                                                                | 7.44 ms: 1.10x slower                                                                                                              |
| unpack_sequence          | 39.0 ns                                                                                                                | 43.2 ns: 1.11x slower                                                                                                              |
| fannkuch                 | 246 ms                                                                                                                 | 272 ms: 1.11x slower                                                                                                               |
| pyflate                  | 292 ms                                                                                                                 | 324 ms: 1.11x slower                                                                                                               |
| chaos                    | 39.8 ms                                                                                                                | 44.5 ms: 1.12x slower                                                                                                              |
| nbody                    | 72.0 ms                                                                                                                | 83.0 ms: 1.15x slower                                                                                                              |
| scimark_fft              | 180 ms                                                                                                                 | 211 ms: 1.17x slower                                                                                                               |
| scimark_monte_carlo      | 40.8 ms                                                                                                                | 48.0 ms: 1.18x slower                                                                                                              |
| hexiom                   | 3.97 ms                                                                                                                | 4.79 ms: 1.21x slower                                                                                                              |
| scimark_sparse_mat_mult  | 2.54 ms                                                                                                                | 3.14 ms: 1.24x slower                                                                                                              |
| comprehensions           | 10.5 us                                                                                                                | 13.1 us: 1.25x slower                                                                                                              |
| regex_v8                 | 14.6 ms                                                                                                                | 18.5 ms: 1.27x slower                                                                                                              |
| deltablue                | 2.06 ms                                                                                                                | 2.64 ms: 1.28x slower                                                                                                              |
| spectral_norm            | 62.2 ms                                                                                                                | 82.2 ms: 1.32x slower                                                                                                              |
| Geometric mean           | (ref)                                                                                                                  | 1.05x slower                                                                                                                       |

Benchmark hidden because not significant (17): async_tree_none, create_gc_cycles, python_startup_no_site, pycparser, asyncio_tcp_ssl, async_tree_memoization, async_tree_cpu_io_mixed, tomli_loads, generators, async_tree_io_tg, pidigits, richards_super, pickle_pure_python, sqlite_synth, gc_traversal, async_tree_cpu_io_mixed_tg, async_tree_memoization_tg


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown