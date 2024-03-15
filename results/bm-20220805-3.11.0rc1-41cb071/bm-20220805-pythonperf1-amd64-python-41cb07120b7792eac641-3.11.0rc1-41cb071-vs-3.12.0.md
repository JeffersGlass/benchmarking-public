
# Results vs. 3.12.0

- fork: python
- ref: 41cb07120b7792eac641
- machine: windows-amd64
- commit hash: 41cb071
- commit date: 2022-08-05
- overall geometric mean: 1.02x slower \*
- HPT reliability: 90.74%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 202 ms: 1.08x faster                                                        |
| chameleon      | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 90.9 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io          | 731 ms                                                      | 739 ms: 1.01x slower                                                        |
| async_tree_none        | 291 ms                                                      | 310 ms: 1.06x slower                                                        |
| async_tree_memoization | 339 ms                                                      | 368 ms: 1.09x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 52.9 ms: 1.07x faster                                                       |
| nbody          | 71.9 ms                                                     | 68.3 ms: 1.05x faster                                                       |
| pidigits       | 152 ms                                                      | 146 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 123 ms: 1.03x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 14.1 ms: 1.01x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 89.4 ms: 1.02x slower                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.66 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.00x slower                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.44 us: 1.15x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.57 us: 1.10x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.64 us: 1.04x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.9 ms: 1.04x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                                       |
| unpickle             | 8.18 us                                                     | 8.11 us: 1.01x faster                                                       |
| json_loads           | 13.9 us                                                     | 14.0 us: 1.01x slower                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 94.8 ms: 1.02x slower                                                       |
| pickle_pure_python   | 195 us                                                      | 202 us: 1.03x slower                                                        |
| unpickle_pure_python | 133 us                                                      | 150 us: 1.13x slower                                                        |
| json_dumps           | 5.70 ms                                                     | 7.73 ms: 1.36x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                                |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                       |
| python_startup         | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.26 ms: 1.02x slower                                                       |
| django_template | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                                       |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071 |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 176 ms: 1.36x faster                                                        |
| pickle                  | 7.43 us                                                     | 6.44 us: 1.15x faster                                                       |
| create_gc_cycles        | 752 us                                                      | 665 us: 1.13x faster                                                        |
| bench_mp_pool           | 69.2 ms                                                     | 61.4 ms: 1.13x faster                                                       |
| pathlib                 | 80.5 ms                                                     | 72.6 ms: 1.11x faster                                                       |
| pickle_list             | 2.83 us                                                     | 2.57 us: 1.10x faster                                                       |
| gc_traversal            | 1.52 ms                                                     | 1.40 ms: 1.08x faster                                                       |
| 2to3                    | 218 ms                                                      | 202 ms: 1.08x faster                                                        |
| float                   | 56.8 ms                                                     | 52.9 ms: 1.07x faster                                                       |
| telco                   | 4.13 ms                                                     | 3.87 ms: 1.07x faster                                                       |
| python_startup_no_site  | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                       |
| xml_etree_generate      | 55.8 ms                                                     | 52.6 ms: 1.06x faster                                                       |
| python_startup          | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                       |
| nbody                   | 71.9 ms                                                     | 68.3 ms: 1.05x faster                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.68 us: 1.05x faster                                                       |
| docutils                | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                      |
| pidigits                | 152 ms                                                      | 146 ms: 1.04x faster                                                        |
| unpickle_list           | 2.75 us                                                     | 2.64 us: 1.04x faster                                                       |
| sqlalchemy_declarative  | 86.4 ms                                                     | 83.4 ms: 1.04x faster                                                       |
| xml_etree_iterparse     | 65.2 ms                                                     | 62.9 ms: 1.04x faster                                                       |
| json                    | 3.05 ms                                                     | 2.94 ms: 1.04x faster                                                       |
| aiohttp                 | 884 us                                                      | 861 us: 1.03x faster                                                        |
| regex_dna               | 126 ms                                                      | 123 ms: 1.03x faster                                                        |
| xml_etree_process       | 37.7 ms                                                     | 36.7 ms: 1.03x faster                                                       |
| dulwich_log             | 44.3 ms                                                     | 43.3 ms: 1.02x faster                                                       |
| deepcopy_reduce         | 2.09 us                                                     | 2.05 us: 1.02x faster                                                       |
| scimark_sor             | 78.8 ms                                                     | 77.3 ms: 1.02x faster                                                       |
| meteor_contest          | 74.6 ms                                                     | 73.3 ms: 1.02x faster                                                       |
| pycparser               | 699 ms                                                      | 689 ms: 1.01x faster                                                        |
| scimark_fft             | 184 ms                                                      | 182 ms: 1.01x faster                                                        |
| regex_v8                | 14.2 ms                                                     | 14.1 ms: 1.01x faster                                                       |
| unpickle                | 8.18 us                                                     | 8.11 us: 1.01x faster                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 48.7 ms: 1.01x slower                                                       |
| json_loads              | 13.9 us                                                     | 14.0 us: 1.01x slower                                                       |
| async_tree_io           | 731 ms                                                      | 739 ms: 1.01x slower                                                        |
| sqlglot_normalize       | 187 ms                                                      | 189 ms: 1.01x slower                                                        |
| chameleon               | 4.98 ms                                                     | 5.05 ms: 1.01x slower                                                       |
| tornado_http            | 89.5 ms                                                     | 90.9 ms: 1.02x slower                                                       |
| scimark_monte_carlo     | 43.7 ms                                                     | 44.4 ms: 1.02x slower                                                       |
| logging_simple          | 6.28 us                                                     | 6.37 us: 1.02x slower                                                       |
| dask                    | 263 ms                                                      | 267 ms: 1.02x slower                                                        |
| xml_etree_parse         | 93.0 ms                                                     | 94.8 ms: 1.02x slower                                                       |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.61 ms: 1.02x slower                                                       |
| regex_compile           | 87.5 ms                                                     | 89.4 ms: 1.02x slower                                                       |
| sympy_expand            | 284 ms                                                      | 290 ms: 1.02x slower                                                        |
| nqueens                 | 62.8 ms                                                     | 64.2 ms: 1.02x slower                                                       |
| mako                    | 7.09 ms                                                     | 7.26 ms: 1.02x slower                                                       |
| regex_effbot            | 1.62 ms                                                     | 1.66 ms: 1.03x slower                                                       |
| pyflate                 | 295 ms                                                      | 303 ms: 1.03x slower                                                        |
| logging_format          | 6.72 us                                                     | 6.90 us: 1.03x slower                                                       |
| sympy_str               | 175 ms                                                      | 180 ms: 1.03x slower                                                        |
| pickle_pure_python      | 195 us                                                      | 202 us: 1.03x slower                                                        |
| django_template         | 22.9 ms                                                     | 23.7 ms: 1.03x slower                                                       |
| coroutines              | 14.3 ms                                                     | 14.8 ms: 1.04x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 13.5 ms: 1.04x slower                                                       |
| raytrace                | 192 ms                                                      | 204 ms: 1.06x slower                                                        |
| sympy_sum               | 91.5 ms                                                     | 97.0 ms: 1.06x slower                                                       |
| async_tree_none         | 291 ms                                                      | 310 ms: 1.06x slower                                                        |
| deepcopy_memo           | 23.7 us                                                     | 25.3 us: 1.07x slower                                                       |
| spectral_norm           | 66.9 ms                                                     | 71.8 ms: 1.07x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.2 us: 1.08x slower                                                       |
| scimark_lu              | 58.9 ms                                                     | 63.7 ms: 1.08x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 368 ms: 1.09x slower                                                        |
| hexiom                  | 4.10 ms                                                     | 4.46 ms: 1.09x slower                                                       |
| go                      | 91.6 ms                                                     | 101 ms: 1.10x slower                                                        |
| richards                | 28.4 ms                                                     | 31.3 ms: 1.10x slower                                                       |
| sqlglot_transpile       | 1.02 ms                                                     | 1.13 ms: 1.11x slower                                                       |
| unpack_sequence         | 37.5 ns                                                     | 41.9 ns: 1.12x slower                                                       |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.4 ms: 1.12x slower                                                       |
| unpickle_pure_python    | 133 us                                                      | 150 us: 1.13x slower                                                        |
| chaos                   | 43.3 ms                                                     | 49.6 ms: 1.15x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 925 us: 1.15x slower                                                        |
| mdp                     | 1.37 sec                                                    | 1.60 sec: 1.17x slower                                                      |
| logging_silent          | 60.5 ns                                                     | 71.9 ns: 1.19x slower                                                       |
| deltablue               | 2.16 ms                                                     | 2.63 ms: 1.22x slower                                                       |
| coverage                | 40.8 ms                                                     | 53.6 ms: 1.31x slower                                                       |
| asyncio_tcp             | 487 ms                                                      | 659 ms: 1.35x slower                                                        |
| json_dumps              | 5.70 ms                                                     | 7.73 ms: 1.36x slower                                                       |
| generators              | 22.5 ms                                                     | 33.8 ms: 1.50x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (8): bench_thread_pool, pprint_pformat, sqlglot_optimize, pprint_safe_repr, pickle_dict, deepcopy, fannkuch, async_tree_cpu_io_mixed
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220805-3.11.0rc1-41cb071/bm-20220805-pythonperf1-amd64-python-41cb07120b7792eac641-3.11.0rc1-41cb071.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 90.74% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown