
# Results vs. 3.11.0

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: windows-amd64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.07x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 222 ms: 1.04x slower                                                       |
| chameleon      | 5.26 ms                                                     | 5.68 ms: 1.08x slower                                                      |
| docutils       | 1.64 sec                                                    | 1.73 sec: 1.05x slower                                                     |
| html5lib       | 38.9 ms                                                     | 41.5 ms: 1.07x slower                                                      |
| tornado_http   | 92.8 ms                                                     | 97.6 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                       | 1.06x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 332 ms                                                      | 296 ms: 1.12x faster                                                       |
| async_tree_io           | 808 ms                                                      | 777 ms: 1.04x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 384 ms: 1.04x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 541 ms: 1.02x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.04x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                      |
| nbody          | 70.3 ms                                                     | 86.8 ms: 1.23x slower                                                      |
| Geometric mean | (ref)                                                       | 1.09x slower                                                               |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 92.3 ms: 1.01x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                                      |
| regex_dna      | 116 ms                                                      | 129 ms: 1.11x slower                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                                      |
| Geometric mean | (ref)                                                       | 1.06x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 16.8 us: 1.10x faster                                                      |
| pickle_list          | 2.70 us                                                     | 2.66 us: 1.01x faster                                                      |
| unpickle_list        | 2.59 us                                                     | 2.56 us: 1.01x faster                                                      |
| pickle               | 6.64 us                                                     | 6.58 us: 1.01x faster                                                      |
| json_dumps           | 8.09 ms                                                     | 8.03 ms: 1.01x faster                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 54.8 ms: 1.04x slower                                                      |
| xml_etree_process    | 37.2 ms                                                     | 40.3 ms: 1.08x slower                                                      |
| unpickle_pure_python | 157 us                                                      | 172 us: 1.09x slower                                                       |
| json_loads           | 13.0 us                                                     | 14.4 us: 1.11x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.48 us: 1.12x slower                                                      |
| pickle_pure_python   | 208 us                                                      | 240 us: 1.15x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.03x slower                                                               |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                                      |
| python_startup         | 19.8 ms                                                     | 20.7 ms: 1.05x slower                                                      |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.3 ms: 1.07x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 37.8 ms: 1.06x faster                                                      |
| django_template | 24.4 ms                                                     | 25.8 ms: 1.06x slower                                                      |
| mako            | 7.58 ms                                                     | 8.12 ms: 1.07x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.00x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| logging_simple          | 6.86 us                                                     | 5.24 us: 1.31x faster                                                      |
| logging_format          | 7.16 us                                                     | 5.64 us: 1.27x faster                                                      |
| generators              | 34.0 ms                                                     | 28.9 ms: 1.17x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 628 ms: 1.15x faster                                                       |
| unpack_sequence         | 46.9 ns                                                     | 41.7 ns: 1.13x faster                                                      |
| async_tree_none         | 332 ms                                                      | 296 ms: 1.12x faster                                                       |
| pickle_dict             | 18.5 us                                                     | 16.8 us: 1.10x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.37 ms: 1.09x faster                                                      |
| python_startup_no_site  | 16.8 ms                                                     | 15.6 ms: 1.08x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 17.3 ms: 1.07x faster                                                      |
| genshi_xml              | 39.9 ms                                                     | 37.8 ms: 1.06x faster                                                      |
| async_tree_io           | 808 ms                                                      | 777 ms: 1.04x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 384 ms: 1.04x faster                                                       |
| telco                   | 4.06 ms                                                     | 3.98 ms: 1.02x faster                                                      |
| pylint                  | 323 ms                                                      | 318 ms: 1.02x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.66 us: 1.01x faster                                                      |
| mdp                     | 1.59 sec                                                    | 1.58 sec: 1.01x faster                                                     |
| unpickle_list           | 2.59 us                                                     | 2.56 us: 1.01x faster                                                      |
| nqueens                 | 68.3 ms                                                     | 67.7 ms: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.58 us: 1.01x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 8.03 ms: 1.01x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 46.1 ms: 1.01x faster                                                      |
| sqlalchemy_declarative  | 85.6 ms                                                     | 86.3 ms: 1.01x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| regex_compile           | 91.0 ms                                                     | 92.3 ms: 1.01x slower                                                      |
| sympy_str               | 185 ms                                                      | 188 ms: 1.01x slower                                                       |
| regex_v8                | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.80 us: 1.02x slower                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 541 ms: 1.02x slower                                                       |
| sympy_integrate         | 14.0 ms                                                     | 14.4 ms: 1.02x slower                                                      |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.7 ms: 1.03x slower                                                      |
| sympy_expand            | 299 ms                                                      | 309 ms: 1.03x slower                                                       |
| pathlib                 | 70.9 ms                                                     | 73.4 ms: 1.04x slower                                                      |
| deepcopy                | 246 us                                                      | 256 us: 1.04x slower                                                       |
| 2to3                    | 214 ms                                                      | 222 ms: 1.04x slower                                                       |
| xml_etree_generate      | 52.5 ms                                                     | 54.8 ms: 1.04x slower                                                      |
| python_startup          | 19.8 ms                                                     | 20.7 ms: 1.05x slower                                                      |
| bench_thread_pool       | 872 us                                                      | 915 us: 1.05x slower                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 2.16 us: 1.05x slower                                                      |
| raytrace                | 213 ms                                                      | 224 ms: 1.05x slower                                                       |
| docutils                | 1.64 sec                                                    | 1.73 sec: 1.05x slower                                                     |
| tornado_http            | 92.8 ms                                                     | 97.6 ms: 1.05x slower                                                      |
| float                   | 54.4 ms                                                     | 57.2 ms: 1.05x slower                                                      |
| sqlglot_normalize       | 190 ms                                                      | 201 ms: 1.06x slower                                                       |
| django_template         | 24.4 ms                                                     | 25.8 ms: 1.06x slower                                                      |
| pprint_pformat          | 1.09 sec                                                    | 1.16 sec: 1.07x slower                                                     |
| html5lib                | 38.9 ms                                                     | 41.5 ms: 1.07x slower                                                      |
| go                      | 101 ms                                                      | 108 ms: 1.07x slower                                                       |
| mako                    | 7.58 ms                                                     | 8.12 ms: 1.07x slower                                                      |
| pprint_safe_repr        | 529 ms                                                      | 570 ms: 1.08x slower                                                       |
| pycparser               | 720 ms                                                      | 777 ms: 1.08x slower                                                       |
| dask                    | 273 ms                                                      | 295 ms: 1.08x slower                                                       |
| chameleon               | 5.26 ms                                                     | 5.68 ms: 1.08x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 40.3 ms: 1.08x slower                                                      |
| thrift                  | 494 us                                                      | 535 us: 1.08x slower                                                       |
| unpickle_pure_python    | 157 us                                                      | 172 us: 1.09x slower                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 37.8 ms: 1.10x slower                                                      |
| deepcopy_memo           | 26.0 us                                                     | 28.6 us: 1.10x slower                                                      |
| fannkuch                | 253 ms                                                      | 279 ms: 1.10x slower                                                       |
| richards                | 31.4 ms                                                     | 34.7 ms: 1.10x slower                                                      |
| regex_dna               | 116 ms                                                      | 129 ms: 1.11x slower                                                       |
| regex_effbot            | 1.50 ms                                                     | 1.66 ms: 1.11x slower                                                      |
| json_loads              | 13.0 us                                                     | 14.4 us: 1.11x slower                                                      |
| unpickle                | 7.57 us                                                     | 8.48 us: 1.12x slower                                                      |
| async_generators        | 177 ms                                                      | 198 ms: 1.12x slower                                                       |
| create_gc_cycles        | 713 us                                                      | 807 us: 1.13x slower                                                       |
| hexiom                  | 4.55 ms                                                     | 5.17 ms: 1.13x slower                                                      |
| chaos                   | 48.4 ms                                                     | 55.0 ms: 1.14x slower                                                      |
| pickle_pure_python      | 208 us                                                      | 240 us: 1.15x slower                                                       |
| deltablue               | 2.70 ms                                                     | 3.12 ms: 1.16x slower                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 52.6 ms: 1.16x slower                                                      |
| logging_silent          | 71.8 ns                                                     | 83.4 ns: 1.16x slower                                                      |
| pyflate                 | 312 ms                                                      | 365 ms: 1.17x slower                                                       |
| crypto_pyaes            | 48.9 ms                                                     | 57.7 ms: 1.18x slower                                                      |
| coroutines              | 15.0 ms                                                     | 17.9 ms: 1.20x slower                                                      |
| scimark_fft             | 179 ms                                                      | 216 ms: 1.20x slower                                                       |
| comprehensions          | 15.6 us                                                     | 19.1 us: 1.22x slower                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 3.18 ms: 1.23x slower                                                      |
| nbody                   | 70.3 ms                                                     | 86.8 ms: 1.23x slower                                                      |
| spectral_norm           | 68.3 ms                                                     | 84.7 ms: 1.24x slower                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.53 ms: 1.32x slower                                                      |
| scimark_lu              | 62.8 ms                                                     | 83.6 ms: 1.33x slower                                                      |
| scimark_sor             | 78.1 ms                                                     | 105 ms: 1.35x slower                                                       |
| sqlglot_parse           | 953 us                                                      | 1.32 ms: 1.38x slower                                                      |
| coverage                | 43.4 ms                                                     | 261 ms: 6.02x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.07x slower                                                               |

Benchmark hidden because not significant (7): bench_mp_pool, xml_etree_iterparse, meteor_contest, sympy_sum, pidigits, xml_etree_parse, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.03x
- 95% likely to have a slowdown of 1.03x
- 99% likely to have a slowdown of 1.02x


# Memory

- memory change: unknown