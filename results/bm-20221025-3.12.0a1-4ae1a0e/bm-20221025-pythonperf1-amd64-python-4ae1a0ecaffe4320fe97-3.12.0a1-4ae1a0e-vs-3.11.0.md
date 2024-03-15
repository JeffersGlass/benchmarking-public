
# Results vs. 3.11.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: windows-amd64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.03x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 202 ms: 1.06x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.99 ms: 1.06x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                     |
| html5lib       | 38.9 ms                                                     | 38.1 ms: 1.02x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 91.5 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.04x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 332 ms                                                      | 316 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 506 ms: 1.05x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 381 ms: 1.05x faster                                                       |
| async_tree_io           | 808 ms                                                      | 775 ms: 1.04x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 67.2 ms: 1.05x faster                                                      |
| float          | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                      |
| pidigits       | 150 ms                                                      | 148 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 86.3 ms: 1.05x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| regex_dna      | 116 ms                                                      | 119 ms: 1.03x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.62 ms: 1.44x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 86.8 ms: 1.12x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 143 us: 1.10x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 196 us: 1.06x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 50.5 ms: 1.04x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                      |
| pickle_list          | 2.70 us                                                     | 2.64 us: 1.02x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.02x faster                                                      |
| pickle               | 6.64 us                                                     | 6.55 us: 1.01x faster                                                      |
| json_loads           | 13.0 us                                                     | 13.5 us: 1.04x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.87 us: 1.17x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 6.93 ms: 1.09x faster                                                      |
| genshi_text     | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 37.8 ms: 1.06x faster                                                      |
| django_template | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.06x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps              | 8.09 ms                                                     | 5.62 ms: 1.44x faster                                                      |
| xml_etree_parse         | 97.6 ms                                                     | 86.8 ms: 1.12x faster                                                      |
| unpack_sequence         | 46.9 ns                                                     | 42.3 ns: 1.11x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 143 us: 1.10x faster                                                       |
| python_startup_no_site  | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.93 ms: 1.09x faster                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.37 ms: 1.09x faster                                                      |
| pprint_pformat          | 1.09 sec                                                    | 1.00 sec: 1.09x faster                                                     |
| python_startup          | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 17.1 ms: 1.08x faster                                                      |
| go                      | 101 ms                                                      | 93.8 ms: 1.08x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 663 us: 1.08x faster                                                       |
| deltablue               | 2.70 ms                                                     | 2.51 ms: 1.07x faster                                                      |
| json                    | 2.98 ms                                                     | 2.77 ms: 1.07x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 495 ms: 1.07x faster                                                       |
| dulwich_log             | 46.4 ms                                                     | 43.5 ms: 1.07x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 196 us: 1.06x faster                                                       |
| fannkuch                | 253 ms                                                      | 238 ms: 1.06x faster                                                       |
| 2to3                    | 214 ms                                                      | 202 ms: 1.06x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 73.8 ms: 1.06x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.85 ms: 1.06x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 37.8 ms: 1.06x faster                                                      |
| chameleon               | 5.26 ms                                                     | 4.99 ms: 1.06x faster                                                      |
| regex_compile           | 91.0 ms                                                     | 86.3 ms: 1.05x faster                                                      |
| async_tree_none         | 332 ms                                                      | 316 ms: 1.05x faster                                                       |
| pyflate                 | 312 ms                                                      | 297 ms: 1.05x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.4 ms: 1.05x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.42 ms: 1.05x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 24.7 us: 1.05x faster                                                      |
| deepcopy                | 246 us                                                      | 235 us: 1.05x faster                                                       |
| raytrace                | 213 ms                                                      | 204 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 506 ms: 1.05x faster                                                       |
| meteor_contest          | 75.2 ms                                                     | 71.8 ms: 1.05x faster                                                      |
| async_tree_memoization  | 399 ms                                                      | 381 ms: 1.05x faster                                                       |
| nbody                   | 70.3 ms                                                     | 67.2 ms: 1.05x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 694 ms: 1.05x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 65.4 ms: 1.04x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 68.8 ns: 1.04x faster                                                      |
| async_tree_io           | 808 ms                                                      | 775 ms: 1.04x faster                                                       |
| chaos                   | 48.4 ms                                                     | 46.5 ms: 1.04x faster                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 50.5 ms: 1.04x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 60.9 ms: 1.04x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 47.2 ms: 1.04x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 43.8 ms: 1.03x faster                                                      |
| bench_thread_pool       | 872 us                                                      | 844 us: 1.03x faster                                                       |
| dask                    | 273 ms                                                      | 265 ms: 1.03x faster                                                       |
| docutils                | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                     |
| xml_etree_iterparse     | 65.6 ms                                                     | 63.6 ms: 1.03x faster                                                      |
| django_template         | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                      |
| xml_etree_process       | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.14 ms: 1.02x faster                                                      |
| pickle_list             | 2.70 us                                                     | 2.64 us: 1.02x faster                                                      |
| html5lib                | 38.9 ms                                                     | 38.1 ms: 1.02x faster                                                      |
| pylint                  | 323 ms                                                      | 317 ms: 1.02x faster                                                       |
| float                   | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 18.2 us: 1.02x faster                                                      |
| thrift                  | 494 us                                                      | 486 us: 1.02x faster                                                       |
| tornado_http            | 92.8 ms                                                     | 91.5 ms: 1.01x faster                                                      |
| richards                | 31.4 ms                                                     | 31.0 ms: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.55 us: 1.01x faster                                                      |
| pidigits                | 150 ms                                                      | 148 ms: 1.01x faster                                                       |
| sympy_str               | 185 ms                                                      | 183 ms: 1.01x faster                                                       |
| sympy_sum               | 100 ms                                                      | 98.9 ms: 1.01x faster                                                      |
| sqlglot_normalize       | 190 ms                                                      | 188 ms: 1.01x faster                                                       |
| sympy_expand            | 299 ms                                                      | 296 ms: 1.01x faster                                                       |
| logging_simple          | 6.86 us                                                     | 6.80 us: 1.01x faster                                                      |
| hexiom                  | 4.55 ms                                                     | 4.51 ms: 1.01x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 34.4 ms: 1.00x faster                                                      |
| mdp                     | 1.59 sec                                                    | 1.59 sec: 1.00x faster                                                     |
| generators              | 34.0 ms                                                     | 34.5 ms: 1.02x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.80 us: 1.02x slower                                                      |
| logging_format          | 7.16 us                                                     | 7.28 us: 1.02x slower                                                      |
| async_generators        | 177 ms                                                      | 181 ms: 1.02x slower                                                       |
| regex_dna               | 116 ms                                                      | 119 ms: 1.03x slower                                                       |
| json_loads              | 13.0 us                                                     | 13.5 us: 1.04x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 74.0 ms: 1.04x slower                                                      |
| scimark_fft             | 179 ms                                                      | 188 ms: 1.05x slower                                                       |
| scimark_lu              | 62.8 ms                                                     | 66.6 ms: 1.06x slower                                                      |
| spectral_norm           | 68.3 ms                                                     | 73.8 ms: 1.08x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.63 ms: 1.09x slower                                                      |
| unpickle                | 7.57 us                                                     | 8.87 us: 1.17x slower                                                      |
| coverage                | 43.4 ms                                                     | 52.1 ms: 1.20x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.03x faster                                                               |

Benchmark hidden because not significant (6): deepcopy_reduce, sqlglot_parse, comprehensions, coroutines, pycparser, unpickle_list
Ignored benchmarks (13) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: unknown