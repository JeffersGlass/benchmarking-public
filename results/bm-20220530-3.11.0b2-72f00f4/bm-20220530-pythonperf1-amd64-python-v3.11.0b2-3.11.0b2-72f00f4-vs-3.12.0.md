
# Results vs. 3.12.0

- fork: python
- ref: v3.11.0b2
- machine: windows-amd64
- commit hash: 72f00f4
- commit date: 2022-05-30
- overall geometric mean: 1.08x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 211 ms: 1.03x faster                                            |
| chameleon      | 4.98 ms                                                     | 5.59 ms: 1.12x slower                                           |
| tornado_http   | 89.5 ms                                                     | 95.3 ms: 1.06x slower                                           |
| Geometric mean | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): docutils

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 520 ms: 1.06x slower                                            |
| async_tree_io           | 731 ms                                                      | 794 ms: 1.09x slower                                            |
| async_tree_none         | 291 ms                                                      | 336 ms: 1.15x slower                                            |
| async_tree_memoization  | 339 ms                                                      | 400 ms: 1.18x slower                                            |
| Geometric mean          | (ref)                                                       | 1.12x slower                                                    |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 54.5 ms: 1.04x faster                                           |
| nbody          | 71.9 ms                                                     | 70.1 ms: 1.03x faster                                           |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmark hidden because not significant (1): pidigits

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.39 ms: 1.17x faster                                           |
| regex_dna      | 126 ms                                                      | 120 ms: 1.06x faster                                            |
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                           |
| regex_compile  | 87.5 ms                                                     | 97.0 ms: 1.11x slower                                           |
| Geometric mean | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.74 us: 1.10x faster                                           |
| pickle_list          | 2.83 us                                                     | 2.64 us: 1.07x faster                                           |
| pickle_dict          | 18.4 us                                                     | 17.4 us: 1.06x faster                                           |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.0 ms: 1.05x faster                                           |
| xml_etree_generate   | 55.8 ms                                                     | 54.1 ms: 1.03x faster                                           |
| unpickle             | 8.18 us                                                     | 8.07 us: 1.01x faster                                           |
| json_loads           | 13.9 us                                                     | 14.1 us: 1.01x slower                                           |
| xml_etree_process    | 37.7 ms                                                     | 39.1 ms: 1.04x slower                                           |
| xml_etree_parse      | 93.0 ms                                                     | 96.7 ms: 1.04x slower                                           |
| pickle_pure_python   | 195 us                                                      | 216 us: 1.11x slower                                            |
| unpickle_pure_python | 133 us                                                      | 164 us: 1.23x slower                                            |
| json_dumps           | 5.70 ms                                                     | 8.21 ms: 1.44x slower                                           |
| Geometric mean       | (ref)                                                       | 1.04x slower                                                    |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.8 ms: 1.03x faster                                           |
| python_startup         | 19.5 ms                                                     | 19.0 ms: 1.02x faster                                           |
| Geometric mean         | (ref)                                                       | 1.02x faster                                                    |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.62 ms: 1.07x slower                                           |
| django_template | 22.9 ms                                                     | 25.1 ms: 1.09x slower                                           |
| Geometric mean  | (ref)                                                       | 1.08x slower                                                    |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 187 ms: 1.28x faster                                            |
| regex_effbot            | 1.62 ms                                                     | 1.39 ms: 1.17x faster                                           |
| create_gc_cycles        | 752 us                                                      | 675 us: 1.11x faster                                            |
| pickle                  | 7.43 us                                                     | 6.74 us: 1.10x faster                                           |
| bench_mp_pool           | 69.2 ms                                                     | 63.3 ms: 1.09x faster                                           |
| pathlib                 | 80.5 ms                                                     | 74.8 ms: 1.08x faster                                           |
| pickle_list             | 2.83 us                                                     | 2.64 us: 1.07x faster                                           |
| pickle_dict             | 18.4 us                                                     | 17.4 us: 1.06x faster                                           |
| regex_dna               | 126 ms                                                      | 120 ms: 1.06x faster                                            |
| logging_simple          | 6.28 us                                                     | 5.94 us: 1.06x faster                                           |
| xml_etree_iterparse     | 65.2 ms                                                     | 62.0 ms: 1.05x faster                                           |
| logging_format          | 6.72 us                                                     | 6.39 us: 1.05x faster                                           |
| gc_traversal            | 1.52 ms                                                     | 1.46 ms: 1.05x faster                                           |
| float                   | 56.8 ms                                                     | 54.5 ms: 1.04x faster                                           |
| sqlalchemy_declarative  | 86.4 ms                                                     | 83.2 ms: 1.04x faster                                           |
| 2to3                    | 218 ms                                                      | 211 ms: 1.03x faster                                            |
| xml_etree_generate      | 55.8 ms                                                     | 54.1 ms: 1.03x faster                                           |
| sqlite_synth            | 1.76 us                                                     | 1.71 us: 1.03x faster                                           |
| python_startup_no_site  | 16.2 ms                                                     | 15.8 ms: 1.03x faster                                           |
| nbody                   | 71.9 ms                                                     | 70.1 ms: 1.03x faster                                           |
| python_startup          | 19.5 ms                                                     | 19.0 ms: 1.02x faster                                           |
| telco                   | 4.13 ms                                                     | 4.05 ms: 1.02x faster                                           |
| unpickle                | 8.18 us                                                     | 8.07 us: 1.01x faster                                           |
| json_loads              | 13.9 us                                                     | 14.1 us: 1.01x slower                                           |
| regex_v8                | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                           |
| scimark_sor             | 78.8 ms                                                     | 80.0 ms: 1.02x slower                                           |
| scimark_fft             | 184 ms                                                      | 191 ms: 1.03x slower                                            |
| xml_etree_process       | 37.7 ms                                                     | 39.1 ms: 1.04x slower                                           |
| bench_thread_pool       | 857 us                                                      | 889 us: 1.04x slower                                            |
| xml_etree_parse         | 93.0 ms                                                     | 96.7 ms: 1.04x slower                                           |
| dulwich_log             | 44.3 ms                                                     | 46.1 ms: 1.04x slower                                           |
| aiohttp                 | 884 us                                                      | 921 us: 1.04x slower                                            |
| deepcopy_reduce         | 2.09 us                                                     | 2.19 us: 1.05x slower                                           |
| scimark_monte_carlo     | 43.7 ms                                                     | 46.0 ms: 1.05x slower                                           |
| spectral_norm           | 66.9 ms                                                     | 70.6 ms: 1.06x slower                                           |
| meteor_contest          | 74.6 ms                                                     | 78.7 ms: 1.06x slower                                           |
| json                    | 3.05 ms                                                     | 3.23 ms: 1.06x slower                                           |
| async_tree_cpu_io_mixed | 489 ms                                                      | 520 ms: 1.06x slower                                            |
| pprint_pformat          | 1.05 sec                                                    | 1.11 sec: 1.06x slower                                          |
| tornado_http            | 89.5 ms                                                     | 95.3 ms: 1.06x slower                                           |
| pyflate                 | 295 ms                                                      | 314 ms: 1.07x slower                                            |
| pprint_safe_repr        | 513 ms                                                      | 548 ms: 1.07x slower                                            |
| dask                    | 263 ms                                                      | 280 ms: 1.07x slower                                            |
| crypto_pyaes            | 48.5 ms                                                     | 51.8 ms: 1.07x slower                                           |
| pycparser               | 699 ms                                                      | 750 ms: 1.07x slower                                            |
| mako                    | 7.09 ms                                                     | 7.62 ms: 1.07x slower                                           |
| fannkuch                | 247 ms                                                      | 266 ms: 1.08x slower                                            |
| sqlglot_normalize       | 187 ms                                                      | 203 ms: 1.08x slower                                            |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.77 ms: 1.08x slower                                           |
| sympy_str               | 175 ms                                                      | 190 ms: 1.08x slower                                            |
| sqlglot_optimize        | 34.5 ms                                                     | 37.5 ms: 1.09x slower                                           |
| async_tree_io           | 731 ms                                                      | 794 ms: 1.09x slower                                            |
| django_template         | 22.9 ms                                                     | 25.1 ms: 1.09x slower                                           |
| coroutines              | 14.3 ms                                                     | 15.6 ms: 1.09x slower                                           |
| go                      | 91.6 ms                                                     | 100 ms: 1.09x slower                                            |
| deepcopy                | 238 us                                                      | 261 us: 1.10x slower                                            |
| nqueens                 | 62.8 ms                                                     | 68.9 ms: 1.10x slower                                           |
| scimark_lu              | 58.9 ms                                                     | 64.6 ms: 1.10x slower                                           |
| sympy_integrate         | 13.0 ms                                                     | 14.2 ms: 1.10x slower                                           |
| sympy_expand            | 284 ms                                                      | 312 ms: 1.10x slower                                            |
| deepcopy_memo           | 23.7 us                                                     | 26.1 us: 1.10x slower                                           |
| pickle_pure_python      | 195 us                                                      | 216 us: 1.11x slower                                            |
| regex_compile           | 87.5 ms                                                     | 97.0 ms: 1.11x slower                                           |
| raytrace                | 192 ms                                                      | 213 ms: 1.11x slower                                            |
| richards                | 28.4 ms                                                     | 31.6 ms: 1.11x slower                                           |
| chameleon               | 4.98 ms                                                     | 5.59 ms: 1.12x slower                                           |
| sympy_sum               | 91.5 ms                                                     | 103 ms: 1.12x slower                                            |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.5 ms: 1.13x slower                                           |
| async_tree_none         | 291 ms                                                      | 336 ms: 1.15x slower                                            |
| async_tree_memoization  | 339 ms                                                      | 400 ms: 1.18x slower                                            |
| hexiom                  | 4.10 ms                                                     | 4.84 ms: 1.18x slower                                           |
| unpack_sequence         | 37.5 ns                                                     | 44.3 ns: 1.18x slower                                           |
| logging_silent          | 60.5 ns                                                     | 72.2 ns: 1.19x slower                                           |
| chaos                   | 43.3 ms                                                     | 51.8 ms: 1.20x slower                                           |
| unpickle_pure_python    | 133 us                                                      | 164 us: 1.23x slower                                            |
| deltablue               | 2.16 ms                                                     | 2.72 ms: 1.26x slower                                           |
| mdp                     | 1.37 sec                                                    | 1.75 sec: 1.28x slower                                          |
| comprehensions          | 14.1 us                                                     | 18.2 us: 1.29x slower                                           |
| sqlglot_transpile       | 1.02 ms                                                     | 1.42 ms: 1.39x slower                                           |
| json_dumps              | 5.70 ms                                                     | 8.21 ms: 1.44x slower                                           |
| sqlglot_parse           | 804 us                                                      | 1.21 ms: 1.50x slower                                           |
| asyncio_tcp             | 487 ms                                                      | 742 ms: 1.52x slower                                            |
| generators              | 22.5 ms                                                     | 35.7 ms: 1.59x slower                                           |
| coverage                | 40.8 ms                                                     | 106 ms: 2.59x slower                                            |
| Geometric mean          | (ref)                                                       | 1.08x slower                                                    |

Benchmark hidden because not significant (3): docutils, unpickle_list, pidigits
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20220530-3.11.0b2-72f00f4/bm-20220530-pythonperf1-amd64-python-v3.11.0b2-3.11.0b2-72f00f4.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.06x
- 95% likely to have a slowdown of 1.06x
- 99% likely to have a slowdown of 1.04x


# Memory

- memory change: unknown