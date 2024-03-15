
# Results vs. 3.11.0

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: windows-amd64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.07x slower \*
- HPT reliability: 99.99%
- HPT 99th percentile: 1.01x slower
- Memory change: unknown

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 214 ms                                                      | 210 ms: 1.02x faster                                                       |
| chameleon      | 5.26 ms                                                     | 5.53 ms: 1.05x slower                                                      |
| docutils       | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                                     |
| html5lib       | 38.9 ms                                                     | 41.4 ms: 1.07x slower                                                      |
| tornado_http   | 92.8 ms                                                     | 98.3 ms: 1.06x slower                                                      |
| Geometric mean | (ref)                                                       | 1.04x slower                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none | 332 ms                                                      | 307 ms: 1.08x faster                                                       |
| async_tree_io   | 808 ms                                                      | 793 ms: 1.02x faster                                                       |
| Geometric mean  | (ref)                                                       | 1.03x faster                                                               |

Benchmark hidden because not significant (2): async_tree_memoization, async_tree_cpu_io_mixed

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pidigits       | 150 ms                                                      | 148 ms: 1.02x faster                                                       |
| float          | 54.4 ms                                                     | 56.1 ms: 1.03x slower                                                      |
| nbody          | 70.3 ms                                                     | 90.3 ms: 1.28x slower                                                      |
| Geometric mean | (ref)                                                       | 1.09x slower                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 91.0 ms                                                     | 90.4 ms: 1.01x faster                                                      |
| regex_dna      | 116 ms                                                      | 131 ms: 1.13x slower                                                       |
| regex_v8       | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                      |
| regex_effbot   | 1.50 ms                                                     | 1.82 ms: 1.21x slower                                                      |
| Geometric mean | (ref)                                                       | 1.12x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_dict          | 18.5 us                                                     | 16.2 us: 1.14x faster                                                      |
| pickle_list          | 2.70 us                                                     | 2.49 us: 1.08x faster                                                      |
| xml_etree_parse      | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                      |
| unpickle_list        | 2.59 us                                                     | 2.54 us: 1.02x faster                                                      |
| json_dumps           | 8.09 ms                                                     | 7.94 ms: 1.02x faster                                                      |
| pickle               | 6.64 us                                                     | 6.61 us: 1.00x faster                                                      |
| unpickle             | 7.57 us                                                     | 7.81 us: 1.03x slower                                                      |
| xml_etree_generate   | 52.5 ms                                                     | 54.7 ms: 1.04x slower                                                      |
| xml_etree_process    | 37.2 ms                                                     | 39.7 ms: 1.07x slower                                                      |
| unpickle_pure_python | 157 us                                                      | 168 us: 1.07x slower                                                       |
| pickle_pure_python   | 208 us                                                      | 228 us: 1.09x slower                                                       |
| json_loads           | 13.0 us                                                     | 14.9 us: 1.15x slower                                                      |
| Geometric mean       | (ref)                                                       | 1.01x slower                                                               |

Benchmark hidden because not significant (1): xml_etree_iterparse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup_no_site | 16.8 ms                                                     | 15.1 ms: 1.12x faster                                                      |
| python_startup         | 19.8 ms                                                     | 18.8 ms: 1.05x faster                                                      |
| Geometric mean         | (ref)                                                       | 1.08x faster                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| genshi_text     | 18.4 ms                                                     | 17.5 ms: 1.05x faster                                                      |
| genshi_xml      | 39.9 ms                                                     | 38.5 ms: 1.04x faster                                                      |
| mako            | 7.58 ms                                                     | 8.07 ms: 1.06x slower                                                      |
| django_template | 24.4 ms                                                     | 26.0 ms: 1.07x slower                                                      |
| Geometric mean  | (ref)                                                       | 1.01x slower                                                               |

All benchmarks:
===============

| Benchmark               | bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509 | bm-20211105-pythonperf1-amd64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:-----------------------------------------------------------:|:--------------------------------------------------------------------------:|
| logging_simple          | 6.86 us                                                     | 5.45 us: 1.26x faster                                                      |
| logging_format          | 7.16 us                                                     | 5.92 us: 1.21x faster                                                      |
| pickle_dict             | 18.5 us                                                     | 16.2 us: 1.14x faster                                                      |
| python_startup_no_site  | 16.8 ms                                                     | 15.1 ms: 1.12x faster                                                      |
| generators              | 34.0 ms                                                     | 31.0 ms: 1.10x faster                                                      |
| gc_traversal            | 1.49 ms                                                     | 1.37 ms: 1.09x faster                                                      |
| pickle_list             | 2.70 us                                                     | 2.49 us: 1.08x faster                                                      |
| async_tree_none         | 332 ms                                                      | 307 ms: 1.08x faster                                                       |
| genshi_text             | 18.4 ms                                                     | 17.5 ms: 1.05x faster                                                      |
| dulwich_log             | 46.4 ms                                                     | 44.1 ms: 1.05x faster                                                      |
| python_startup          | 19.8 ms                                                     | 18.8 ms: 1.05x faster                                                      |
| asyncio_tcp             | 726 ms                                                      | 695 ms: 1.04x faster                                                       |
| xml_etree_parse         | 97.6 ms                                                     | 93.8 ms: 1.04x faster                                                      |
| telco                   | 4.06 ms                                                     | 3.91 ms: 1.04x faster                                                      |
| create_gc_cycles        | 713 us                                                      | 686 us: 1.04x faster                                                       |
| genshi_xml              | 39.9 ms                                                     | 38.5 ms: 1.04x faster                                                      |
| bench_mp_pool           | 63.2 ms                                                     | 61.4 ms: 1.03x faster                                                      |
| unpickle_list           | 2.59 us                                                     | 2.54 us: 1.02x faster                                                      |
| json_dumps              | 8.09 ms                                                     | 7.94 ms: 1.02x faster                                                      |
| async_tree_io           | 808 ms                                                      | 793 ms: 1.02x faster                                                       |
| pidigits                | 150 ms                                                      | 148 ms: 1.02x faster                                                       |
| nqueens                 | 68.3 ms                                                     | 67.3 ms: 1.02x faster                                                      |
| 2to3                    | 214 ms                                                      | 210 ms: 1.02x faster                                                       |
| regex_compile           | 91.0 ms                                                     | 90.4 ms: 1.01x faster                                                      |
| pickle                  | 6.64 us                                                     | 6.61 us: 1.00x faster                                                      |
| logging_silent          | 71.8 ns                                                     | 72.1 ns: 1.00x slower                                                      |
| flaskblogging           | 2.03 sec                                                    | 2.05 sec: 1.01x slower                                                     |
| mdp                     | 1.59 sec                                                    | 1.61 sec: 1.01x slower                                                     |
| meteor_contest          | 75.2 ms                                                     | 76.2 ms: 1.01x slower                                                      |
| sqlite_synth            | 1.77 us                                                     | 1.80 us: 1.02x slower                                                      |
| sympy_sum               | 100 ms                                                      | 102 ms: 1.02x slower                                                       |
| sqlalchemy_imperative   | 10.4 ms                                                     | 10.6 ms: 1.02x slower                                                      |
| docutils                | 1.64 sec                                                    | 1.67 sec: 1.02x slower                                                     |
| sympy_integrate         | 14.0 ms                                                     | 14.4 ms: 1.02x slower                                                      |
| float                   | 54.4 ms                                                     | 56.1 ms: 1.03x slower                                                      |
| unpickle                | 7.57 us                                                     | 7.81 us: 1.03x slower                                                      |
| sympy_str               | 185 ms                                                      | 191 ms: 1.03x slower                                                       |
| sqlglot_normalize       | 190 ms                                                      | 196 ms: 1.03x slower                                                       |
| sqlalchemy_declarative  | 85.6 ms                                                     | 88.5 ms: 1.03x slower                                                      |
| pprint_safe_repr        | 529 ms                                                      | 547 ms: 1.03x slower                                                       |
| pprint_pformat          | 1.09 sec                                                    | 1.13 sec: 1.04x slower                                                     |
| pathlib                 | 70.9 ms                                                     | 73.4 ms: 1.04x slower                                                      |
| bench_thread_pool       | 872 us                                                      | 906 us: 1.04x slower                                                       |
| sympy_expand            | 299 ms                                                      | 311 ms: 1.04x slower                                                       |
| xml_etree_generate      | 52.5 ms                                                     | 54.7 ms: 1.04x slower                                                      |
| go                      | 101 ms                                                      | 106 ms: 1.05x slower                                                       |
| chameleon               | 5.26 ms                                                     | 5.53 ms: 1.05x slower                                                      |
| deltablue               | 2.70 ms                                                     | 2.86 ms: 1.06x slower                                                      |
| tornado_http            | 92.8 ms                                                     | 98.3 ms: 1.06x slower                                                      |
| mako                    | 7.58 ms                                                     | 8.07 ms: 1.06x slower                                                      |
| html5lib                | 38.9 ms                                                     | 41.4 ms: 1.07x slower                                                      |
| django_template         | 24.4 ms                                                     | 26.0 ms: 1.07x slower                                                      |
| xml_etree_process       | 37.2 ms                                                     | 39.7 ms: 1.07x slower                                                      |
| thrift                  | 494 us                                                      | 528 us: 1.07x slower                                                       |
| pycparser               | 720 ms                                                      | 769 ms: 1.07x slower                                                       |
| unpickle_pure_python    | 157 us                                                      | 168 us: 1.07x slower                                                       |
| deepcopy                | 246 us                                                      | 266 us: 1.08x slower                                                       |
| dask                    | 273 ms                                                      | 295 ms: 1.08x slower                                                       |
| richards                | 31.4 ms                                                     | 34.0 ms: 1.08x slower                                                      |
| async_generators        | 177 ms                                                      | 192 ms: 1.08x slower                                                       |
| deepcopy_memo           | 26.0 us                                                     | 28.1 us: 1.08x slower                                                      |
| deepcopy_reduce         | 2.06 us                                                     | 2.23 us: 1.08x slower                                                      |
| sqlglot_optimize        | 34.5 ms                                                     | 37.5 ms: 1.08x slower                                                      |
| fannkuch                | 253 ms                                                      | 275 ms: 1.09x slower                                                       |
| pickle_pure_python      | 208 us                                                      | 228 us: 1.09x slower                                                       |
| unpack_sequence         | 46.9 ns                                                     | 51.9 ns: 1.11x slower                                                      |
| hexiom                  | 4.55 ms                                                     | 5.06 ms: 1.11x slower                                                      |
| chaos                   | 48.4 ms                                                     | 53.9 ms: 1.11x slower                                                      |
| regex_dna               | 116 ms                                                      | 131 ms: 1.13x slower                                                       |
| scimark_monte_carlo     | 45.3 ms                                                     | 51.7 ms: 1.14x slower                                                      |
| pyflate                 | 312 ms                                                      | 358 ms: 1.15x slower                                                       |
| json_loads              | 13.0 us                                                     | 14.9 us: 1.15x slower                                                      |
| regex_v8                | 14.2 ms                                                     | 16.6 ms: 1.17x slower                                                      |
| scimark_fft             | 179 ms                                                      | 212 ms: 1.18x slower                                                       |
| crypto_pyaes            | 48.9 ms                                                     | 58.9 ms: 1.20x slower                                                      |
| coroutines              | 15.0 ms                                                     | 18.1 ms: 1.21x slower                                                      |
| spectral_norm           | 68.3 ms                                                     | 82.7 ms: 1.21x slower                                                      |
| regex_effbot            | 1.50 ms                                                     | 1.82 ms: 1.21x slower                                                      |
| comprehensions          | 15.6 us                                                     | 19.1 us: 1.22x slower                                                      |
| scimark_sparse_mat_mult | 2.58 ms                                                     | 3.18 ms: 1.23x slower                                                      |
| nbody                   | 70.3 ms                                                     | 90.3 ms: 1.28x slower                                                      |
| sqlglot_transpile       | 1.16 ms                                                     | 1.50 ms: 1.28x slower                                                      |
| scimark_lu              | 62.8 ms                                                     | 81.5 ms: 1.30x slower                                                      |
| scimark_sor             | 78.1 ms                                                     | 101 ms: 1.30x slower                                                       |
| sqlglot_parse           | 953 us                                                      | 1.29 ms: 1.36x slower                                                      |
| coverage                | 43.4 ms                                                     | 262 ms: 6.03x slower                                                       |
| Geometric mean          | (ref)                                                       | 1.07x slower                                                               |

Benchmark hidden because not significant (6): async_tree_memoization, pylint, xml_etree_iterparse, async_tree_cpu_io_mixed, raytrace, json
Ignored benchmarks (10) of results/bm-20221024-3.11.0-deaf509/bm-20221024-pythonperf1-amd64-python-v3.11.0-3.11.0-deaf509.json: aiohttp, async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_tcp_ssl, mypy2, richards_super, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 99.99% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: unknown