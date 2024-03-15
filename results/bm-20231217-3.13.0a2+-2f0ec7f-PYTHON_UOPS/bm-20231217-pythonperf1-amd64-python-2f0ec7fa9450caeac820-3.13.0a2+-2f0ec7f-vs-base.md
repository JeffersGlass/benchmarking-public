# Results vs. base

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: windows-amd64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| 2to3           | 215 ms                                                                                                                 | 217 ms: 1.01x slower                                                                                                               |
| chameleon      | 4.86 ms                                                                                                                | 5.01 ms: 1.03x slower                                                                                                              |
| docutils       | 1.56 sec                                                                                                               | 1.57 sec: 1.01x slower                                                                                                             |
| Geometric mean | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| async_tree_io              | 724 ms                                                                                                                 | 733 ms: 1.01x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 448 ms                                                                                                                 | 455 ms: 1.01x slower                                                                                                               |
| async_tree_cpu_io_mixed_tg | 463 ms                                                                                                                 | 471 ms: 1.02x slower                                                                                                               |
| Geometric mean             | (ref)                                                                                                                  | 1.01x slower                                                                                                                       |

Benchmark hidden because not significant (5): async_tree_memoization, async_tree_none_tg, async_tree_memoization_tg, async_tree_io_tg, async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                                                                                 | 150 ms: 1.00x slower                                                                                                               |
| float          | 51.9 ms                                                                                                                | 58.1 ms: 1.12x slower                                                                                                              |
| nbody          | 69.5 ms                                                                                                                | 82.6 ms: 1.19x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.10x slower                                                                                                                       |

Benchmarks with tag 'regex':
============================

| Benchmark      | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| regex_dna      | 122 ms                                                                                                                 | 117 ms: 1.04x faster                                                                                                               |
| regex_v8       | 15.3 ms                                                                                                                | 14.7 ms: 1.04x faster                                                                                                              |
| regex_effbot   | 1.61 ms                                                                                                                | 1.56 ms: 1.03x faster                                                                                                              |
| regex_compile  | 77.9 ms                                                                                                                | 84.8 ms: 1.09x slower                                                                                                              |
| Geometric mean | (ref)                                                                                                                  | 1.00x faster                                                                                                                       |

Benchmarks with tag 'serialize':
================================

| Benchmark            | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| unpickle_list        | 2.69 us                                                                                                                | 2.56 us: 1.05x faster                                                                                                              |
| json_loads           | 13.6 us                                                                                                                | 13.3 us: 1.02x faster                                                                                                              |
| pickle_pure_python   | 181 us                                                                                                                 | 180 us: 1.01x faster                                                                                                               |
| json_dumps           | 5.49 ms                                                                                                                | 5.58 ms: 1.02x slower                                                                                                              |
| xml_etree_process    | 36.7 ms                                                                                                                | 37.3 ms: 1.02x slower                                                                                                              |
| pickle_dict          | 18.3 us                                                                                                                | 18.6 us: 1.02x slower                                                                                                              |
| xml_etree_parse      | 92.0 ms                                                                                                                | 94.0 ms: 1.02x slower                                                                                                              |
| xml_etree_generate   | 53.1 ms                                                                                                                | 54.9 ms: 1.03x slower                                                                                                              |
| pickle               | 7.02 us                                                                                                                | 7.30 us: 1.04x slower                                                                                                              |
| unpickle_pure_python | 129 us                                                                                                                 | 135 us: 1.05x slower                                                                                                               |
| tomli_loads          | 1.40 sec                                                                                                               | 1.48 sec: 1.05x slower                                                                                                             |
| xml_etree_iterparse  | 63.0 ms                                                                                                                | 66.5 ms: 1.06x slower                                                                                                              |
| pickle_list          | 2.86 us                                                                                                                | 3.36 us: 1.17x slower                                                                                                              |
| Geometric mean       | (ref)                                                                                                                  | 1.03x slower                                                                                                                       |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| python_startup_no_site | 18.8 ms                                                                                                                | 18.2 ms: 1.03x faster                                                                                                              |
| python_startup         | 20.6 ms                                                                                                                | 20.4 ms: 1.01x faster                                                                                                              |
| Geometric mean         | (ref)                                                                                                                  | 1.02x faster                                                                                                                       |

Benchmarks with tag 'template':
===============================

| Benchmark | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|-----------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| mako      | 6.41 ms                                                                                                                | 7.67 ms: 1.20x slower                                                                                                              |

All benchmarks:
===============

| Benchmark                  | results/bm-20231217-3.13.0a2+-2f0ec7f/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json | results/bm-20231217-3.13.0a2+-2f0ec7f-PYTHON_UOPS/bm-20231217-pythonperf1-amd64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f.json |
|----------------------------|:----------------------------------------------------------------------------------------------------------------------:|:----------------------------------------------------------------------------------------------------------------------------------:|
| asyncio_tcp_ssl            | 1.83 sec                                                                                                               | 1.65 sec: 1.11x faster                                                                                                             |
| unpickle_list              | 2.69 us                                                                                                                | 2.56 us: 1.05x faster                                                                                                              |
| bench_mp_pool              | 69.8 ms                                                                                                                | 66.7 ms: 1.05x faster                                                                                                              |
| telco                      | 4.92 ms                                                                                                                | 4.72 ms: 1.04x faster                                                                                                              |
| regex_dna                  | 122 ms                                                                                                                 | 117 ms: 1.04x faster                                                                                                               |
| regex_v8                   | 15.3 ms                                                                                                                | 14.7 ms: 1.04x faster                                                                                                              |
| python_startup_no_site     | 18.8 ms                                                                                                                | 18.2 ms: 1.03x faster                                                                                                              |
| regex_effbot               | 1.61 ms                                                                                                                | 1.56 ms: 1.03x faster                                                                                                              |
| coverage                   | 45.9 ms                                                                                                                | 44.7 ms: 1.03x faster                                                                                                              |
| json_loads                 | 13.6 us                                                                                                                | 13.3 us: 1.02x faster                                                                                                              |
| coroutines                 | 13.1 ms                                                                                                                | 12.9 ms: 1.02x faster                                                                                                              |
| dask                       | 258 ms                                                                                                                 | 255 ms: 1.01x faster                                                                                                               |
| python_startup             | 20.6 ms                                                                                                                | 20.4 ms: 1.01x faster                                                                                                              |
| pathlib                    | 79.8 ms                                                                                                                | 79.1 ms: 1.01x faster                                                                                                              |
| richards_super             | 31.2 ms                                                                                                                | 31.0 ms: 1.01x faster                                                                                                              |
| pickle_pure_python         | 181 us                                                                                                                 | 180 us: 1.01x faster                                                                                                               |
| pidigits                   | 150 ms                                                                                                                 | 150 ms: 1.00x slower                                                                                                               |
| sqlite_synth               | 1.56 us                                                                                                                | 1.57 us: 1.01x slower                                                                                                              |
| docutils                   | 1.56 sec                                                                                                               | 1.57 sec: 1.01x slower                                                                                                             |
| scimark_lu                 | 55.4 ms                                                                                                                | 55.9 ms: 1.01x slower                                                                                                              |
| 2to3                       | 215 ms                                                                                                                 | 217 ms: 1.01x slower                                                                                                               |
| sqlglot_parse              | 765 us                                                                                                                 | 773 us: 1.01x slower                                                                                                               |
| async_tree_io              | 724 ms                                                                                                                 | 733 ms: 1.01x slower                                                                                                               |
| richards                   | 27.5 ms                                                                                                                | 27.9 ms: 1.01x slower                                                                                                              |
| mypy2                      | 414 ms                                                                                                                 | 420 ms: 1.01x slower                                                                                                               |
| async_tree_cpu_io_mixed    | 448 ms                                                                                                                 | 455 ms: 1.01x slower                                                                                                               |
| gc_traversal               | 1.49 ms                                                                                                                | 1.51 ms: 1.02x slower                                                                                                              |
| scimark_sor                | 79.9 ms                                                                                                                | 81.1 ms: 1.02x slower                                                                                                              |
| json_dumps                 | 5.49 ms                                                                                                                | 5.58 ms: 1.02x slower                                                                                                              |
| sympy_expand               | 272 ms                                                                                                                 | 277 ms: 1.02x slower                                                                                                               |
| xml_etree_process          | 36.7 ms                                                                                                                | 37.3 ms: 1.02x slower                                                                                                              |
| pickle_dict                | 18.3 us                                                                                                                | 18.6 us: 1.02x slower                                                                                                              |
| async_tree_cpu_io_mixed_tg | 463 ms                                                                                                                 | 471 ms: 1.02x slower                                                                                                               |
| deepcopy_reduce            | 1.95 us                                                                                                                | 1.99 us: 1.02x slower                                                                                                              |
| xml_etree_parse            | 92.0 ms                                                                                                                | 94.0 ms: 1.02x slower                                                                                                              |
| async_generators           | 224 ms                                                                                                                 | 229 ms: 1.02x slower                                                                                                               |
| dulwich_log                | 41.9 ms                                                                                                                | 42.9 ms: 1.02x slower                                                                                                              |
| sqlglot_transpile          | 980 us                                                                                                                 | 1.00 ms: 1.02x slower                                                                                                              |
| logging_silent             | 53.8 ns                                                                                                                | 55.3 ns: 1.03x slower                                                                                                              |
| chameleon                  | 4.86 ms                                                                                                                | 5.01 ms: 1.03x slower                                                                                                              |
| deepcopy                   | 220 us                                                                                                                 | 227 us: 1.03x slower                                                                                                               |
| logging_format             | 6.47 us                                                                                                                | 6.68 us: 1.03x slower                                                                                                              |
| xml_etree_generate         | 53.1 ms                                                                                                                | 54.9 ms: 1.03x slower                                                                                                              |
| pickle                     | 7.02 us                                                                                                                | 7.30 us: 1.04x slower                                                                                                              |
| logging_simple             | 5.99 us                                                                                                                | 6.24 us: 1.04x slower                                                                                                              |
| typing_runtime_protocols   | 72.3 us                                                                                                                | 75.4 us: 1.04x slower                                                                                                              |
| sympy_sum                  | 83.3 ms                                                                                                                | 87.0 ms: 1.04x slower                                                                                                              |
| meteor_contest             | 73.0 ms                                                                                                                | 76.3 ms: 1.04x slower                                                                                                              |
| sqlglot_normalize          | 177 ms                                                                                                                 | 185 ms: 1.04x slower                                                                                                               |
| deepcopy_memo              | 21.9 us                                                                                                                | 22.9 us: 1.05x slower                                                                                                              |
| sympy_str                  | 160 ms                                                                                                                 | 167 ms: 1.05x slower                                                                                                               |
| sqlglot_optimize           | 33.8 ms                                                                                                                | 35.4 ms: 1.05x slower                                                                                                              |
| unpickle_pure_python       | 129 us                                                                                                                 | 135 us: 1.05x slower                                                                                                               |
| go                         | 88.5 ms                                                                                                                | 93.0 ms: 1.05x slower                                                                                                              |
| tomli_loads                | 1.40 sec                                                                                                               | 1.48 sec: 1.05x slower                                                                                                             |
| raytrace                   | 166 ms                                                                                                                 | 175 ms: 1.06x slower                                                                                                               |
| xml_etree_iterparse        | 63.0 ms                                                                                                                | 66.5 ms: 1.06x slower                                                                                                              |
| sympy_integrate            | 12.4 ms                                                                                                                | 13.2 ms: 1.06x slower                                                                                                              |
| pprint_safe_repr           | 488 ms                                                                                                                 | 531 ms: 1.09x slower                                                                                                               |
| regex_compile              | 77.9 ms                                                                                                                | 84.8 ms: 1.09x slower                                                                                                              |
| mdp                        | 1.41 sec                                                                                                               | 1.53 sec: 1.09x slower                                                                                                             |
| pprint_pformat             | 996 ms                                                                                                                 | 1.09 sec: 1.09x slower                                                                                                             |
| unpack_sequence            | 36.4 ns                                                                                                                | 40.3 ns: 1.11x slower                                                                                                              |
| fannkuch                   | 240 ms                                                                                                                 | 268 ms: 1.12x slower                                                                                                               |
| float                      | 51.9 ms                                                                                                                | 58.1 ms: 1.12x slower                                                                                                              |
| pyflate                    | 287 ms                                                                                                                 | 323 ms: 1.12x slower                                                                                                               |
| crypto_pyaes               | 43.3 ms                                                                                                                | 48.9 ms: 1.13x slower                                                                                                              |
| nqueens                    | 58.1 ms                                                                                                                | 65.9 ms: 1.13x slower                                                                                                              |
| scimark_fft                | 182 ms                                                                                                                 | 210 ms: 1.15x slower                                                                                                               |
| chaos                      | 39.2 ms                                                                                                                | 45.2 ms: 1.15x slower                                                                                                              |
| pickle_list                | 2.86 us                                                                                                                | 3.36 us: 1.17x slower                                                                                                              |
| nbody                      | 69.5 ms                                                                                                                | 82.6 ms: 1.19x slower                                                                                                              |
| mako                       | 6.41 ms                                                                                                                | 7.67 ms: 1.20x slower                                                                                                              |
| scimark_monte_carlo        | 40.1 ms                                                                                                                | 49.5 ms: 1.24x slower                                                                                                              |
| comprehensions             | 10.5 us                                                                                                                | 13.3 us: 1.27x slower                                                                                                              |
| scimark_sparse_mat_mult    | 2.36 ms                                                                                                                | 3.12 ms: 1.33x slower                                                                                                              |
| hexiom                     | 3.80 ms                                                                                                                | 5.07 ms: 1.33x slower                                                                                                              |
| deltablue                  | 2.01 ms                                                                                                                | 2.77 ms: 1.38x slower                                                                                                              |
| spectral_norm              | 60.2 ms                                                                                                                | 85.0 ms: 1.41x slower                                                                                                              |
| Geometric mean             | (ref)                                                                                                                  | 1.05x slower                                                                                                                       |

Benchmark hidden because not significant (13): pycparser, json, async_tree_memoization, async_tree_none_tg, unpickle, bench_thread_pool, tornado_http, generators, async_tree_memoization_tg, create_gc_cycles, asyncio_tcp, async_tree_io_tg, async_tree_none


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown