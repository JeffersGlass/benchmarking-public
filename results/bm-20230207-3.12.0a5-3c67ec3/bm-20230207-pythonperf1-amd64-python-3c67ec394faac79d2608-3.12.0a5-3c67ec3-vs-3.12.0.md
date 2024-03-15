
# Results vs. 3.12.0

- fork: python
- ref: 3c67ec394faac79d2608
- machine: windows-amd64
- commit hash: 3c67ec3
- commit date: 2023-02-07
- overall geometric mean: 1.07x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.05x faster
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 192 ms: 1.14x faster                                                       |
| chameleon      | 4.98 ms                                                     | 4.41 ms: 1.13x faster                                                      |
| docutils       | 1.66 sec                                                    | 1.50 sec: 1.11x faster                                                     |
| tornado_http   | 89.5 ms                                                     | 90.5 ms: 1.01x slower                                                      |
| Geometric mean | (ref)                                                       | 1.09x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 480 ms: 1.02x faster                                                       |
| async_tree_io           | 731 ms                                                      | 748 ms: 1.02x slower                                                       |
| async_tree_none         | 291 ms                                                      | 302 ms: 1.04x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 356 ms: 1.05x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.02x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| nbody          | 71.9 ms                                                     | 59.1 ms: 1.22x faster                                                      |
| float          | 56.8 ms                                                     | 47.3 ms: 1.20x faster                                                      |
| pidigits       | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                       | 1.15x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 78.8 ms: 1.11x faster                                                      |
| regex_dna      | 126 ms                                                      | 121 ms: 1.04x faster                                                       |
| regex_v8       | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| regex_effbot   | 1.62 ms                                                     | 1.68 ms: 1.04x slower                                                      |
| Geometric mean | (ref)                                                       | 1.04x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 195 us                                                      | 166 us: 1.18x faster                                                       |
| xml_etree_generate   | 55.8 ms                                                     | 49.5 ms: 1.13x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 33.5 ms: 1.13x faster                                                      |
| unpickle_pure_python | 133 us                                                      | 120 us: 1.11x faster                                                       |
| pickle               | 7.43 us                                                     | 6.77 us: 1.10x faster                                                      |
| json_dumps           | 5.70 ms                                                     | 5.38 ms: 1.06x faster                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 88.5 ms: 1.05x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.70 us: 1.05x faster                                                      |
| xml_etree_iterparse  | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.65 us: 1.04x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 18.5 us: 1.01x slower                                                      |
| json_loads           | 13.9 us                                                     | 14.2 us: 1.02x slower                                                      |
| unpickle             | 8.18 us                                                     | 9.39 us: 1.15x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.05x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| python_startup_no_site | 16.2 ms                                                     | 15.5 ms: 1.05x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 6.15 ms: 1.15x faster                                                      |
| django_template | 22.9 ms                                                     | 20.2 ms: 1.14x faster                                                      |
| Geometric mean  | (ref)                                                       | 1.14x faster                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| unpack_sequence         | 37.5 ns                                                     | 25.6 ns: 1.46x faster                                                      |
| async_generators        | 239 ms                                                      | 167 ms: 1.43x faster                                                       |
| nbody                   | 71.9 ms                                                     | 59.1 ms: 1.22x faster                                                      |
| comprehensions          | 14.1 us                                                     | 11.7 us: 1.21x faster                                                      |
| float                   | 56.8 ms                                                     | 47.3 ms: 1.20x faster                                                      |
| richards                | 28.4 ms                                                     | 23.9 ms: 1.19x faster                                                      |
| pickle_pure_python      | 195 us                                                      | 166 us: 1.18x faster                                                       |
| scimark_sor             | 78.8 ms                                                     | 67.0 ms: 1.18x faster                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.18 ms: 1.17x faster                                                      |
| go                      | 91.6 ms                                                     | 78.8 ms: 1.16x faster                                                      |
| fannkuch                | 247 ms                                                      | 213 ms: 1.16x faster                                                       |
| scimark_monte_carlo     | 43.7 ms                                                     | 37.9 ms: 1.15x faster                                                      |
| pprint_safe_repr        | 513 ms                                                      | 445 ms: 1.15x faster                                                       |
| mako                    | 7.09 ms                                                     | 6.15 ms: 1.15x faster                                                      |
| pprint_pformat          | 1.05 sec                                                    | 907 ms: 1.15x faster                                                       |
| nqueens                 | 62.8 ms                                                     | 54.6 ms: 1.15x faster                                                      |
| django_template         | 22.9 ms                                                     | 20.2 ms: 1.14x faster                                                      |
| 2to3                    | 218 ms                                                      | 192 ms: 1.14x faster                                                       |
| chameleon               | 4.98 ms                                                     | 4.41 ms: 1.13x faster                                                      |
| raytrace                | 192 ms                                                      | 170 ms: 1.13x faster                                                       |
| xml_etree_generate      | 55.8 ms                                                     | 49.5 ms: 1.13x faster                                                      |
| deepcopy                | 238 us                                                      | 211 us: 1.13x faster                                                       |
| xml_etree_process       | 37.7 ms                                                     | 33.5 ms: 1.13x faster                                                      |
| deepcopy_memo           | 23.7 us                                                     | 21.1 us: 1.12x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 61.7 ms: 1.12x faster                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 1.88 us: 1.11x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 676 us: 1.11x faster                                                       |
| unpickle_pure_python    | 133 us                                                      | 120 us: 1.11x faster                                                       |
| scimark_fft             | 184 ms                                                      | 166 ms: 1.11x faster                                                       |
| regex_compile           | 87.5 ms                                                     | 78.8 ms: 1.11x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.72 ms: 1.11x faster                                                      |
| docutils                | 1.66 sec                                                    | 1.50 sec: 1.11x faster                                                     |
| deltablue               | 2.16 ms                                                     | 1.96 ms: 1.10x faster                                                      |
| pycparser               | 699 ms                                                      | 633 ms: 1.10x faster                                                       |
| pyflate                 | 295 ms                                                      | 267 ms: 1.10x faster                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 44.0 ms: 1.10x faster                                                      |
| hexiom                  | 4.10 ms                                                     | 3.73 ms: 1.10x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.77 us: 1.10x faster                                                      |
| sqlglot_normalize       | 187 ms                                                      | 171 ms: 1.10x faster                                                       |
| chaos                   | 43.3 ms                                                     | 39.6 ms: 1.09x faster                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 31.6 ms: 1.09x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 73.7 ms: 1.09x faster                                                      |
| spectral_norm           | 66.9 ms                                                     | 61.5 ms: 1.09x faster                                                      |
| json                    | 3.05 ms                                                     | 2.81 ms: 1.08x faster                                                      |
| meteor_contest          | 74.6 ms                                                     | 69.1 ms: 1.08x faster                                                      |
| sympy_str               | 175 ms                                                      | 164 ms: 1.07x faster                                                       |
| logging_format          | 6.72 us                                                     | 6.28 us: 1.07x faster                                                      |
| python_startup          | 19.5 ms                                                     | 18.2 ms: 1.07x faster                                                      |
| json_dumps              | 5.70 ms                                                     | 5.38 ms: 1.06x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 41.9 ms: 1.06x faster                                                      |
| sympy_expand            | 284 ms                                                      | 269 ms: 1.05x faster                                                       |
| xml_etree_parse         | 93.0 ms                                                     | 88.5 ms: 1.05x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.5 ms: 1.05x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.45 ms: 1.05x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.70 us: 1.05x faster                                                      |
| xml_etree_iterparse     | 65.2 ms                                                     | 62.3 ms: 1.05x faster                                                      |
| sympy_integrate         | 13.0 ms                                                     | 12.4 ms: 1.05x faster                                                      |
| asyncio_tcp             | 487 ms                                                      | 466 ms: 1.05x faster                                                       |
| logging_simple          | 6.28 us                                                     | 6.01 us: 1.04x faster                                                      |
| regex_dna               | 126 ms                                                      | 121 ms: 1.04x faster                                                       |
| pidigits                | 152 ms                                                      | 146 ms: 1.04x faster                                                       |
| regex_v8                | 14.2 ms                                                     | 13.7 ms: 1.04x faster                                                      |
| logging_silent          | 60.5 ns                                                     | 58.1 ns: 1.04x faster                                                      |
| bench_thread_pool       | 857 us                                                      | 823 us: 1.04x faster                                                       |
| unpickle_list           | 2.75 us                                                     | 2.65 us: 1.04x faster                                                      |
| sympy_sum               | 91.5 ms                                                     | 89.5 ms: 1.02x faster                                                      |
| async_tree_cpu_io_mixed | 489 ms                                                      | 480 ms: 1.02x faster                                                       |
| pickle_dict             | 18.4 us                                                     | 18.5 us: 1.01x slower                                                      |
| tornado_http            | 89.5 ms                                                     | 90.5 ms: 1.01x slower                                                      |
| json_loads              | 13.9 us                                                     | 14.2 us: 1.02x slower                                                      |
| async_tree_io           | 731 ms                                                      | 748 ms: 1.02x slower                                                       |
| sqlglot_transpile       | 1.02 ms                                                     | 1.05 ms: 1.03x slower                                                      |
| async_tree_none         | 291 ms                                                      | 302 ms: 1.04x slower                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.82 us: 1.04x slower                                                      |
| coroutines              | 14.3 ms                                                     | 14.8 ms: 1.04x slower                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.68 ms: 1.04x slower                                                      |
| async_tree_memoization  | 339 ms                                                      | 356 ms: 1.05x slower                                                       |
| sqlglot_parse           | 804 us                                                      | 851 us: 1.06x slower                                                       |
| mdp                     | 1.37 sec                                                    | 1.48 sec: 1.08x slower                                                     |
| unpickle                | 8.18 us                                                     | 9.39 us: 1.15x slower                                                      |
| coverage                | 40.8 ms                                                     | 51.8 ms: 1.27x slower                                                      |
| dask                    | 263 ms                                                      | 349 ms: 1.33x slower                                                       |
| generators              | 22.5 ms                                                     | 33.0 ms: 1.47x slower                                                      |
| Geometric mean          | (ref)                                                       | 1.07x faster                                                               |

Benchmark hidden because not significant (1): scimark_lu
Ignored benchmarks (12) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols
Ignored benchmarks (4) of results/bm-20230207-3.12.0a5-3c67ec3/bm-20230207-pythonperf1-amd64-python-3c67ec394faac79d2608-3.12.0a5-3c67ec3.json: genshi_text, genshi_xml, html5lib, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.06x
- 95% likely to have a speedup of 1.06x
- 99% likely to have a speedup of 1.05x


# Memory

- memory change: unknown