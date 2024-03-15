
# Results vs. 3.12.0

- fork: python
- ref: f9774e57d84162ff0cba
- machine: windows-amd64
- commit hash: f9774e5
- commit date: 2023-03-07
- overall geometric mean: 1.05x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.04x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 194 ms: 1.12x faster                                                       |
| chameleon      | 4.98 ms                                                     | 4.76 ms: 1.05x faster                                                      |
| docutils       | 1.66 sec                                                    | 1.51 sec: 1.10x faster                                                     |
| tornado_http   | 89.5 ms                                                     | 90.6 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 479 ms: 1.02x faster                                                       |
| async_tree_io           | 731 ms                                                      | 744 ms: 1.02x slower                                                       |
| async_tree_none         | 291 ms                                                      | 304 ms: 1.04x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 356 ms: 1.05x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 56.8 ms                                                     | 47.4 ms: 1.20x faster                                                      |
| nbody          | 71.9 ms                                                     | 63.3 ms: 1.14x faster                                                      |
| pidigits       | 152 ms                                                      | 147 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.12x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 115 ms: 1.10x faster                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.50 ms: 1.08x faster                                                      |
| regex_v8       | 14.2 ms                                                     | 13.4 ms: 1.07x faster                                                      |
| regex_compile  | 87.5 ms                                                     | 83.5 ms: 1.05x faster                                                      |
| Geometric mean | (ref)                                                       | 1.07x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 175 us: 1.12x faster                                                       |
| unpickle_pure_python | 133 us                                                      | 124 us: 1.08x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 52.1 ms: 1.07x faster                                                      |
| pickle               | 7.43 us                                                     | 6.96 us: 1.07x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 35.6 ms: 1.06x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 88.4 ms: 1.05x faster                                                      |
| json_loads           | 13.9 us                                                     | 13.4 us: 1.04x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                      |
| unpickle             | 8.18 us                                                     | 7.98 us: 1.03x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 18.7 us: 1.02x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                               |

Benchmark hidden because not significant (2): pickle_list, unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.5 ms: 1.05x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.20 ms: 1.14x faster                                                      |
| django_template | 22.9 ms                                                     | 20.9 ms: 1.10x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.12x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 37.5 ns                                                     | 27.9 ns: 1.34x faster                                                      |
| float                   | 56.8 ms                                                     | 47.4 ms: 1.20x faster                                                      |
| richards                | 28.4 ms                                                     | 24.5 ms: 1.16x faster                                                      |
| fannkuch                | 247 ms                                                      | 216 ms: 1.14x faster                                                       |
| mako                    | 7.09 ms                                                     | 6.20 ms: 1.14x faster                                                      |
| nbody                   | 71.9 ms                                                     | 63.3 ms: 1.14x faster                                                      |
| 2to3                    | 218 ms                                                      | 194 ms: 1.12x faster                                                       |
| deltablue               | 2.16 ms                                                     | 1.92 ms: 1.12x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 671 us: 1.12x faster                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 43.3 ms: 1.12x faster                                                      |
| pickle_pure_python      | 195 us                                                      | 175 us: 1.12x faster                                                       |
| sqlglot_normalize       | 187 ms                                                      | 168 ms: 1.11x faster                                                       |
| json                    | 3.05 ms                                                     | 2.74 ms: 1.11x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 1.88 us: 1.11x faster                                                      |
| go                      | 91.6 ms                                                     | 82.6 ms: 1.11x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 31.2 ms: 1.11x faster                                                      |
| nqueens                 | 62.8 ms                                                     | 56.9 ms: 1.10x faster                                                      |
| scimark_sor             | 78.8 ms                                                     | 71.6 ms: 1.10x faster                                                      |
| docutils                | 1.66 sec                                                    | 1.51 sec: 1.10x faster                                                     |
| django_template         | 22.9 ms                                                     | 20.9 ms: 1.10x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 68.0 ms: 1.10x faster                                                      |
| regex_dna               | 126 ms                                                      | 115 ms: 1.10x faster                                                       |
| bench_mp_pool           | 69.2 ms                                                     | 63.1 ms: 1.10x faster                                                      |
| scimark_fft             | 184 ms                                                      | 169 ms: 1.09x faster                                                       |
| pyflate                 | 295 ms                                                      | 270 ms: 1.09x faster                                                       |
| pathlib                 | 80.5 ms                                                     | 73.9 ms: 1.09x faster                                                      |
| deepcopy                | 238 us                                                      | 219 us: 1.09x faster                                                       |
| scimark_monte_carlo     | 43.7 ms                                                     | 40.4 ms: 1.08x faster                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.50 ms: 1.08x faster                                                      |
| unpickle_pure_python    | 133 us                                                      | 124 us: 1.08x faster                                                       |
| async_generators        | 239 ms                                                      | 223 ms: 1.07x faster                                                       |
| pprint_safe_repr        | 513 ms                                                      | 478 ms: 1.07x faster                                                       |
| xml_etree_generate      | 55.8 ms                                                     | 52.1 ms: 1.07x faster                                                      |
| hexiom                  | 4.10 ms                                                     | 3.83 ms: 1.07x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.86 ms: 1.07x faster                                                      |
| logging_silent          | 60.5 ns                                                     | 56.5 ns: 1.07x faster                                                      |
| pprint_pformat          | 1.05 sec                                                    | 977 ms: 1.07x faster                                                       |
| pickle                  | 7.43 us                                                     | 6.96 us: 1.07x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| raytrace                | 192 ms                                                      | 180 ms: 1.07x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.4 ms: 1.07x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 61.3 ms: 1.06x faster                                                      |
| xml_etree_process       | 37.7 ms                                                     | 35.6 ms: 1.06x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.44 ms: 1.06x faster                                                      |
| pycparser               | 699 ms                                                      | 663 ms: 1.05x faster                                                       |
| xml_etree_parse         | 93.0 ms                                                     | 88.4 ms: 1.05x faster                                                      |
| asyncio_tcp             | 487 ms                                                      | 463 ms: 1.05x faster                                                       |
| deepcopy_memo           | 23.7 us                                                     | 22.6 us: 1.05x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.5 ms: 1.05x faster                                                      |
| regex_compile           | 87.5 ms                                                     | 83.5 ms: 1.05x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 42.2 ms: 1.05x faster                                                      |
| chameleon               | 4.98 ms                                                     | 4.76 ms: 1.05x faster                                                      |
| pidigits                | 152 ms                                                      | 147 ms: 1.04x faster                                                       |
| bench_thread_pool       | 857 us                                                      | 827 us: 1.04x faster                                                       |
| json_loads              | 13.9 us                                                     | 13.4 us: 1.04x faster                                                      |
| json_dumps              | 5.70 ms                                                     | 5.51 ms: 1.03x faster                                                      |
| chaos                   | 43.3 ms                                                     | 42.0 ms: 1.03x faster                                                      |
| logging_simple          | 6.28 us                                                     | 6.10 us: 1.03x faster                                                      |
| generators              | 22.5 ms                                                     | 21.9 ms: 1.03x faster                                                      |
| logging_format          | 6.72 us                                                     | 6.55 us: 1.03x faster                                                      |
| unpickle                | 8.18 us                                                     | 7.98 us: 1.03x faster                                                      |
| sympy_expand            | 284 ms                                                      | 277 ms: 1.02x faster                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 479 ms: 1.02x faster                                                       |
| coroutines              | 14.3 ms                                                     | 14.0 ms: 1.02x faster                                                      |
| sympy_str               | 175 ms                                                      | 173 ms: 1.01x faster                                                       |
| spectral_norm           | 66.9 ms                                                     | 67.2 ms: 1.00x slower                                                      |
| sympy_integrate         | 13.0 ms                                                     | 13.1 ms: 1.01x slower                                                      |
| tornado_http            | 89.5 ms                                                     | 90.6 ms: 1.01x slower                                                      |
| pickle_dict             | 18.4 us                                                     | 18.7 us: 1.02x slower                                                      |
| sqlite_synth            | 1.76 us                                                     | 1.79 us: 1.02x slower                                                      |
| async_tree_io           | 731 ms                                                      | 744 ms: 1.02x slower                                                       |
| sqlglot_transpile       | 1.02 ms                                                     | 1.06 ms: 1.04x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.43 sec: 1.04x slower                                                     |
| async_tree_none         | 291 ms                                                      | 304 ms: 1.04x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 356 ms: 1.05x slower                                                       |
| sympy_sum               | 91.5 ms                                                     | 96.6 ms: 1.06x slower                                                      |
| sqlglot_parse           | 804 us                                                      | 871 us: 1.08x slower                                                       |
| comprehensions          | 14.1 us                                                     | 15.9 us: 1.13x slower                                                      |
| coverage                | 40.8 ms                                                     | 49.9 ms: 1.22x slower                                                      |
| dask                    | 263 ms                                                      | 352 ms: 1.34x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.05x faster                                                               |

Benchmark hidden because not significant (4): pickle_list, unpickle_list, scimark_lu, scimark_sparse_mat_mult
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230307-3.12.0a6-f9774e5/bm-20230307-pythonperf1-amd64-python-f9774e57d84162ff0cba-3.12.0a6-f9774e5.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.05x
- 95% likely to have a speedup of 1.04x
- 99% likely to have a speedup of 1.04x


# Memory

- memory change: unknown