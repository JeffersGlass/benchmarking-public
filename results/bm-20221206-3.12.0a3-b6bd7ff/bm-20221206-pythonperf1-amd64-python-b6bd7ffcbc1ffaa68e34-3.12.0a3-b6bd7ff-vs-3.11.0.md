
# Results vs. 3.11.0

- fork: python
- ref: b6bd7ffcbc1ffaa68e34
- machine: windows-amd64
- commit hash: b6bd7ff
- commit date: 2022-12-06
- overall geometric mean: 1.09x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 196 ms: 1.09x faster                                                       |
| chameleon      | 5.26 ms                                                     | 4.53 ms: 1.16x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                     |
| html5lib       | 38.9 ms                                                     | 35.0 ms: 1.11x faster                                                      |
| Geometric mean | (ref)                                                       | 1.10x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 530 ms                                                      | 501 ms: 1.06x faster                                                       |
| async_tree_none         | 332 ms                                                      | 317 ms: 1.05x faster                                                       |
| async_tree_io           | 808 ms                                                      | 780 ms: 1.04x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 388 ms: 1.03x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.04x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 70.3 ms                                                     | 62.3 ms: 1.13x faster                                                      |
| float          | 54.4 ms                                                     | 50.1 ms: 1.08x faster                                                      |
| pidigits       | 150 ms                                                      | 151 ms: 1.00x slower                                                       |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 82.5 ms: 1.10x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                                      |
| regex_effbot   | 1.50 ms                                                     | 1.54 ms: 1.03x slower                                                      |
| regex_dna      | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.01x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| json_dumps           | 8.09 ms                                                     | 5.17 ms: 1.57x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 121 us: 1.30x faster                                                       |
| pickle_pure_python   | 208 us                                                      | 179 us: 1.17x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 90.5 ms: 1.08x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 35.0 ms: 1.06x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 49.7 ms: 1.06x faster                                                      |
| xml_etree_iterparse  | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| json_loads           | 13.0 us                                                     | 12.9 us: 1.01x faster                                                      |
| unpickle_list        | 2.59 us                                                     | 2.61 us: 1.01x slower                                                      |
| pickle               | 6.64 us                                                     | 6.90 us: 1.04x slower                                                      |
| pickle_dict          | 18.5 us                                                     | 19.4 us: 1.05x slower                                                      |
| unpickle             | 7.57 us                                                     | 7.99 us: 1.05x slower                                                      |
| pickle_list          | 2.70 us                                                     | 2.85 us: 1.06x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.8 ms                                                     | 18.5 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.8 ms                                                     | 15.7 ms: 1.07x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 13.8 ms: 1.34x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 32.3 ms: 1.24x faster                                                      |
| mako            | 7.58 ms                                                     | 6.19 ms: 1.23x faster                                                      |
| django_template | 24.4 ms                                                     | 21.4 ms: 1.14x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.23x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20221206-pythonperf1-amd64-python-b6bd7ffcbc1ffaa68e34-3.12.0a3-b6bd7ff |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 46.9 ns                                                     | 26.4 ns: 1.77x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 5.17 ms: 1.57x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 13.8 ms: 1.34x faster                                                      |
| deltablue               | 2.70 ms                                                     | 2.07 ms: 1.30x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 121 us: 1.30x faster                                                       |
| richards                | 31.4 ms                                                     | 24.5 ms: 1.28x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 57.2 ns: 1.26x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 32.3 ms: 1.24x faster                                                      |
| deepcopy_memo           | 26.0 us                                                     | 21.2 us: 1.23x faster                                                      |
| mako                    | 7.58 ms                                                     | 6.19 ms: 1.23x faster                                                      |
| scimark_sor             | 78.1 ms                                                     | 64.6 ms: 1.21x faster                                                      |
| raytrace                | 213 ms                                                      | 179 ms: 1.19x faster                                                       |
| go                      | 101 ms                                                      | 84.8 ms: 1.19x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 38.1 ms: 1.19x faster                                                      |
| pyflate                 | 312 ms                                                      | 264 ms: 1.19x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 57.9 ms: 1.18x faster                                                      |
| hexiom                  | 4.55 ms                                                     | 3.89 ms: 1.17x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 179 us: 1.17x faster                                                       |
| chameleon               | 5.26 ms                                                     | 4.53 ms: 1.16x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 458 ms: 1.16x faster                                                       |
| deepcopy                | 246 us                                                      | 214 us: 1.15x faster                                                       |
| pprint_pformat          | 1.09 sec                                                    | 947 ms: 1.15x faster                                                       |
| scimark_lu              | 62.8 ms                                                     | 54.8 ms: 1.15x faster                                                      |
| django_template         | 24.4 ms                                                     | 21.4 ms: 1.14x faster                                                      |
| fannkuch                | 253 ms                                                      | 222 ms: 1.14x faster                                                       |
| nbody                   | 70.3 ms                                                     | 62.3 ms: 1.13x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 41.2 ms: 1.13x faster                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.30 ms: 1.12x faster                                                      |
| chaos                   | 48.4 ms                                                     | 43.2 ms: 1.12x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.64 ms: 1.12x faster                                                      |
| spectral_norm           | 68.3 ms                                                     | 61.4 ms: 1.11x faster                                                      |
| html5lib                | 38.9 ms                                                     | 35.0 ms: 1.11x faster                                                      |
| sqlglot_parse           | 953 us                                                      | 860 us: 1.11x faster                                                       |
| sqlglot_normalize       | 190 ms                                                      | 172 ms: 1.11x faster                                                       |
| regex_compile           | 91.0 ms                                                     | 82.5 ms: 1.10x faster                                                      |
| logging_simple          | 6.86 us                                                     | 6.22 us: 1.10x faster                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.06 ms: 1.10x faster                                                      |
| deepcopy_reduce         | 2.06 us                                                     | 1.88 us: 1.10x faster                                                      |
| meteor_contest          | 75.2 ms                                                     | 68.8 ms: 1.09x faster                                                      |
| 2to3                    | 214 ms                                                      | 196 ms: 1.09x faster                                                       |
| json                    | 2.98 ms                                                     | 2.74 ms: 1.09x faster                                                      |
| float                   | 54.4 ms                                                     | 50.1 ms: 1.08x faster                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 45.1 ms: 1.08x faster                                                      |
| logging_format          | 7.16 us                                                     | 6.64 us: 1.08x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 32.0 ms: 1.08x faster                                                      |
| xml_etree_parse         | 97.6 ms                                                     | 90.5 ms: 1.08x faster                                                      |
| python_startup          | 19.8 ms                                                     | 18.5 ms: 1.07x faster                                                      |
| python_startup_no_site  | 16.8 ms                                                     | 15.7 ms: 1.07x faster                                                      |
| sympy_str               | 185 ms                                                      | 173 ms: 1.07x faster                                                       |
| xml_etree_process       | 37.2 ms                                                     | 35.0 ms: 1.06x faster                                                      |
| dask                    | 273 ms                                                      | 258 ms: 1.06x faster                                                       |
| xml_etree_generate      | 52.5 ms                                                     | 49.7 ms: 1.06x faster                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 501 ms: 1.06x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.3 ms: 1.05x faster                                                      |
| xml_etree_iterparse     | 65.6 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| thrift                  | 494 us                                                      | 469 us: 1.05x faster                                                       |
| docutils                | 1.64 sec                                                    | 1.56 sec: 1.05x faster                                                     |
| async_tree_none         | 332 ms                                                      | 317 ms: 1.05x faster                                                       |
| create_gc_cycles        | 713 us                                                      | 682 us: 1.05x faster                                                       |
| sympy_expand            | 299 ms                                                      | 286 ms: 1.05x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 837 us: 1.04x faster                                                       |
| pycparser               | 720 ms                                                      | 691 ms: 1.04x faster                                                       |
| async_tree_io           | 808 ms                                                      | 780 ms: 1.04x faster                                                       |
| gc_traversal            | 1.49 ms                                                     | 1.44 ms: 1.04x faster                                                      |
| async_tree_memoization  | 399 ms                                                      | 388 ms: 1.03x faster                                                       |
| sqlite_synth            | 1.77 us                                                     | 1.73 us: 1.02x faster                                                      |
| scimark_fft             | 179 ms                                                      | 177 ms: 1.02x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 14.0 ms: 1.01x faster                                                      |
| sympy_sum               | 100 ms                                                      | 99.0 ms: 1.01x faster                                                      |
| json_loads              | 13.0 us                                                     | 12.9 us: 1.01x faster                                                      |
| comprehensions          | 15.6 us                                                     | 15.5 us: 1.01x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 62.8 ms: 1.01x faster                                                      |
| pidigits                | 150 ms                                                      | 151 ms: 1.00x slower                                                       |
| mdp                     | 1.59 sec                                                    | 1.61 sec: 1.01x slower                                                     |
| coroutines              | 15.0 ms                                                     | 15.1 ms: 1.01x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.61 us: 1.01x slower                                                      |
| async_generators        | 177 ms                                                      | 179 ms: 1.01x slower                                                       |
| pathlib                 | 70.9 ms                                                     | 72.1 ms: 1.02x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.54 ms: 1.03x slower                                                      |
| regex_dna               | 116 ms                                                      | 120 ms: 1.03x slower                                                       |
| pickle                  | 6.64 us                                                     | 6.90 us: 1.04x slower                                                      |
| pickle_dict             | 18.5 us                                                     | 19.4 us: 1.05x slower                                                      |
| unpickle                | 7.57 us                                                     | 7.99 us: 1.05x slower                                                      |
| pickle_list             | 2.70 us                                                     | 2.85 us: 1.06x slower                                                      |
| coverage                | 43.4 ms                                                     | 51.6 ms: 1.19x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.09x faster                                                               |

Benchmark hidden because not significant (2): generators, asyncio_tcp
Ignored benchmarks (15) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, flaskblogging, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, tornado_http, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown