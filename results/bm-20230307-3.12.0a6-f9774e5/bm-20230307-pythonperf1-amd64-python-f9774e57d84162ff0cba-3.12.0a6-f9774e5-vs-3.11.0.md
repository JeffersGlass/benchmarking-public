
# Results vs. 3.11.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: windows-amd64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.10x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 194 ms: 1.10x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.76 ms: 1.10x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.51 sec: 1.09x faster                                                     |
| html5lib       | 38.9 ms                                                     | 34.8 ms: 1.11x faster                                                      |
| tornado_http   | 92.8 ms                                                     | 90.6 ms: 1.02x faster                                                      |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_memoization  | 399 ms                                                      | 356 ms: 1.12x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 479 ms: 1.11x faster                                                       |
| async_tree_none         | 332 ms                                                      | 304 ms: 1.09x faster                                                       |
| async_tree_io           | 808 ms                                                      | 744 ms: 1.09x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 47.4 ms: 1.15x faster                                                      |
| nbody          | 70.3 ms                                                     | 63.3 ms: 1.11x faster                                                      |
| pidigits       | 150 ms                                                      | 147 ms: 1.02x faster                                                       |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 83.5 ms: 1.09x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| regex_dna      | 116 ms                                                      | 115 ms: 1.01x faster                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                               |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 124 us: 1.27x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 175 us: 1.19x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 88.4 ms: 1.10x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 61.3 ms: 1.07x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 35.6 ms: 1.04x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 52.1 ms: 1.01x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.7 us: 1.01x slower                                                      |
| json_loads           | 13.0 us                                                     | 13.4 us: 1.03x slower                                                      |
| pickle_list          | 2.70 us                                                     | 2.80 us: 1.04x slower                                                      |
| pickle               | 6.64 us                                                     | 6.96 us: 1.05x slower                                                      |
| unpickle             | 7.57 us                                                     | 7.98 us: 1.05x slower                                                      |
| unpickle_list        | 2.59 us                                                     | 2.74 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.5 ms: 1.09x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 13.9 ms: 1.33x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 30.9 ms: 1.29x faster                                                      |
| mako            | 7.58 ms                                                     | 6.20 ms: 1.22x faster                                                      |
| django_template | 24.4 ms                                                     | 20.9 ms: 1.17x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.25x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 27.9 ns: 1.68x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 463 ms: 1.57x faster                                                       |
| generators              | 34.0 ms                                                     | 21.9 ms: 1.55x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 5.51 ms: 1.47x faster                                                      |
| deltablue               | 2.70 ms                                                     | 1.92 ms: 1.40x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 13.9 ms: 1.33x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 30.9 ms: 1.29x faster                                                      |
| richards                | 31.4 ms                                                     | 24.5 ms: 1.28x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 56.5 ns: 1.27x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 124 us: 1.27x faster                                                       |
| go                      | 101 ms                                                      | 82.6 ms: 1.22x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.20 ms: 1.22x faster                                                      |
| nqueens                 | 68.3 ms                                                     | 56.9 ms: 1.20x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 175 us: 1.19x faster                                                       |
| hexiom                  | 4.55 ms                                                     | 3.83 ms: 1.19x faster                                                      |
| raytrace                | 213 ms                                                      | 180 ms: 1.18x faster                                                       |
| fannkuch                | 253 ms                                                      | 216 ms: 1.17x faster                                                       |
| django_template         | 24.4 ms                                                     | 20.9 ms: 1.17x faster                                                      |
| pyflate                 | 312 ms                                                      | 270 ms: 1.16x faster                                                       |
| chaos                   | 48.4 ms                                                     | 42.0 ms: 1.15x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 22.6 us: 1.15x faster                                                      |
| float                   | 54.4 ms                                                     | 47.4 ms: 1.15x faster                                                      |
| sqlglot_normalize       | 190 ms                                                      | 168 ms: 1.13x faster                                                       |
| crypto_pyaes            | 48.9 ms                                                     | 43.3 ms: 1.13x faster                                                      |
| deepcopy                | 246 us                                                      | 219 us: 1.13x faster                                                       |
| logging_simple          | 6.86 us                                                     | 6.10 us: 1.12x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 40.4 ms: 1.12x faster                                                      |
| async_tree_memoization  | 399 ms                                                      | 356 ms: 1.12x faster                                                       |
| html5lib                | 38.9 ms                                                     | 34.8 ms: 1.11x faster                                                      |
| mdp                     | 1.59 sec                                                    | 1.43 sec: 1.11x faster                                                     |
| pprint_pformat          | 1.09 sec                                                    | 977 ms: 1.11x faster                                                       |
| nbody                   | 70.3 ms                                                     | 63.3 ms: 1.11x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 478 ms: 1.11x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 479 ms: 1.11x faster                                                       |
| meteor_contest          | 75.2 ms                                                     | 68.0 ms: 1.11x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 31.2 ms: 1.11x faster                                                      |
| chameleon               | 5.26 ms                                                     | 4.76 ms: 1.10x faster                                                      |
| xml_etree_parse         | 97.6 ms                                                     | 88.4 ms: 1.10x faster                                                      |
| 2to3                    | 214 ms                                                      | 194 ms: 1.10x faster                                                       |
| dulwich_log             | 46.4 ms                                                     | 42.2 ms: 1.10x faster                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.06 ms: 1.10x faster                                                      |
| sqlglot_parse           | 953 us                                                      | 871 us: 1.09x faster                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 1.88 us: 1.09x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.55 us: 1.09x faster                                                      |
| async_tree_none         | 332 ms                                                      | 304 ms: 1.09x faster                                                       |
| scimark_sor             | 78.1 ms                                                     | 71.6 ms: 1.09x faster                                                      |
| regex_compile           | 91.0 ms                                                     | 83.5 ms: 1.09x faster                                                      |
| docutils                | 1.64 sec                                                    | 1.51 sec: 1.09x faster                                                     |
| python_startup_no_site  | 16.8 ms                                                     | 15.5 ms: 1.09x faster                                                      |
| json                    | 2.98 ms                                                     | 2.74 ms: 1.09x faster                                                      |
| async_tree_io           | 808 ms                                                      | 744 ms: 1.09x faster                                                       |
| pycparser               | 720 ms                                                      | 663 ms: 1.09x faster                                                       |
| python_startup          | 19.8 ms                                                     | 18.2 ms: 1.08x faster                                                      |
| sympy_expand            | 299 ms                                                      | 277 ms: 1.08x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.1 ms: 1.07x faster                                                      |
| sympy_str               | 185 ms                                                      | 173 ms: 1.07x faster                                                       |
| coroutines              | 15.0 ms                                                     | 14.0 ms: 1.07x faster                                                      |
| xml_etree_iterparse     | 65.6 ms                                                     | 61.3 ms: 1.07x faster                                                      |
| scimark_lu              | 62.8 ms                                                     | 58.7 ms: 1.07x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 671 us: 1.06x faster                                                       |
| scimark_fft             | 179 ms                                                      | 169 ms: 1.06x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| bench_thread_pool       | 872 us                                                      | 827 us: 1.05x faster                                                       |
| telco                   | 4.06 ms                                                     | 3.86 ms: 1.05x faster                                                      |
| xml_etree_process       | 37.2 ms                                                     | 35.6 ms: 1.04x faster                                                      |
| thrift                  | 494 us                                                      | 476 us: 1.04x faster                                                       |
| sympy_sum               | 100 ms                                                      | 96.6 ms: 1.04x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.44 ms: 1.04x faster                                                      |
| tornado_http            | 92.8 ms                                                     | 90.6 ms: 1.02x faster                                                      |
| pidigits                | 150 ms                                                      | 147 ms: 1.02x faster                                                       |
| spectral_norm           | 68.3 ms                                                     | 67.2 ms: 1.02x faster                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 52.1 ms: 1.01x faster                                                      |
| regex_dna               | 116 ms                                                      | 115 ms: 1.01x faster                                                       |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.56 ms: 1.01x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 18.7 us: 1.01x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.79 us: 1.01x slower                                                      |
| comprehensions          | 15.6 us                                                     | 15.9 us: 1.02x slower                                                      |
| json_loads              | 13.0 us                                                     | 13.4 us: 1.03x slower                                                      |
| pickle_list             | 2.70 us                                                     | 2.80 us: 1.04x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 73.9 ms: 1.04x slower                                                      |
| pickle                  | 6.64 us                                                     | 6.96 us: 1.05x slower                                                      |
| unpickle                | 7.57 us                                                     | 7.98 us: 1.05x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.74 us: 1.06x slower                                                      |
| coverage                | 43.4 ms                                                     | 49.9 ms: 1.15x slower                                                      |
| async_generators        | 177 ms                                                      | 223 ms: 1.26x slower                                                       |
| dask                    | 273 ms                                                      | 352 ms: 1.29x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.10x faster                                                               |

Benchmark hidden because not significant (2): regex_effbot, bench_mp_pool
Ignored benchmarks (14) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.08x
- 95% likely to have a speedup of 1.08x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: unknown