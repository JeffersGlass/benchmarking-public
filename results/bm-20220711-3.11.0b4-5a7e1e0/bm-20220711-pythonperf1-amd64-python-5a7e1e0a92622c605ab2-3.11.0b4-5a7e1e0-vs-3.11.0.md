
# Results vs. 3.11.0

- fork: python
- ref: 5a7e1e0a92622c605ab2
- machine: windows-amd64
- commit hash: 5a7e1e0
- commit date: 2022-07-11
- overall geometric mean: 1.01x faster \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.00x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 206 ms: 1.04x faster                                                       |
| chameleon      | 5.26 ms                                                     | 5.14 ms: 1.02x faster                                                      |
| docutils       | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                     |
| tornado_http   | 92.8 ms                                                     | 91.9 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmark hidden because not significant (1): html5lib

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 808 ms                                                      | 753 ms: 1.07x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 375 ms: 1.06x faster                                                       |
| async_tree_none         | 332 ms                                                      | 317 ms: 1.05x faster                                                       |
| async_tree_cpu_io_mixed | 530 ms                                                      | 508 ms: 1.04x faster                                                       |
| Geometric mean          | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| nbody          | 70.3 ms                                                     | 68.7 ms: 1.02x faster                                                      |
| float          | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| regex_dna      | 116 ms                                                      | 114 ms: 1.02x faster                                                       |
| regex_effbot   | 1.50 ms                                                     | 1.70 ms: 1.13x slower                                                      |
| Geometric mean | (ref)                                                       | 1.01x slower                                                               |

Benchmark hidden because not significant (1): regex_compile

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| xml_etree_iterparse  | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                      |
| json_dumps           | 8.09 ms                                                     | 7.78 ms: 1.04x faster                                                      |
| unpickle_pure_python | 157 us                                                      | 152 us: 1.03x faster                                                       |
| xml_etree_parse      | 97.6 ms                                                     | 95.1 ms: 1.03x faster                                                      |
| pickle               | 6.64 us                                                     | 6.48 us: 1.02x faster                                                      |
| pickle_pure_python   | 208 us                                                      | 204 us: 1.02x faster                                                       |
| pickle_list          | 2.70 us                                                     | 2.65 us: 1.02x faster                                                      |
| pickle_dict          | 18.5 us                                                     | 18.4 us: 1.00x faster                                                      |
| xml_etree_process    | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 53.4 ms: 1.02x slower                                                      |
| unpickle_list        | 2.59 us                                                     | 2.80 us: 1.08x slower                                                      |
| json_loads           | 13.0 us                                                     | 14.1 us: 1.08x slower                                                      |
| unpickle             | 7.57 us                                                     | 8.32 us: 1.10x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.6 ms: 1.05x faster                                                      |
| mako            | 7.58 ms                                                     | 7.23 ms: 1.05x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 38.6 ms: 1.04x faster                                                      |
| django_template | 24.4 ms                                                     | 25.0 ms: 1.02x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.03x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20220711-pythonperf1-amd64-python-5a7e1e0a92622c605ab2-3.11.0b4-5a7e1e0 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site  | 16.8 ms                                                     | 15.4 ms: 1.09x faster                                                      |
| python_startup          | 19.8 ms                                                     | 18.4 ms: 1.08x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 675 ms: 1.08x faster                                                       |
| create_gc_cycles        | 713 us                                                      | 664 us: 1.07x faster                                                       |
| async_tree_io           | 808 ms                                                      | 753 ms: 1.07x faster                                                       |
| async_tree_memoization  | 399 ms                                                      | 375 ms: 1.06x faster                                                       |
| gc_traversal            | 1.49 ms                                                     | 1.41 ms: 1.06x faster                                                      |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 44.2 ms: 1.05x faster                                                      |
| genshi_text             | 18.4 ms                                                     | 17.6 ms: 1.05x faster                                                      |
| mako                    | 7.58 ms                                                     | 7.23 ms: 1.05x faster                                                      |
| async_tree_none         | 332 ms                                                      | 317 ms: 1.05x faster                                                       |
| raytrace                | 213 ms                                                      | 204 ms: 1.05x faster                                                       |
| xml_etree_iterparse     | 65.6 ms                                                     | 62.7 ms: 1.05x faster                                                      |
| sympy_sum               | 100 ms                                                      | 95.8 ms: 1.04x faster                                                      |
| async_tree_cpu_io_mixed | 530 ms                                                      | 508 ms: 1.04x faster                                                       |
| sqlite_synth            | 1.77 us                                                     | 1.70 us: 1.04x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 7.78 ms: 1.04x faster                                                      |
| docutils                | 1.64 sec                                                    | 1.58 sec: 1.04x faster                                                     |
| 2to3                    | 214 ms                                                      | 206 ms: 1.04x faster                                                       |
| genshi_xml              | 39.9 ms                                                     | 38.6 ms: 1.04x faster                                                      |
| unpack_sequence         | 46.9 ns                                                     | 45.4 ns: 1.03x faster                                                      |
| unpickle_pure_python    | 157 us                                                      | 152 us: 1.03x faster                                                       |
| sqlglot_transpile       | 1.16 ms                                                     | 1.13 ms: 1.03x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 61.4 ms: 1.03x faster                                                      |
| logging_simple          | 6.86 us                                                     | 6.68 us: 1.03x faster                                                      |
| pprint_safe_repr        | 529 ms                                                      | 515 ms: 1.03x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 95.1 ms: 1.03x faster                                                      |
| aiohttp                 | 883 us                                                      | 860 us: 1.03x faster                                                       |
| pidigits                | 150 ms                                                      | 146 ms: 1.03x faster                                                       |
| sympy_integrate         | 14.0 ms                                                     | 13.7 ms: 1.03x faster                                                      |
| sympy_expand            | 299 ms                                                      | 291 ms: 1.03x faster                                                       |
| deepcopy_memo           | 26.0 us                                                     | 25.3 us: 1.02x faster                                                      |
| chameleon               | 5.26 ms                                                     | 5.14 ms: 1.02x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.48 us: 1.02x faster                                                      |
| nbody                   | 70.3 ms                                                     | 68.7 ms: 1.02x faster                                                      |
| scimark_monte_carlo     | 45.3 ms                                                     | 44.3 ms: 1.02x faster                                                      |
| pickle_pure_python      | 208 us                                                      | 204 us: 1.02x faster                                                       |
| pyflate                 | 312 ms                                                      | 306 ms: 1.02x faster                                                       |
| pprint_pformat          | 1.09 sec                                                    | 1.07 sec: 1.02x faster                                                     |
| pycparser               | 720 ms                                                      | 706 ms: 1.02x faster                                                       |
| sqlglot_parse           | 953 us                                                      | 936 us: 1.02x faster                                                       |
| sympy_str               | 185 ms                                                      | 182 ms: 1.02x faster                                                       |
| bench_thread_pool       | 872 us                                                      | 858 us: 1.02x faster                                                       |
| go                      | 101 ms                                                      | 99.5 ms: 1.02x faster                                                      |
| regex_dna               | 116 ms                                                      | 114 ms: 1.02x faster                                                       |
| pickle_list             | 2.70 us                                                     | 2.65 us: 1.02x faster                                                      |
| deltablue               | 2.70 ms                                                     | 2.66 ms: 1.01x faster                                                      |
| coroutines              | 15.0 ms                                                     | 14.8 ms: 1.01x faster                                                      |
| telco                   | 4.06 ms                                                     | 4.02 ms: 1.01x faster                                                      |
| sqlalchemy_declarative  | 85.6 ms                                                     | 84.7 ms: 1.01x faster                                                      |
| nqueens                 | 68.3 ms                                                     | 67.6 ms: 1.01x faster                                                      |
| tornado_http            | 92.8 ms                                                     | 91.9 ms: 1.01x faster                                                      |
| float                   | 54.4 ms                                                     | 53.9 ms: 1.01x faster                                                      |
| fannkuch                | 253 ms                                                      | 251 ms: 1.01x faster                                                       |
| meteor_contest          | 75.2 ms                                                     | 74.8 ms: 1.01x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 18.4 us: 1.00x faster                                                      |
| scimark_sor             | 78.1 ms                                                     | 78.5 ms: 1.00x slower                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 34.8 ms: 1.01x slower                                                      |
| comprehensions          | 15.6 us                                                     | 15.7 us: 1.01x slower                                                      |
| chaos                   | 48.4 ms                                                     | 48.7 ms: 1.01x slower                                                      |
| logging_silent          | 71.8 ns                                                     | 72.4 ns: 1.01x slower                                                      |
| sqlglot_normalize       | 190 ms                                                      | 192 ms: 1.01x slower                                                       |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| richards                | 31.4 ms                                                     | 31.7 ms: 1.01x slower                                                      |
| hexiom                  | 4.55 ms                                                     | 4.61 ms: 1.01x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 37.8 ms: 1.02x slower                                                      |
| xml_etree_generate      | 52.5 ms                                                     | 53.4 ms: 1.02x slower                                                      |
| pathlib                 | 70.9 ms                                                     | 72.4 ms: 1.02x slower                                                      |
| django_template         | 24.4 ms                                                     | 25.0 ms: 1.02x slower                                                      |
| crypto_pyaes            | 48.9 ms                                                     | 50.6 ms: 1.04x slower                                                      |
| scimark_fft             | 179 ms                                                      | 186 ms: 1.04x slower                                                       |
| deepcopy_reduce         | 2.06 us                                                     | 2.14 us: 1.04x slower                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 2.68 ms: 1.04x slower                                                      |
| mdp                     | 1.59 sec                                                    | 1.67 sec: 1.05x slower                                                     |
| thrift                  | 494 us                                                      | 518 us: 1.05x slower                                                       |
| spectral_norm           | 68.3 ms                                                     | 73.7 ms: 1.08x slower                                                      |
| unpickle_list           | 2.59 us                                                     | 2.80 us: 1.08x slower                                                      |
| json_loads              | 13.0 us                                                     | 14.1 us: 1.08x slower                                                      |
| unpickle                | 7.57 us                                                     | 8.32 us: 1.10x slower                                                      |
| json                    | 2.98 ms                                                     | 3.32 ms: 1.12x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.70 ms: 1.13x slower                                                      |
| coverage                | 43.4 ms                                                     | 54.1 ms: 1.25x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.01x faster                                                               |

Benchmark hidden because not significant (10): pylint, dask, deepcopy, sqlalchemy_imperative, regex_compile, scimark_lu, generators, html5lib, async_generators, logging_format
Ignored benchmarks (9) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.99% likely to be faster
- 90% likely to have a speedup of 1.01x
- 95% likely to have a speedup of 1.01x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: unknown