
# Results vs. 3.11.0

- fork: python
- ref: 41cb07120b7792eac641
- machine: windows-amd64
- commit hash: 41cb071
- commit date: 2022-08-05
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 202 ms: 1.05x faster                                                        |
| chameleon      | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| html5lib       | 38.9 ms                                                     | 38.4 ms: 1.01x faster                                                       |
| tornado_http   | 92.8 ms                                                     | 90.9 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 739 ms: 1.09x faster                                                        |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 491 ms: 1.08x faster                                                        |
| async_tree_none         | 332 ms                                                      | 310 ms: 1.07x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 68.3 ms: 1.03x faster                                                       |
| float          | 54.4 ms                                                     | 52.9 ms: 1.03x faster                                                       |
| pidigits       | 150 ms                                                      | 146 ms: 1.03x faster                                                        |
| Geometric mean | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 89.4 ms: 1.02x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 14.1 ms: 1.00x faster                                                       |
| regex_dna      | 116 ms                                                      | 123 ms: 1.06x slower                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                                       |
| Geometric mean | (ref)                                                       | 1.03x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle_list          | 2.70 us                                                     | 2.57 us: 1.05x faster                                                       |
| json_dumps           | 8.09 ms                                                     | 7.73 ms: 1.05x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 150 us: 1.04x faster                                                        |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.9 ms: 1.04x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 202 us: 1.03x faster                                                        |
| pickle               | 6.64 us                                                     | 6.44 us: 1.03x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 94.8 ms: 1.03x faster                                                       |
| xml_etree_process    | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| unpickle_list        | 2.59 us                                                     | 2.64 us: 1.02x slower                                                       |
| unpickle             | 7.57 us                                                     | 8.11 us: 1.07x slower                                                       |
| json_loads           | 13.0 us                                                     | 14.0 us: 1.08x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmark hidden because not significant (1): xml_etree_generate

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.2 ms: 1.10x faster                                                       |
| python_startup         | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 16.7 ms: 1.10x faster                                                       |
| genshi_xml      | 39.9 ms                                                     | 37.7 ms: 1.06x faster                                                       |
| mako            | 7.58 ms                                                     | 7.26 ms: 1.05x faster                                                       |
| django_template | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.06x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 41.9 ns: 1.12x faster                                                       |
| genshi_text             | 18.4 ms                                                     | 16.7 ms: 1.10x faster                                                       |
| python_startup_no_site  | 16.8 ms                                                     | 15.2 ms: 1.10x faster                                                       |
| asyncio_tcp             | 726 ms                                                      | 659 ms: 1.10x faster                                                        |
| async_tree_io           | 808 ms                                                      | 739 ms: 1.09x faster                                                        |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 491 ms: 1.08x faster                                                        |
| python_startup          | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                       |
| logging_simple          | 6.86 us                                                     | 6.37 us: 1.08x faster                                                       |
| create_gc_cycles        | 713 us                                                      | 665 us: 1.07x faster                                                        |
| async_tree_none         | 332 ms                                                      | 310 ms: 1.07x faster                                                        |
| dulwich_log             | 46.4 ms                                                     | 43.3 ms: 1.07x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 64.2 ms: 1.06x faster                                                       |
| gc_traversal            | 1.49 ms                                                     | 1.40 ms: 1.06x faster                                                       |
| genshi_xml              | 39.9 ms                                                     | 37.7 ms: 1.06x faster                                                       |
| 2to3                    | 214 ms                                                      | 202 ms: 1.05x faster                                                        |
| sqlite_synth            | 1.77 us                                                     | 1.68 us: 1.05x faster                                                       |
| telco                   | 4.06 ms                                                     | 3.87 ms: 1.05x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.57 us: 1.05x faster                                                       |
| raytrace                | 213 ms                                                      | 204 ms: 1.05x faster                                                        |
| json_dumps              | 8.09 ms                                                     | 7.73 ms: 1.05x faster                                                       |
| mako                    | 7.58 ms                                                     | 7.26 ms: 1.05x faster                                                       |
| pycparser               | 720 ms                                                      | 689 ms: 1.04x faster                                                        |
| unpickle_pure_python    | 157 us                                                      | 150 us: 1.04x faster                                                        |
| xml_etree_iterparse     | 65.6 ms                                                     | 62.9 ms: 1.04x faster                                                       |
| chameleon               | 5.26 ms                                                     | 5.05 ms: 1.04x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                                       |
| pprint_pformat          | 1.09 sec                                                    | 1.04 sec: 1.04x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.90 us: 1.04x faster                                                       |
| deepcopy                | 246 us                                                      | 238 us: 1.03x faster                                                        |
| pyflate                 | 312 ms                                                      | 303 ms: 1.03x faster                                                        |
| sympy_sum               | 100 ms                                                      | 97.0 ms: 1.03x faster                                                       |
| pickle_pure_python      | 208 us                                                      | 202 us: 1.03x faster                                                        |
| pickle                  | 6.64 us                                                     | 6.44 us: 1.03x faster                                                       |
| docutils                | 1.64 sec                                                    | 1.59 sec: 1.03x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 513 ms: 1.03x faster                                                        |
| django_template         | 24.4 ms                                                     | 23.7 ms: 1.03x faster                                                       |
| sympy_expand            | 299 ms                                                      | 290 ms: 1.03x faster                                                        |
| sqlglot_parse           | 953 us                                                      | 925 us: 1.03x faster                                                        |
| bench_mp_pool           | 63.2 ms                                                     | 61.4 ms: 1.03x faster                                                       |
| sqlglot_transpile       | 1.16 ms                                                     | 1.13 ms: 1.03x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 94.8 ms: 1.03x faster                                                       |
| comprehensions          | 15.6 us                                                     | 15.2 us: 1.03x faster                                                       |
| nbody                   | 70.3 ms                                                     | 68.3 ms: 1.03x faster                                                       |
| sympy_str               | 185 ms                                                      | 180 ms: 1.03x faster                                                        |
| float                   | 54.4 ms                                                     | 52.9 ms: 1.03x faster                                                       |
| pidigits                | 150 ms                                                      | 146 ms: 1.03x faster                                                        |
| deltablue               | 2.70 ms                                                     | 2.63 ms: 1.03x faster                                                       |
| sqlalchemy_declarative  | 85.6 ms                                                     | 83.4 ms: 1.03x faster                                                       |
| aiohttp                 | 883 us                                                      | 861 us: 1.03x faster                                                        |
| meteor_contest          | 75.2 ms                                                     | 73.3 ms: 1.03x faster                                                       |
| deepcopy_memo           | 26.0 us                                                     | 25.3 us: 1.03x faster                                                       |
| thrift                  | 494 us                                                      | 482 us: 1.02x faster                                                        |
| fannkuch                | 253 ms                                                      | 247 ms: 1.02x faster                                                        |
| hexiom                  | 4.55 ms                                                     | 4.46 ms: 1.02x faster                                                       |
| dask                    | 273 ms                                                      | 267 ms: 1.02x faster                                                        |
| tornado_http            | 92.8 ms                                                     | 90.9 ms: 1.02x faster                                                       |
| scimark_monte_carlo     | 45.3 ms                                                     | 44.4 ms: 1.02x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 856 us: 1.02x faster                                                        |
| regex_compile           | 91.0 ms                                                     | 89.4 ms: 1.02x faster                                                       |
| pylint                  | 323 ms                                                      | 318 ms: 1.02x faster                                                        |
| coroutines              | 15.0 ms                                                     | 14.8 ms: 1.01x faster                                                       |
| xml_etree_process       | 37.2 ms                                                     | 36.7 ms: 1.01x faster                                                       |
| html5lib                | 38.9 ms                                                     | 38.4 ms: 1.01x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 77.3 ms: 1.01x faster                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 2.05 us: 1.01x faster                                                       |
| async_generators        | 177 ms                                                      | 176 ms: 1.01x faster                                                        |
| sqlglot_normalize       | 190 ms                                                      | 189 ms: 1.01x faster                                                        |
| go                      | 101 ms                                                      | 101 ms: 1.00x faster                                                        |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.4 ms: 1.00x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 14.1 ms: 1.00x faster                                                       |
| pickle_dict             | 18.5 us                                                     | 18.4 us: 1.00x faster                                                       |
| mdp                     | 1.59 sec                                                    | 1.60 sec: 1.00x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.61 ms: 1.01x slower                                                       |
| scimark_lu              | 62.8 ms                                                     | 63.7 ms: 1.01x slower                                                       |
| scimark_fft             | 179 ms                                                      | 182 ms: 1.02x slower                                                        |
| unpickle_list           | 2.59 us                                                     | 2.64 us: 1.02x slower                                                       |
| pathlib                 | 70.9 ms                                                     | 72.6 ms: 1.02x slower                                                       |
| chaos                   | 48.4 ms                                                     | 49.6 ms: 1.03x slower                                                       |
| spectral_norm           | 68.3 ms                                                     | 71.8 ms: 1.05x slower                                                       |
| regex_dna               | 116 ms                                                      | 123 ms: 1.06x slower                                                        |
| unpickle                | 7.57 us                                                     | 8.11 us: 1.07x slower                                                       |
| json_loads              | 13.0 us                                                     | 14.0 us: 1.08x slower                                                       |
| regex_effbot            | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                                       |
| coverage                | 43.4 ms                                                     | 53.6 ms: 1.24x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (7): json, generators, richards, crypto_pyaes, sqlglot_optimize, xml_etree_generate, logging_silent
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown