
# Results vs. 3.10.4

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: windows-amd64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.15x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.11x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 246 ms                                                      | 202 ms: 1.22x faster                                                       |
| chameleon      | 5.79 ms                                                     | 4.99 ms: 1.16x faster                                                      |
| docutils       | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                     |
| html5lib       | 51.0 ms                                                     | 38.1 ms: 1.34x faster                                                      |
| tornado_http   | 108 ms                                                      | 91.5 ms: 1.18x faster                                                      |
| Geometric mean | (ref)                                                       | 1.22x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 1.11 sec                                                    | 775 ms: 1.43x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 381 ms: 1.38x faster                                                       |
| async_tree_none         | 435 ms                                                      | 316 ms: 1.38x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 506 ms: 1.26x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.36x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                      |
| nbody          | 71.3 ms                                                     | 67.2 ms: 1.06x faster                                                      |
| pidigits       | 149 ms                                                      | 148 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 106 ms                                                      | 86.3 ms: 1.23x faster                                                      |
| regex_dna      | 136 ms                                                      | 119 ms: 1.14x faster                                                       |
| regex_v8       | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                                      |
| regex_effbot   | 1.66 ms                                                     | 1.63 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.13x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 9.16 ms                                                     | 5.62 ms: 1.63x faster                                                      |
| pickle_pure_python   | 270 us                                                      | 196 us: 1.38x faster                                                       |
| unpickle_pure_python | 183 us                                                      | 143 us: 1.28x faster                                                       |
| xml_etree_process    | 44.5 ms                                                     | 36.3 ms: 1.22x faster                                                      |
| xml_etree_parse      | 96.8 ms                                                     | 86.8 ms: 1.11x faster                                                      |
| xml_etree_generate   | 55.5 ms                                                     | 50.5 ms: 1.10x faster                                                      |
| pickle               | 6.85 us                                                     | 6.55 us: 1.05x faster                                                      |
| pickle_list          | 2.75 us                                                     | 2.64 us: 1.04x faster                                                      |
| unpickle_list        | 2.71 us                                                     | 2.60 us: 1.04x faster                                                      |
| json_loads           | 14.0 us                                                     | 13.5 us: 1.04x faster                                                      |
| unpickle             | 9.09 us                                                     | 8.87 us: 1.03x faster                                                      |
| xml_etree_iterparse  | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                      |
| pickle_dict          | 17.2 us                                                     | 18.2 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.13x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| python_startup_no_site | 15.5 ms                                                     | 15.4 ms: 1.01x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 9.03 ms                                                     | 6.93 ms: 1.30x faster                                                      |
| django_template | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                      |
| genshi_text     | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                                      |
| genshi_xml      | 41.0 ms                                                     | 37.8 ms: 1.08x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.19x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| deltablue               | 4.19 ms                                                     | 2.51 ms: 1.67x faster                                                      |
| json_dumps              | 9.16 ms                                                     | 5.62 ms: 1.63x faster                                                      |
| go                      | 139 ms                                                      | 93.8 ms: 1.48x faster                                                      |
| scimark_sor             | 106 ms                                                      | 73.8 ms: 1.44x faster                                                      |
| async_tree_io           | 1.11 sec                                                    | 775 ms: 1.43x faster                                                       |
| async_tree_memoization  | 526 ms                                                      | 381 ms: 1.38x faster                                                       |
| async_tree_none         | 435 ms                                                      | 316 ms: 1.38x faster                                                       |
| pyflate                 | 409 ms                                                      | 297 ms: 1.38x faster                                                       |
| pickle_pure_python      | 270 us                                                      | 196 us: 1.38x faster                                                       |
| logging_silent          | 94.6 ns                                                     | 68.8 ns: 1.37x faster                                                      |
| richards                | 42.4 ms                                                     | 31.0 ms: 1.37x faster                                                      |
| raytrace                | 273 ms                                                      | 204 ms: 1.34x faster                                                       |
| html5lib                | 51.0 ms                                                     | 38.1 ms: 1.34x faster                                                      |
| chaos                   | 61.7 ms                                                     | 46.5 ms: 1.33x faster                                                      |
| crypto_pyaes            | 62.5 ms                                                     | 47.2 ms: 1.33x faster                                                      |
| scimark_monte_carlo     | 57.3 ms                                                     | 43.8 ms: 1.31x faster                                                      |
| mako                    | 9.03 ms                                                     | 6.93 ms: 1.30x faster                                                      |
| sqlglot_transpile       | 1.48 ms                                                     | 1.14 ms: 1.30x faster                                                      |
| pycparser               | 930 ms                                                      | 721 ms: 1.29x faster                                                       |
| scimark_lu              | 85.8 ms                                                     | 66.6 ms: 1.29x faster                                                      |
| unpickle_pure_python    | 183 us                                                      | 143 us: 1.28x faster                                                       |
| sqlglot_parse           | 1.22 ms                                                     | 951 us: 1.28x faster                                                       |
| hexiom                  | 5.74 ms                                                     | 4.51 ms: 1.27x faster                                                      |
| thrift                  | 617 us                                                      | 486 us: 1.27x faster                                                       |
| async_tree_cpu_io_mixed | 638 ms                                                      | 506 ms: 1.26x faster                                                       |
| regex_compile           | 106 ms                                                      | 86.3 ms: 1.23x faster                                                      |
| xml_etree_process       | 44.5 ms                                                     | 36.3 ms: 1.22x faster                                                      |
| async_generators        | 222 ms                                                      | 181 ms: 1.22x faster                                                       |
| pprint_pformat          | 1.22 sec                                                    | 1.00 sec: 1.22x faster                                                     |
| 2to3                    | 246 ms                                                      | 202 ms: 1.22x faster                                                       |
| django_template         | 28.9 ms                                                     | 23.8 ms: 1.21x faster                                                      |
| create_gc_cycles        | 800 us                                                      | 663 us: 1.21x faster                                                       |
| docutils                | 1.92 sec                                                    | 1.59 sec: 1.21x faster                                                     |
| pprint_safe_repr        | 592 ms                                                      | 495 ms: 1.20x faster                                                       |
| tornado_http            | 108 ms                                                      | 91.5 ms: 1.18x faster                                                      |
| dask                    | 313 ms                                                      | 265 ms: 1.18x faster                                                       |
| deepcopy_memo           | 28.8 us                                                     | 24.7 us: 1.16x faster                                                      |
| chameleon               | 5.79 ms                                                     | 4.99 ms: 1.16x faster                                                      |
| dulwich_log             | 50.5 ms                                                     | 43.5 ms: 1.16x faster                                                      |
| genshi_text             | 19.8 ms                                                     | 17.1 ms: 1.16x faster                                                      |
| sqlglot_optimize        | 39.8 ms                                                     | 34.4 ms: 1.16x faster                                                      |
| float                   | 61.7 ms                                                     | 53.5 ms: 1.15x faster                                                      |
| scimark_sparse_mat_mult | 2.72 ms                                                     | 2.37 ms: 1.15x faster                                                      |
| sympy_integrate         | 15.3 ms                                                     | 13.4 ms: 1.14x faster                                                      |
| regex_dna               | 136 ms                                                      | 119 ms: 1.14x faster                                                       |
| bench_thread_pool       | 958 us                                                      | 844 us: 1.13x faster                                                       |
| json                    | 3.14 ms                                                     | 2.77 ms: 1.13x faster                                                      |
| regex_v8                | 15.4 ms                                                     | 13.7 ms: 1.13x faster                                                      |
| python_startup          | 20.6 ms                                                     | 18.2 ms: 1.13x faster                                                      |
| mdp                     | 1.78 sec                                                    | 1.59 sec: 1.12x faster                                                     |
| xml_etree_parse         | 96.8 ms                                                     | 86.8 ms: 1.11x faster                                                      |
| pylint                  | 350 ms                                                      | 317 ms: 1.10x faster                                                       |
| xml_etree_generate      | 55.5 ms                                                     | 50.5 ms: 1.10x faster                                                      |
| sqlglot_normalize       | 205 ms                                                      | 188 ms: 1.09x faster                                                       |
| deepcopy                | 255 us                                                      | 235 us: 1.09x faster                                                       |
| genshi_xml              | 41.0 ms                                                     | 37.8 ms: 1.08x faster                                                      |
| sympy_sum               | 107 ms                                                      | 98.9 ms: 1.08x faster                                                      |
| fannkuch                | 256 ms                                                      | 238 ms: 1.07x faster                                                       |
| deepcopy_reduce         | 2.20 us                                                     | 2.05 us: 1.07x faster                                                      |
| coroutines              | 16.0 ms                                                     | 15.0 ms: 1.07x faster                                                      |
| sqlite_synth            | 1.91 us                                                     | 1.80 us: 1.06x faster                                                      |
| sympy_str               | 194 ms                                                      | 183 ms: 1.06x faster                                                       |
| sympy_expand            | 314 ms                                                      | 296 ms: 1.06x faster                                                       |
| nbody                   | 71.3 ms                                                     | 67.2 ms: 1.06x faster                                                      |
| meteor_contest          | 75.9 ms                                                     | 71.8 ms: 1.06x faster                                                      |
| asyncio_tcp             | 732 ms                                                      | 694 ms: 1.06x faster                                                       |
| comprehensions          | 16.5 us                                                     | 15.6 us: 1.05x faster                                                      |
| spectral_norm           | 77.3 ms                                                     | 73.8 ms: 1.05x faster                                                      |
| pickle                  | 6.85 us                                                     | 6.55 us: 1.05x faster                                                      |
| pickle_list             | 2.75 us                                                     | 2.64 us: 1.04x faster                                                      |
| unpickle_list           | 2.71 us                                                     | 2.60 us: 1.04x faster                                                      |
| json_loads              | 14.0 us                                                     | 13.5 us: 1.04x faster                                                      |
| unpickle                | 9.09 us                                                     | 8.87 us: 1.03x faster                                                      |
| telco                   | 3.94 ms                                                     | 3.85 ms: 1.02x faster                                                      |
| pathlib                 | 75.7 ms                                                     | 74.0 ms: 1.02x faster                                                      |
| xml_etree_iterparse     | 65.0 ms                                                     | 63.6 ms: 1.02x faster                                                      |
| bench_mp_pool           | 62.0 ms                                                     | 60.9 ms: 1.02x faster                                                      |
| nqueens                 | 66.6 ms                                                     | 65.4 ms: 1.02x faster                                                      |
| regex_effbot            | 1.66 ms                                                     | 1.63 ms: 1.01x faster                                                      |
| python_startup_no_site  | 15.5 ms                                                     | 15.4 ms: 1.01x faster                                                      |
| pidigits                | 149 ms                                                      | 148 ms: 1.01x faster                                                       |
| gc_traversal            | 1.41 ms                                                     | 1.42 ms: 1.01x slower                                                      |
| pickle_dict             | 17.2 us                                                     | 18.2 us: 1.06x slower                                                      |
| generators              | 32.4 ms                                                     | 34.5 ms: 1.07x slower                                                      |
| unpack_sequence         | 39.6 ns                                                     | 42.3 ns: 1.07x slower                                                      |
| logging_format          | 6.76 us                                                     | 7.28 us: 1.08x slower                                                      |
| logging_simple          | 6.22 us                                                     | 6.80 us: 1.09x slower                                                      |
| coverage                | 39.0 ms                                                     | 52.1 ms: 1.34x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.15x faster                                                               |

Benchmark hidden because not significant (1): scimark_fft
Ignored benchmarks (9) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf1-amd64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp_ssl, flaskblogging, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.13x
- 95% likely to have a speedup of 1.13x
- 99% likely to have a speedup of 1.11x


# Memory

- memory change: unknown