
# Results vs. 3.12.0

- fork: python
- ref: aad5f6a89125ad4529ab
- machine: windows-amd64
- commit hash: aad5f6a
- commit date: 2023-02-07
- overall geometric mean: 1.15x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 231 ms: 1.06x slower                                                      |
| chameleon      | 4.98 ms                                                     | 5.49 ms: 1.10x slower                                                     |
| docutils       | 1.66 sec                                                    | 1.84 sec: 1.11x slower                                                    |
| tornado_http   | 89.5 ms                                                     | 109 ms: 1.22x slower                                                      |
| Geometric mean | (ref)                                                       | 1.12x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 615 ms: 1.26x slower                                                      |
| async_tree_io           | 731 ms                                                      | 1.05 sec: 1.43x slower                                                    |
| async_tree_none         | 291 ms                                                      | 417 ms: 1.43x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 490 ms: 1.44x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.39x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                      |
| float          | 56.8 ms                                                     | 60.6 ms: 1.07x slower                                                     |
| Geometric mean | (ref)                                                       | 1.01x slower                                                              |

Benchmark hidden because not significant (1): nbody

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 132 ms: 1.04x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 15.0 ms: 1.05x slower                                                     |
| regex_effbot   | 1.62 ms                                                     | 1.81 ms: 1.12x slower                                                     |
| regex_compile  | 87.5 ms                                                     | 103 ms: 1.18x slower                                                      |
| Geometric mean | (ref)                                                       | 1.10x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 7.00 us: 1.06x faster                                                     |
| xml_etree_generate   | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                     |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.4 ms: 1.01x faster                                                     |
| json_loads           | 13.9 us                                                     | 14.2 us: 1.02x slower                                                     |
| pickle_list          | 2.83 us                                                     | 2.91 us: 1.03x slower                                                     |
| xml_etree_parse      | 93.0 ms                                                     | 96.6 ms: 1.04x slower                                                     |
| pickle_dict          | 18.4 us                                                     | 19.1 us: 1.04x slower                                                     |
| unpickle             | 8.18 us                                                     | 9.05 us: 1.11x slower                                                     |
| xml_etree_process    | 37.7 ms                                                     | 42.7 ms: 1.13x slower                                                     |
| unpickle_pure_python | 133 us                                                      | 180 us: 1.35x slower                                                      |
| pickle_pure_python   | 195 us                                                      | 267 us: 1.37x slower                                                      |
| json_dumps           | 5.70 ms                                                     | 8.93 ms: 1.57x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.10x slower                                                              |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.0 ms: 1.08x faster                                                     |
| python_startup         | 19.5 ms                                                     | 19.8 ms: 1.02x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 8.84 ms: 1.25x slower                                                     |
| django_template | 22.9 ms                                                     | 29.2 ms: 1.27x slower                                                     |
| Geometric mean  | (ref)                                                       | 1.26x slower                                                              |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| bench_mp_pool           | 69.2 ms                                                     | 60.0 ms: 1.15x faster                                                     |
| gc_traversal            | 1.52 ms                                                     | 1.40 ms: 1.09x faster                                                     |
| python_startup_no_site  | 16.2 ms                                                     | 15.0 ms: 1.08x faster                                                     |
| pathlib                 | 80.5 ms                                                     | 75.0 ms: 1.07x faster                                                     |
| telco                   | 4.13 ms                                                     | 3.88 ms: 1.07x faster                                                     |
| pickle                  | 7.43 us                                                     | 7.00 us: 1.06x faster                                                     |
| async_generators        | 239 ms                                                      | 227 ms: 1.06x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 53.3 ms: 1.05x faster                                                     |
| pidigits                | 152 ms                                                      | 148 ms: 1.03x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 72.9 ms: 1.02x faster                                                     |
| coverage                | 40.8 ms                                                     | 40.0 ms: 1.02x faster                                                     |
| xml_etree_iterparse     | 65.2 ms                                                     | 64.4 ms: 1.01x faster                                                     |
| logging_format          | 6.72 us                                                     | 6.81 us: 1.01x slower                                                     |
| python_startup          | 19.5 ms                                                     | 19.8 ms: 1.02x slower                                                     |
| json_loads              | 13.9 us                                                     | 14.2 us: 1.02x slower                                                     |
| deepcopy_reduce         | 2.09 us                                                     | 2.14 us: 1.02x slower                                                     |
| logging_simple          | 6.28 us                                                     | 6.45 us: 1.03x slower                                                     |
| pickle_list             | 2.83 us                                                     | 2.91 us: 1.03x slower                                                     |
| create_gc_cycles        | 752 us                                                      | 776 us: 1.03x slower                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 96.6 ms: 1.04x slower                                                     |
| pickle_dict             | 18.4 us                                                     | 19.1 us: 1.04x slower                                                     |
| nqueens                 | 62.8 ms                                                     | 65.3 ms: 1.04x slower                                                     |
| regex_dna               | 126 ms                                                      | 132 ms: 1.04x slower                                                      |
| fannkuch                | 247 ms                                                      | 259 ms: 1.05x slower                                                      |
| scimark_fft             | 184 ms                                                      | 194 ms: 1.05x slower                                                      |
| regex_v8                | 14.2 ms                                                     | 15.0 ms: 1.05x slower                                                     |
| sqlite_synth            | 1.76 us                                                     | 1.86 us: 1.06x slower                                                     |
| 2to3                    | 218 ms                                                      | 231 ms: 1.06x slower                                                      |
| float                   | 56.8 ms                                                     | 60.6 ms: 1.07x slower                                                     |
| sqlglot_normalize       | 187 ms                                                      | 202 ms: 1.08x slower                                                      |
| deepcopy                | 238 us                                                      | 258 us: 1.08x slower                                                      |
| unpack_sequence         | 37.5 ns                                                     | 40.8 ns: 1.09x slower                                                     |
| sympy_str               | 175 ms                                                      | 191 ms: 1.09x slower                                                      |
| chameleon               | 4.98 ms                                                     | 5.49 ms: 1.10x slower                                                     |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.82 ms: 1.10x slower                                                     |
| bench_thread_pool       | 857 us                                                      | 944 us: 1.10x slower                                                      |
| sympy_expand            | 284 ms                                                      | 314 ms: 1.11x slower                                                      |
| unpickle                | 8.18 us                                                     | 9.05 us: 1.11x slower                                                     |
| dulwich_log             | 44.3 ms                                                     | 49.0 ms: 1.11x slower                                                     |
| comprehensions          | 14.1 us                                                     | 15.7 us: 1.11x slower                                                     |
| aiohttp                 | 884 us                                                      | 980 us: 1.11x slower                                                      |
| docutils                | 1.66 sec                                                    | 1.84 sec: 1.11x slower                                                    |
| coroutines              | 14.3 ms                                                     | 15.9 ms: 1.11x slower                                                     |
| sqlglot_optimize        | 34.5 ms                                                     | 38.5 ms: 1.11x slower                                                     |
| regex_effbot            | 1.62 ms                                                     | 1.81 ms: 1.12x slower                                                     |
| pprint_safe_repr        | 513 ms                                                      | 576 ms: 1.12x slower                                                      |
| sqlalchemy_declarative  | 86.4 ms                                                     | 97.2 ms: 1.12x slower                                                     |
| pprint_pformat          | 1.05 sec                                                    | 1.18 sec: 1.13x slower                                                    |
| sympy_integrate         | 13.0 ms                                                     | 14.6 ms: 1.13x slower                                                     |
| xml_etree_process       | 37.7 ms                                                     | 42.7 ms: 1.13x slower                                                     |
| sympy_sum               | 91.5 ms                                                     | 106 ms: 1.16x slower                                                      |
| regex_compile           | 87.5 ms                                                     | 103 ms: 1.18x slower                                                      |
| dask                    | 263 ms                                                      | 314 ms: 1.20x slower                                                      |
| tornado_http            | 89.5 ms                                                     | 109 ms: 1.22x slower                                                      |
| pycparser               | 699 ms                                                      | 855 ms: 1.22x slower                                                      |
| deepcopy_memo           | 23.7 us                                                     | 29.1 us: 1.23x slower                                                     |
| spectral_norm           | 66.9 ms                                                     | 82.5 ms: 1.23x slower                                                     |
| sqlalchemy_imperative   | 9.29 ms                                                     | 11.5 ms: 1.23x slower                                                     |
| mdp                     | 1.37 sec                                                    | 1.71 sec: 1.25x slower                                                    |
| mako                    | 7.09 ms                                                     | 8.84 ms: 1.25x slower                                                     |
| async_tree_cpu_io_mixed | 489 ms                                                      | 615 ms: 1.26x slower                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 55.2 ms: 1.26x slower                                                     |
| django_template         | 22.9 ms                                                     | 29.2 ms: 1.27x slower                                                     |
| crypto_pyaes            | 48.5 ms                                                     | 63.1 ms: 1.30x slower                                                     |
| hexiom                  | 4.10 ms                                                     | 5.38 ms: 1.31x slower                                                     |
| scimark_sor             | 78.8 ms                                                     | 104 ms: 1.32x slower                                                      |
| pyflate                 | 295 ms                                                      | 393 ms: 1.33x slower                                                      |
| chaos                   | 43.3 ms                                                     | 58.2 ms: 1.34x slower                                                     |
| unpickle_pure_python    | 133 us                                                      | 180 us: 1.35x slower                                                      |
| pickle_pure_python      | 195 us                                                      | 267 us: 1.37x slower                                                      |
| raytrace                | 192 ms                                                      | 266 ms: 1.38x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 678 ms: 1.39x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 83.2 ms: 1.41x slower                                                     |
| sqlglot_transpile       | 1.02 ms                                                     | 1.45 ms: 1.42x slower                                                     |
| async_tree_io           | 731 ms                                                      | 1.05 sec: 1.43x slower                                                    |
| async_tree_none         | 291 ms                                                      | 417 ms: 1.43x slower                                                      |
| generators              | 22.5 ms                                                     | 32.5 ms: 1.44x slower                                                     |
| async_tree_memoization  | 339 ms                                                      | 490 ms: 1.44x slower                                                      |
| richards                | 28.4 ms                                                     | 42.3 ms: 1.49x slower                                                     |
| go                      | 91.6 ms                                                     | 138 ms: 1.51x slower                                                      |
| sqlglot_parse           | 804 us                                                      | 1.23 ms: 1.53x slower                                                     |
| json_dumps              | 5.70 ms                                                     | 8.93 ms: 1.57x slower                                                     |
| logging_silent          | 60.5 ns                                                     | 99.1 ns: 1.64x slower                                                     |
| deltablue               | 2.16 ms                                                     | 4.16 ms: 1.93x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.15x slower                                                              |

Benchmark hidden because not significant (3): unpickle_list, nbody, json
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230207-3.10.10-aad5f6a/bm-20230207-pythonperf1-amd64-python-aad5f6a89125ad4529ab-3.10.10-aad5f6a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.10x
- 99% likely to have a slowdown of 1.09x


# Memory

- memory change: unknown