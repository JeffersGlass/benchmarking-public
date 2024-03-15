
# Results vs. 3.11.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: windows-amd64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.12x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 192 ms: 1.11x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.41 ms: 1.19x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.50 sec: 1.10x faster                                                     |
| html5lib       | 38.9 ms                                                     | 34.1 ms: 1.14x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 90.5 ms: 1.03x faster                                                      |
| Geometric mean | (ref)                                                       | 1.11x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 356 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 480 ms: 1.10x faster                                                       |
| async_tree_none         | 332 ms                                                      | 302 ms: 1.10x faster                                                       |
| async_tree_io           | 808 ms                                                      | 748 ms: 1.08x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 59.1 ms: 1.19x faster                                                      |
| float          | 54.4 ms                                                     | 47.3 ms: 1.15x faster                                                      |
| pidigits       | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 78.8 ms: 1.16x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.68 ms: 1.12x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.38 ms: 1.50x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 120 us: 1.31x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 166 us: 1.25x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 33.5 ms: 1.11x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 88.5 ms: 1.10x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 49.5 ms: 1.06x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| pickle               | 6.64 us                                                     | 6.77 us: 1.02x slower                                                      |
| unpickle_list        | 2.59 us                                                     | 2.65 us: 1.02x slower                                                      |
| json_loads           | 13.0 us                                                     | 14.2 us: 1.09x slower                                                      |
| unpickle             | 7.57 us                                                     | 9.39 us: 1.24x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.07x faster                                                               |

Benchmark hidden because not significant (2): pickle_list, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.5 ms: 1.09x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 14.2 ms: 1.30x faster                                                      |
| mako            | 7.58 ms                                                     | 6.15 ms: 1.23x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 32.6 ms: 1.23x faster                                                      |
| django_template | 24.4 ms                                                     | 20.2 ms: 1.21x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.24x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 25.6 ns: 1.83x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 466 ms: 1.56x faster                                                       |
| json_dumps              | 8.09 ms                                                     | 5.38 ms: 1.50x faster                                                      |
| deltablue               | 2.70 ms                                                     | 1.96 ms: 1.38x faster                                                      |
| comprehensions          | 15.6 us                                                     | 11.7 us: 1.34x faster                                                      |
| richards                | 31.4 ms                                                     | 23.9 ms: 1.31x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 120 us: 1.31x faster                                                       |
| genshi_text             | 18.4 ms                                                     | 14.2 ms: 1.30x faster                                                      |
| go                      | 101 ms                                                      | 78.8 ms: 1.28x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 166 us: 1.25x faster                                                       |
| raytrace                | 213 ms                                                      | 170 ms: 1.25x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 54.6 ms: 1.25x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 58.1 ns: 1.24x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.15 ms: 1.23x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 21.1 us: 1.23x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 32.6 ms: 1.23x faster                                                      |
| chaos                   | 48.4 ms                                                     | 39.6 ms: 1.22x faster                                                      |
| hexiom                  | 4.55 ms                                                     | 3.73 ms: 1.22x faster                                                      |
| django_template         | 24.4 ms                                                     | 20.2 ms: 1.21x faster                                                      |
| pprint_pformat          | 1.09 sec                                                    | 907 ms: 1.20x faster                                                       |
| scimark_monte_carlo     | 45.3 ms                                                     | 37.9 ms: 1.20x faster                                                      |
| chameleon               | 5.26 ms                                                     | 4.41 ms: 1.19x faster                                                      |
| fannkuch                | 253 ms                                                      | 213 ms: 1.19x faster                                                       |
| nbody                   | 70.3 ms                                                     | 59.1 ms: 1.19x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 445 ms: 1.19x faster                                                       |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.18 ms: 1.18x faster                                                      |
| pyflate                 | 312 ms                                                      | 267 ms: 1.17x faster                                                       |
| deepcopy                | 246 us                                                      | 211 us: 1.17x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 67.0 ms: 1.17x faster                                                      |
| regex_compile           | 91.0 ms                                                     | 78.8 ms: 1.16x faster                                                      |
| float                   | 54.4 ms                                                     | 47.3 ms: 1.15x faster                                                      |
| logging_simple          | 6.86 us                                                     | 6.01 us: 1.14x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.28 us: 1.14x faster                                                      |
| html5lib                | 38.9 ms                                                     | 34.1 ms: 1.14x faster                                                      |
| pycparser               | 720 ms                                                      | 633 ms: 1.14x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 12.4 ms: 1.13x faster                                                      |
| sympy_str               | 185 ms                                                      | 164 ms: 1.13x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 356 ms: 1.12x faster                                                       |
| sqlglot_parse           | 953 us                                                      | 851 us: 1.12x faster                                                       |
| sympy_sum               | 100 ms                                                      | 89.5 ms: 1.12x faster                                                      |
| sqlglot_normalize       | 190 ms                                                      | 171 ms: 1.11x faster                                                       |
| 2to3                    | 214 ms                                                      | 192 ms: 1.11x faster                                                       |
| spectral_norm           | 68.3 ms                                                     | 61.5 ms: 1.11x faster                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 44.0 ms: 1.11x faster                                                      |
| xml_etree_process       | 37.2 ms                                                     | 33.5 ms: 1.11x faster                                                      |
| sympy_expand            | 299 ms                                                      | 269 ms: 1.11x faster                                                       |
| sqlglot_transpile       | 1.16 ms                                                     | 1.05 ms: 1.11x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 41.9 ms: 1.11x faster                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 480 ms: 1.10x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 88.5 ms: 1.10x faster                                                      |
| async_tree_none         | 332 ms                                                      | 302 ms: 1.10x faster                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 1.88 us: 1.10x faster                                                      |
| docutils                | 1.64 sec                                                    | 1.50 sec: 1.10x faster                                                     |
| sqlglot_optimize        | 34.5 ms                                                     | 31.6 ms: 1.09x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.72 ms: 1.09x faster                                                      |
| thrift                  | 494 us                                                      | 452 us: 1.09x faster                                                       |
| python_startup_no_site  | 16.8 ms                                                     | 15.5 ms: 1.09x faster                                                      |
| meteor_contest          | 75.2 ms                                                     | 69.1 ms: 1.09x faster                                                      |
| python_startup          | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| scimark_fft             | 179 ms                                                      | 166 ms: 1.08x faster                                                       |
| async_tree_io           | 808 ms                                                      | 748 ms: 1.08x faster                                                       |
| mdp                     | 1.59 sec                                                    | 1.48 sec: 1.08x faster                                                     |
| scimark_lu              | 62.8 ms                                                     | 58.7 ms: 1.07x faster                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 49.5 ms: 1.06x faster                                                      |
| async_generators        | 177 ms                                                      | 167 ms: 1.06x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 823 us: 1.06x faster                                                       |
| json                    | 2.98 ms                                                     | 2.81 ms: 1.06x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 676 us: 1.06x faster                                                       |
| xml_etree_iterparse     | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.45 ms: 1.03x faster                                                      |
| generators              | 34.0 ms                                                     | 33.0 ms: 1.03x faster                                                      |
| pidigits                | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| tornado_http            | 92.8 ms                                                     | 90.5 ms: 1.03x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 61.7 ms: 1.02x faster                                                      |
| coroutines              | 15.0 ms                                                     | 14.8 ms: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.77 us: 1.02x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.65 us: 1.02x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.82 us: 1.03x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 73.7 ms: 1.04x slower                                                      |
| regex_dna               | 116 ms                                                      | 121 ms: 1.04x slower                                                       |
| json_loads              | 13.0 us                                                     | 14.2 us: 1.09x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.68 ms: 1.12x slower                                                      |
| coverage                | 43.4 ms                                                     | 51.8 ms: 1.19x slower                                                      |
| unpickle                | 7.57 us                                                     | 9.39 us: 1.24x slower                                                      |
| dask                    | 273 ms                                                      | 349 ms: 1.28x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.12x faster                                                               |

Benchmark hidden because not significant (2): pickle_list, pickle_dict
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.09x


# Memory

- memory change: unknown