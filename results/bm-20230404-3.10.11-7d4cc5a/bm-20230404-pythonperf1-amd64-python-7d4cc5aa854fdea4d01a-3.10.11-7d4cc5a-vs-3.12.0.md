
# Results vs. 3.12.0

- fork: python
- ref: 7d4cc5aa854fdea4d01a
- machine: windows-amd64
- commit hash: 7d4cc5a
- commit date: 2023-04-04
- overall geometric mean: 1.15x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 233 ms: 1.07x slower                                                      |
| chameleon      | 4.98 ms                                                     | 5.67 ms: 1.14x slower                                                     |
| docutils       | 1.66 sec                                                    | 1.82 sec: 1.10x slower                                                    |
| tornado_http   | 89.5 ms                                                     | 108 ms: 1.21x slower                                                      |
| Geometric mean | (ref)                                                       | 1.13x slower                                                              |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 598 ms: 1.22x slower                                                      |
| async_tree_io           | 731 ms                                                      | 1.04 sec: 1.42x slower                                                    |
| async_tree_memoization  | 339 ms                                                      | 481 ms: 1.42x slower                                                      |
| async_tree_none         | 291 ms                                                      | 414 ms: 1.42x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.37x slower                                                              |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                      |
| nbody          | 71.9 ms                                                     | 75.5 ms: 1.05x slower                                                     |
| float          | 56.8 ms                                                     | 60.7 ms: 1.07x slower                                                     |
| Geometric mean | (ref)                                                       | 1.03x slower                                                              |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| regex_effbot   | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                     |
| regex_dna      | 126 ms                                                      | 129 ms: 1.02x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| regex_compile  | 87.5 ms                                                     | 102 ms: 1.17x slower                                                      |
| Geometric mean | (ref)                                                       | 1.05x slower                                                              |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|----------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| unpickle_list        | 2.75 us                                                     | 2.66 us: 1.03x faster                                                     |
| xml_etree_generate   | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                     |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                     |
| json_loads           | 13.9 us                                                     | 13.7 us: 1.01x faster                                                     |
| pickle               | 7.43 us                                                     | 7.34 us: 1.01x faster                                                     |
| pickle_dict          | 18.4 us                                                     | 18.7 us: 1.02x slower                                                     |
| xml_etree_parse      | 93.0 ms                                                     | 96.4 ms: 1.04x slower                                                     |
| unpickle             | 8.18 us                                                     | 9.30 us: 1.14x slower                                                     |
| xml_etree_process    | 37.7 ms                                                     | 43.5 ms: 1.15x slower                                                     |
| unpickle_pure_python | 133 us                                                      | 177 us: 1.33x slower                                                      |
| pickle_pure_python   | 195 us                                                      | 266 us: 1.36x slower                                                      |
| json_dumps           | 5.70 ms                                                     | 8.90 ms: 1.56x slower                                                     |
| Geometric mean       | (ref)                                                       | 1.10x slower                                                              |

Benchmark hidden because not significant (1): pickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                                     |
| python_startup         | 19.5 ms                                                     | 21.1 ms: 1.08x slower                                                     |
| Geometric mean         | (ref)                                                       | 1.02x slower                                                              |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-----------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 8.76 ms: 1.24x slower                                                     |
| django_template | 22.9 ms                                                     | 28.9 ms: 1.26x slower                                                     |
| Geometric mean  | (ref)                                                       | 1.25x slower                                                              |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a |
|-------------------------|:-----------------------------------------------------------:|:-------------------------------------------------------------------------:|
| bench_mp_pool           | 69.2 ms                                                     | 60.4 ms: 1.15x faster                                                     |
| async_generators        | 239 ms                                                      | 218 ms: 1.10x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 74.4 ms: 1.08x faster                                                     |
| gc_traversal            | 1.52 ms                                                     | 1.42 ms: 1.07x faster                                                     |
| telco                   | 4.13 ms                                                     | 3.93 ms: 1.05x faster                                                     |
| coverage                | 40.8 ms                                                     | 39.2 ms: 1.04x faster                                                     |
| python_startup_no_site  | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                                     |
| pidigits                | 152 ms                                                      | 147 ms: 1.04x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 72.1 ms: 1.04x faster                                                     |
| unpickle_list           | 2.75 us                                                     | 2.66 us: 1.03x faster                                                     |
| xml_etree_generate      | 55.8 ms                                                     | 54.3 ms: 1.03x faster                                                     |
| xml_etree_iterparse     | 65.2 ms                                                     | 63.4 ms: 1.03x faster                                                     |
| json_loads              | 13.9 us                                                     | 13.7 us: 1.01x faster                                                     |
| pickle                  | 7.43 us                                                     | 7.34 us: 1.01x faster                                                     |
| regex_effbot            | 1.62 ms                                                     | 1.60 ms: 1.01x faster                                                     |
| json                    | 3.05 ms                                                     | 3.02 ms: 1.01x faster                                                     |
| logging_format          | 6.72 us                                                     | 6.76 us: 1.01x slower                                                     |
| pickle_dict             | 18.4 us                                                     | 18.7 us: 1.02x slower                                                     |
| deepcopy_reduce         | 2.09 us                                                     | 2.13 us: 1.02x slower                                                     |
| regex_dna               | 126 ms                                                      | 129 ms: 1.02x slower                                                      |
| regex_v8                | 14.2 ms                                                     | 14.6 ms: 1.03x slower                                                     |
| create_gc_cycles        | 752 us                                                      | 777 us: 1.03x slower                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 96.4 ms: 1.04x slower                                                     |
| sqlite_synth            | 1.76 us                                                     | 1.84 us: 1.05x slower                                                     |
| nbody                   | 71.9 ms                                                     | 75.5 ms: 1.05x slower                                                     |
| 2to3                    | 218 ms                                                      | 233 ms: 1.07x slower                                                      |
| float                   | 56.8 ms                                                     | 60.7 ms: 1.07x slower                                                     |
| dulwich_log             | 44.3 ms                                                     | 47.6 ms: 1.07x slower                                                     |
| nqueens                 | 62.8 ms                                                     | 67.5 ms: 1.08x slower                                                     |
| sympy_str               | 175 ms                                                      | 188 ms: 1.08x slower                                                      |
| sqlglot_normalize       | 187 ms                                                      | 202 ms: 1.08x slower                                                      |
| python_startup          | 19.5 ms                                                     | 21.1 ms: 1.08x slower                                                     |
| bench_thread_pool       | 857 us                                                      | 928 us: 1.08x slower                                                      |
| aiohttp                 | 884 us                                                      | 962 us: 1.09x slower                                                      |
| deepcopy                | 238 us                                                      | 260 us: 1.09x slower                                                      |
| docutils                | 1.66 sec                                                    | 1.82 sec: 1.10x slower                                                    |
| scimark_fft             | 184 ms                                                      | 203 ms: 1.10x slower                                                      |
| coroutines              | 14.3 ms                                                     | 15.7 ms: 1.10x slower                                                     |
| sympy_expand            | 284 ms                                                      | 312 ms: 1.10x slower                                                      |
| comprehensions          | 14.1 us                                                     | 15.6 us: 1.10x slower                                                     |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.83 ms: 1.11x slower                                                     |
| sqlalchemy_declarative  | 86.4 ms                                                     | 95.8 ms: 1.11x slower                                                     |
| sqlglot_optimize        | 34.5 ms                                                     | 38.5 ms: 1.12x slower                                                     |
| fannkuch                | 247 ms                                                      | 276 ms: 1.12x slower                                                      |
| unpack_sequence         | 37.5 ns                                                     | 42.1 ns: 1.12x slower                                                     |
| unpickle                | 8.18 us                                                     | 9.30 us: 1.14x slower                                                     |
| chameleon               | 4.98 ms                                                     | 5.67 ms: 1.14x slower                                                     |
| pprint_safe_repr        | 513 ms                                                      | 584 ms: 1.14x slower                                                      |
| sympy_integrate         | 13.0 ms                                                     | 14.8 ms: 1.14x slower                                                     |
| sympy_sum               | 91.5 ms                                                     | 105 ms: 1.14x slower                                                      |
| pprint_pformat          | 1.05 sec                                                    | 1.19 sec: 1.14x slower                                                    |
| dask                    | 263 ms                                                      | 303 ms: 1.15x slower                                                      |
| xml_etree_process       | 37.7 ms                                                     | 43.5 ms: 1.15x slower                                                     |
| regex_compile           | 87.5 ms                                                     | 102 ms: 1.17x slower                                                      |
| sqlalchemy_imperative   | 9.29 ms                                                     | 11.1 ms: 1.20x slower                                                     |
| pycparser               | 699 ms                                                      | 839 ms: 1.20x slower                                                      |
| deepcopy_memo           | 23.7 us                                                     | 28.6 us: 1.21x slower                                                     |
| tornado_http            | 89.5 ms                                                     | 108 ms: 1.21x slower                                                      |
| spectral_norm           | 66.9 ms                                                     | 81.4 ms: 1.22x slower                                                     |
| async_tree_cpu_io_mixed | 489 ms                                                      | 598 ms: 1.22x slower                                                      |
| mako                    | 7.09 ms                                                     | 8.76 ms: 1.24x slower                                                     |
| mdp                     | 1.37 sec                                                    | 1.71 sec: 1.25x slower                                                    |
| django_template         | 22.9 ms                                                     | 28.9 ms: 1.26x slower                                                     |
| crypto_pyaes            | 48.5 ms                                                     | 63.2 ms: 1.30x slower                                                     |
| hexiom                  | 4.10 ms                                                     | 5.40 ms: 1.32x slower                                                     |
| pyflate                 | 295 ms                                                      | 391 ms: 1.33x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 177 us: 1.33x slower                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 58.9 ms: 1.35x slower                                                     |
| pickle_pure_python      | 195 us                                                      | 266 us: 1.36x slower                                                      |
| scimark_sor             | 78.8 ms                                                     | 107 ms: 1.36x slower                                                      |
| chaos                   | 43.3 ms                                                     | 59.2 ms: 1.37x slower                                                     |
| sqlglot_transpile       | 1.02 ms                                                     | 1.42 ms: 1.39x slower                                                     |
| raytrace                | 192 ms                                                      | 271 ms: 1.41x slower                                                      |
| async_tree_io           | 731 ms                                                      | 1.04 sec: 1.42x slower                                                    |
| async_tree_memoization  | 339 ms                                                      | 481 ms: 1.42x slower                                                      |
| async_tree_none         | 291 ms                                                      | 414 ms: 1.42x slower                                                      |
| generators              | 22.5 ms                                                     | 32.1 ms: 1.42x slower                                                     |
| scimark_lu              | 58.9 ms                                                     | 84.5 ms: 1.44x slower                                                     |
| richards                | 28.4 ms                                                     | 40.9 ms: 1.44x slower                                                     |
| sqlglot_parse           | 804 us                                                      | 1.19 ms: 1.47x slower                                                     |
| go                      | 91.6 ms                                                     | 137 ms: 1.49x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 755 ms: 1.55x slower                                                      |
| json_dumps              | 5.70 ms                                                     | 8.90 ms: 1.56x slower                                                     |
| logging_silent          | 60.5 ns                                                     | 97.2 ns: 1.61x slower                                                     |
| deltablue               | 2.16 ms                                                     | 4.11 ms: 1.90x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.15x slower                                                              |

Benchmark hidden because not significant (2): logging_simple, pickle_list
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20230404-3.10.11-7d4cc5a/bm-20230404-pythonperf1-amd64-python-7d4cc5aa854fdea4d01a-3.10.11-7d4cc5a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.11x
- 95% likely to have a slowdown of 1.10x
- 99% likely to have a slowdown of 1.09x


# Memory

- memory change: unknown