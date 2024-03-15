
# Results vs. 3.12.0

- fork: python
- ref: 8d32a5c8c4e9c90b0a21
- machine: windows-amd64
- commit hash: 8d32a5c
- commit date: 2022-05-06
- overall geometric mean: 1.04x slower \*
- HPT reliability: 99.60%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 203 ms: 1.07x faster                                                       |
| chameleon      | 4.98 ms                                                     | 5.45 ms: 1.09x slower                                                      |
| docutils       | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                     |
| Geometric mean | (ref)                                                       | 1.01x faster                                                               |

Benchmark hidden because not significant (1): tornado_http

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 499 ms: 1.02x slower                                                       |
| async_tree_io           | 731 ms                                                      | 751 ms: 1.03x slower                                                       |
| async_tree_none         | 291 ms                                                      | 311 ms: 1.07x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 370 ms: 1.09x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.05x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                      |
| nbody          | 71.9 ms                                                     | 67.9 ms: 1.06x faster                                                      |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.47 ms: 1.10x faster                                                      |
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                                      |
| regex_compile  | 87.5 ms                                                     | 90.5 ms: 1.03x slower                                                      |
| Geometric mean | (ref)                                                       | 1.03x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.59 us: 1.13x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 17.1 us: 1.08x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.58 us: 1.07x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 61.1 ms: 1.07x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.67 us: 1.06x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 53.0 ms: 1.05x faster                                                      |
| unpickle             | 8.18 us                                                     | 7.87 us: 1.04x faster                                                      |
| json_loads           | 13.9 us                                                     | 13.4 us: 1.04x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 37.6 ms: 1.00x faster                                                      |
| pickle_pure_python   | 195 us                                                      | 204 us: 1.04x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 152 us: 1.14x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 7.72 ms: 1.36x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.00x faster                                                               |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                      |
| python_startup         | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 24.0 ms: 1.05x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.03x slower                                                               |

Benchmark hidden because not significant (1): mako

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 182 ms: 1.31x faster                                                       |
| bench_mp_pool           | 69.2 ms                                                     | 60.6 ms: 1.14x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 663 us: 1.14x faster                                                       |
| pickle                  | 7.43 us                                                     | 6.59 us: 1.13x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 71.4 ms: 1.13x faster                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.47 ms: 1.10x faster                                                      |
| logging_simple          | 6.28 us                                                     | 5.80 us: 1.08x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 17.1 us: 1.08x faster                                                      |
| logging_format          | 6.72 us                                                     | 6.25 us: 1.07x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.42 ms: 1.07x faster                                                      |
| 2to3                    | 218 ms                                                      | 203 ms: 1.07x faster                                                       |
| python_startup_no_site  | 16.2 ms                                                     | 15.2 ms: 1.07x faster                                                      |
| unpickle_list           | 2.75 us                                                     | 2.58 us: 1.07x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 61.1 ms: 1.07x faster                                                      |
| float                   | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                      |
| nbody                   | 71.9 ms                                                     | 67.9 ms: 1.06x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.4 ms: 1.06x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.67 us: 1.06x faster                                                      |
| docutils                | 1.66 sec                                                    | 1.57 sec: 1.06x faster                                                     |
| xml_etree_generate      | 55.8 ms                                                     | 53.0 ms: 1.05x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.94 ms: 1.05x faster                                                      |
| regex_dna               | 126 ms                                                      | 121 ms: 1.04x faster                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.69 us: 1.04x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 42.5 ms: 1.04x faster                                                      |
| unpickle                | 8.18 us                                                     | 7.87 us: 1.04x faster                                                      |
| pidigits                | 152 ms                                                      | 147 ms: 1.04x faster                                                       |
| json_loads              | 13.9 us                                                     | 13.4 us: 1.04x faster                                                      |
| aiohttp                 | 884 us                                                      | 854 us: 1.04x faster                                                       |
| scimark_fft             | 184 ms                                                      | 180 ms: 1.03x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.9 ms: 1.02x faster                                                      |
| scimark_sor             | 78.8 ms                                                     | 77.1 ms: 1.02x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 37.6 ms: 1.00x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 2.12 us: 1.01x slower                                                      |
| crypto_pyaes            | 48.5 ms                                                     | 49.1 ms: 1.01x slower                                                      |
| meteor_contest          | 74.6 ms                                                     | 75.5 ms: 1.01x slower                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.60 ms: 1.02x slower                                                      |
| async_tree_cpu_io_mixed | 489 ms                                                      | 499 ms: 1.02x slower                                                       |
| pprint_safe_repr        | 513 ms                                                      | 525 ms: 1.02x slower                                                       |
| dask                    | 263 ms                                                      | 268 ms: 1.02x slower                                                       |
| fannkuch                | 247 ms                                                      | 252 ms: 1.02x slower                                                       |
| async_tree_io           | 731 ms                                                      | 751 ms: 1.03x slower                                                       |
| pyflate                 | 295 ms                                                      | 303 ms: 1.03x slower                                                       |
| scimark_monte_carlo     | 43.7 ms                                                     | 45.0 ms: 1.03x slower                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 35.6 ms: 1.03x slower                                                      |
| sympy_expand            | 284 ms                                                      | 293 ms: 1.03x slower                                                       |
| pprint_pformat          | 1.05 sec                                                    | 1.08 sec: 1.03x slower                                                     |
| regex_compile           | 87.5 ms                                                     | 90.5 ms: 1.03x slower                                                      |
| bench_thread_pool       | 857 us                                                      | 888 us: 1.04x slower                                                       |
| spectral_norm           | 66.9 ms                                                     | 69.6 ms: 1.04x slower                                                      |
| pickle_pure_python      | 195 us                                                      | 204 us: 1.04x slower                                                       |
| sympy_str               | 175 ms                                                      | 183 ms: 1.04x slower                                                       |
| django_template         | 22.9 ms                                                     | 24.0 ms: 1.05x slower                                                      |
| sqlglot_normalize       | 187 ms                                                      | 196 ms: 1.05x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 13.6 ms: 1.05x slower                                                      |
| raytrace                | 192 ms                                                      | 203 ms: 1.06x slower                                                       |
| deepcopy_memo           | 23.7 us                                                     | 25.1 us: 1.06x slower                                                      |
| sympy_sum               | 91.5 ms                                                     | 96.9 ms: 1.06x slower                                                      |
| deepcopy                | 238 us                                                      | 252 us: 1.06x slower                                                       |
| richards                | 28.4 ms                                                     | 30.1 ms: 1.06x slower                                                      |
| coroutines              | 14.3 ms                                                     | 15.2 ms: 1.06x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 62.7 ms: 1.07x slower                                                      |
| json                    | 3.05 ms                                                     | 3.25 ms: 1.07x slower                                                      |
| async_tree_none         | 291 ms                                                      | 311 ms: 1.07x slower                                                       |
| go                      | 91.6 ms                                                     | 97.9 ms: 1.07x slower                                                      |
| pycparser               | 699 ms                                                      | 748 ms: 1.07x slower                                                       |
| nqueens                 | 62.8 ms                                                     | 67.6 ms: 1.08x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 370 ms: 1.09x slower                                                       |
| chameleon               | 4.98 ms                                                     | 5.45 ms: 1.09x slower                                                      |
| hexiom                  | 4.10 ms                                                     | 4.59 ms: 1.12x slower                                                      |
| unpack_sequence         | 37.5 ns                                                     | 42.2 ns: 1.13x slower                                                      |
| chaos                   | 43.3 ms                                                     | 48.9 ms: 1.13x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 152 us: 1.14x slower                                                       |
| logging_silent          | 60.5 ns                                                     | 70.2 ns: 1.16x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.63 sec: 1.19x slower                                                     |
| deltablue               | 2.16 ms                                                     | 2.66 ms: 1.23x slower                                                      |
| comprehensions          | 14.1 us                                                     | 17.8 us: 1.26x slower                                                      |
| sqlglot_transpile       | 1.02 ms                                                     | 1.37 ms: 1.34x slower                                                      |
| json_dumps              | 5.70 ms                                                     | 7.72 ms: 1.36x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 673 ms: 1.38x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 1.15 ms: 1.43x slower                                                      |
| generators              | 22.5 ms                                                     | 33.9 ms: 1.50x slower                                                      |
| coverage                | 40.8 ms                                                     | 103 ms: 2.51x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.04x slower                                                               |

Benchmark hidden because not significant (3): xml_etree_parse, tornado_http, mako
Ignored benchmarks (11) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20220506-3.11.0b1-8d32a5c/bm-20220506-pythonperf1-amd64-python-8d32a5c8c4e9c90b0a21-3.11.0b1-8d32a5c.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 99.60% likely to be slow
- 90% likely to have a slowdown of 1.01x
- 95% likely to have a slowdown of 1.01x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown