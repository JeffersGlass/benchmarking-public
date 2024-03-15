
# Results vs. 3.11.0

- fork: python
- ref: f3909b8bc83675b7ab09
- machine: windows-amd64
- commit hash: f3909b8
- commit date: 2023-04-04
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 206 ms: 1.03x faster                                                     |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                   |
| html5lib       | 38.9 ms                                                     | 39.8 ms: 1.02x slower                                                    |
| tornado_http   | 92.8 ms                                                     | 90.1 ms: 1.03x faster                                                    |
| Geometric mean | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 739 ms: 1.09x faster                                                     |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                     |
| async_tree_cpu_io_mixed | 530 ms                                                      | 500 ms: 1.06x faster                                                     |
| async_tree_none         | 332 ms                                                      | 314 ms: 1.06x faster                                                     |
| Geometric mean          | (ref)                                                       | 1.07x faster                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 52.6 ms: 1.03x faster                                                    |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                     |
| nbody          | 70.3 ms                                                     | 69.8 ms: 1.01x faster                                                    |
| Geometric mean | (ref)                                                       | 1.02x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 89.7 ms: 1.02x faster                                                    |
| regex_v8       | 14.2 ms                                                     | 14.3 ms: 1.01x slower                                                    |
| regex_dna      | 116 ms                                                      | 120 ms: 1.04x slower                                                     |
| regex_effbot   | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                    |
| Geometric mean | (ref)                                                       | 1.02x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| xml_etree_parse      | 97.6 ms                                                     | 91.3 ms: 1.07x faster                                                    |
| xml_etree_iterparse  | 65.6 ms                                                     | 61.4 ms: 1.07x faster                                                    |
| json_dumps           | 8.09 ms                                                     | 7.60 ms: 1.06x faster                                                    |
| pickle_pure_python   | 208 us                                                      | 198 us: 1.05x faster                                                     |
| unpickle_pure_python | 157 us                                                      | 150 us: 1.05x faster                                                     |
| xml_etree_process    | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                    |
| xml_etree_generate   | 52.5 ms                                                     | 51.8 ms: 1.02x faster                                                    |
| pickle               | 6.64 us                                                     | 6.73 us: 1.01x slower                                                    |
| pickle_list          | 2.70 us                                                     | 2.78 us: 1.03x slower                                                    |
| unpickle_list        | 2.59 us                                                     | 2.68 us: 1.03x slower                                                    |
| unpickle             | 7.57 us                                                     | 7.97 us: 1.05x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (2): json_loads, pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                                    |
| python_startup         | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                                    |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.3 ms: 1.06x faster                                                    |
| genshi_xml      | 39.9 ms                                                     | 37.6 ms: 1.06x faster                                                    |
| mako            | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                    |
| django_template | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                    |
| Geometric mean  | (ref)                                                       | 1.05x faster                                                             |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site  | 16.8 ms                                                     | 15.3 ms: 1.10x faster                                                    |
| async_tree_io           | 808 ms                                                      | 739 ms: 1.09x faster                                                     |
| dulwich_log             | 46.4 ms                                                     | 42.5 ms: 1.09x faster                                                    |
| async_tree_memoization  | 399 ms                                                      | 368 ms: 1.08x faster                                                     |
| create_gc_cycles        | 713 us                                                      | 664 us: 1.07x faster                                                     |
| python_startup          | 19.8 ms                                                     | 18.4 ms: 1.07x faster                                                    |
| xml_etree_parse         | 97.6 ms                                                     | 91.3 ms: 1.07x faster                                                    |
| xml_etree_iterparse     | 65.6 ms                                                     | 61.4 ms: 1.07x faster                                                    |
| json_dumps              | 8.09 ms                                                     | 7.60 ms: 1.06x faster                                                    |
| genshi_text             | 18.4 ms                                                     | 17.3 ms: 1.06x faster                                                    |
| genshi_xml              | 39.9 ms                                                     | 37.6 ms: 1.06x faster                                                    |
| async_tree_cpu_io_mixed | 530 ms                                                      | 500 ms: 1.06x faster                                                     |
| async_tree_none         | 332 ms                                                      | 314 ms: 1.06x faster                                                     |
| sqlalchemy_declarative  | 85.6 ms                                                     | 81.1 ms: 1.06x faster                                                    |
| pickle_pure_python      | 208 us                                                      | 198 us: 1.05x faster                                                     |
| raytrace                | 213 ms                                                      | 203 ms: 1.05x faster                                                     |
| mako                    | 7.58 ms                                                     | 7.22 ms: 1.05x faster                                                    |
| unpickle_pure_python    | 157 us                                                      | 150 us: 1.05x faster                                                     |
| gc_traversal            | 1.49 ms                                                     | 1.43 ms: 1.05x faster                                                    |
| deepcopy_memo           | 26.0 us                                                     | 24.8 us: 1.05x faster                                                    |
| dask                    | 273 ms                                                      | 261 ms: 1.04x faster                                                     |
| sqlite_synth            | 1.77 us                                                     | 1.69 us: 1.04x faster                                                    |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.0 ms: 1.04x faster                                                    |
| nqueens                 | 68.3 ms                                                     | 65.6 ms: 1.04x faster                                                    |
| scimark_sor             | 78.1 ms                                                     | 75.2 ms: 1.04x faster                                                    |
| docutils                | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                   |
| pyflate                 | 312 ms                                                      | 301 ms: 1.04x faster                                                     |
| 2to3                    | 214 ms                                                      | 206 ms: 1.03x faster                                                     |
| float                   | 54.4 ms                                                     | 52.6 ms: 1.03x faster                                                    |
| richards                | 31.4 ms                                                     | 30.4 ms: 1.03x faster                                                    |
| sympy_expand            | 299 ms                                                      | 290 ms: 1.03x faster                                                     |
| sympy_integrate         | 14.0 ms                                                     | 13.6 ms: 1.03x faster                                                    |
| aiohttp                 | 883 us                                                      | 857 us: 1.03x faster                                                     |
| tornado_http            | 92.8 ms                                                     | 90.1 ms: 1.03x faster                                                    |
| logging_simple          | 6.86 us                                                     | 6.67 us: 1.03x faster                                                    |
| bench_thread_pool       | 872 us                                                      | 848 us: 1.03x faster                                                     |
| sqlglot_transpile       | 1.16 ms                                                     | 1.13 ms: 1.03x faster                                                    |
| django_template         | 24.4 ms                                                     | 23.8 ms: 1.03x faster                                                    |
| logging_format          | 7.16 us                                                     | 6.99 us: 1.02x faster                                                    |
| thrift                  | 494 us                                                      | 482 us: 1.02x faster                                                     |
| sqlglot_parse           | 953 us                                                      | 931 us: 1.02x faster                                                     |
| pprint_pformat          | 1.09 sec                                                    | 1.06 sec: 1.02x faster                                                   |
| xml_etree_process       | 37.2 ms                                                     | 36.3 ms: 1.02x faster                                                    |
| logging_silent          | 71.8 ns                                                     | 70.1 ns: 1.02x faster                                                    |
| pycparser               | 720 ms                                                      | 703 ms: 1.02x faster                                                     |
| pidigits                | 150 ms                                                      | 147 ms: 1.02x faster                                                     |
| unpack_sequence         | 46.9 ns                                                     | 46.0 ns: 1.02x faster                                                    |
| go                      | 101 ms                                                      | 99.2 ms: 1.02x faster                                                    |
| bench_mp_pool           | 63.2 ms                                                     | 62.0 ms: 1.02x faster                                                    |
| sympy_str               | 185 ms                                                      | 182 ms: 1.02x faster                                                     |
| comprehensions          | 15.6 us                                                     | 15.4 us: 1.02x faster                                                    |
| sympy_sum               | 100 ms                                                      | 98.4 ms: 1.02x faster                                                    |
| deltablue               | 2.70 ms                                                     | 2.65 ms: 1.02x faster                                                    |
| xml_etree_generate      | 52.5 ms                                                     | 51.8 ms: 1.02x faster                                                    |
| regex_compile           | 91.0 ms                                                     | 89.7 ms: 1.02x faster                                                    |
| deepcopy                | 246 us                                                      | 243 us: 1.01x faster                                                     |
| crypto_pyaes            | 48.9 ms                                                     | 48.2 ms: 1.01x faster                                                    |
| spectral_norm           | 68.3 ms                                                     | 67.6 ms: 1.01x faster                                                    |
| deepcopy_reduce         | 2.06 us                                                     | 2.04 us: 1.01x faster                                                    |
| telco                   | 4.06 ms                                                     | 4.02 ms: 1.01x faster                                                    |
| async_generators        | 177 ms                                                      | 176 ms: 1.01x faster                                                     |
| nbody                   | 70.3 ms                                                     | 69.8 ms: 1.01x faster                                                    |
| meteor_contest          | 75.2 ms                                                     | 74.7 ms: 1.01x faster                                                    |
| sqlglot_optimize        | 34.5 ms                                                     | 34.7 ms: 1.00x slower                                                    |
| regex_v8                | 14.2 ms                                                     | 14.3 ms: 1.01x slower                                                    |
| scimark_lu              | 62.8 ms                                                     | 63.3 ms: 1.01x slower                                                    |
| fannkuch                | 253 ms                                                      | 256 ms: 1.01x slower                                                     |
| chaos                   | 48.4 ms                                                     | 48.9 ms: 1.01x slower                                                    |
| coroutines              | 15.0 ms                                                     | 15.1 ms: 1.01x slower                                                    |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                   |
| pickle                  | 6.64 us                                                     | 6.73 us: 1.01x slower                                                    |
| html5lib                | 38.9 ms                                                     | 39.8 ms: 1.02x slower                                                    |
| scimark_fft             | 179 ms                                                      | 185 ms: 1.03x slower                                                     |
| pickle_list             | 2.70 us                                                     | 2.78 us: 1.03x slower                                                    |
| pathlib                 | 70.9 ms                                                     | 73.2 ms: 1.03x slower                                                    |
| unpickle_list           | 2.59 us                                                     | 2.68 us: 1.03x slower                                                    |
| regex_dna               | 116 ms                                                      | 120 ms: 1.04x slower                                                     |
| regex_effbot            | 1.50 ms                                                     | 1.57 ms: 1.05x slower                                                    |
| unpickle                | 7.57 us                                                     | 7.97 us: 1.05x slower                                                    |
| json                    | 2.98 ms                                                     | 3.25 ms: 1.09x slower                                                    |
| mdp                     | 1.59 sec                                                    | 1.74 sec: 1.09x slower                                                   |
| coverage                | 43.4 ms                                                     | 53.2 ms: 1.23x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.02x faster                                                             |

Benchmark hidden because not significant (11): asyncio_tcp, pprint_safe_repr, pylint, scimark_monte_carlo, json_loads, generators, scimark_sparse_mat_mult, chameleon, hexiom, sqlglot_normalize, pickle_dict
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: unknown