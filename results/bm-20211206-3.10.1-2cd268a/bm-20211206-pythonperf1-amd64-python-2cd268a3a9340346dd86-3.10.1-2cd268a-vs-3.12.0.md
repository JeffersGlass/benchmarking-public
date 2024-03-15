
# Results vs. 3.12.0

- fork: python
- ref: 2cd268a3a9340346dd86
- machine: windows-amd64
- commit hash: 2cd268a
- commit date: 2021-12-06
- overall geometric mean: 1.15x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.09x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 232 ms: 1.07x slower                                                     |
| chameleon      | 4.98 ms                                                     | 5.89 ms: 1.18x slower                                                    |
| docutils       | 1.66 sec                                                    | 1.88 sec: 1.13x slower                                                   |
| tornado_http   | 89.5 ms                                                     | 109 ms: 1.22x slower                                                     |
| Geometric mean | (ref)                                                       | 1.15x slower                                                             |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| async_tree_cpu_io_mixed | 489 ms                                                      | 615 ms: 1.26x slower                                                     |
| async_tree_io           | 731 ms                                                      | 1.03 sec: 1.40x slower                                                   |
| async_tree_memoization  | 339 ms                                                      | 484 ms: 1.43x slower                                                     |
| async_tree_none         | 291 ms                                                      | 417 ms: 1.43x slower                                                     |
| Geometric mean          | (ref)                                                       | 1.38x slower                                                             |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 149 ms: 1.02x faster                                                     |
| nbody          | 71.9 ms                                                     | 77.2 ms: 1.07x slower                                                    |
| float          | 56.8 ms                                                     | 61.8 ms: 1.09x slower                                                    |
| Geometric mean | (ref)                                                       | 1.05x slower                                                             |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| regex_dna      | 126 ms                                                      | 129 ms: 1.02x slower                                                     |
| regex_v8       | 14.2 ms                                                     | 15.0 ms: 1.05x slower                                                    |
| regex_effbot   | 1.62 ms                                                     | 1.74 ms: 1.07x slower                                                    |
| regex_compile  | 87.5 ms                                                     | 103 ms: 1.18x slower                                                     |
| Geometric mean | (ref)                                                       | 1.08x slower                                                             |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|----------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| pickle               | 7.43 us                                                     | 6.84 us: 1.09x faster                                                    |
| pickle_dict          | 18.4 us                                                     | 17.0 us: 1.08x faster                                                    |
| pickle_list          | 2.83 us                                                     | 2.70 us: 1.05x faster                                                    |
| unpickle_list        | 2.75 us                                                     | 2.64 us: 1.04x faster                                                    |
| xml_etree_generate   | 55.8 ms                                                     | 55.0 ms: 1.02x faster                                                    |
| xml_etree_iterparse  | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                                    |
| xml_etree_parse      | 93.0 ms                                                     | 98.0 ms: 1.05x slower                                                    |
| json_loads           | 13.9 us                                                     | 15.0 us: 1.08x slower                                                    |
| xml_etree_process    | 37.7 ms                                                     | 44.0 ms: 1.17x slower                                                    |
| unpickle_pure_python | 133 us                                                      | 177 us: 1.33x slower                                                     |
| pickle_pure_python   | 195 us                                                      | 267 us: 1.37x slower                                                     |
| json_dumps           | 5.70 ms                                                     | 8.45 ms: 1.48x slower                                                    |
| Geometric mean       | (ref)                                                       | 1.08x slower                                                             |

Benchmark hidden because not significant (1): unpickle

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.1 ms: 1.08x faster                                                    |
| python_startup         | 19.5 ms                                                     | 19.7 ms: 1.01x slower                                                    |
| Geometric mean         | (ref)                                                       | 1.03x faster                                                             |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-----------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| mako            | 7.09 ms                                                     | 8.56 ms: 1.21x slower                                                    |
| django_template | 22.9 ms                                                     | 29.2 ms: 1.27x slower                                                    |
| Geometric mean  | (ref)                                                       | 1.24x slower                                                             |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a |
|-------------------------|:-----------------------------------------------------------:|:------------------------------------------------------------------------:|
| bench_mp_pool           | 69.2 ms                                                     | 60.4 ms: 1.15x faster                                                    |
| gc_traversal            | 1.52 ms                                                     | 1.37 ms: 1.11x faster                                                    |
| pickle                  | 7.43 us                                                     | 6.84 us: 1.09x faster                                                    |
| pickle_dict             | 18.4 us                                                     | 17.0 us: 1.08x faster                                                    |
| python_startup_no_site  | 16.2 ms                                                     | 15.1 ms: 1.08x faster                                                    |
| async_generators        | 239 ms                                                      | 224 ms: 1.07x faster                                                     |
| telco                   | 4.13 ms                                                     | 3.86 ms: 1.07x faster                                                    |
| pathlib                 | 80.5 ms                                                     | 75.9 ms: 1.06x faster                                                    |
| coverage                | 40.8 ms                                                     | 38.8 ms: 1.05x faster                                                    |
| pickle_list             | 2.83 us                                                     | 2.70 us: 1.05x faster                                                    |
| unpickle_list           | 2.75 us                                                     | 2.64 us: 1.04x faster                                                    |
| pidigits                | 152 ms                                                      | 149 ms: 1.02x faster                                                     |
| meteor_contest          | 74.6 ms                                                     | 73.2 ms: 1.02x faster                                                    |
| xml_etree_generate      | 55.8 ms                                                     | 55.0 ms: 1.02x faster                                                    |
| xml_etree_iterparse     | 65.2 ms                                                     | 64.6 ms: 1.01x faster                                                    |
| logging_simple          | 6.28 us                                                     | 6.24 us: 1.01x faster                                                    |
| python_startup          | 19.5 ms                                                     | 19.7 ms: 1.01x slower                                                    |
| create_gc_cycles        | 752 us                                                      | 770 us: 1.02x slower                                                     |
| regex_dna               | 126 ms                                                      | 129 ms: 1.02x slower                                                     |
| json                    | 3.05 ms                                                     | 3.13 ms: 1.03x slower                                                    |
| deepcopy_reduce         | 2.09 us                                                     | 2.15 us: 1.03x slower                                                    |
| nqueens                 | 62.8 ms                                                     | 65.5 ms: 1.04x slower                                                    |
| sqlite_synth            | 1.76 us                                                     | 1.85 us: 1.05x slower                                                    |
| regex_v8                | 14.2 ms                                                     | 15.0 ms: 1.05x slower                                                    |
| xml_etree_parse         | 93.0 ms                                                     | 98.0 ms: 1.05x slower                                                    |
| scimark_fft             | 184 ms                                                      | 195 ms: 1.06x slower                                                     |
| 2to3                    | 218 ms                                                      | 232 ms: 1.07x slower                                                     |
| deepcopy                | 238 us                                                      | 254 us: 1.07x slower                                                     |
| nbody                   | 71.9 ms                                                     | 77.2 ms: 1.07x slower                                                    |
| regex_effbot            | 1.62 ms                                                     | 1.74 ms: 1.07x slower                                                    |
| fannkuch                | 247 ms                                                      | 266 ms: 1.08x slower                                                     |
| json_loads              | 13.9 us                                                     | 15.0 us: 1.08x slower                                                    |
| unpack_sequence         | 37.5 ns                                                     | 40.5 ns: 1.08x slower                                                    |
| sqlglot_normalize       | 187 ms                                                      | 203 ms: 1.09x slower                                                     |
| float                   | 56.8 ms                                                     | 61.8 ms: 1.09x slower                                                    |
| sympy_str               | 175 ms                                                      | 191 ms: 1.09x slower                                                     |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 2.80 ms: 1.10x slower                                                    |
| dulwich_log             | 44.3 ms                                                     | 48.7 ms: 1.10x slower                                                    |
| sympy_expand            | 284 ms                                                      | 316 ms: 1.11x slower                                                     |
| coroutines              | 14.3 ms                                                     | 15.9 ms: 1.11x slower                                                    |
| aiohttp                 | 884 us                                                      | 990 us: 1.12x slower                                                     |
| comprehensions          | 14.1 us                                                     | 15.8 us: 1.12x slower                                                    |
| bench_thread_pool       | 857 us                                                      | 965 us: 1.13x slower                                                     |
| docutils                | 1.66 sec                                                    | 1.88 sec: 1.13x slower                                                   |
| sqlglot_optimize        | 34.5 ms                                                     | 39.2 ms: 1.14x slower                                                    |
| sqlalchemy_declarative  | 86.4 ms                                                     | 98.4 ms: 1.14x slower                                                    |
| sympy_sum               | 91.5 ms                                                     | 104 ms: 1.14x slower                                                     |
| sympy_integrate         | 13.0 ms                                                     | 14.9 ms: 1.15x slower                                                    |
| xml_etree_process       | 37.7 ms                                                     | 44.0 ms: 1.17x slower                                                    |
| pprint_safe_repr        | 513 ms                                                      | 601 ms: 1.17x slower                                                     |
| regex_compile           | 87.5 ms                                                     | 103 ms: 1.18x slower                                                     |
| chameleon               | 4.98 ms                                                     | 5.89 ms: 1.18x slower                                                    |
| spectral_norm           | 66.9 ms                                                     | 79.4 ms: 1.19x slower                                                    |
| pprint_pformat          | 1.05 sec                                                    | 1.24 sec: 1.19x slower                                                   |
| mako                    | 7.09 ms                                                     | 8.56 ms: 1.21x slower                                                    |
| deepcopy_memo           | 23.7 us                                                     | 28.7 us: 1.21x slower                                                    |
| dask                    | 263 ms                                                      | 319 ms: 1.21x slower                                                     |
| tornado_http            | 89.5 ms                                                     | 109 ms: 1.22x slower                                                     |
| sqlalchemy_imperative   | 9.29 ms                                                     | 11.4 ms: 1.22x slower                                                    |
| pycparser               | 699 ms                                                      | 861 ms: 1.23x slower                                                     |
| mdp                     | 1.37 sec                                                    | 1.72 sec: 1.25x slower                                                   |
| async_tree_cpu_io_mixed | 489 ms                                                      | 615 ms: 1.26x slower                                                     |
| django_template         | 22.9 ms                                                     | 29.2 ms: 1.27x slower                                                    |
| scimark_monte_carlo     | 43.7 ms                                                     | 56.9 ms: 1.30x slower                                                    |
| hexiom                  | 4.10 ms                                                     | 5.42 ms: 1.32x slower                                                    |
| unpickle_pure_python    | 133 us                                                      | 177 us: 1.33x slower                                                     |
| pyflate                 | 295 ms                                                      | 394 ms: 1.34x slower                                                     |
| scimark_sor             | 78.8 ms                                                     | 106 ms: 1.34x slower                                                     |
| crypto_pyaes            | 48.5 ms                                                     | 65.5 ms: 1.35x slower                                                    |
| generators              | 22.5 ms                                                     | 30.7 ms: 1.36x slower                                                    |
| pickle_pure_python      | 195 us                                                      | 267 us: 1.37x slower                                                     |
| chaos                   | 43.3 ms                                                     | 59.4 ms: 1.37x slower                                                    |
| async_tree_io           | 731 ms                                                      | 1.03 sec: 1.40x slower                                                   |
| scimark_lu              | 58.9 ms                                                     | 83.4 ms: 1.42x slower                                                    |
| raytrace                | 192 ms                                                      | 273 ms: 1.42x slower                                                     |
| sqlglot_transpile       | 1.02 ms                                                     | 1.45 ms: 1.42x slower                                                    |
| async_tree_memoization  | 339 ms                                                      | 484 ms: 1.43x slower                                                     |
| async_tree_none         | 291 ms                                                      | 417 ms: 1.43x slower                                                     |
| richards                | 28.4 ms                                                     | 40.9 ms: 1.44x slower                                                    |
| asyncio_tcp             | 487 ms                                                      | 713 ms: 1.46x slower                                                     |
| json_dumps              | 5.70 ms                                                     | 8.45 ms: 1.48x slower                                                    |
| sqlglot_parse           | 804 us                                                      | 1.21 ms: 1.50x slower                                                    |
| go                      | 91.6 ms                                                     | 137 ms: 1.50x slower                                                     |
| logging_silent          | 60.5 ns                                                     | 98.0 ns: 1.62x slower                                                    |
| deltablue               | 2.16 ms                                                     | 4.13 ms: 1.91x slower                                                    |
| Geometric mean          | (ref)                                                       | 1.15x slower                                                             |

Benchmark hidden because not significant (2): unpickle, logging_format
Ignored benchmarks (9) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20211206-3.10.1-2cd268a/bm-20211206-pythonperf1-amd64-python-2cd268a3a9340346dd86-3.10.1-2cd268a.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.12x
- 95% likely to have a slowdown of 1.11x
- 99% likely to have a slowdown of 1.09x


# Memory

- memory change: unknown