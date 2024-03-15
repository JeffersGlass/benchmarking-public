# Results vs. base

- fork: python
- ref: d1fd0606591e1258eb08
- machine: windows-amd64
- commit hash: d1fd060
- commit date: 2024-03-03
- overall geometric mean: 1.03x slower
- HPT reliability: 99.80%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 213 ms                                                                                                                 | 226 ms: 1.06x slower                                                                                                       |
| docutils       | 1.55 sec                                                                                                               | 1.61 sec: 1.04x slower                                                                                                     |
| tornado_http   | 83.4 ms                                                                                                                | 85.2 ms: 1.02x slower                                                                                                      |
| Geometric mean | (ref)                                                                                                                  | 1.03x slower                                                                                                               |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

Benchmark hidden because not significant (8): async_tree_io, async_tree_cpu_io_mixed_tg, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_none_tg, async_tree_memoization, async_tree_none, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody          | 69.7 ms                                                                                                                | 60.2 ms: 1.16x faster                                                                                                      |
| float          | 52.9 ms                                                                                                                | 49.5 ms: 1.07x faster                                                                                                      |
| pidigits       | 147 ms                                                                                                                 | 150 ms: 1.02x slower                                                                                                       |
| Geometric mean | (ref)                                                                                                                  | 1.07x faster                                                                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 121 ms                                                                                                                 | 116 ms: 1.04x faster                                                                                                       |
| regex_effbot   | 1.59 ms                                                                                                                | 1.55 ms: 1.03x faster                                                                                                      |
| regex_compile  | 77.5 ms                                                                                                                | 90.7 ms: 1.17x slower                                                                                                      |
| Geometric mean | (ref)                                                                                                                  | 1.02x slower                                                                                                               |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| tomli_loads          | 1.44 sec                                                                                                               | 1.29 sec: 1.12x faster                                                                                                     |
| pickle_dict          | 18.4 us                                                                                                                | 17.6 us: 1.05x faster                                                                                                      |
| pickle_pure_python   | 181 us                                                                                                                 | 176 us: 1.03x faster                                                                                                       |
| json_loads           | 13.7 us                                                                                                                | 13.9 us: 1.02x slower                                                                                                      |
| unpickle             | 8.28 us                                                                                                                | 8.46 us: 1.02x slower                                                                                                      |
| xml_etree_process    | 36.0 ms                                                                                                                | 36.9 ms: 1.02x slower                                                                                                      |
| pickle               | 7.14 us                                                                                                                | 7.33 us: 1.03x slower                                                                                                      |
| xml_etree_generate   | 52.2 ms                                                                                                                | 54.3 ms: 1.04x slower                                                                                                      |
| unpickle_pure_python | 127 us                                                                                                                 | 139 us: 1.09x slower                                                                                                       |
| Geometric mean       | (ref)                                                                                                                  | 1.00x slower                                                                                                               |

Benchmark hidden because not significant (5): pickle_list, json_dumps, xml_etree_parse, xml_etree_iterparse, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| python_startup         | 20.0 ms                                                                                                                | 24.3 ms: 1.22x slower                                                                                                      |
| python_startup_no_site | 17.8 ms                                                                                                                | 22.2 ms: 1.25x slower                                                                                                      |
| Geometric mean         | (ref)                                                                                                                  | 1.23x slower                                                                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.48 ms                                                                                                                | 6.12 ms: 1.06x faster                                                                                                      |

All benchmarks:
===============

| Benchmark                | results/bm-20240303-3.13.0a4+-d1fd060/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json | results/bm-20240303-3.13.0a4+-d1fd060-JIT/bm-20240303-pythonperf1-amd64-python-d1fd0606591e1258eb08-3.13.0a4+-d1fd060.json |
|--------------------------|:----------------------------------------------------------------------------------------------------------------------:|:--------------------------------------------------------------------------------------------------------------------------:|
| nbody                    | 69.7 ms                                                                                                                | 60.2 ms: 1.16x faster                                                                                                      |
| tomli_loads              | 1.44 sec                                                                                                               | 1.29 sec: 1.12x faster                                                                                                     |
| json                     | 3.28 ms                                                                                                                | 3.00 ms: 1.09x faster                                                                                                      |
| float                    | 52.9 ms                                                                                                                | 49.5 ms: 1.07x faster                                                                                                      |
| spectral_norm            | 60.8 ms                                                                                                                | 57.0 ms: 1.07x faster                                                                                                      |
| mako                     | 6.48 ms                                                                                                                | 6.12 ms: 1.06x faster                                                                                                      |
| scimark_sparse_mat_mult  | 2.41 ms                                                                                                                | 2.29 ms: 1.05x faster                                                                                                      |
| pycparser                | 714 ms                                                                                                                 | 681 ms: 1.05x faster                                                                                                       |
| pickle_dict              | 18.4 us                                                                                                                | 17.6 us: 1.05x faster                                                                                                      |
| regex_dna                | 121 ms                                                                                                                 | 116 ms: 1.04x faster                                                                                                       |
| deepcopy_reduce          | 2.00 us                                                                                                                | 1.94 us: 1.03x faster                                                                                                      |
| telco                    | 4.85 ms                                                                                                                | 4.70 ms: 1.03x faster                                                                                                      |
| coverage                 | 47.0 ms                                                                                                                | 45.7 ms: 1.03x faster                                                                                                      |
| regex_effbot             | 1.59 ms                                                                                                                | 1.55 ms: 1.03x faster                                                                                                      |
| typing_runtime_protocols | 72.7 us                                                                                                                | 70.9 us: 1.03x faster                                                                                                      |
| pickle_pure_python       | 181 us                                                                                                                 | 176 us: 1.03x faster                                                                                                       |
| deepcopy                 | 227 us                                                                                                                 | 222 us: 1.02x faster                                                                                                       |
| sqlglot_normalize        | 179 ms                                                                                                                 | 176 ms: 1.02x faster                                                                                                       |
| logging_silent           | 56.1 ns                                                                                                                | 55.4 ns: 1.01x faster                                                                                                      |
| deepcopy_memo            | 22.4 us                                                                                                                | 22.1 us: 1.01x faster                                                                                                      |
| logging_simple           | 5.95 us                                                                                                                | 5.90 us: 1.01x faster                                                                                                      |
| gc_traversal             | 1.51 ms                                                                                                                | 1.50 ms: 1.01x faster                                                                                                      |
| meteor_contest           | 73.1 ms                                                                                                                | 73.4 ms: 1.00x slower                                                                                                      |
| sqlite_synth             | 1.56 us                                                                                                                | 1.58 us: 1.01x slower                                                                                                      |
| scimark_fft              | 177 ms                                                                                                                 | 180 ms: 1.01x slower                                                                                                       |
| json_loads               | 13.7 us                                                                                                                | 13.9 us: 1.02x slower                                                                                                      |
| pidigits                 | 147 ms                                                                                                                 | 150 ms: 1.02x slower                                                                                                       |
| deltablue                | 2.02 ms                                                                                                                | 2.06 ms: 1.02x slower                                                                                                      |
| tornado_http             | 83.4 ms                                                                                                                | 85.2 ms: 1.02x slower                                                                                                      |
| unpickle                 | 8.28 us                                                                                                                | 8.46 us: 1.02x slower                                                                                                      |
| xml_etree_process        | 36.0 ms                                                                                                                | 36.9 ms: 1.02x slower                                                                                                      |
| dulwich_log              | 39.9 ms                                                                                                                | 40.8 ms: 1.02x slower                                                                                                      |
| comprehensions           | 10.7 us                                                                                                                | 11.0 us: 1.03x slower                                                                                                      |
| pickle                   | 7.14 us                                                                                                                | 7.33 us: 1.03x slower                                                                                                      |
| sqlglot_optimize         | 33.7 ms                                                                                                                | 35.0 ms: 1.04x slower                                                                                                      |
| pyflate                  | 290 ms                                                                                                                 | 301 ms: 1.04x slower                                                                                                       |
| pprint_safe_repr         | 499 ms                                                                                                                 | 518 ms: 1.04x slower                                                                                                       |
| xml_etree_generate       | 52.2 ms                                                                                                                | 54.3 ms: 1.04x slower                                                                                                      |
| docutils                 | 1.55 sec                                                                                                               | 1.61 sec: 1.04x slower                                                                                                     |
| pprint_pformat           | 1.02 sec                                                                                                               | 1.07 sec: 1.05x slower                                                                                                     |
| sqlglot_transpile        | 967 us                                                                                                                 | 1.02 ms: 1.05x slower                                                                                                      |
| chaos                    | 39.1 ms                                                                                                                | 41.3 ms: 1.06x slower                                                                                                      |
| 2to3                     | 213 ms                                                                                                                 | 226 ms: 1.06x slower                                                                                                       |
| sqlglot_parse            | 749 us                                                                                                                 | 796 us: 1.06x slower                                                                                                       |
| mdp                      | 1.39 sec                                                                                                               | 1.48 sec: 1.06x slower                                                                                                     |
| crypto_pyaes             | 41.8 ms                                                                                                                | 44.5 ms: 1.07x slower                                                                                                      |
| mypy2                    | 413 ms                                                                                                                 | 441 ms: 1.07x slower                                                                                                       |
| sympy_str                | 155 ms                                                                                                                 | 166 ms: 1.08x slower                                                                                                       |
| async_generators         | 228 ms                                                                                                                 | 247 ms: 1.08x slower                                                                                                       |
| sympy_sum                | 81.1 ms                                                                                                                | 87.9 ms: 1.08x slower                                                                                                      |
| fannkuch                 | 241 ms                                                                                                                 | 261 ms: 1.09x slower                                                                                                       |
| unpickle_pure_python     | 127 us                                                                                                                 | 139 us: 1.09x slower                                                                                                       |
| sympy_expand             | 262 ms                                                                                                                 | 287 ms: 1.09x slower                                                                                                       |
| sympy_integrate          | 12.1 ms                                                                                                                | 13.4 ms: 1.11x slower                                                                                                      |
| raytrace                 | 164 ms                                                                                                                 | 182 ms: 1.11x slower                                                                                                       |
| richards_super           | 30.3 ms                                                                                                                | 34.2 ms: 1.13x slower                                                                                                      |
| scimark_sor              | 76.6 ms                                                                                                                | 87.3 ms: 1.14x slower                                                                                                      |
| richards                 | 27.0 ms                                                                                                                | 30.8 ms: 1.14x slower                                                                                                      |
| nqueens                  | 57.1 ms                                                                                                                | 65.3 ms: 1.14x slower                                                                                                      |
| bench_mp_pool            | 64.1 ms                                                                                                                | 73.4 ms: 1.15x slower                                                                                                      |
| regex_compile            | 77.5 ms                                                                                                                | 90.7 ms: 1.17x slower                                                                                                      |
| scimark_monte_carlo      | 39.6 ms                                                                                                                | 46.6 ms: 1.18x slower                                                                                                      |
| go                       | 84.7 ms                                                                                                                | 99.5 ms: 1.18x slower                                                                                                      |
| python_startup           | 20.0 ms                                                                                                                | 24.3 ms: 1.22x slower                                                                                                      |
| python_startup_no_site   | 17.8 ms                                                                                                                | 22.2 ms: 1.25x slower                                                                                                      |
| hexiom                   | 3.76 ms                                                                                                                | 5.04 ms: 1.34x slower                                                                                                      |
| scimark_lu               | 52.5 ms                                                                                                                | 74.0 ms: 1.41x slower                                                                                                      |
| unpack_sequence          | 39.3 ns                                                                                                                | 57.1 ns: 1.45x slower                                                                                                      |
| Geometric mean           | (ref)                                                                                                                  | 1.03x slower                                                                                                               |

Benchmark hidden because not significant (24): asyncio_tcp_ssl, pickle_list, async_tree_io, async_tree_cpu_io_mixed_tg, asyncio_tcp, logging_format, json_dumps, chameleon, async_tree_cpu_io_mixed, async_tree_io_tg, async_tree_none_tg, async_tree_memoization, coroutines, pathlib, regex_v8, async_tree_none, dask, xml_etree_parse, generators, xml_etree_iterparse, unpickle_list, create_gc_cycles, bench_thread_pool, async_tree_memoization_tg


# HPT report

- Reliability score: 99.80% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown