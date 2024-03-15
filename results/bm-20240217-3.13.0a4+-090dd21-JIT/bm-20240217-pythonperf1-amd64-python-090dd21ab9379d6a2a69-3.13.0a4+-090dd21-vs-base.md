# Results vs. base

- fork: python
- ref: 090dd21ab9379d6a2a69
- machine: windows-amd64
- commit hash: 090dd21
- commit date: 2024-02-17
- overall geometric mean: 1.00x slower
- HPT reliability: 60.44%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 210 ms                                                                                                                 | 216 ms: 1.03x slower                                                                                                       |
| chameleon      | 4.88 ms                                                                                                                | 4.74 ms: 1.03x faster                                                                                                      |
| docutils       | 1.55 sec                                                                                                               | 1.56 sec: 1.00x slower                                                                                                     |
| Geometric mean | (ref)                                                                                                                  | 1.00x slower                                                                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| async_tree_memoization_tg  | 358 ms                                                                                                                 | 343 ms: 1.04x faster                                                                                                       |
| async_tree_none_tg         | 280 ms                                                                                                                 | 269 ms: 1.04x faster                                                                                                       |
| async_tree_cpu_io_mixed_tg | 475 ms                                                                                                                 | 460 ms: 1.03x faster                                                                                                       |
| async_tree_memoization     | 350 ms                                                                                                                 | 339 ms: 1.03x faster                                                                                                       |
| async_tree_io_tg           | 770 ms                                                                                                                 | 747 ms: 1.03x faster                                                                                                       |
| async_tree_none            | 272 ms                                                                                                                 | 266 ms: 1.02x faster                                                                                                       |
| async_tree_cpu_io_mixed    | 456 ms                                                                                                                 | 449 ms: 1.02x faster                                                                                                       |
| Geometric mean             | (ref)                                                                                                                  | 1.03x faster                                                                                                               |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody          | 70.0 ms                                                                                                                | 59.8 ms: 1.17x faster                                                                                                      |
| float          | 53.3 ms                                                                                                                | 50.2 ms: 1.06x faster                                                                                                      |
| pidigits       | 147 ms                                                                                                                 | 152 ms: 1.03x slower                                                                                                       |
| Geometric mean | (ref)                                                                                                                  | 1.06x faster                                                                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| regex_compile  | 78.2 ms                                                                                                                | 79.2 ms: 1.01x slower                                                                                                      |
| regex_v8       | 14.5 ms                                                                                                                | 15.2 ms: 1.04x slower                                                                                                      |
| regex_dna      | 116 ms                                                                                                                 | 121 ms: 1.04x slower                                                                                                       |
| regex_effbot   | 1.55 ms                                                                                                                | 1.64 ms: 1.06x slower                                                                                                      |
| Geometric mean | (ref)                                                                                                                  | 1.04x slower                                                                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| tomli_loads          | 1.45 sec                                                                                                               | 1.29 sec: 1.12x faster                                                                                                     |
| pickle_dict          | 18.6 us                                                                                                                | 17.4 us: 1.07x faster                                                                                                      |
| pickle_list          | 2.95 us                                                                                                                | 2.77 us: 1.06x faster                                                                                                      |
| pickle_pure_python   | 183 us                                                                                                                 | 175 us: 1.05x faster                                                                                                       |
| xml_etree_process    | 37.5 ms                                                                                                                | 36.0 ms: 1.04x faster                                                                                                      |
| xml_etree_generate   | 54.1 ms                                                                                                                | 52.7 ms: 1.03x faster                                                                                                      |
| unpickle             | 8.54 us                                                                                                                | 8.44 us: 1.01x faster                                                                                                      |
| json_dumps           | 5.65 ms                                                                                                                | 5.59 ms: 1.01x faster                                                                                                      |
| unpickle_pure_python | 127 us                                                                                                                 | 126 us: 1.01x faster                                                                                                       |
| xml_etree_parse      | 90.8 ms                                                                                                                | 91.6 ms: 1.01x slower                                                                                                      |
| json_loads           | 13.6 us                                                                                                                | 13.7 us: 1.01x slower                                                                                                      |
| xml_etree_iterparse  | 63.3 ms                                                                                                                | 64.0 ms: 1.01x slower                                                                                                      |
| unpickle_list        | 2.73 us                                                                                                                | 2.81 us: 1.03x slower                                                                                                      |
| pickle               | 7.24 us                                                                                                                | 7.47 us: 1.03x slower                                                                                                      |
| Geometric mean       | (ref)                                                                                                                  | 1.02x faster                                                                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 20.0 ms                                                                                                                | 20.4 ms: 1.02x slower                                                                                                      |
| python_startup_no_site | 17.9 ms                                                                                                                | 18.4 ms: 1.03x slower                                                                                                      |
| Geometric mean         | (ref)                                                                                                                  | 1.03x slower                                                                                                               |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                  | results/bm-20240217-3.13.0a4+-090dd21/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json | results/bm-20240217-3.13.0a4+-090dd21-JIT/bm-20240217-pythonperf1-amd64-python-090dd21ab9379d6a2a69-3.13.0a4+-090dd21.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody                      | 70.0 ms                                                                                                                | 59.8 ms: 1.17x faster                                                                                                      |
| tomli_loads                | 1.45 sec                                                                                                               | 1.29 sec: 1.12x faster                                                                                                     |
| richards_super             | 31.8 ms                                                                                                                | 28.4 ms: 1.12x faster                                                                                                      |
| richards                   | 28.1 ms                                                                                                                | 25.8 ms: 1.09x faster                                                                                                      |
| json                       | 3.32 ms                                                                                                                | 3.08 ms: 1.08x faster                                                                                                      |
| pickle_dict                | 18.6 us                                                                                                                | 17.4 us: 1.07x faster                                                                                                      |
| pickle_list                | 2.95 us                                                                                                                | 2.77 us: 1.06x faster                                                                                                      |
| deepcopy_reduce            | 2.04 us                                                                                                                | 1.91 us: 1.06x faster                                                                                                      |
| float                      | 53.3 ms                                                                                                                | 50.2 ms: 1.06x faster                                                                                                      |
| pickle_pure_python         | 183 us                                                                                                                 | 175 us: 1.05x faster                                                                                                       |
| deepcopy_memo              | 22.4 us                                                                                                                | 21.4 us: 1.05x faster                                                                                                      |
| deepcopy                   | 228 us                                                                                                                 | 218 us: 1.05x faster                                                                                                       |
| async_tree_memoization_tg  | 358 ms                                                                                                                 | 343 ms: 1.04x faster                                                                                                       |
| xml_etree_process          | 37.5 ms                                                                                                                | 36.0 ms: 1.04x faster                                                                                                      |
| pprint_pformat             | 1.02 sec                                                                                                               | 978 ms: 1.04x faster                                                                                                       |
| pprint_safe_repr           | 496 ms                                                                                                                 | 476 ms: 1.04x faster                                                                                                       |
| sqlglot_normalize          | 181 ms                                                                                                                 | 174 ms: 1.04x faster                                                                                                       |
| async_tree_none_tg         | 280 ms                                                                                                                 | 269 ms: 1.04x faster                                                                                                       |
| sqlglot_parse              | 788 us                                                                                                                 | 759 us: 1.04x faster                                                                                                       |
| sqlglot_transpile          | 1.00 ms                                                                                                                | 971 us: 1.03x faster                                                                                                       |
| async_tree_cpu_io_mixed_tg | 475 ms                                                                                                                 | 460 ms: 1.03x faster                                                                                                       |
| generators                 | 21.3 ms                                                                                                                | 20.7 ms: 1.03x faster                                                                                                      |
| async_tree_memoization     | 350 ms                                                                                                                 | 339 ms: 1.03x faster                                                                                                       |
| async_tree_io_tg           | 770 ms                                                                                                                 | 747 ms: 1.03x faster                                                                                                       |
| fannkuch                   | 247 ms                                                                                                                 | 240 ms: 1.03x faster                                                                                                       |
| chameleon                  | 4.88 ms                                                                                                                | 4.74 ms: 1.03x faster                                                                                                      |
| telco                      | 4.80 ms                                                                                                                | 4.67 ms: 1.03x faster                                                                                                      |
| scimark_sor                | 76.3 ms                                                                                                                | 74.3 ms: 1.03x faster                                                                                                      |
| create_gc_cycles           | 748 us                                                                                                                 | 729 us: 1.03x faster                                                                                                       |
| xml_etree_generate         | 54.1 ms                                                                                                                | 52.7 ms: 1.03x faster                                                                                                      |
| async_tree_none            | 272 ms                                                                                                                 | 266 ms: 1.02x faster                                                                                                       |
| logging_format             | 6.52 us                                                                                                                | 6.39 us: 1.02x faster                                                                                                      |
| sqlite_synth               | 1.52 us                                                                                                                | 1.49 us: 1.02x faster                                                                                                      |
| logging_simple             | 6.07 us                                                                                                                | 5.96 us: 1.02x faster                                                                                                      |
| coverage                   | 46.4 ms                                                                                                                | 45.6 ms: 1.02x faster                                                                                                      |
| async_tree_cpu_io_mixed    | 456 ms                                                                                                                 | 449 ms: 1.02x faster                                                                                                       |
| typing_runtime_protocols   | 71.0 us                                                                                                                | 70.0 us: 1.01x faster                                                                                                      |
| unpickle                   | 8.54 us                                                                                                                | 8.44 us: 1.01x faster                                                                                                      |
| json_dumps                 | 5.65 ms                                                                                                                | 5.59 ms: 1.01x faster                                                                                                      |
| unpickle_pure_python       | 127 us                                                                                                                 | 126 us: 1.01x faster                                                                                                       |
| nqueens                    | 59.4 ms                                                                                                                | 59.0 ms: 1.01x faster                                                                                                      |
| gc_traversal               | 1.51 ms                                                                                                                | 1.50 ms: 1.01x faster                                                                                                      |
| sqlglot_optimize           | 34.0 ms                                                                                                                | 33.9 ms: 1.00x faster                                                                                                      |
| docutils                   | 1.55 sec                                                                                                               | 1.56 sec: 1.00x slower                                                                                                     |
| scimark_lu                 | 55.6 ms                                                                                                                | 55.9 ms: 1.00x slower                                                                                                      |
| xml_etree_parse            | 90.8 ms                                                                                                                | 91.6 ms: 1.01x slower                                                                                                      |
| json_loads                 | 13.6 us                                                                                                                | 13.7 us: 1.01x slower                                                                                                      |
| xml_etree_iterparse        | 63.3 ms                                                                                                                | 64.0 ms: 1.01x slower                                                                                                      |
| comprehensions             | 10.7 us                                                                                                                | 10.8 us: 1.01x slower                                                                                                      |
| dulwich_log                | 39.8 ms                                                                                                                | 40.3 ms: 1.01x slower                                                                                                      |
| regex_compile              | 78.2 ms                                                                                                                | 79.2 ms: 1.01x slower                                                                                                      |
| raytrace                   | 165 ms                                                                                                                 | 167 ms: 1.02x slower                                                                                                       |
| python_startup             | 20.0 ms                                                                                                                | 20.4 ms: 1.02x slower                                                                                                      |
| sympy_str                  | 160 ms                                                                                                                 | 163 ms: 1.02x slower                                                                                                       |
| spectral_norm              | 62.6 ms                                                                                                                | 64.1 ms: 1.03x slower                                                                                                      |
| sympy_integrate            | 12.4 ms                                                                                                                | 12.7 ms: 1.03x slower                                                                                                      |
| 2to3                       | 210 ms                                                                                                                 | 216 ms: 1.03x slower                                                                                                       |
| mypy2                      | 413 ms                                                                                                                 | 423 ms: 1.03x slower                                                                                                       |
| chaos                      | 40.5 ms                                                                                                                | 41.6 ms: 1.03x slower                                                                                                      |
| crypto_pyaes               | 44.1 ms                                                                                                                | 45.4 ms: 1.03x slower                                                                                                      |
| sympy_expand               | 272 ms                                                                                                                 | 280 ms: 1.03x slower                                                                                                       |
| unpickle_list              | 2.73 us                                                                                                                | 2.81 us: 1.03x slower                                                                                                      |
| pickle                     | 7.24 us                                                                                                                | 7.47 us: 1.03x slower                                                                                                      |
| python_startup_no_site     | 17.9 ms                                                                                                                | 18.4 ms: 1.03x slower                                                                                                      |
| pidigits                   | 147 ms                                                                                                                 | 152 ms: 1.03x slower                                                                                                       |
| bench_mp_pool              | 63.9 ms                                                                                                                | 66.7 ms: 1.04x slower                                                                                                      |
| coroutines                 | 13.0 ms                                                                                                                | 13.5 ms: 1.04x slower                                                                                                      |
| regex_v8                   | 14.5 ms                                                                                                                | 15.2 ms: 1.04x slower                                                                                                      |
| meteor_contest             | 72.7 ms                                                                                                                | 75.9 ms: 1.04x slower                                                                                                      |
| regex_dna                  | 116 ms                                                                                                                 | 121 ms: 1.04x slower                                                                                                       |
| sympy_sum                  | 83.3 ms                                                                                                                | 87.0 ms: 1.04x slower                                                                                                      |
| async_generators           | 229 ms                                                                                                                 | 240 ms: 1.05x slower                                                                                                       |
| regex_effbot               | 1.55 ms                                                                                                                | 1.64 ms: 1.06x slower                                                                                                      |
| pyflate                    | 288 ms                                                                                                                 | 306 ms: 1.06x slower                                                                                                       |
| unpack_sequence            | 36.2 ns                                                                                                                | 38.6 ns: 1.07x slower                                                                                                      |
| pycparser                  | 713 ms                                                                                                                 | 764 ms: 1.07x slower                                                                                                       |
| scimark_fft                | 174 ms                                                                                                                 | 186 ms: 1.07x slower                                                                                                       |
| mdp                        | 1.48 sec                                                                                                               | 1.61 sec: 1.09x slower                                                                                                     |
| go                         | 85.5 ms                                                                                                                | 95.8 ms: 1.12x slower                                                                                                      |
| scimark_sparse_mat_mult    | 2.36 ms                                                                                                                | 2.70 ms: 1.14x slower                                                                                                      |
| hexiom                     | 3.87 ms                                                                                                                | 5.11 ms: 1.32x slower                                                                                                      |
| scimark_monte_carlo        | 39.5 ms                                                                                                                | 56.4 ms: 1.43x slower                                                                                                      |
| Geometric mean             | (ref)                                                                                                                  | 1.00x slower                                                                                                               |

Benchmark hidden because not significant (10): asyncio_tcp_ssl, deltablue, mako, pathlib, dask, logging_silent, tornado_http, async_tree_io, asyncio_tcp, bench_thread_pool


# HPT report

- Reliability score: 60.44% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown