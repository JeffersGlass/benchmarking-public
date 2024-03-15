
# Results vs. 3.12.0

- fork: python
- ref: f3909b8bc83675b7ab09
- machine: windows-amd64
- commit hash: f3909b8
- commit date: 2023-04-04
- overall geometric mean: 1.03x slower \*
- HPT reliability: 96.99%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 206 ms: 1.06x faster                                                     |
| chameleon      | 4.98 ms                                                     | 5.27 ms: 1.06x slower                                                    |
| docutils       | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                   |
| Geometric mean | (ref)                                                       | 1.01x faster                                                             |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 500 ms: 1.02x slower                                                     |
| async_tree_none         | 291 ms                                                      | 314 ms: 1.08x slower                                                     |
| async_tree_memoization  | 339 ms                                                      | 368 ms: 1.08x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.05x slower                                                             |

Benchmark hidden because not significant (1): async_tree_io

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 52.6 ms: 1.08x faster                                                    |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                     |
| nbody          | 71.9 ms                                                     | 69.8 ms: 1.03x faster                                                    |
| Geometric mean | (ref)                                                       | 1.05x faster                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 120 ms: 1.05x faster                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                    |
| regex_compile  | 87.5 ms                                                     | 89.7 ms: 1.02x slower                                                    |
| Geometric mean | (ref)                                                       | 1.01x faster                                                             |

Benchmark hidden because not significant (1): regex_v8

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.73 us: 1.11x faster                                                    |
| xml_etree_generate   | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                                    |
| json_loads           | 13.9 us                                                     | 13.0 us: 1.07x faster                                                    |
| xml_etree_iterparse  | 65.2 ms                                                     | 61.4 ms: 1.06x faster                                                    |
| xml_etree_process    | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                    |
| unpickle_list        | 2.75 us                                                     | 2.68 us: 1.03x faster                                                    |
| unpickle             | 8.18 us                                                     | 7.97 us: 1.03x faster                                                    |
| xml_etree_parse      | 93.0 ms                                                     | 91.3 ms: 1.02x faster                                                    |
| pickle_list          | 2.83 us                                                     | 2.78 us: 1.02x faster                                                    |
| pickle_pure_python   | 195 us                                                      | 198 us: 1.01x slower                                                     |
| unpickle_pure_python | 133 us                                                      | 150 us: 1.12x slower                                                     |
| json_dumps           | 5.70 ms                                                     | 7.60 ms: 1.34x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                             |

Benchmark hidden because not significant (1): pickle_dict

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                                    |
| python_startup         | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                    |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                    |
| django_template | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                    |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                             |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8 |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 176 ms: 1.36x faster                                                     |
| create_gc_cycles        | 752 us                                                      | 664 us: 1.13x faster                                                     |
| bench_mp_pool           | 69.2 ms                                                     | 62.0 ms: 1.12x faster                                                    |
| pickle                  | 7.43 us                                                     | 6.73 us: 1.11x faster                                                    |
| pathlib                 | 80.5 ms                                                     | 73.2 ms: 1.10x faster                                                    |
| float                   | 56.8 ms                                                     | 52.6 ms: 1.08x faster                                                    |
| xml_etree_generate      | 55.8 ms                                                     | 51.8 ms: 1.08x faster                                                    |
| json_loads              | 13.9 us                                                     | 13.0 us: 1.07x faster                                                    |
| gc_traversal            | 1.52 ms                                                     | 1.43 ms: 1.07x faster                                                    |
| sqlalchemy_declarative  | 86.4 ms                                                     | 81.1 ms: 1.06x faster                                                    |
| xml_etree_iterparse     | 65.2 ms                                                     | 61.4 ms: 1.06x faster                                                    |
| python_startup_no_site  | 16.2 ms                                                     | 15.3 ms: 1.06x faster                                                    |
| python_startup          | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                    |
| 2to3                    | 218 ms                                                      | 206 ms: 1.06x faster                                                     |
| regex_dna               | 126 ms                                                      | 120 ms: 1.05x faster                                                     |
| docutils                | 1.66 sec                                                    | 1.58 sec: 1.05x faster                                                   |
| scimark_sor             | 78.8 ms                                                     | 75.2 ms: 1.05x faster                                                    |
| dulwich_log             | 44.3 ms                                                     | 42.5 ms: 1.04x faster                                                    |
| sqlite_synth            | 1.76 us                                                     | 1.69 us: 1.04x faster                                                    |
| xml_etree_process       | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                    |
| pidigits                | 152 ms                                                      | 147 ms: 1.04x faster                                                     |
| aiohttp                 | 884 us                                                      | 857 us: 1.03x faster                                                     |
| regex_effbot            | 1.62 ms                                                     | 1.57 ms: 1.03x faster                                                    |
| nbody                   | 71.9 ms                                                     | 69.8 ms: 1.03x faster                                                    |
| unpickle_list           | 2.75 us                                                     | 2.68 us: 1.03x faster                                                    |
| deepcopy_reduce         | 2.09 us                                                     | 2.04 us: 1.03x faster                                                    |
| unpickle                | 8.18 us                                                     | 7.97 us: 1.03x faster                                                    |
| telco                   | 4.13 ms                                                     | 4.02 ms: 1.03x faster                                                    |
| xml_etree_parse         | 93.0 ms                                                     | 91.3 ms: 1.02x faster                                                    |
| pickle_list             | 2.83 us                                                     | 2.78 us: 1.02x faster                                                    |
| crypto_pyaes            | 48.5 ms                                                     | 48.2 ms: 1.01x faster                                                    |
| sqlglot_optimize        | 34.5 ms                                                     | 34.7 ms: 1.00x slower                                                    |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.58 ms: 1.01x slower                                                    |
| spectral_norm           | 66.9 ms                                                     | 67.6 ms: 1.01x slower                                                    |
| pickle_pure_python      | 195 us                                                      | 198 us: 1.01x slower                                                     |
| pprint_pformat          | 1.05 sec                                                    | 1.06 sec: 1.02x slower                                                   |
| mako                    | 7.09 ms                                                     | 7.22 ms: 1.02x slower                                                    |
| deepcopy                | 238 us                                                      | 243 us: 1.02x slower                                                     |
| sympy_expand            | 284 ms                                                      | 290 ms: 1.02x slower                                                     |
| async_tree_cpu_io_mixed | 489 ms                                                      | 500 ms: 1.02x slower                                                     |
| sqlglot_normalize       | 187 ms                                                      | 191 ms: 1.02x slower                                                     |
| pyflate                 | 295 ms                                                      | 301 ms: 1.02x slower                                                     |
| pprint_safe_repr        | 513 ms                                                      | 526 ms: 1.02x slower                                                     |
| regex_compile           | 87.5 ms                                                     | 89.7 ms: 1.02x slower                                                    |
| scimark_monte_carlo     | 43.7 ms                                                     | 45.1 ms: 1.03x slower                                                    |
| fannkuch                | 247 ms                                                      | 256 ms: 1.04x slower                                                     |
| sympy_str               | 175 ms                                                      | 182 ms: 1.04x slower                                                     |
| django_template         | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                    |
| logging_format          | 6.72 us                                                     | 6.99 us: 1.04x slower                                                    |
| nqueens                 | 62.8 ms                                                     | 65.6 ms: 1.04x slower                                                    |
| deepcopy_memo           | 23.7 us                                                     | 24.8 us: 1.05x slower                                                    |
| sympy_integrate         | 13.0 ms                                                     | 13.6 ms: 1.05x slower                                                    |
| raytrace                | 192 ms                                                      | 203 ms: 1.05x slower                                                     |
| chameleon               | 4.98 ms                                                     | 5.27 ms: 1.06x slower                                                    |
| coroutines              | 14.3 ms                                                     | 15.1 ms: 1.06x slower                                                    |
| logging_simple          | 6.28 us                                                     | 6.67 us: 1.06x slower                                                    |
| json                    | 3.05 ms                                                     | 3.25 ms: 1.07x slower                                                    |
| richards                | 28.4 ms                                                     | 30.4 ms: 1.07x slower                                                    |
| sympy_sum               | 91.5 ms                                                     | 98.4 ms: 1.07x slower                                                    |
| scimark_lu              | 58.9 ms                                                     | 63.3 ms: 1.08x slower                                                    |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.0 ms: 1.08x slower                                                    |
| async_tree_none         | 291 ms                                                      | 314 ms: 1.08x slower                                                     |
| go                      | 91.6 ms                                                     | 99.2 ms: 1.08x slower                                                    |
| async_tree_memoization  | 339 ms                                                      | 368 ms: 1.08x slower                                                     |
| comprehensions          | 14.1 us                                                     | 15.4 us: 1.09x slower                                                    |
| sqlglot_transpile       | 1.02 ms                                                     | 1.13 ms: 1.11x slower                                                    |
| hexiom                  | 4.10 ms                                                     | 4.56 ms: 1.11x slower                                                    |
| unpickle_pure_python    | 133 us                                                      | 150 us: 1.12x slower                                                     |
| chaos                   | 43.3 ms                                                     | 48.9 ms: 1.13x slower                                                    |
| sqlglot_parse           | 804 us                                                      | 931 us: 1.16x slower                                                     |
| logging_silent          | 60.5 ns                                                     | 70.1 ns: 1.16x slower                                                    |
| unpack_sequence         | 37.5 ns                                                     | 46.0 ns: 1.23x slower                                                    |
| deltablue               | 2.16 ms                                                     | 2.65 ms: 1.23x slower                                                    |
| mdp                     | 1.37 sec                                                    | 1.74 sec: 1.27x slower                                                   |
| coverage                | 40.8 ms                                                     | 53.2 ms: 1.30x slower                                                    |
| json_dumps              | 5.70 ms                                                     | 7.60 ms: 1.34x slower                                                    |
| asyncio_tcp             | 487 ms                                                      | 718 ms: 1.47x slower                                                     |
| generators              | 22.5 ms                                                     | 34.0 ms: 1.51x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.03x slower                                                             |

Benchmark hidden because not significant (9): bench_thread_pool, dask, meteor_contest, scimark_fft, regex_v8, pycparser, tornado_http, async_tree_io, pickle_dict
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230404-3.11.3-f3909b8/bm-20230404-pythonperf1-amd64-python-f3909b8bc83675b7ab09-3.11.3-f3909b8.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 96.99% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown