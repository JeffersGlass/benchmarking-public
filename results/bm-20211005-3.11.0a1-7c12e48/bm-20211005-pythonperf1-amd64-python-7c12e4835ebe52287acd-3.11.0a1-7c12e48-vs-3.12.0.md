
# Results vs. 3.12.0

- fork: python
- ref: 7c12e4835ebe52287acd
- machine: windows-amd64
- commit hash: 7c12e48
- commit date: 2021-10-05
- overall geometric mean: 1.13x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.07x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 222 ms: 1.02x slower                                                       |
| chameleon      | 4.98 ms                                                     | 5.68 ms: 1.14x slower                                                      |
| docutils       | 1.66 sec                                                    | 1.73 sec: 1.04x slower                                                     |
| tornado_http   | 89.5 ms                                                     | 97.6 ms: 1.09x slower                                                      |
| Geometric mean | (ref)                                                       | 1.07x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_io           | 731 ms                                                      | 777 ms: 1.06x slower                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 541 ms: 1.11x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 384 ms: 1.13x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.08x slower                                                               |

Benchmark hidden because not significant (1): async_tree_none

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 150 ms: 1.01x faster                                                       |
| float          | 56.8 ms                                                     | 57.2 ms: 1.01x slower                                                      |
| nbody          | 71.9 ms                                                     | 86.8 ms: 1.21x slower                                                      |
| Geometric mean | (ref)                                                       | 1.06x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_v8       | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                                      |
| regex_dna      | 126 ms                                                      | 129 ms: 1.02x slower                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.66 ms: 1.03x slower                                                      |
| regex_compile  | 87.5 ms                                                     | 92.3 ms: 1.05x slower                                                      |
| Geometric mean | (ref)                                                       | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.58 us: 1.13x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 16.8 us: 1.10x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.56 us: 1.07x faster                                                      |
| pickle_list          | 2.83 us                                                     | 2.66 us: 1.06x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 54.8 ms: 1.02x faster                                                      |
| unpickle             | 8.18 us                                                     | 8.48 us: 1.04x slower                                                      |
| json_loads           | 13.9 us                                                     | 14.4 us: 1.04x slower                                                      |
| xml_etree_parse      | 93.0 ms                                                     | 98.4 ms: 1.06x slower                                                      |
| xml_etree_process    | 37.7 ms                                                     | 40.3 ms: 1.07x slower                                                      |
| pickle_pure_python   | 195 us                                                      | 240 us: 1.23x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 172 us: 1.29x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 8.03 ms: 1.41x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.05x slower                                                               |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                                      |
| python_startup         | 19.5 ms                                                     | 20.7 ms: 1.06x slower                                                      |
| Geometric mean         | (ref)                                                       | 1.01x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 25.8 ms: 1.13x slower                                                      |
| mako            | 7.09 ms                                                     | 8.12 ms: 1.15x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.14x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48 |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 198 ms: 1.21x faster                                                       |
| logging_simple          | 6.28 us                                                     | 5.24 us: 1.20x faster                                                      |
| logging_format          | 6.72 us                                                     | 5.64 us: 1.19x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.58 us: 1.13x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.37 ms: 1.11x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 63.0 ms: 1.10x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 16.8 us: 1.10x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 73.4 ms: 1.10x faster                                                      |
| unpickle_list           | 2.75 us                                                     | 2.56 us: 1.07x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.66 us: 1.06x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.6 ms: 1.04x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.98 ms: 1.04x faster                                                      |
| xml_etree_generate      | 55.8 ms                                                     | 54.8 ms: 1.02x faster                                                      |
| pidigits                | 152 ms                                                      | 150 ms: 1.01x faster                                                       |
| json                    | 3.05 ms                                                     | 3.01 ms: 1.01x faster                                                      |
| float                   | 56.8 ms                                                     | 57.2 ms: 1.01x slower                                                      |
| meteor_contest          | 74.6 ms                                                     | 75.3 ms: 1.01x slower                                                      |
| regex_v8                | 14.2 ms                                                     | 14.4 ms: 1.01x slower                                                      |
| regex_dna               | 126 ms                                                      | 129 ms: 1.02x slower                                                       |
| 2to3                    | 218 ms                                                      | 222 ms: 1.02x slower                                                       |
| sqlite_synth            | 1.76 us                                                     | 1.80 us: 1.02x slower                                                      |
| regex_effbot            | 1.62 ms                                                     | 1.66 ms: 1.03x slower                                                      |
| deepcopy_reduce         | 2.09 us                                                     | 2.16 us: 1.03x slower                                                      |
| unpickle                | 8.18 us                                                     | 8.48 us: 1.04x slower                                                      |
| json_loads              | 13.9 us                                                     | 14.4 us: 1.04x slower                                                      |
| docutils                | 1.66 sec                                                    | 1.73 sec: 1.04x slower                                                     |
| dulwich_log             | 44.3 ms                                                     | 46.1 ms: 1.04x slower                                                      |
| regex_compile           | 87.5 ms                                                     | 92.3 ms: 1.05x slower                                                      |
| xml_etree_parse         | 93.0 ms                                                     | 98.4 ms: 1.06x slower                                                      |
| async_tree_io           | 731 ms                                                      | 777 ms: 1.06x slower                                                       |
| python_startup          | 19.5 ms                                                     | 20.7 ms: 1.06x slower                                                      |
| bench_thread_pool       | 857 us                                                      | 915 us: 1.07x slower                                                       |
| xml_etree_process       | 37.7 ms                                                     | 40.3 ms: 1.07x slower                                                      |
| sympy_str               | 175 ms                                                      | 188 ms: 1.07x slower                                                       |
| create_gc_cycles        | 752 us                                                      | 807 us: 1.07x slower                                                       |
| sqlglot_normalize       | 187 ms                                                      | 201 ms: 1.07x slower                                                       |
| deepcopy                | 238 us                                                      | 256 us: 1.08x slower                                                       |
| nqueens                 | 62.8 ms                                                     | 67.7 ms: 1.08x slower                                                      |
| sympy_expand            | 284 ms                                                      | 309 ms: 1.09x slower                                                       |
| tornado_http            | 89.5 ms                                                     | 97.6 ms: 1.09x slower                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 37.8 ms: 1.10x slower                                                      |
| sympy_sum               | 91.5 ms                                                     | 100 ms: 1.10x slower                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 541 ms: 1.11x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 14.4 ms: 1.11x slower                                                      |
| pprint_safe_repr        | 513 ms                                                      | 570 ms: 1.11x slower                                                       |
| pprint_pformat          | 1.05 sec                                                    | 1.16 sec: 1.11x slower                                                     |
| pycparser               | 699 ms                                                      | 777 ms: 1.11x slower                                                       |
| unpack_sequence         | 37.5 ns                                                     | 41.7 ns: 1.11x slower                                                      |
| dask                    | 263 ms                                                      | 295 ms: 1.12x slower                                                       |
| django_template         | 22.9 ms                                                     | 25.8 ms: 1.13x slower                                                      |
| fannkuch                | 247 ms                                                      | 279 ms: 1.13x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 384 ms: 1.13x slower                                                       |
| chameleon               | 4.98 ms                                                     | 5.68 ms: 1.14x slower                                                      |
| mako                    | 7.09 ms                                                     | 8.12 ms: 1.15x slower                                                      |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.7 ms: 1.15x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.58 sec: 1.15x slower                                                     |
| raytrace                | 192 ms                                                      | 224 ms: 1.17x slower                                                       |
| scimark_fft             | 184 ms                                                      | 216 ms: 1.17x slower                                                       |
| go                      | 91.6 ms                                                     | 108 ms: 1.18x slower                                                       |
| crypto_pyaes            | 48.5 ms                                                     | 57.7 ms: 1.19x slower                                                      |
| scimark_monte_carlo     | 43.7 ms                                                     | 52.6 ms: 1.20x slower                                                      |
| deepcopy_memo           | 23.7 us                                                     | 28.6 us: 1.20x slower                                                      |
| nbody                   | 71.9 ms                                                     | 86.8 ms: 1.21x slower                                                      |
| richards                | 28.4 ms                                                     | 34.7 ms: 1.22x slower                                                      |
| pickle_pure_python      | 195 us                                                      | 240 us: 1.23x slower                                                       |
| pyflate                 | 295 ms                                                      | 365 ms: 1.24x slower                                                       |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 3.18 ms: 1.24x slower                                                      |
| coroutines              | 14.3 ms                                                     | 17.9 ms: 1.26x slower                                                      |
| hexiom                  | 4.10 ms                                                     | 5.17 ms: 1.26x slower                                                      |
| spectral_norm           | 66.9 ms                                                     | 84.7 ms: 1.27x slower                                                      |
| chaos                   | 43.3 ms                                                     | 55.0 ms: 1.27x slower                                                      |
| generators              | 22.5 ms                                                     | 28.9 ms: 1.28x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 172 us: 1.29x slower                                                       |
| asyncio_tcp             | 487 ms                                                      | 628 ms: 1.29x slower                                                       |
| scimark_sor             | 78.8 ms                                                     | 105 ms: 1.34x slower                                                       |
| comprehensions          | 14.1 us                                                     | 19.1 us: 1.36x slower                                                      |
| logging_silent          | 60.5 ns                                                     | 83.4 ns: 1.38x slower                                                      |
| json_dumps              | 5.70 ms                                                     | 8.03 ms: 1.41x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 83.6 ms: 1.42x slower                                                      |
| deltablue               | 2.16 ms                                                     | 3.12 ms: 1.44x slower                                                      |
| sqlglot_transpile       | 1.02 ms                                                     | 1.53 ms: 1.50x slower                                                      |
| sqlglot_parse           | 804 us                                                      | 1.32 ms: 1.64x slower                                                      |
| coverage                | 40.8 ms                                                     | 261 ms: 6.40x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.13x slower                                                               |

Benchmark hidden because not significant (3): sqlalchemy_declarative, xml_etree_iterparse, async_tree_none
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20211005-3.11.0a1-7c12e48/bm-20211005-pythonperf1-amd64-python-7c12e4835ebe52287acd-3.11.0a1-7c12e48.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.08x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.07x


# Memory

- memory change: unknown