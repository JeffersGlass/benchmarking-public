
# Results vs. 3.10.4

- fork: python
- ref: e2b4e4bab90b69fbd361
- machine: linux-x86_64
- commit hash: e2b4e4b
- commit date: 2021-11-05
- overall geometric mean: 1.13x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.08x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 299 ms: 1.17x faster                                                        |
| chameleon      | 9.44 ms                                                      | 9.27 ms: 1.02x faster                                                       |
| docutils       | 3.41 sec                                                     | 3.05 sec: 1.12x faster                                                      |
| html5lib       | 94.6 ms                                                      | 80.0 ms: 1.18x faster                                                       |
| tornado_http   | 157 ms                                                       | 136 ms: 1.16x faster                                                        |
| Geometric mean | (ref)                                                        | 1.13x faster                                                                |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 532 ms: 1.30x faster                                                        |
| async_tree_io           | 1.60 sec                                                     | 1.27 sec: 1.26x faster                                                      |
| async_tree_memoization  | 819 ms                                                       | 668 ms: 1.23x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 818 ms: 1.14x faster                                                        |
| Geometric mean          | (ref)                                                        | 1.23x faster                                                                |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 86.1 ms: 1.29x faster                                                       |
| nbody          | 134 ms                                                       | 113 ms: 1.19x faster                                                        |
| pidigits       | 271 ms                                                       | 264 ms: 1.02x faster                                                        |
| Geometric mean | (ref)                                                        | 1.16x faster                                                                |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 158 ms: 1.20x faster                                                        |
| regex_v8       | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                       |
| regex_effbot   | 3.09 ms                                                      | 3.06 ms: 1.01x faster                                                       |
| regex_dna      | 261 ms                                                       | 262 ms: 1.00x slower                                                        |
| Geometric mean | (ref)                                                        | 1.06x faster                                                                |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|----------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| json_loads           | 30.3 us                                                      | 24.7 us: 1.23x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 61.7 ms: 1.23x faster                                                       |
| pickle_pure_python   | 455 us                                                       | 386 us: 1.18x faster                                                        |
| unpickle_pure_python | 312 us                                                       | 277 us: 1.12x faster                                                        |
| json_dumps           | 14.5 ms                                                      | 13.4 ms: 1.08x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 85.8 ms: 1.08x faster                                                       |
| xml_etree_iterparse  | 110 ms                                                       | 107 ms: 1.03x faster                                                        |
| unpickle_list        | 4.65 us                                                      | 4.55 us: 1.02x faster                                                       |
| xml_etree_parse      | 160 ms                                                       | 157 ms: 1.02x faster                                                        |
| unpickle             | 13.5 us                                                      | 13.4 us: 1.01x faster                                                       |
| pickle_list          | 4.12 us                                                      | 4.17 us: 1.01x slower                                                       |
| pickle_dict          | 29.5 us                                                      | 30.2 us: 1.02x slower                                                       |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                       |
| Geometric mean       | (ref)                                                        | 1.07x faster                                                                |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 11.2 ms: 1.03x faster                                                       |
| python_startup_no_site | 7.33 ms                                                      | 7.43 ms: 1.01x slower                                                       |
| Geometric mean         | (ref)                                                        | 1.01x faster                                                                |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-----------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 12.9 ms: 1.14x faster                                                       |
| genshi_text     | 31.4 ms                                                      | 28.2 ms: 1.12x faster                                                       |
| genshi_xml      | 63.3 ms                                                      | 57.9 ms: 1.09x faster                                                       |
| django_template | 50.2 ms                                                      | 47.4 ms: 1.06x faster                                                       |
| Geometric mean  | (ref)                                                        | 1.10x faster                                                                |

All benchmarks:
===============

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20211105-pythonperf2-x86_64-python-e2b4e4bab90b69fbd361-3.11.0a2-e2b4e4b |
|-------------------------|:------------------------------------------------------------:|:---------------------------------------------------------------------------:|
| deltablue               | 7.50 ms                                                      | 5.07 ms: 1.48x faster                                                       |
| raytrace                | 489 ms                                                       | 349 ms: 1.40x faster                                                        |
| logging_silent          | 167 ns                                                       | 121 ns: 1.39x faster                                                        |
| chaos                   | 109 ms                                                       | 79.2 ms: 1.37x faster                                                       |
| scimark_monte_carlo     | 107 ms                                                       | 79.5 ms: 1.35x faster                                                       |
| go                      | 262 ms                                                       | 194 ms: 1.35x faster                                                        |
| spectral_norm           | 139 ms                                                       | 104 ms: 1.33x faster                                                        |
| unpack_sequence         | 59.9 ns                                                      | 46.0 ns: 1.30x faster                                                       |
| async_tree_none         | 692 ms                                                       | 532 ms: 1.30x faster                                                        |
| async_generators        | 421 ms                                                       | 325 ms: 1.29x faster                                                        |
| float                   | 111 ms                                                       | 86.1 ms: 1.29x faster                                                       |
| scimark_sor             | 180 ms                                                       | 140 ms: 1.29x faster                                                        |
| richards                | 75.1 ms                                                      | 59.0 ms: 1.27x faster                                                       |
| bench_mp_pool           | 6.37 ms                                                      | 5.01 ms: 1.27x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.27 sec: 1.26x faster                                                      |
| pyflate                 | 733 ms                                                       | 582 ms: 1.26x faster                                                        |
| scimark_lu              | 167 ms                                                       | 132 ms: 1.26x faster                                                        |
| crypto_pyaes            | 119 ms                                                       | 94.9 ms: 1.26x faster                                                       |
| json_loads              | 30.3 us                                                      | 24.7 us: 1.23x faster                                                       |
| xml_etree_process       | 75.9 ms                                                      | 61.7 ms: 1.23x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 668 ms: 1.23x faster                                                        |
| thrift                  | 1.18 ms                                                      | 961 us: 1.22x faster                                                        |
| logging_simple          | 8.88 us                                                      | 7.35 us: 1.21x faster                                                       |
| regex_compile           | 190 ms                                                       | 158 ms: 1.20x faster                                                        |
| hexiom                  | 9.42 ms                                                      | 7.87 ms: 1.20x faster                                                       |
| pprint_safe_repr        | 1.05 sec                                                     | 877 ms: 1.20x faster                                                        |
| logging_format          | 9.64 us                                                      | 8.08 us: 1.19x faster                                                       |
| nbody                   | 134 ms                                                       | 113 ms: 1.19x faster                                                        |
| html5lib                | 94.6 ms                                                      | 80.0 ms: 1.18x faster                                                       |
| gunicorn                | 1.16 ms                                                      | 980 us: 1.18x faster                                                        |
| pprint_pformat          | 2.15 sec                                                     | 1.82 sec: 1.18x faster                                                      |
| pickle_pure_python      | 455 us                                                       | 386 us: 1.18x faster                                                        |
| 2to3                    | 350 ms                                                       | 299 ms: 1.17x faster                                                        |
| scimark_fft             | 361 ms                                                       | 311 ms: 1.16x faster                                                        |
| deepcopy_memo           | 49.8 us                                                      | 42.9 us: 1.16x faster                                                       |
| tornado_http            | 157 ms                                                       | 136 ms: 1.16x faster                                                        |
| async_tree_cpu_io_mixed | 936 ms                                                       | 818 ms: 1.14x faster                                                        |
| mako                    | 14.7 ms                                                      | 12.9 ms: 1.14x faster                                                       |
| nqueens                 | 115 ms                                                       | 102 ms: 1.13x faster                                                        |
| json                    | 5.86 ms                                                      | 5.19 ms: 1.13x faster                                                       |
| pycparser               | 1.67 sec                                                     | 1.48 sec: 1.13x faster                                                      |
| unpickle_pure_python    | 312 us                                                       | 277 us: 1.12x faster                                                        |
| docutils                | 3.41 sec                                                     | 3.05 sec: 1.12x faster                                                      |
| dulwich_log             | 81.1 ms                                                      | 72.4 ms: 1.12x faster                                                       |
| genshi_text             | 31.4 ms                                                      | 28.2 ms: 1.12x faster                                                       |
| scimark_sparse_mat_mult | 5.08 ms                                                      | 4.56 ms: 1.11x faster                                                       |
| deepcopy                | 468 us                                                       | 428 us: 1.09x faster                                                        |
| genshi_xml              | 63.3 ms                                                      | 57.9 ms: 1.09x faster                                                       |
| generators              | 57.3 ms                                                      | 52.7 ms: 1.09x faster                                                       |
| bench_thread_pool       | 1.14 ms                                                      | 1.05 ms: 1.09x faster                                                       |
| sqlite_synth            | 2.99 us                                                      | 2.75 us: 1.09x faster                                                       |
| sqlglot_normalize       | 144 ms                                                       | 132 ms: 1.09x faster                                                        |
| json_dumps              | 14.5 ms                                                      | 13.4 ms: 1.08x faster                                                       |
| sqlglot_optimize        | 70.1 ms                                                      | 64.9 ms: 1.08x faster                                                       |
| meteor_contest          | 138 ms                                                       | 128 ms: 1.08x faster                                                        |
| xml_etree_generate      | 92.3 ms                                                      | 85.8 ms: 1.08x faster                                                       |
| pathlib                 | 21.4 ms                                                      | 20.0 ms: 1.07x faster                                                       |
| sympy_expand            | 600 ms                                                       | 563 ms: 1.06x faster                                                        |
| telco                   | 7.23 ms                                                      | 6.81 ms: 1.06x faster                                                       |
| sympy_integrate         | 28.2 ms                                                      | 26.5 ms: 1.06x faster                                                       |
| dask                    | 472 ms                                                       | 445 ms: 1.06x faster                                                        |
| django_template         | 50.2 ms                                                      | 47.4 ms: 1.06x faster                                                       |
| sympy_str               | 360 ms                                                       | 340 ms: 1.06x faster                                                        |
| create_gc_cycles        | 1.76 ms                                                      | 1.67 ms: 1.06x faster                                                       |
| fannkuch                | 483 ms                                                       | 458 ms: 1.05x faster                                                        |
| regex_v8                | 27.2 ms                                                      | 25.8 ms: 1.05x faster                                                       |
| deepcopy_reduce         | 4.01 us                                                      | 3.81 us: 1.05x faster                                                       |
| sympy_sum               | 193 ms                                                       | 183 ms: 1.05x faster                                                        |
| mdp                     | 3.01 sec                                                     | 2.87 sec: 1.05x faster                                                      |
| xml_etree_iterparse     | 110 ms                                                       | 107 ms: 1.03x faster                                                        |
| python_startup          | 11.5 ms                                                      | 11.2 ms: 1.03x faster                                                       |
| coroutines              | 30.3 ms                                                      | 29.5 ms: 1.03x faster                                                       |
| pidigits                | 271 ms                                                       | 264 ms: 1.02x faster                                                        |
| unpickle_list           | 4.65 us                                                      | 4.55 us: 1.02x faster                                                       |
| chameleon               | 9.44 ms                                                      | 9.27 ms: 1.02x faster                                                       |
| sqlglot_transpile       | 2.68 ms                                                      | 2.63 ms: 1.02x faster                                                       |
| xml_etree_parse         | 160 ms                                                       | 157 ms: 1.02x faster                                                        |
| unpickle                | 13.5 us                                                      | 13.4 us: 1.01x faster                                                       |
| regex_effbot            | 3.09 ms                                                      | 3.06 ms: 1.01x faster                                                       |
| regex_dna               | 261 ms                                                       | 262 ms: 1.00x slower                                                        |
| pickle_list             | 4.12 us                                                      | 4.17 us: 1.01x slower                                                       |
| python_startup_no_site  | 7.33 ms                                                      | 7.43 ms: 1.01x slower                                                       |
| pickle_dict             | 29.5 us                                                      | 30.2 us: 1.02x slower                                                       |
| pickle                  | 9.89 us                                                      | 10.3 us: 1.04x slower                                                       |
| comprehensions          | 26.7 us                                                      | 28.8 us: 1.08x slower                                                       |
| coverage                | 63.3 ms                                                      | 68.7 ms: 1.09x slower                                                       |
| flaskblogging           | 4.39 ms                                                      | 4.84 ms: 1.10x slower                                                       |
| gc_traversal            | 3.42 ms                                                      | 3.77 ms: 1.10x slower                                                       |
| Geometric mean          | (ref)                                                        | 1.13x faster                                                                |

Benchmark hidden because not significant (1): sqlglot_parse
Ignored benchmarks (11) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, asyncio_tcp, asyncio_tcp_ssl, asyncio_websockets, mypy2, pylint, richards_super, sqlalchemy_declarative, sqlalchemy_imperative, tomli_loads, typing_runtime_protocols


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.10x
- 95% likely to have a speedup of 1.09x
- 99% likely to have a speedup of 1.08x


# Memory

- memory change: 1.07x