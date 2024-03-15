
# Results vs. 3.12.0

- fork: python
- ref: ed7c3ff15680c1939fad
- machine: windows-amd64
- commit hash: ed7c3ff
- commit date: 2022-09-11
- overall geometric mean: 1.02x slower \*
- HPT reliability: 87.08%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 202 ms: 1.08x faster                                                        |
| chameleon      | 4.98 ms                                                     | 5.09 ms: 1.02x slower                                                       |
| docutils       | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| tornado_http   | 89.5 ms                                                     | 92.1 ms: 1.03x slower                                                       |
| Geometric mean | (ref)                                                       | 1.02x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_io          | 731 ms                                                      | 740 ms: 1.01x slower                                                        |
| async_tree_none        | 291 ms                                                      | 310 ms: 1.06x slower                                                        |
| async_tree_memoization | 339 ms                                                      | 368 ms: 1.09x slower                                                        |
| Geometric mean         | (ref)                                                       | 1.04x slower                                                                |

Benchmark hidden because not significant (1): async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                                       |
| nbody          | 71.9 ms                                                     | 68.6 ms: 1.05x faster                                                       |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| Geometric mean | (ref)                                                       | 1.05x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 115 ms: 1.10x faster                                                        |
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                       |
| regex_compile  | 87.5 ms                                                     | 89.5 ms: 1.02x slower                                                       |
| Geometric mean | (ref)                                                       | 1.04x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|----------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.60 us: 1.13x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 51.2 ms: 1.09x faster                                                       |
| unpickle_list        | 2.75 us                                                     | 2.55 us: 1.08x faster                                                       |
| pickle_list          | 2.83 us                                                     | 2.65 us: 1.07x faster                                                       |
| unpickle             | 8.18 us                                                     | 7.70 us: 1.06x faster                                                       |
| xml_etree_iterparse  | 65.2 ms                                                     | 61.9 ms: 1.05x faster                                                       |
| xml_etree_process    | 37.7 ms                                                     | 35.9 ms: 1.05x faster                                                       |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| xml_etree_parse      | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                                       |
| pickle_dict          | 18.4 us                                                     | 18.2 us: 1.01x faster                                                       |
| pickle_pure_python   | 195 us                                                      | 197 us: 1.01x slower                                                        |
| unpickle_pure_python | 133 us                                                      | 149 us: 1.12x slower                                                        |
| json_dumps           | 5.70 ms                                                     | 7.66 ms: 1.35x slower                                                       |
| Geometric mean       | (ref)                                                       | 1.01x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                                       |
| python_startup         | 19.5 ms                                                     | 18.5 ms: 1.05x faster                                                       |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-----------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                       |
| django_template | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                       |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                                |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff |
|-------------------------|:-----------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 176 ms: 1.36x faster                                                        |
| bench_mp_pool           | 69.2 ms                                                     | 61.2 ms: 1.13x faster                                                       |
| create_gc_cycles        | 752 us                                                      | 667 us: 1.13x faster                                                        |
| pickle                  | 7.43 us                                                     | 6.60 us: 1.13x faster                                                       |
| pathlib                 | 80.5 ms                                                     | 72.1 ms: 1.12x faster                                                       |
| regex_dna               | 126 ms                                                      | 115 ms: 1.10x faster                                                        |
| xml_etree_generate      | 55.8 ms                                                     | 51.2 ms: 1.09x faster                                                       |
| gc_traversal            | 1.52 ms                                                     | 1.41 ms: 1.08x faster                                                       |
| 2to3                    | 218 ms                                                      | 202 ms: 1.08x faster                                                        |
| unpickle_list           | 2.75 us                                                     | 2.55 us: 1.08x faster                                                       |
| pickle_list             | 2.83 us                                                     | 2.65 us: 1.07x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.06x faster                                                       |
| unpickle                | 8.18 us                                                     | 7.70 us: 1.06x faster                                                       |
| python_startup_no_site  | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                                       |
| sqlalchemy_declarative  | 86.4 ms                                                     | 81.7 ms: 1.06x faster                                                       |
| telco                   | 4.13 ms                                                     | 3.91 ms: 1.06x faster                                                       |
| docutils                | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                      |
| float                   | 56.8 ms                                                     | 53.9 ms: 1.05x faster                                                       |
| xml_etree_iterparse     | 65.2 ms                                                     | 61.9 ms: 1.05x faster                                                       |
| python_startup          | 19.5 ms                                                     | 18.5 ms: 1.05x faster                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.67 us: 1.05x faster                                                       |
| xml_etree_process       | 37.7 ms                                                     | 35.9 ms: 1.05x faster                                                       |
| nbody                   | 71.9 ms                                                     | 68.6 ms: 1.05x faster                                                       |
| deepcopy_reduce         | 2.09 us                                                     | 2.00 us: 1.04x faster                                                       |
| pidigits                | 152 ms                                                      | 147 ms: 1.04x faster                                                        |
| aiohttp                 | 884 us                                                      | 857 us: 1.03x faster                                                        |
| pycparser               | 699 ms                                                      | 683 ms: 1.02x faster                                                        |
| scimark_sor             | 78.8 ms                                                     | 77.3 ms: 1.02x faster                                                       |
| json_loads              | 13.9 us                                                     | 13.7 us: 1.02x faster                                                       |
| xml_etree_parse         | 93.0 ms                                                     | 91.6 ms: 1.02x faster                                                       |
| dulwich_log             | 44.3 ms                                                     | 43.6 ms: 1.02x faster                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 34.0 ms: 1.01x faster                                                       |
| regex_effbot            | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                       |
| pickle_dict             | 18.4 us                                                     | 18.2 us: 1.01x faster                                                       |
| sqlglot_normalize       | 187 ms                                                      | 186 ms: 1.01x faster                                                        |
| meteor_contest          | 74.6 ms                                                     | 74.3 ms: 1.00x faster                                                       |
| pprint_pformat          | 1.05 sec                                                    | 1.05 sec: 1.01x slower                                                      |
| pickle_pure_python      | 195 us                                                      | 197 us: 1.01x slower                                                        |
| async_tree_io           | 731 ms                                                      | 740 ms: 1.01x slower                                                        |
| dask                    | 263 ms                                                      | 267 ms: 1.02x slower                                                        |
| scimark_monte_carlo     | 43.7 ms                                                     | 44.6 ms: 1.02x slower                                                       |
| mako                    | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                       |
| chameleon               | 4.98 ms                                                     | 5.09 ms: 1.02x slower                                                       |
| regex_compile           | 87.5 ms                                                     | 89.5 ms: 1.02x slower                                                       |
| pyflate                 | 295 ms                                                      | 303 ms: 1.03x slower                                                        |
| scimark_fft             | 184 ms                                                      | 189 ms: 1.03x slower                                                        |
| tornado_http            | 89.5 ms                                                     | 92.1 ms: 1.03x slower                                                       |
| nqueens                 | 62.8 ms                                                     | 64.6 ms: 1.03x slower                                                       |
| sympy_expand            | 284 ms                                                      | 294 ms: 1.03x slower                                                        |
| logging_format          | 6.72 us                                                     | 6.97 us: 1.04x slower                                                       |
| fannkuch                | 247 ms                                                      | 256 ms: 1.04x slower                                                        |
| django_template         | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                       |
| sympy_str               | 175 ms                                                      | 182 ms: 1.04x slower                                                        |
| coroutines              | 14.3 ms                                                     | 14.9 ms: 1.04x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 13.5 ms: 1.05x slower                                                       |
| logging_simple          | 6.28 us                                                     | 6.57 us: 1.05x slower                                                       |
| async_tree_none         | 291 ms                                                      | 310 ms: 1.06x slower                                                        |
| go                      | 91.6 ms                                                     | 97.5 ms: 1.06x slower                                                       |
| deepcopy_memo           | 23.7 us                                                     | 25.4 us: 1.07x slower                                                       |
| sympy_sum               | 91.5 ms                                                     | 98.2 ms: 1.07x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.2 us: 1.07x slower                                                       |
| scimark_lu              | 58.9 ms                                                     | 63.4 ms: 1.08x slower                                                       |
| richards                | 28.4 ms                                                     | 30.6 ms: 1.08x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 368 ms: 1.09x slower                                                        |
| hexiom                  | 4.10 ms                                                     | 4.48 ms: 1.09x slower                                                       |
| spectral_norm           | 66.9 ms                                                     | 73.2 ms: 1.09x slower                                                       |
| raytrace                | 192 ms                                                      | 211 ms: 1.10x slower                                                        |
| sqlglot_transpile       | 1.02 ms                                                     | 1.12 ms: 1.10x slower                                                       |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.81 ms: 1.10x slower                                                       |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.3 ms: 1.10x slower                                                       |
| chaos                   | 43.3 ms                                                     | 48.0 ms: 1.11x slower                                                       |
| unpickle_pure_python    | 133 us                                                      | 149 us: 1.12x slower                                                        |
| unpack_sequence         | 37.5 ns                                                     | 42.7 ns: 1.14x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 920 us: 1.14x slower                                                        |
| mdp                     | 1.37 sec                                                    | 1.59 sec: 1.16x slower                                                      |
| logging_silent          | 60.5 ns                                                     | 70.9 ns: 1.17x slower                                                       |
| deltablue               | 2.16 ms                                                     | 2.61 ms: 1.21x slower                                                       |
| coverage                | 40.8 ms                                                     | 53.2 ms: 1.30x slower                                                       |
| json_dumps              | 5.70 ms                                                     | 7.66 ms: 1.35x slower                                                       |
| asyncio_tcp             | 487 ms                                                      | 688 ms: 1.41x slower                                                        |
| generators              | 22.5 ms                                                     | 33.5 ms: 1.49x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                                |

Benchmark hidden because not significant (6): bench_thread_pool, async_tree_cpu_io_mixed, pprint_safe_repr, crypto_pyaes, deepcopy, json
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220911-3.11.0rc2-ed7c3ff/bm-20220911-pythonperf1-amd64-python-ed7c3ff15680c1939fad-3.11.0rc2-ed7c3ff.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 87.08% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown