# Results vs. base

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.04x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 210 ms                                                                                                                 | 220 ms: 1.04x slower                                                                                                               |
| chameleon      | 4.88 ms                                                                                                                | 5.12 ms: 1.05x slower                                                                                                              |
| docutils       | 1.55 sec                                                                                                               | 1.59 sec: 1.03x slower                                                                                                             |
| tornado_http   | 84.5 ms                                                                                                                | 85.4 ms: 1.01x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmarks with tag 'asyncio':
==============================

| Benchmark          | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|--------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_none_tg | 280 ms                                                                                                                 | 274 ms: 1.02x faster                                                                                                               |
| Geometric mean     | (ref)                                                                                                                  | 1.01x faster                                                                                                                       |

Benchmark hidden because not significant (7): async_tree_memoization_tg, async_tree_memoization, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_none, async_tree_cpu_io_mixed, async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 147 ms                                                                                                                 | 147 ms: 1.00x slower                                                                                                               |
| nbody          | 70.0 ms                                                                                                                | 75.6 ms: 1.08x slower                                                                                                              |
| float          | 53.3 ms                                                                                                                | 58.3 ms: 1.09x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.06x slower                                                                                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_v8       | 14.5 ms                                                                                                                | 14.7 ms: 1.01x slower                                                                                                              |
| regex_effbot   | 1.55 ms                                                                                                                | 1.57 ms: 1.01x slower                                                                                                              |
| regex_dna      | 116 ms                                                                                                                 | 119 ms: 1.03x slower                                                                                                               |
| regex_compile  | 78.2 ms                                                                                                                | 84.8 ms: 1.08x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pickle_list          | 2.95 us                                                                                                                | 2.85 us: 1.04x faster                                                                                                              |
| pickle               | 7.24 us                                                                                                                | 7.10 us: 1.02x faster                                                                                                              |
| pickle_dict          | 18.6 us                                                                                                                | 18.3 us: 1.02x faster                                                                                                              |
| unpickle             | 8.54 us                                                                                                                | 8.43 us: 1.01x faster                                                                                                              |
| json_loads           | 13.6 us                                                                                                                | 13.5 us: 1.01x faster                                                                                                              |
| pickle_pure_python   | 183 us                                                                                                                 | 184 us: 1.01x slower                                                                                                               |
| xml_etree_parse      | 90.8 ms                                                                                                                | 92.9 ms: 1.02x slower                                                                                                              |
| tomli_loads          | 1.45 sec                                                                                                               | 1.51 sec: 1.04x slower                                                                                                             |
| unpickle_list        | 2.73 us                                                                                                                | 2.86 us: 1.05x slower                                                                                                              |
| xml_etree_iterparse  | 63.3 ms                                                                                                                | 67.4 ms: 1.06x slower                                                                                                              |
| unpickle_pure_python | 127 us                                                                                                                 | 140 us: 1.10x slower                                                                                                               |
| Geometric mean       | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (3): xml_etree_process, xml_etree_generate, json_dumps

Benchmarks with tag 'startup':
==============================

Benchmark hidden because not significant (2): python_startup, python_startup_no_site

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.60 ms                                                                                                                | 7.67 ms: 1.16x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-PYTHON_UOPS/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|--------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| json                     | 3.32 ms                                                                                                                | 3.06 ms: 1.08x faster                                                                                                              |
| asyncio_tcp_ssl          | 1.76 sec                                                                                                               | 1.64 sec: 1.07x faster                                                                                                             |
| generators               | 21.3 ms                                                                                                                | 20.3 ms: 1.05x faster                                                                                                              |
| pickle_list              | 2.95 us                                                                                                                | 2.85 us: 1.04x faster                                                                                                              |
| richards                 | 28.1 ms                                                                                                                | 27.3 ms: 1.03x faster                                                                                                              |
| richards_super           | 31.8 ms                                                                                                                | 31.0 ms: 1.02x faster                                                                                                              |
| deepcopy_reduce          | 2.04 us                                                                                                                | 1.99 us: 1.02x faster                                                                                                              |
| async_tree_none_tg       | 280 ms                                                                                                                 | 274 ms: 1.02x faster                                                                                                               |
| pickle                   | 7.24 us                                                                                                                | 7.10 us: 1.02x faster                                                                                                              |
| gc_traversal             | 1.51 ms                                                                                                                | 1.49 ms: 1.02x faster                                                                                                              |
| pickle_dict              | 18.6 us                                                                                                                | 18.3 us: 1.02x faster                                                                                                              |
| unpickle                 | 8.54 us                                                                                                                | 8.43 us: 1.01x faster                                                                                                              |
| create_gc_cycles         | 748 us                                                                                                                 | 738 us: 1.01x faster                                                                                                               |
| json_loads               | 13.6 us                                                                                                                | 13.5 us: 1.01x faster                                                                                                              |
| mdp                      | 1.48 sec                                                                                                               | 1.47 sec: 1.01x faster                                                                                                             |
| pidigits                 | 147 ms                                                                                                                 | 147 ms: 1.00x slower                                                                                                               |
| pathlib                  | 75.1 ms                                                                                                                | 75.5 ms: 1.01x slower                                                                                                              |
| pickle_pure_python       | 183 us                                                                                                                 | 184 us: 1.01x slower                                                                                                               |
| sqlglot_transpile        | 1.00 ms                                                                                                                | 1.01 ms: 1.01x slower                                                                                                              |
| sqlglot_normalize        | 181 ms                                                                                                                 | 182 ms: 1.01x slower                                                                                                               |
| regex_v8                 | 14.5 ms                                                                                                                | 14.7 ms: 1.01x slower                                                                                                              |
| tornado_http             | 84.5 ms                                                                                                                | 85.4 ms: 1.01x slower                                                                                                              |
| dask                     | 254 ms                                                                                                                 | 257 ms: 1.01x slower                                                                                                               |
| deepcopy                 | 228 us                                                                                                                 | 231 us: 1.01x slower                                                                                                               |
| async_generators         | 229 ms                                                                                                                 | 231 ms: 1.01x slower                                                                                                               |
| telco                    | 4.80 ms                                                                                                                | 4.87 ms: 1.01x slower                                                                                                              |
| regex_effbot             | 1.55 ms                                                                                                                | 1.57 ms: 1.01x slower                                                                                                              |
| coverage                 | 46.4 ms                                                                                                                | 47.0 ms: 1.01x slower                                                                                                              |
| coroutines               | 13.0 ms                                                                                                                | 13.2 ms: 1.02x slower                                                                                                              |
| bench_mp_pool            | 63.9 ms                                                                                                                | 65.1 ms: 1.02x slower                                                                                                              |
| xml_etree_parse          | 90.8 ms                                                                                                                | 92.9 ms: 1.02x slower                                                                                                              |
| scimark_lu               | 55.6 ms                                                                                                                | 56.9 ms: 1.02x slower                                                                                                              |
| sqlglot_optimize         | 34.0 ms                                                                                                                | 34.8 ms: 1.02x slower                                                                                                              |
| regex_dna                | 116 ms                                                                                                                 | 119 ms: 1.03x slower                                                                                                               |
| mypy2                    | 413 ms                                                                                                                 | 424 ms: 1.03x slower                                                                                                               |
| docutils                 | 1.55 sec                                                                                                               | 1.59 sec: 1.03x slower                                                                                                             |
| logging_silent           | 54.2 ns                                                                                                                | 56.0 ns: 1.03x slower                                                                                                              |
| sqlite_synth             | 1.52 us                                                                                                                | 1.58 us: 1.03x slower                                                                                                              |
| deepcopy_memo            | 22.4 us                                                                                                                | 23.2 us: 1.03x slower                                                                                                              |
| logging_format           | 6.52 us                                                                                                                | 6.75 us: 1.04x slower                                                                                                              |
| logging_simple           | 6.07 us                                                                                                                | 6.29 us: 1.04x slower                                                                                                              |
| dulwich_log              | 39.8 ms                                                                                                                | 41.5 ms: 1.04x slower                                                                                                              |
| typing_runtime_protocols | 71.0 us                                                                                                                | 74.0 us: 1.04x slower                                                                                                              |
| 2to3                     | 210 ms                                                                                                                 | 220 ms: 1.04x slower                                                                                                               |
| tomli_loads              | 1.45 sec                                                                                                               | 1.51 sec: 1.04x slower                                                                                                             |
| sympy_expand             | 272 ms                                                                                                                 | 284 ms: 1.05x slower                                                                                                               |
| sympy_integrate          | 12.4 ms                                                                                                                | 13.0 ms: 1.05x slower                                                                                                              |
| meteor_contest           | 72.7 ms                                                                                                                | 76.0 ms: 1.05x slower                                                                                                              |
| unpickle_list            | 2.73 us                                                                                                                | 2.86 us: 1.05x slower                                                                                                              |
| unpack_sequence          | 36.2 ns                                                                                                                | 37.9 ns: 1.05x slower                                                                                                              |
| chameleon                | 4.88 ms                                                                                                                | 5.12 ms: 1.05x slower                                                                                                              |
| sympy_str                | 160 ms                                                                                                                 | 168 ms: 1.05x slower                                                                                                               |
| raytrace                 | 165 ms                                                                                                                 | 174 ms: 1.05x slower                                                                                                               |
| pprint_safe_repr         | 496 ms                                                                                                                 | 523 ms: 1.06x slower                                                                                                               |
| pprint_pformat           | 1.02 sec                                                                                                               | 1.08 sec: 1.06x slower                                                                                                             |
| sympy_sum                | 83.3 ms                                                                                                                | 88.4 ms: 1.06x slower                                                                                                              |
| xml_etree_iterparse      | 63.3 ms                                                                                                                | 67.4 ms: 1.06x slower                                                                                                              |
| crypto_pyaes             | 44.1 ms                                                                                                                | 47.5 ms: 1.08x slower                                                                                                              |
| fannkuch                 | 247 ms                                                                                                                 | 266 ms: 1.08x slower                                                                                                               |
| deltablue                | 1.99 ms                                                                                                                | 2.15 ms: 1.08x slower                                                                                                              |
| nbody                    | 70.0 ms                                                                                                                | 75.6 ms: 1.08x slower                                                                                                              |
| regex_compile            | 78.2 ms                                                                                                                | 84.8 ms: 1.08x slower                                                                                                              |
| nqueens                  | 59.4 ms                                                                                                                | 64.4 ms: 1.08x slower                                                                                                              |
| float                    | 53.3 ms                                                                                                                | 58.3 ms: 1.09x slower                                                                                                              |
| go                       | 85.5 ms                                                                                                                | 93.7 ms: 1.10x slower                                                                                                              |
| scimark_sor              | 76.3 ms                                                                                                                | 83.8 ms: 1.10x slower                                                                                                              |
| chaos                    | 40.5 ms                                                                                                                | 44.5 ms: 1.10x slower                                                                                                              |
| unpickle_pure_python     | 127 us                                                                                                                 | 140 us: 1.10x slower                                                                                                               |
| pyflate                  | 288 ms                                                                                                                 | 328 ms: 1.14x slower                                                                                                               |
| pycparser                | 713 ms                                                                                                                 | 823 ms: 1.16x slower                                                                                                               |
| mako                     | 6.60 ms                                                                                                                | 7.67 ms: 1.16x slower                                                                                                              |
| comprehensions           | 10.7 us                                                                                                                | 12.5 us: 1.18x slower                                                                                                              |
| scimark_fft              | 174 ms                                                                                                                 | 205 ms: 1.18x slower                                                                                                               |
| scimark_monte_carlo      | 39.5 ms                                                                                                                | 49.4 ms: 1.25x slower                                                                                                              |
| hexiom                   | 3.87 ms                                                                                                                | 5.00 ms: 1.29x slower                                                                                                              |
| spectral_norm            | 62.6 ms                                                                                                                | 81.0 ms: 1.29x slower                                                                                                              |
| scimark_sparse_mat_mult  | 2.36 ms                                                                                                                | 3.22 ms: 1.36x slower                                                                                                              |
| Geometric mean           | (ref)                                                                                                                  | 1.04x slower                                                                                                                       |

Benchmark hidden because not significant (15): async_tree_memoization_tg, async_tree_memoization, asyncio_tcp, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_none, xml_etree_process, xml_etree_generate, json_dumps, sqlglot_parse, python_startup, async_tree_cpu_io_mixed, async_tree_io, python_startup_no_site, bench_thread_pool


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown