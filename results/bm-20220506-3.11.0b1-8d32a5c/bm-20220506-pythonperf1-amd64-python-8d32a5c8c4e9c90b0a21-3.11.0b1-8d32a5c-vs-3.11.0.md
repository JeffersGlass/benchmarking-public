
# Results vs. 3.11.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: windows-amd64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.91%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 203 ms: 1.05x faster                                                       |
| chameleon      | 5.26 ms                                                     | 5.45 ms: 1.04x slower                                                      |
| docutils       | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                     |
| html5lib       | 38.9 ms                                                     | 38.3 ms: 1.02x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 89.7 ms: 1.03x faster                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 370 ms: 1.08x faster                                                       |
| async_tree_io           | 808 ms                                                      | 751 ms: 1.08x faster                                                       |
| async_tree_none         | 332 ms                                                      | 311 ms: 1.07x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 499 ms: 1.06x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 67.9 ms: 1.04x faster                                                      |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                       |
| float          | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                       | 1.03x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 1.50 ms                                                     | 1.47 ms: 1.02x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                                      |
| regex_compile  | 91.0 ms                                                     | 90.5 ms: 1.01x faster                                                      |
| regex_dna      | 116 ms                                                      | 121 ms: 1.04x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 17.1 us: 1.08x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 61.1 ms: 1.07x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 93.1 ms: 1.05x faster                                                      |
| json_dumps           | 8.09 ms                                                     | 7.72 ms: 1.05x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 152 us: 1.03x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 204 us: 1.02x faster                                                       |
| pickle_list          | 2.70 us                                                     | 2.67 us: 1.01x faster                                                      |
| pickle               | 6.64 us                                                     | 6.59 us: 1.01x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 53.0 ms: 1.01x slower                                                      |
| xml_etree_process    | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                                      |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                                      |
| unpickle             | 7.57 us                                                     | 7.87 us: 1.04x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.02x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.2 ms: 1.10x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.58 ms                                                     | 7.13 ms: 1.06x faster                                                      |
| genshi_text     | 18.4 ms                                                     | 17.7 ms: 1.04x faster                                                      |
| django_template | 24.4 ms                                                     | 24.0 ms: 1.02x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.03x faster                                                               |

Benchmark hidden because not significant (1): genshi_xml

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| logging_simple          | 6.86 us                                                     | 5.80 us: 1.18x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.25 us: 1.15x faster                                                      |
| unpack_sequence         | 46.9 ns                                                     | 42.2 ns: 1.11x faster                                                      |
| python_startup_no_site  | 16.8 ms                                                     | 15.2 ms: 1.10x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 42.5 ms: 1.09x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 17.1 us: 1.08x faster                                                      |
| async_tree_memoization  | 399 ms                                                      | 370 ms: 1.08x faster                                                       |
| asyncio_tcp             | 726 ms                                                      | 673 ms: 1.08x faster                                                       |
| create_gc_cycles        | 713 us                                                      | 663 us: 1.08x faster                                                       |
| async_tree_io           | 808 ms                                                      | 751 ms: 1.08x faster                                                       |
| python_startup          | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                      |
| xml_etree_iterparse     | 65.6 ms                                                     | 61.1 ms: 1.07x faster                                                      |
| async_tree_none         | 332 ms                                                      | 311 ms: 1.07x faster                                                       |
| mako                    | 7.58 ms                                                     | 7.13 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 499 ms: 1.06x faster                                                       |
| gc_traversal            | 1.49 ms                                                     | 1.42 ms: 1.05x faster                                                      |
| 2to3                    | 214 ms                                                      | 203 ms: 1.05x faster                                                       |
| raytrace                | 213 ms                                                      | 203 ms: 1.05x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 93.1 ms: 1.05x faster                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.69 us: 1.05x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 7.72 ms: 1.05x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 17.7 ms: 1.04x faster                                                      |
| docutils                | 1.64 sec                                                    | 1.57 sec: 1.04x faster                                                     |
| bench_mp_pool           | 63.2 ms                                                     | 60.6 ms: 1.04x faster                                                      |
| richards                | 31.4 ms                                                     | 30.1 ms: 1.04x faster                                                      |
| nbody                   | 70.3 ms                                                     | 67.9 ms: 1.04x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 25.1 us: 1.03x faster                                                      |
| aiohttp                 | 883 us                                                      | 854 us: 1.03x faster                                                       |
| tornado_http            | 92.8 ms                                                     | 89.7 ms: 1.03x faster                                                      |
| sympy_sum               | 100 ms                                                      | 96.9 ms: 1.03x faster                                                      |
| go                      | 101 ms                                                      | 97.9 ms: 1.03x faster                                                      |
| sympy_integrate         | 14.0 ms                                                     | 13.6 ms: 1.03x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.94 ms: 1.03x faster                                                      |
| pyflate                 | 312 ms                                                      | 303 ms: 1.03x faster                                                       |
| pylint                  | 323 ms                                                      | 314 ms: 1.03x faster                                                       |
| unpickle_pure_python    | 157 us                                                      | 152 us: 1.03x faster                                                       |
| logging_silent          | 71.8 ns                                                     | 70.2 ns: 1.02x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 204 us: 1.02x faster                                                       |
| pidigits                | 150 ms                                                      | 147 ms: 1.02x faster                                                       |
| sympy_expand            | 299 ms                                                      | 293 ms: 1.02x faster                                                       |
| regex_effbot            | 1.50 ms                                                     | 1.47 ms: 1.02x faster                                                      |
| django_template         | 24.4 ms                                                     | 24.0 ms: 1.02x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                                      |
| float                   | 54.4 ms                                                     | 53.5 ms: 1.02x faster                                                      |
| dask                    | 273 ms                                                      | 268 ms: 1.02x faster                                                       |
| html5lib                | 38.9 ms                                                     | 38.3 ms: 1.02x faster                                                      |
| deltablue               | 2.70 ms                                                     | 2.66 ms: 1.01x faster                                                      |
| scimark_sor             | 78.1 ms                                                     | 77.1 ms: 1.01x faster                                                      |
| sympy_str               | 185 ms                                                      | 183 ms: 1.01x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 67.6 ms: 1.01x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 525 ms: 1.01x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.67 us: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.59 us: 1.01x faster                                                      |
| pprint_pformat          | 1.09 sec                                                    | 1.08 sec: 1.01x faster                                                     |
| regex_compile           | 91.0 ms                                                     | 90.5 ms: 1.01x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 45.0 ms: 1.01x faster                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 49.1 ms: 1.00x slower                                                      |
| meteor_contest          | 75.2 ms                                                     | 75.5 ms: 1.00x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 71.4 ms: 1.01x slower                                                      |
| hexiom                  | 4.55 ms                                                     | 4.59 ms: 1.01x slower                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 53.0 ms: 1.01x slower                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.60 ms: 1.01x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 37.6 ms: 1.01x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| chaos                   | 48.4 ms                                                     | 48.9 ms: 1.01x slower                                                      |
| coroutines              | 15.0 ms                                                     | 15.2 ms: 1.01x slower                                                      |
| spectral_norm           | 68.3 ms                                                     | 69.6 ms: 1.02x slower                                                      |
| bench_thread_pool       | 872 us                                                      | 888 us: 1.02x slower                                                       |
| thrift                  | 494 us                                                      | 504 us: 1.02x slower                                                       |
| deepcopy                | 246 us                                                      | 252 us: 1.02x slower                                                       |
| mdp                     | 1.59 sec                                                    | 1.63 sec: 1.03x slower                                                     |
| deepcopy_reduce         | 2.06 us                                                     | 2.12 us: 1.03x slower                                                      |
| sqlglot_normalize       | 190 ms                                                      | 196 ms: 1.03x slower                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 35.6 ms: 1.03x slower                                                      |
| async_generators        | 177 ms                                                      | 182 ms: 1.03x slower                                                       |
| json_loads              | 13.0 us                                                     | 13.4 us: 1.03x slower                                                      |
| chameleon               | 5.26 ms                                                     | 5.45 ms: 1.04x slower                                                      |
| pycparser               | 720 ms                                                      | 748 ms: 1.04x slower                                                       |
| unpickle                | 7.57 us                                                     | 7.87 us: 1.04x slower                                                      |
| regex_dna               | 116 ms                                                      | 121 ms: 1.04x slower                                                       |
| json                    | 2.98 ms                                                     | 3.25 ms: 1.09x slower                                                      |
| comprehensions          | 15.6 us                                                     | 17.8 us: 1.14x slower                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.37 ms: 1.17x slower                                                      |
| sqlglot_parse           | 953 us                                                      | 1.15 ms: 1.21x slower                                                      |
| coverage                | 43.4 ms                                                     | 103 ms: 2.36x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                               |

Benchmark hidden because not significant (6): unpickle_list, genshi_xml, fannkuch, generators, scimark_lu, scimark_fft
Ignored benchmarks (11) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.91% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown