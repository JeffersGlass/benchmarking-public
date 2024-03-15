# Results vs. base

- fork: python
- ref: 948acd6ed856251dc588
- machine: windows-amd64
- commit hash: 948acd6
- commit date: 2024-02-24
- overall geometric mean: 1.06x slower
- HPT reliability: 99.96%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 212 ms                                                                                                                 | 227 ms: 1.07x slower                                                                                                       |
| chameleon      | 4.98 ms                                                                                                                | 4.80 ms: 1.04x faster                                                                                                      |
| docutils       | 1.57 sec                                                                                                               | 1.67 sec: 1.07x slower                                                                                                     |
| tornado_http   | 84.0 ms                                                                                                                | 85.6 ms: 1.02x slower                                                                                                      |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|---------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| async_tree_memoization_tg | 354 ms                                                                                                                 | 344 ms: 1.03x faster                                                                                                       |
| async_tree_io             | 738 ms                                                                                                                 | 728 ms: 1.01x faster                                                                                                       |
| async_tree_none_tg        | 275 ms                                                                                                                 | 272 ms: 1.01x faster                                                                                                       |
| Geometric mean            | (ref)                                                                                                                  | 1.01x faster                                                                                                               |

Benchmark hidden because not significant (5): async_tree_none, async_tree_memoization, async_tree_io_tg, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody          | 72.9 ms                                                                                                                | 61.9 ms: 1.18x faster                                                                                                      |
| float          | 54.3 ms                                                                                                                | 50.0 ms: 1.09x faster                                                                                                      |
| pidigits       | 148 ms                                                                                                                 | 152 ms: 1.03x slower                                                                                                       |
| Geometric mean | (ref)                                                                                                                  | 1.08x faster                                                                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 120 ms                                                                                                                 | 119 ms: 1.02x faster                                                                                                       |
| regex_effbot   | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                      |
| regex_compile  | 79.8 ms                                                                                                                | 104 ms: 1.30x slower                                                                                                       |
| Geometric mean | (ref)                                                                                                                  | 1.08x slower                                                                                                               |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| tomli_loads          | 1.41 sec                                                                                                               | 1.32 sec: 1.07x faster                                                                                                     |
| pickle_pure_python   | 185 us                                                                                                                 | 176 us: 1.05x faster                                                                                                       |
| pickle_dict          | 18.2 us                                                                                                                | 17.6 us: 1.04x faster                                                                                                      |
| xml_etree_parse      | 94.1 ms                                                                                                                | 92.3 ms: 1.02x faster                                                                                                      |
| xml_etree_generate   | 53.9 ms                                                                                                                | 53.3 ms: 1.01x faster                                                                                                      |
| json_loads           | 14.0 us                                                                                                                | 13.8 us: 1.01x faster                                                                                                      |
| json_dumps           | 5.65 ms                                                                                                                | 5.59 ms: 1.01x faster                                                                                                      |
| unpickle             | 8.58 us                                                                                                                | 8.50 us: 1.01x faster                                                                                                      |
| xml_etree_process    | 36.7 ms                                                                                                                | 36.9 ms: 1.01x slower                                                                                                      |
| unpickle_list        | 2.71 us                                                                                                                | 2.78 us: 1.03x slower                                                                                                      |
| pickle               | 7.14 us                                                                                                                | 7.33 us: 1.03x slower                                                                                                      |
| unpickle_pure_python | 133 us                                                                                                                 | 142 us: 1.07x slower                                                                                                       |
| Geometric mean       | (ref)                                                                                                                  | 1.00x faster                                                                                                               |

Benchmark hidden because not significant (2): xml_etree_iterparse, pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 19.9 ms                                                                                                                | 23.2 ms: 1.17x slower                                                                                                      |
| python_startup_no_site | 17.6 ms                                                                                                                | 20.9 ms: 1.19x slower                                                                                                      |
| Geometric mean         | (ref)                                                                                                                  | 1.18x slower                                                                                                               |

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                 | results/bm-20240224-3.13.0a4+-948acd6/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json | results/bm-20240224-3.13.0a4+-948acd6-JIT/bm-20240224-pythonperf1-amd64-python-948acd6ed856251dc588-3.13.0a4+-948acd6.json |
|---------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody                     | 72.9 ms                                                                                                                | 61.9 ms: 1.18x faster                                                                                                      |
| float                     | 54.3 ms                                                                                                                | 50.0 ms: 1.09x faster                                                                                                      |
| json                      | 3.28 ms                                                                                                                | 3.02 ms: 1.09x faster                                                                                                      |
| tomli_loads               | 1.41 sec                                                                                                               | 1.32 sec: 1.07x faster                                                                                                     |
| telco                     | 4.86 ms                                                                                                                | 4.59 ms: 1.06x faster                                                                                                      |
| pickle_pure_python        | 185 us                                                                                                                 | 176 us: 1.05x faster                                                                                                       |
| pickle_dict               | 18.2 us                                                                                                                | 17.6 us: 1.04x faster                                                                                                      |
| chameleon                 | 4.98 ms                                                                                                                | 4.80 ms: 1.04x faster                                                                                                      |
| async_tree_memoization_tg | 354 ms                                                                                                                 | 344 ms: 1.03x faster                                                                                                       |
| typing_runtime_protocols  | 72.8 us                                                                                                                | 70.8 us: 1.03x faster                                                                                                      |
| generators                | 21.5 ms                                                                                                                | 20.9 ms: 1.03x faster                                                                                                      |
| deepcopy_reduce           | 1.99 us                                                                                                                | 1.94 us: 1.03x faster                                                                                                      |
| coroutines                | 13.5 ms                                                                                                                | 13.2 ms: 1.03x faster                                                                                                      |
| deepcopy_memo             | 22.3 us                                                                                                                | 21.8 us: 1.02x faster                                                                                                      |
| xml_etree_parse           | 94.1 ms                                                                                                                | 92.3 ms: 1.02x faster                                                                                                      |
| sqlite_synth              | 1.59 us                                                                                                                | 1.57 us: 1.02x faster                                                                                                      |
| deepcopy                  | 227 us                                                                                                                 | 224 us: 1.02x faster                                                                                                       |
| regex_dna                 | 120 ms                                                                                                                 | 119 ms: 1.02x faster                                                                                                       |
| async_tree_io             | 738 ms                                                                                                                 | 728 ms: 1.01x faster                                                                                                       |
| async_tree_none_tg        | 275 ms                                                                                                                 | 272 ms: 1.01x faster                                                                                                       |
| xml_etree_generate        | 53.9 ms                                                                                                                | 53.3 ms: 1.01x faster                                                                                                      |
| json_loads                | 14.0 us                                                                                                                | 13.8 us: 1.01x faster                                                                                                      |
| json_dumps                | 5.65 ms                                                                                                                | 5.59 ms: 1.01x faster                                                                                                      |
| unpickle                  | 8.58 us                                                                                                                | 8.50 us: 1.01x faster                                                                                                      |
| gc_traversal              | 1.51 ms                                                                                                                | 1.50 ms: 1.01x faster                                                                                                      |
| regex_effbot              | 1.58 ms                                                                                                                | 1.57 ms: 1.01x faster                                                                                                      |
| spectral_norm             | 64.4 ms                                                                                                                | 64.5 ms: 1.00x slower                                                                                                      |
| xml_etree_process         | 36.7 ms                                                                                                                | 36.9 ms: 1.01x slower                                                                                                      |
| logging_simple            | 6.06 us                                                                                                                | 6.13 us: 1.01x slower                                                                                                      |
| bench_thread_pool         | 828 us                                                                                                                 | 841 us: 1.02x slower                                                                                                       |
| coverage                  | 47.2 ms                                                                                                                | 48.0 ms: 1.02x slower                                                                                                      |
| tornado_http              | 84.0 ms                                                                                                                | 85.6 ms: 1.02x slower                                                                                                      |
| unpickle_list             | 2.71 us                                                                                                                | 2.78 us: 1.03x slower                                                                                                      |
| asyncio_tcp               | 463 ms                                                                                                                 | 475 ms: 1.03x slower                                                                                                       |
| pidigits                  | 148 ms                                                                                                                 | 152 ms: 1.03x slower                                                                                                       |
| pickle                    | 7.14 us                                                                                                                | 7.33 us: 1.03x slower                                                                                                      |
| pprint_safe_repr          | 501 ms                                                                                                                 | 517 ms: 1.03x slower                                                                                                       |
| create_gc_cycles          | 714 us                                                                                                                 | 738 us: 1.03x slower                                                                                                       |
| sqlglot_transpile         | 1.00 ms                                                                                                                | 1.04 ms: 1.04x slower                                                                                                      |
| sqlglot_normalize         | 177 ms                                                                                                                 | 184 ms: 1.04x slower                                                                                                       |
| pprint_pformat            | 1.03 sec                                                                                                               | 1.07 sec: 1.04x slower                                                                                                     |
| crypto_pyaes              | 44.3 ms                                                                                                                | 46.1 ms: 1.04x slower                                                                                                      |
| sqlglot_parse             | 781 us                                                                                                                 | 824 us: 1.06x slower                                                                                                       |
| fannkuch                  | 249 ms                                                                                                                 | 263 ms: 1.06x slower                                                                                                       |
| docutils                  | 1.57 sec                                                                                                               | 1.67 sec: 1.07x slower                                                                                                     |
| unpickle_pure_python      | 133 us                                                                                                                 | 142 us: 1.07x slower                                                                                                       |
| dulwich_log               | 40.4 ms                                                                                                                | 43.2 ms: 1.07x slower                                                                                                      |
| meteor_contest            | 71.9 ms                                                                                                                | 76.9 ms: 1.07x slower                                                                                                      |
| scimark_sparse_mat_mult   | 2.45 ms                                                                                                                | 2.63 ms: 1.07x slower                                                                                                      |
| deltablue                 | 2.03 ms                                                                                                                | 2.18 ms: 1.07x slower                                                                                                      |
| 2to3                      | 212 ms                                                                                                                 | 227 ms: 1.07x slower                                                                                                       |
| chaos                     | 40.4 ms                                                                                                                | 43.5 ms: 1.08x slower                                                                                                      |
| scimark_fft               | 179 ms                                                                                                                 | 194 ms: 1.08x slower                                                                                                       |
| sqlglot_optimize          | 33.4 ms                                                                                                                | 36.1 ms: 1.08x slower                                                                                                      |
| nqueens                   | 59.8 ms                                                                                                                | 64.7 ms: 1.08x slower                                                                                                      |
| bench_mp_pool             | 64.0 ms                                                                                                                | 69.4 ms: 1.08x slower                                                                                                      |
| mypy2                     | 415 ms                                                                                                                 | 459 ms: 1.11x slower                                                                                                       |
| richards_super            | 31.3 ms                                                                                                                | 35.0 ms: 1.12x slower                                                                                                      |
| sympy_str                 | 160 ms                                                                                                                 | 179 ms: 1.12x slower                                                                                                       |
| sympy_integrate           | 12.5 ms                                                                                                                | 14.0 ms: 1.12x slower                                                                                                      |
| sympy_sum                 | 83.7 ms                                                                                                                | 94.2 ms: 1.13x slower                                                                                                      |
| pyflate                   | 291 ms                                                                                                                 | 328 ms: 1.13x slower                                                                                                       |
| async_generators          | 226 ms                                                                                                                 | 255 ms: 1.13x slower                                                                                                       |
| sympy_expand              | 275 ms                                                                                                                 | 310 ms: 1.13x slower                                                                                                       |
| richards                  | 27.7 ms                                                                                                                | 31.4 ms: 1.14x slower                                                                                                      |
| raytrace                  | 166 ms                                                                                                                 | 191 ms: 1.15x slower                                                                                                       |
| comprehensions            | 10.6 us                                                                                                                | 12.2 us: 1.16x slower                                                                                                      |
| scimark_monte_carlo       | 41.0 ms                                                                                                                | 47.6 ms: 1.16x slower                                                                                                      |
| python_startup            | 19.9 ms                                                                                                                | 23.2 ms: 1.17x slower                                                                                                      |
| python_startup_no_site    | 17.6 ms                                                                                                                | 20.9 ms: 1.19x slower                                                                                                      |
| mdp                       | 1.37 sec                                                                                                               | 1.68 sec: 1.23x slower                                                                                                     |
| go                        | 85.7 ms                                                                                                                | 109 ms: 1.27x slower                                                                                                       |
| regex_compile             | 79.8 ms                                                                                                                | 104 ms: 1.30x slower                                                                                                       |
| scimark_sor               | 77.2 ms                                                                                                                | 102 ms: 1.32x slower                                                                                                       |
| scimark_lu                | 52.9 ms                                                                                                                | 76.6 ms: 1.45x slower                                                                                                      |
| hexiom                    | 3.89 ms                                                                                                                | 6.28 ms: 1.61x slower                                                                                                      |
| unpack_sequence           | 36.7 ns                                                                                                                | 88.5 ns: 2.41x slower                                                                                                      |
| Geometric mean            | (ref)                                                                                                                  | 1.06x slower                                                                                                               |

Benchmark hidden because not significant (14): pycparser, async_tree_none, xml_etree_iterparse, mako, async_tree_memoization, async_tree_io_tg, async_tree_cpu_io_mixed_tg, logging_silent, pathlib, logging_format, async_tree_cpu_io_mixed, asyncio_tcp_ssl, pickle_list, regex_v8


# HPT report

- Reliability score: 99.96% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown