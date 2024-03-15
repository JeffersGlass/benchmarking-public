
# Results vs. 3.12.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: windows-amd64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.12x slower \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.06x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 218 ms                                                      | 210 ms: 1.04x faster                                                       |
| chameleon      | 4.98 ms                                                     | 5.53 ms: 1.11x slower                                                      |
| docutils       | 1.66 sec                                                    | 1.67 sec: 1.01x slower                                                     |
| tornado_http   | 89.5 ms                                                     | 98.3 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                       | 1.04x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 291 ms                                                      | 307 ms: 1.05x slower                                                       |
| async_tree_cpu_io_mixed | 489 ms                                                      | 530 ms: 1.08x slower                                                       |
| async_tree_io           | 731 ms                                                      | 793 ms: 1.08x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 395 ms: 1.17x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.10x slower                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 152 ms                                                      | 148 ms: 1.03x faster                                                       |
| float          | 56.8 ms                                                     | 56.1 ms: 1.01x faster                                                      |
| nbody          | 71.9 ms                                                     | 90.3 ms: 1.26x slower                                                      |
| Geometric mean | (ref)                                                       | 1.06x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 87.5 ms                                                     | 90.4 ms: 1.03x slower                                                      |
| regex_dna      | 126 ms                                                      | 131 ms: 1.04x slower                                                       |
| regex_effbot   | 1.62 ms                                                     | 1.82 ms: 1.12x slower                                                      |
| regex_v8       | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                      |
| Geometric mean | (ref)                                                       | 1.09x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_list          | 2.83 us                                                     | 2.49 us: 1.14x faster                                                      |
| pickle_dict          | 18.4 us                                                     | 16.2 us: 1.13x faster                                                      |
| pickle               | 7.43 us                                                     | 6.61 us: 1.13x faster                                                      |
| unpickle_list        | 2.75 us                                                     | 2.54 us: 1.08x faster                                                      |
| unpickle             | 8.18 us                                                     | 7.81 us: 1.05x faster                                                      |
| xml_etree_generate   | 55.8 ms                                                     | 54.7 ms: 1.02x faster                                                      |
| xml_etree_process    | 37.7 ms                                                     | 39.7 ms: 1.05x slower                                                      |
| json_loads           | 13.9 us                                                     | 14.9 us: 1.07x slower                                                      |
| pickle_pure_python   | 195 us                                                      | 228 us: 1.16x slower                                                       |
| unpickle_pure_python | 133 us                                                      | 168 us: 1.26x slower                                                       |
| json_dumps           | 5.70 ms                                                     | 7.94 ms: 1.39x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.03x slower                                                               |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.2 ms                                                     | 15.1 ms: 1.08x faster                                                      |
| python_startup         | 19.5 ms                                                     | 18.8 ms: 1.03x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.06x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| django_template | 22.9 ms                                                     | 26.0 ms: 1.14x slower                                                      |
| mako            | 7.09 ms                                                     | 8.07 ms: 1.14x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.14x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_generators        | 239 ms                                                      | 192 ms: 1.25x faster                                                       |
| logging_simple          | 6.28 us                                                     | 5.45 us: 1.15x faster                                                      |
| pickle_list             | 2.83 us                                                     | 2.49 us: 1.14x faster                                                      |
| logging_format          | 6.72 us                                                     | 5.92 us: 1.13x faster                                                      |
| pickle_dict             | 18.4 us                                                     | 16.2 us: 1.13x faster                                                      |
| bench_mp_pool           | 69.2 ms                                                     | 61.4 ms: 1.13x faster                                                      |
| pickle                  | 7.43 us                                                     | 6.61 us: 1.13x faster                                                      |
| gc_traversal            | 1.52 ms                                                     | 1.37 ms: 1.11x faster                                                      |
| pathlib                 | 80.5 ms                                                     | 73.4 ms: 1.10x faster                                                      |
| create_gc_cycles        | 752 us                                                      | 686 us: 1.10x faster                                                       |
| unpickle_list           | 2.75 us                                                     | 2.54 us: 1.08x faster                                                      |
| python_startup_no_site  | 16.2 ms                                                     | 15.1 ms: 1.08x faster                                                      |
| telco                   | 4.13 ms                                                     | 3.91 ms: 1.06x faster                                                      |
| unpickle                | 8.18 us                                                     | 7.81 us: 1.05x faster                                                      |
| 2to3                    | 218 ms                                                      | 210 ms: 1.04x faster                                                       |
| python_startup          | 19.5 ms                                                     | 18.8 ms: 1.03x faster                                                      |
| pidigits                | 152 ms                                                      | 148 ms: 1.03x faster                                                       |
| xml_etree_generate      | 55.8 ms                                                     | 54.7 ms: 1.02x faster                                                      |
| float                   | 56.8 ms                                                     | 56.1 ms: 1.01x faster                                                      |
| dulwich_log             | 44.3 ms                                                     | 44.1 ms: 1.00x faster                                                      |
| json                    | 3.05 ms                                                     | 3.06 ms: 1.01x slower                                                      |
| docutils                | 1.66 sec                                                    | 1.67 sec: 1.01x slower                                                     |
| sqlite_synth            | 1.76 us                                                     | 1.80 us: 1.02x slower                                                      |
| meteor_contest          | 74.6 ms                                                     | 76.2 ms: 1.02x slower                                                      |
| sqlalchemy_declarative  | 86.4 ms                                                     | 88.5 ms: 1.02x slower                                                      |
| regex_compile           | 87.5 ms                                                     | 90.4 ms: 1.03x slower                                                      |
| regex_dna               | 126 ms                                                      | 131 ms: 1.04x slower                                                       |
| sqlglot_normalize       | 187 ms                                                      | 196 ms: 1.05x slower                                                       |
| xml_etree_process       | 37.7 ms                                                     | 39.7 ms: 1.05x slower                                                      |
| async_tree_none         | 291 ms                                                      | 307 ms: 1.05x slower                                                       |
| bench_thread_pool       | 857 us                                                      | 906 us: 1.06x slower                                                       |
| pprint_safe_repr        | 513 ms                                                      | 547 ms: 1.07x slower                                                       |
| deepcopy_reduce         | 2.09 us                                                     | 2.23 us: 1.07x slower                                                      |
| nqueens                 | 62.8 ms                                                     | 67.3 ms: 1.07x slower                                                      |
| json_loads              | 13.9 us                                                     | 14.9 us: 1.07x slower                                                      |
| pprint_pformat          | 1.05 sec                                                    | 1.13 sec: 1.08x slower                                                     |
| async_tree_cpu_io_mixed | 489 ms                                                      | 530 ms: 1.08x slower                                                       |
| async_tree_io           | 731 ms                                                      | 793 ms: 1.08x slower                                                       |
| sqlglot_optimize        | 34.5 ms                                                     | 37.5 ms: 1.09x slower                                                      |
| sympy_str               | 175 ms                                                      | 191 ms: 1.09x slower                                                       |
| sympy_expand            | 284 ms                                                      | 311 ms: 1.10x slower                                                       |
| tornado_http            | 89.5 ms                                                     | 98.3 ms: 1.10x slower                                                      |
| pycparser               | 699 ms                                                      | 769 ms: 1.10x slower                                                       |
| sympy_integrate         | 13.0 ms                                                     | 14.4 ms: 1.11x slower                                                      |
| chameleon               | 4.98 ms                                                     | 5.53 ms: 1.11x slower                                                      |
| raytrace                | 192 ms                                                      | 214 ms: 1.11x slower                                                       |
| sympy_sum               | 91.5 ms                                                     | 102 ms: 1.11x slower                                                       |
| fannkuch                | 247 ms                                                      | 275 ms: 1.11x slower                                                       |
| deepcopy                | 238 us                                                      | 266 us: 1.12x slower                                                       |
| dask                    | 263 ms                                                      | 295 ms: 1.12x slower                                                       |
| regex_effbot            | 1.62 ms                                                     | 1.82 ms: 1.12x slower                                                      |
| django_template         | 22.9 ms                                                     | 26.0 ms: 1.14x slower                                                      |
| mako                    | 7.09 ms                                                     | 8.07 ms: 1.14x slower                                                      |
| sqlalchemy_imperative   | 9.29 ms                                                     | 10.6 ms: 1.14x slower                                                      |
| scimark_fft             | 184 ms                                                      | 212 ms: 1.15x slower                                                       |
| go                      | 91.6 ms                                                     | 106 ms: 1.16x slower                                                       |
| pickle_pure_python      | 195 us                                                      | 228 us: 1.16x slower                                                       |
| async_tree_memoization  | 339 ms                                                      | 395 ms: 1.17x slower                                                       |
| regex_v8                | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                      |
| mdp                     | 1.37 sec                                                    | 1.61 sec: 1.18x slower                                                     |
| scimark_monte_carlo     | 43.7 ms                                                     | 51.7 ms: 1.18x slower                                                      |
| deepcopy_memo           | 23.7 us                                                     | 28.1 us: 1.19x slower                                                      |
| logging_silent          | 60.5 ns                                                     | 72.1 ns: 1.19x slower                                                      |
| richards                | 28.4 ms                                                     | 34.0 ms: 1.20x slower                                                      |
| crypto_pyaes            | 48.5 ms                                                     | 58.9 ms: 1.21x slower                                                      |
| pyflate                 | 295 ms                                                      | 358 ms: 1.21x slower                                                       |
| hexiom                  | 4.10 ms                                                     | 5.06 ms: 1.23x slower                                                      |
| spectral_norm           | 66.9 ms                                                     | 82.7 ms: 1.24x slower                                                      |
| scimark_sparse_mat_mult | 2.56 ms                                                     | 3.18 ms: 1.24x slower                                                      |
| chaos                   | 43.3 ms                                                     | 53.9 ms: 1.24x slower                                                      |
| nbody                   | 71.9 ms                                                     | 90.3 ms: 1.26x slower                                                      |
| unpickle_pure_python    | 133 us                                                      | 168 us: 1.26x slower                                                       |
| coroutines              | 14.3 ms                                                     | 18.1 ms: 1.27x slower                                                      |
| scimark_sor             | 78.8 ms                                                     | 101 ms: 1.29x slower                                                       |
| deltablue               | 2.16 ms                                                     | 2.86 ms: 1.32x slower                                                      |
| comprehensions          | 14.1 us                                                     | 19.1 us: 1.35x slower                                                      |
| generators              | 22.5 ms                                                     | 31.0 ms: 1.37x slower                                                      |
| scimark_lu              | 58.9 ms                                                     | 81.5 ms: 1.38x slower                                                      |
| unpack_sequence         | 37.5 ns                                                     | 51.9 ns: 1.38x slower                                                      |
| json_dumps              | 5.70 ms                                                     | 7.94 ms: 1.39x slower                                                      |
| asyncio_tcp             | 487 ms                                                      | 695 ms: 1.43x slower                                                       |
| sqlglot_transpile       | 1.02 ms                                                     | 1.50 ms: 1.46x slower                                                      |
| sqlglot_parse           | 804 us                                                      | 1.29 ms: 1.61x slower                                                      |
| coverage                | 40.8 ms                                                     | 262 ms: 6.42x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.12x slower                                                               |

Benchmark hidden because not significant (2): xml_etree_iterparse, xml_etree_parse
Ignored benchmarks (10) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-pythonperf1-amd64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols
Ignored benchmarks (6) of results/bm-20211105-3.11.0a2-e2b4e4b/bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b.json: flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.07x
- 95% likely to have a slowdown of 1.07x
- 99% likely to have a slowdown of 1.06x


# Memory

- memory change: unknown