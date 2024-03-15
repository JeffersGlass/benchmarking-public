
# Results vs. 3.11.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: windows-amd64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 202 ms: 1.06x faster                                                        |
| chameleon      | 5.26 ms                                                     | 5.09 ms: 1.03x faster                                                       |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| html5lib       | 38.9 ms                                                     | 37.2 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 740 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 488 ms: 1.09x faster                                                        |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                        |
| async_tree_none         | 332 ms                                                      | 310 ms: 1.07x faster                                                        |
| Geometric mean          | (ref)                                                       | 1.08x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 68.6 ms: 1.02x faster                                                       |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| float          | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| regex_compile  | 91.0 ms                                                     | 89.5 ms: 1.02x faster                                                       |
| regex_dna      | 116 ms                                                      | 115 ms: 1.01x faster                                                        |
| regex_effbot   | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| xml_etree_parse      | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                                       |
| xml_etree_iterparse  | 65.6 ms                                                     | 61.9 ms: 1.06x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 197 us: 1.06x faster                                                        |
| json_dumps           | 8.09 ms                                                     | 7.66 ms: 1.06x faster                                                       |
| unpickle_pure_python | 157 us                                                      | 149 us: 1.05x faster                                                        |
| xml_etree_process    | 37.2 ms                                                     | 35.9 ms: 1.03x faster                                                       |
| xml_etree_generate   | 52.5 ms                                                     | 51.2 ms: 1.03x faster                                                       |
| pickle_dict          | 18.5 us                                                     | 18.2 us: 1.02x faster                                                       |
| pickle_list          | 2.70 us                                                     | 2.65 us: 1.02x faster                                                       |
| unpickle_list        | 2.59 us                                                     | 2.55 us: 1.01x faster                                                       |
| pickle               | 6.64 us                                                     | 6.60 us: 1.01x faster                                                       |
| unpickle             | 7.57 us                                                     | 7.70 us: 1.02x slower                                                       |
| json_loads           | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                                       |
| python_startup         | 19.8 ms                                                     | 18.5 ms: 1.07x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.08x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 16.7 ms: 1.11x faster                                                       |
| mako            | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                       |
| genshi_xml      | 39.9 ms                                                     | 38.3 ms: 1.04x faster                                                       |
| django_template | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.06x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| genshi_text             | 18.4 ms                                                     | 16.7 ms: 1.11x faster                                                       |
| unpack_sequence         | 46.9 ns                                                     | 42.7 ns: 1.10x faster                                                       |
| python_startup_no_site  | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                                       |
| async_tree_io           | 808 ms                                                      | 740 ms: 1.09x faster                                                        |
| async_tree_cpu_io_mixed | 530 ms                                                      | 488 ms: 1.09x faster                                                        |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                        |
| async_tree_none         | 332 ms                                                      | 310 ms: 1.07x faster                                                        |
| create_gc_cycles        | 713 us                                                      | 667 us: 1.07x faster                                                        |
| python_startup          | 19.8 ms                                                     | 18.5 ms: 1.07x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 91.6 ms: 1.07x faster                                                       |
| dulwich_log             | 46.4 ms                                                     | 43.6 ms: 1.06x faster                                                       |
| gc_traversal            | 1.49 ms                                                     | 1.41 ms: 1.06x faster                                                       |
| xml_etree_iterparse     | 65.6 ms                                                     | 61.9 ms: 1.06x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| pickle_pure_python      | 208 us                                                      | 197 us: 1.06x faster                                                        |
| nqueens                 | 68.3 ms                                                     | 64.6 ms: 1.06x faster                                                       |
| 2to3                    | 214 ms                                                      | 202 ms: 1.06x faster                                                        |
| json_dumps              | 8.09 ms                                                     | 7.66 ms: 1.06x faster                                                       |
| sqlite_synth            | 1.77 us                                                     | 1.67 us: 1.06x faster                                                       |
| asyncio_tcp             | 726 ms                                                      | 688 ms: 1.05x faster                                                        |
| pycparser               | 720 ms                                                      | 683 ms: 1.05x faster                                                        |
| unpickle_pure_python    | 157 us                                                      | 149 us: 1.05x faster                                                        |
| mako                    | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                       |
| sqlalchemy_declarative  | 85.6 ms                                                     | 81.7 ms: 1.05x faster                                                       |
| logging_simple          | 6.86 us                                                     | 6.57 us: 1.05x faster                                                       |
| docutils                | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 38.3 ms: 1.04x faster                                                       |
| html5lib                | 38.9 ms                                                     | 37.2 ms: 1.04x faster                                                       |
| telco                   | 4.06 ms                                                     | 3.91 ms: 1.04x faster                                                       |
| sqlglot_transpile       | 1.16 ms                                                     | 1.12 ms: 1.04x faster                                                       |
| go                      | 101 ms                                                      | 97.5 ms: 1.04x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.5 ms: 1.04x faster                                                       |
| sqlglot_parse           | 953 us                                                      | 920 us: 1.04x faster                                                        |
| xml_etree_process       | 37.2 ms                                                     | 35.9 ms: 1.03x faster                                                       |
| chameleon               | 5.26 ms                                                     | 5.09 ms: 1.03x faster                                                       |
| pprint_pformat          | 1.09 sec                                                    | 1.05 sec: 1.03x faster                                                      |
| deepcopy                | 246 us                                                      | 239 us: 1.03x faster                                                        |
| deltablue               | 2.70 ms                                                     | 2.61 ms: 1.03x faster                                                       |
| pprint_safe_repr        | 529 ms                                                      | 512 ms: 1.03x faster                                                        |
| bench_mp_pool           | 63.2 ms                                                     | 61.2 ms: 1.03x faster                                                       |
| pyflate                 | 312 ms                                                      | 303 ms: 1.03x faster                                                        |
| comprehensions          | 15.6 us                                                     | 15.2 us: 1.03x faster                                                       |
| aiohttp                 | 883 us                                                      | 857 us: 1.03x faster                                                        |
| deepcopy_reduce         | 2.06 us                                                     | 2.00 us: 1.03x faster                                                       |
| logging_format          | 7.16 us                                                     | 6.97 us: 1.03x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 849 us: 1.03x faster                                                        |
| richards                | 31.4 ms                                                     | 30.6 ms: 1.03x faster                                                       |
| xml_etree_generate      | 52.5 ms                                                     | 51.2 ms: 1.03x faster                                                       |
| django_template         | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                       |
| nbody                   | 70.3 ms                                                     | 68.6 ms: 1.02x faster                                                       |
| pylint                  | 323 ms                                                      | 316 ms: 1.02x faster                                                        |
| pidigits                | 150 ms                                                      | 147 ms: 1.02x faster                                                        |
| sqlglot_normalize       | 190 ms                                                      | 186 ms: 1.02x faster                                                        |
| deepcopy_memo           | 26.0 us                                                     | 25.4 us: 1.02x faster                                                       |
| dask                    | 273 ms                                                      | 267 ms: 1.02x faster                                                        |
| sympy_sum               | 100 ms                                                      | 98.2 ms: 1.02x faster                                                       |
| regex_compile           | 91.0 ms                                                     | 89.5 ms: 1.02x faster                                                       |
| sympy_expand            | 299 ms                                                      | 294 ms: 1.02x faster                                                        |
| pickle_dict             | 18.5 us                                                     | 18.2 us: 1.02x faster                                                       |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.3 ms: 1.02x faster                                                       |
| scimark_monte_carlo     | 45.3 ms                                                     | 44.6 ms: 1.02x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.65 us: 1.02x faster                                                       |
| sympy_str               | 185 ms                                                      | 182 ms: 1.02x faster                                                        |
| hexiom                  | 4.55 ms                                                     | 4.48 ms: 1.02x faster                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 34.0 ms: 1.02x faster                                                       |
| unpickle_list           | 2.59 us                                                     | 2.55 us: 1.01x faster                                                       |
| raytrace                | 213 ms                                                      | 211 ms: 1.01x faster                                                        |
| generators              | 34.0 ms                                                     | 33.5 ms: 1.01x faster                                                       |
| regex_dna               | 116 ms                                                      | 115 ms: 1.01x faster                                                        |
| logging_silent          | 71.8 ns                                                     | 70.9 ns: 1.01x faster                                                       |
| meteor_contest          | 75.2 ms                                                     | 74.3 ms: 1.01x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 77.3 ms: 1.01x faster                                                       |
| async_generators        | 177 ms                                                      | 176 ms: 1.01x faster                                                        |
| float                   | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                                       |
| crypto_pyaes            | 48.9 ms                                                     | 48.5 ms: 1.01x faster                                                       |
| chaos                   | 48.4 ms                                                     | 48.0 ms: 1.01x faster                                                       |
| coroutines              | 15.0 ms                                                     | 14.9 ms: 1.01x faster                                                       |
| pickle                  | 6.64 us                                                     | 6.60 us: 1.01x faster                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.04 sec: 1.01x slower                                                      |
| scimark_lu              | 62.8 ms                                                     | 63.4 ms: 1.01x slower                                                       |
| fannkuch                | 253 ms                                                      | 256 ms: 1.01x slower                                                        |
| unpickle                | 7.57 us                                                     | 7.70 us: 1.02x slower                                                       |
| pathlib                 | 70.9 ms                                                     | 72.1 ms: 1.02x slower                                                       |
| json_loads              | 13.0 us                                                     | 13.7 us: 1.05x slower                                                       |
| scimark_fft             | 179 ms                                                      | 189 ms: 1.06x slower                                                        |
| regex_effbot            | 1.50 ms                                                     | 1.60 ms: 1.07x slower                                                       |
| spectral_norm           | 68.3 ms                                                     | 73.2 ms: 1.07x slower                                                       |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.81 ms: 1.09x slower                                                       |
| coverage                | 43.4 ms                                                     | 53.2 ms: 1.23x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x faster                                                                |

Benchmark hidden because not significant (4): tornado_http, thrift, mdp, json
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown