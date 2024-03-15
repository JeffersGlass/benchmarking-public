# Results vs. base

- fork: Fidget-Spinner
- ref: tier2_abstract_inter
- machine: windows-amd64
- commit hash: 913d95b
- commit date: 2024-01-30
- overall geometric mean: 1.00x faster
- HPT reliability: 91.04%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| 2to3           | 221 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| tornado_http   | 87.6 ms                                                                     | 86.7 ms: 1.01x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (2): chameleon, docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark                 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|---------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| async_tree_memoization_tg | 364 ms                                                                      | 356 ms: 1.02x faster                                                                  |
| async_tree_memoization    | 340 ms                                                                      | 346 ms: 1.02x slower                                                                  |
| Geometric mean            | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (6): async_tree_io, async_tree_cpu_io_mixed, async_tree_none, async_tree_none_tg, async_tree_io_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                                      | 154 ms: 1.01x slower                                                                  |
| nbody          | 60.9 ms                                                                     | 62.2 ms: 1.02x slower                                                                 |
| float          | 51.0 ms                                                                     | 52.1 ms: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.02x slower                                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_v8       | 21.9 ms                                                                     | 14.6 ms: 1.50x faster                                                                 |
| regex_dna      | 124 ms                                                                      | 122 ms: 1.01x faster                                                                  |
| regex_effbot   | 1.60 ms                                                                     | 1.58 ms: 1.01x faster                                                                 |
| regex_compile  | 81.0 ms                                                                     | 82.7 ms: 1.02x slower                                                                 |
| Geometric mean | (ref)                                                                       | 1.11x faster                                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| xml_etree_process    | 37.0 ms                                                                     | 35.8 ms: 1.03x faster                                                                 |
| xml_etree_generate   | 53.5 ms                                                                     | 52.2 ms: 1.02x faster                                                                 |
| json_dumps           | 5.55 ms                                                                     | 5.44 ms: 1.02x faster                                                                 |
| xml_etree_iterparse  | 65.9 ms                                                                     | 64.7 ms: 1.02x faster                                                                 |
| json_loads           | 13.7 us                                                                     | 13.5 us: 1.02x faster                                                                 |
| unpickle_list        | 2.87 us                                                                     | 2.84 us: 1.01x faster                                                                 |
| pickle               | 7.28 us                                                                     | 7.31 us: 1.00x slower                                                                 |
| xml_etree_parse      | 94.6 ms                                                                     | 95.2 ms: 1.01x slower                                                                 |
| pickle_list          | 2.77 us                                                                     | 2.82 us: 1.02x slower                                                                 |
| pickle_pure_python   | 173 us                                                                      | 177 us: 1.02x slower                                                                  |
| unpickle_pure_python | 125 us                                                                      | 131 us: 1.05x slower                                                                  |
| Geometric mean       | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (3): unpickle, tomli_loads, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark      | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|----------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| python_startup | 21.3 ms                                                                     | 21.1 ms: 1.01x faster                                                                 |
| Geometric mean | (ref)                                                                       | 1.01x faster                                                                          |

Benchmark hidden because not significant (1): python_startup_no_site

Benchmarks with tag 'template':
===============================

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark                 | bm-20240129-pythonperf1-amd64-python-742ba6081c92744ba30f-3.13.0a3+-742ba60 | bm-20240130-pythonperf1-amd64-Fidget%2dSpinner-tier2_abstract_inter-3.13.0a3+-913d95b |
|---------------------------|:---------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------:|
| regex_v8                  | 21.9 ms                                                                     | 14.6 ms: 1.50x faster                                                                 |
| asyncio_tcp_ssl           | 1.87 sec                                                                    | 1.52 sec: 1.22x faster                                                                |
| spectral_norm             | 65.8 ms                                                                     | 62.9 ms: 1.05x faster                                                                 |
| unpack_sequence           | 40.7 ns                                                                     | 39.1 ns: 1.04x faster                                                                 |
| xml_etree_process         | 37.0 ms                                                                     | 35.8 ms: 1.03x faster                                                                 |
| dulwich_log               | 43.3 ms                                                                     | 42.2 ms: 1.03x faster                                                                 |
| typing_runtime_protocols  | 69.9 us                                                                     | 68.1 us: 1.03x faster                                                                 |
| logging_silent            | 53.5 ns                                                                     | 52.2 ns: 1.02x faster                                                                 |
| xml_etree_generate        | 53.5 ms                                                                     | 52.2 ms: 1.02x faster                                                                 |
| pathlib                   | 81.7 ms                                                                     | 79.8 ms: 1.02x faster                                                                 |
| async_tree_memoization_tg | 364 ms                                                                      | 356 ms: 1.02x faster                                                                  |
| json_dumps                | 5.55 ms                                                                     | 5.44 ms: 1.02x faster                                                                 |
| xml_etree_iterparse       | 65.9 ms                                                                     | 64.7 ms: 1.02x faster                                                                 |
| json_loads                | 13.7 us                                                                     | 13.5 us: 1.02x faster                                                                 |
| gc_traversal              | 1.54 ms                                                                     | 1.52 ms: 1.02x faster                                                                 |
| telco                     | 4.67 ms                                                                     | 4.59 ms: 1.02x faster                                                                 |
| scimark_sparse_mat_mult   | 2.76 ms                                                                     | 2.72 ms: 1.01x faster                                                                 |
| regex_dna                 | 124 ms                                                                      | 122 ms: 1.01x faster                                                                  |
| python_startup            | 21.3 ms                                                                     | 21.1 ms: 1.01x faster                                                                 |
| unpickle_list             | 2.87 us                                                                     | 2.84 us: 1.01x faster                                                                 |
| regex_effbot              | 1.60 ms                                                                     | 1.58 ms: 1.01x faster                                                                 |
| deepcopy_memo             | 21.4 us                                                                     | 21.2 us: 1.01x faster                                                                 |
| tornado_http              | 87.6 ms                                                                     | 86.7 ms: 1.01x faster                                                                 |
| richards                  | 25.1 ms                                                                     | 24.9 ms: 1.01x faster                                                                 |
| async_generators          | 244 ms                                                                      | 242 ms: 1.01x faster                                                                  |
| generators                | 21.1 ms                                                                     | 20.9 ms: 1.01x faster                                                                 |
| pickle                    | 7.28 us                                                                     | 7.31 us: 1.00x slower                                                                 |
| deepcopy                  | 217 us                                                                      | 218 us: 1.01x slower                                                                  |
| mypy2                     | 432 ms                                                                      | 435 ms: 1.01x slower                                                                  |
| xml_etree_parse           | 94.6 ms                                                                     | 95.2 ms: 1.01x slower                                                                 |
| coverage                  | 45.5 ms                                                                     | 45.8 ms: 1.01x slower                                                                 |
| richards_super            | 28.1 ms                                                                     | 28.3 ms: 1.01x slower                                                                 |
| sqlglot_transpile         | 976 us                                                                      | 984 us: 1.01x slower                                                                  |
| scimark_fft               | 193 ms                                                                      | 195 ms: 1.01x slower                                                                  |
| 2to3                      | 221 ms                                                                      | 224 ms: 1.01x slower                                                                  |
| pidigits                  | 152 ms                                                                      | 154 ms: 1.01x slower                                                                  |
| nqueens                   | 59.0 ms                                                                     | 59.7 ms: 1.01x slower                                                                 |
| sqlglot_parse             | 750 us                                                                      | 760 us: 1.01x slower                                                                  |
| logging_format            | 6.40 us                                                                     | 6.48 us: 1.01x slower                                                                 |
| go                        | 96.0 ms                                                                     | 97.4 ms: 1.01x slower                                                                 |
| pyflate                   | 312 ms                                                                      | 316 ms: 1.01x slower                                                                  |
| pickle_list               | 2.77 us                                                                     | 2.82 us: 1.02x slower                                                                 |
| async_tree_memoization    | 340 ms                                                                      | 346 ms: 1.02x slower                                                                  |
| fannkuch                  | 246 ms                                                                      | 251 ms: 1.02x slower                                                                  |
| scimark_lu                | 54.1 ms                                                                     | 55.2 ms: 1.02x slower                                                                 |
| pickle_pure_python        | 173 us                                                                      | 177 us: 1.02x slower                                                                  |
| deepcopy_reduce           | 1.89 us                                                                     | 1.93 us: 1.02x slower                                                                 |
| crypto_pyaes              | 46.9 ms                                                                     | 47.9 ms: 1.02x slower                                                                 |
| sympy_sum                 | 88.8 ms                                                                     | 90.7 ms: 1.02x slower                                                                 |
| regex_compile             | 81.0 ms                                                                     | 82.7 ms: 1.02x slower                                                                 |
| nbody                     | 60.9 ms                                                                     | 62.2 ms: 1.02x slower                                                                 |
| float                     | 51.0 ms                                                                     | 52.1 ms: 1.02x slower                                                                 |
| sqlglot_optimize          | 34.1 ms                                                                     | 34.9 ms: 1.02x slower                                                                 |
| logging_simple            | 5.89 us                                                                     | 6.02 us: 1.02x slower                                                                 |
| scimark_monte_carlo       | 57.0 ms                                                                     | 58.3 ms: 1.02x slower                                                                 |
| raytrace                  | 168 ms                                                                      | 172 ms: 1.02x slower                                                                  |
| comprehensions            | 11.4 us                                                                     | 11.7 us: 1.03x slower                                                                 |
| meteor_contest            | 78.0 ms                                                                     | 80.1 ms: 1.03x slower                                                                 |
| bench_mp_pool             | 69.1 ms                                                                     | 71.4 ms: 1.03x slower                                                                 |
| sympy_str                 | 164 ms                                                                      | 170 ms: 1.04x slower                                                                  |
| scimark_sor               | 74.7 ms                                                                     | 77.6 ms: 1.04x slower                                                                 |
| sqlglot_normalize         | 173 ms                                                                      | 180 ms: 1.04x slower                                                                  |
| mdp                       | 1.55 sec                                                                    | 1.62 sec: 1.04x slower                                                                |
| bench_thread_pool         | 821 us                                                                      | 859 us: 1.05x slower                                                                  |
| coroutines                | 12.9 ms                                                                     | 13.5 ms: 1.05x slower                                                                 |
| unpickle_pure_python      | 125 us                                                                      | 131 us: 1.05x slower                                                                  |
| hexiom                    | 5.18 ms                                                                     | 5.44 ms: 1.05x slower                                                                 |
| sympy_integrate           | 13.2 ms                                                                     | 13.9 ms: 1.05x slower                                                                 |
| json                      | 3.03 ms                                                                     | 3.33 ms: 1.10x slower                                                                 |
| Geometric mean            | (ref)                                                                       | 1.00x faster                                                                          |

Benchmark hidden because not significant (23): asyncio_tcp, async_tree_io, unpickle, async_tree_cpu_io_mixed, tomli_loads, chameleon, sqlite_synth, async_tree_none, async_tree_none_tg, pprint_safe_repr, async_tree_io_tg, sympy_expand, python_startup_no_site, docutils, pickle_dict, deltablue, chaos, create_gc_cycles, async_tree_cpu_io_mixed_tg, dask, mako, pprint_pformat, pycparser


# HPT report

- Reliability score: 91.04% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown