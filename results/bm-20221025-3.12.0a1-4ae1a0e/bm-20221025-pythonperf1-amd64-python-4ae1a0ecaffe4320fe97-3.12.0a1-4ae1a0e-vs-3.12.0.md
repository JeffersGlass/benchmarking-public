
# Results vs. 3.12.0

- fork: python
- ref: 4ae1a0ecaffe4320fe97
- machine: windows-amd64
- commit hash: 4ae1a0e
- commit date: 2022-10-25
- overall geometric mean: 1.02x slower \*
- HPT reliability: 56.20%
- HPT 99th percentile: 1.00x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 202 ms: 1.08x faster                                                       |
| docutils       | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                     |
| tornado_http   | 89.5 ms                                                     | 91.5 ms: 1.02x slower                                                      |
| Geometric mean | (ref)                                                       | 1.02x faster                                                               |

Benchmark hidden because not significant (1): chameleon

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 506 ms: 1.03x slower                                                       |
| async_tree_io           | 731 ms                                                      | 775 ms: 1.06x slower                                                       |
| async_tree_none         | 291 ms                                                      | 316 ms: 1.08x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 381 ms: 1.12x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.07x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 67.2 ms: 1.07x faster                                                      |
| float          | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                      |
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 119 ms: 1.06x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| regex_compile  | 87.5 ms                                                     | 86.3 ms: 1.01x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.03x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.55 us: 1.14x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 50.5 ms: 1.10x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.64 us: 1.07x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 86.8 ms: 1.07x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.60 us: 1.06x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                      |
| json_loads           | 13.9 us                                                     | 13.5 us: 1.03x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.62 ms: 1.01x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 18.2 us: 1.01x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 143 us: 1.07x slower                                                       |
| unpickle             | 8.18 us                                                     | 8.87 us: 1.08x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.03x faster                                                               |

Benchmark hidden because not significant (1): pickle_pure_python

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.93 ms: 1.02x faster                                                      |
| django_template | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.01x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 181 ms: 1.32x faster                                                       |
| bench_mp_pool           | 69.2 ms                                                     | 60.9 ms: 1.14x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.55 us: 1.14x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 663 us: 1.13x faster                                                       |
| xml_etree_generate      | 55.8 ms                                                     | 50.5 ms: 1.10x faster                                                      |
| json                    | 3.05 ms                                                     | 2.77 ms: 1.10x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 74.0 ms: 1.09x faster                                                      |
| 2to3                    | 218 ms                                                      | 202 ms: 1.08x faster                                                       |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.37 ms: 1.08x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.85 ms: 1.07x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.64 us: 1.07x faster                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 86.8 ms: 1.07x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.42 ms: 1.07x faster                                                      |
| nbody                   | 71.9 ms                                                     | 67.2 ms: 1.07x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| scimark_sor             | 78.8 ms                                                     | 73.8 ms: 1.07x faster                                                      |
| float                   | 56.8 ms                                                     | 53.5 ms: 1.06x faster                                                      |
| regex_dna               | 126 ms                                                      | 119 ms: 1.06x faster                                                       |
| python_startup_no_site  | 16.2 ms                                                     | 15.4 ms: 1.06x faster                                                      |
| unpickle_list           | 2.75 us                                                     | 2.60 us: 1.06x faster                                                      |
| pprint_pformat          | 1.05 sec                                                    | 1.00 sec: 1.04x faster                                                     |
| docutils                | 1.66 sec                                                    | 1.59 sec: 1.04x faster                                                     |
| regex_v8                | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 71.8 ms: 1.04x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 36.3 ms: 1.04x faster                                                      |
| pprint_safe_repr        | 513 ms                                                      | 495 ms: 1.04x faster                                                       |
| fannkuch                | 247 ms                                                      | 238 ms: 1.04x faster                                                       |
| pidigits                | 152 ms                                                      | 148 ms: 1.03x faster                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 47.2 ms: 1.03x faster                                                      |
| json_loads              | 13.9 us                                                     | 13.5 us: 1.03x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 63.6 ms: 1.02x faster                                                      |
| mako                    | 7.09 ms                                                     | 6.93 ms: 1.02x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 2.05 us: 1.02x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 43.5 ms: 1.02x faster                                                      |
| bench_thread_pool       | 857 us                                                      | 844 us: 1.01x faster                                                       |
| json_dumps              | 5.70 ms                                                     | 5.62 ms: 1.01x faster                                                      |
| deepcopy                | 238 us                                                      | 235 us: 1.01x faster                                                       |
| regex_compile           | 87.5 ms                                                     | 86.3 ms: 1.01x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 18.2 us: 1.01x faster                                                      |
| sqlglot_normalize       | 187 ms                                                      | 188 ms: 1.01x slower                                                       |
| pyflate                 | 295 ms                                                      | 297 ms: 1.01x slower                                                       |
| regex_effbot            | 1.62 ms                                                     | 1.63 ms: 1.01x slower                                                      |
| scimark_fft             | 184 ms                                                      | 188 ms: 1.02x slower                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.80 us: 1.02x slower                                                      |
| tornado_http            | 89.5 ms                                                     | 91.5 ms: 1.02x slower                                                      |
| go                      | 91.6 ms                                                     | 93.8 ms: 1.02x slower                                                      |
| sympy_integrate         | 13.0 ms                                                     | 13.4 ms: 1.03x slower                                                      |
| async_tree_cpu_io_mixed | 489 ms                                                      | 506 ms: 1.03x slower                                                       |
| django_template         | 22.9 ms                                                     | 23.8 ms: 1.04x slower                                                      |
| nqueens                 | 62.8 ms                                                     | 65.4 ms: 1.04x slower                                                      |
| sympy_expand            | 284 ms                                                      | 296 ms: 1.04x slower                                                       |
| deepcopy_memo           | 23.7 us                                                     | 24.7 us: 1.04x slower                                                      |
| sympy_str               | 175 ms                                                      | 183 ms: 1.04x slower                                                       |
| coroutines              | 14.3 ms                                                     | 15.0 ms: 1.05x slower                                                      |
| raytrace                | 192 ms                                                      | 204 ms: 1.06x slower                                                       |
| async_tree_io           | 731 ms                                                      | 775 ms: 1.06x slower                                                       |
| chaos                   | 43.3 ms                                                     | 46.5 ms: 1.07x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 143 us: 1.07x slower                                                       |
| sympy_sum               | 91.5 ms                                                     | 98.9 ms: 1.08x slower                                                      |
| async_tree_none         | 291 ms                                                      | 316 ms: 1.08x slower                                                       |
| unpickle                | 8.18 us                                                     | 8.87 us: 1.08x slower                                                      |
| logging_simple          | 6.28 us                                                     | 6.80 us: 1.08x slower                                                      |
| logging_format          | 6.72 us                                                     | 7.28 us: 1.08x slower                                                      |
| richards                | 28.4 ms                                                     | 31.0 ms: 1.09x slower                                                      |
| hexiom                  | 4.10 ms                                                     | 4.51 ms: 1.10x slower                                                      |
| spectral_norm           | 66.9 ms                                                     | 73.8 ms: 1.10x slower                                                      |
| comprehensions          | 14.1 us                                                     | 15.6 us: 1.11x slower                                                      |
| sqlglot_transpile       | 1.02 ms                                                     | 1.14 ms: 1.11x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 381 ms: 1.12x slower                                                       |
| unpack_sequence         | 37.5 ns                                                     | 42.3 ns: 1.13x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 66.6 ms: 1.13x slower                                                      |
| logging_silent          | 60.5 ns                                                     | 68.8 ns: 1.14x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.59 sec: 1.16x slower                                                     |
| deltablue               | 2.16 ms                                                     | 2.51 ms: 1.16x slower                                                      |
| sqlglot_parse           | 804 us                                                      | 951 us: 1.18x slower                                                       |
| coverage                | 40.8 ms                                                     | 52.1 ms: 1.28x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 694 ms: 1.42x slower                                                       |
| generators              | 22.5 ms                                                     | 34.5 ms: 1.53x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                               |

Benchmark hidden because not significant (6): sqlglot_optimize, chameleon, scimark_monte_carlo, pickle_pure_python, dask, pycparser
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (5) of results/bm-20221025-3.12.0a1-4ae1a0e/bm-20221025-pythonperf1-amd64-python-4ae1a0ecaffe4320fe97-3.12.0a1-4ae1a0e.json: genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 56.20% likely to be slow
- 90% likely to have a slowdown of 1.00x
- 95% likely to have a slowdown of 1.00x
- 99% likely to have a slowdown of 1.00x


# Memory

- memory change: unknown