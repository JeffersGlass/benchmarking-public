# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_jumps
- machine: linux-x86_64
- commit hash: 594cca3
- commit date: 2024-02-29
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.36x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 307 ms: 1.14x faster                                                       |
| chameleon      | 9.44 ms                                                      | 7.48 ms: 1.26x faster                                                      |
| docutils       | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                     |
| tornado_http   | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                        | 1.21x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 443 ms: 1.56x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 560 ms: 1.46x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                     |
| async_tree_cpu_io_mixed | 936 ms                                                       | 711 ms: 1.32x faster                                                       |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 78.4 ms: 1.42x faster                                                      |
| nbody          | 134 ms                                                       | 101 ms: 1.33x faster                                                       |
| pidigits       | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| Geometric mean | (ref)                                                        | 1.25x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 148 ms: 1.28x faster                                                       |
| regex_dna      | 261 ms                                                       | 237 ms: 1.10x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                      |
| regex_effbot   | 3.09 ms                                                      | 3.63 ms: 1.18x slower                                                      |
| Geometric mean | (ref)                                                        | 1.07x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 317 us: 1.43x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                      |
| tomli_loads          | 2.92 sec                                                     | 2.14 sec: 1.36x faster                                                     |
| unpickle_pure_python | 312 us                                                       | 233 us: 1.34x faster                                                       |
| xml_etree_process    | 75.9 ms                                                      | 58.0 ms: 1.31x faster                                                      |
| json_loads           | 30.3 us                                                      | 25.5 us: 1.19x faster                                                      |
| xml_etree_parse      | 160 ms                                                       | 146 ms: 1.10x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                      |
| xml_etree_iterparse  | 110 ms                                                       | 103 ms: 1.07x faster                                                       |
| unpickle_list        | 4.65 us                                                      | 4.72 us: 1.02x slower                                                      |
| pickle_dict          | 29.5 us                                                      | 30.5 us: 1.03x slower                                                      |
| pickle_list          | 4.12 us                                                      | 4.28 us: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| unpickle             | 13.5 us                                                      | 15.5 us: 1.15x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.13x faster                                                               |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 15.5 ms: 1.35x slower                                                      |
| python_startup_no_site | 7.33 ms                                                      | 14.1 ms: 1.92x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.61x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|-----------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako      | 14.7 ms                                                      | 10.00 ms: 1.47x faster                                                     |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 123 us: 4.35x faster                                                       |
| asyncio_tcp              | 779 ms                                                       | 376 ms: 2.07x faster                                                       |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.96x faster                                                     |
| deltablue                | 7.50 ms                                                      | 3.83 ms: 1.96x faster                                                      |
| generators               | 57.3 ms                                                      | 33.4 ms: 1.71x faster                                                      |
| logging_silent           | 167 ns                                                       | 99.0 ns: 1.69x faster                                                      |
| raytrace                 | 489 ms                                                       | 300 ms: 1.63x faster                                                       |
| chaos                    | 109 ms                                                       | 67.2 ms: 1.61x faster                                                      |
| async_tree_none          | 692 ms                                                       | 443 ms: 1.56x faster                                                       |
| sqlglot_parse            | 2.24 ms                                                      | 1.43 ms: 1.56x faster                                                      |
| richards_super           | 90.6 ms                                                      | 58.3 ms: 1.55x faster                                                      |
| crypto_pyaes             | 119 ms                                                       | 77.0 ms: 1.55x faster                                                      |
| spectral_norm            | 139 ms                                                       | 92.9 ms: 1.50x faster                                                      |
| go                       | 262 ms                                                       | 176 ms: 1.49x faster                                                       |
| mako                     | 14.7 ms                                                      | 10.00 ms: 1.47x faster                                                     |
| richards                 | 75.1 ms                                                      | 51.2 ms: 1.47x faster                                                      |
| async_tree_memoization   | 819 ms                                                       | 560 ms: 1.46x faster                                                       |
| async_tree_io            | 1.60 sec                                                     | 1.10 sec: 1.46x faster                                                     |
| sqlglot_transpile        | 2.68 ms                                                      | 1.86 ms: 1.45x faster                                                      |
| pickle_pure_python       | 455 us                                                       | 317 us: 1.43x faster                                                       |
| comprehensions           | 26.7 us                                                      | 18.7 us: 1.43x faster                                                      |
| float                    | 111 ms                                                       | 78.4 ms: 1.42x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.5 ms: 1.39x faster                                                      |
| pyflate                  | 733 ms                                                       | 529 ms: 1.39x faster                                                       |
| scimark_monte_carlo      | 107 ms                                                       | 77.7 ms: 1.38x faster                                                      |
| tomli_loads              | 2.92 sec                                                     | 2.14 sec: 1.36x faster                                                     |
| coroutines               | 30.3 ms                                                      | 22.3 ms: 1.36x faster                                                      |
| scimark_lu               | 167 ms                                                       | 124 ms: 1.35x faster                                                       |
| logging_simple           | 8.88 us                                                      | 6.60 us: 1.34x faster                                                      |
| unpickle_pure_python     | 312 us                                                       | 233 us: 1.34x faster                                                       |
| nbody                    | 134 ms                                                       | 101 ms: 1.33x faster                                                       |
| logging_format           | 9.64 us                                                      | 7.28 us: 1.32x faster                                                      |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 711 ms: 1.32x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 58.0 ms: 1.31x faster                                                      |
| regex_compile            | 190 ms                                                       | 148 ms: 1.28x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 7.34 ms: 1.28x faster                                                      |
| tornado_http             | 157 ms                                                       | 124 ms: 1.26x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.48 ms: 1.26x faster                                                      |
| pycparser                | 1.67 sec                                                     | 1.33 sec: 1.26x faster                                                     |
| deepcopy_memo            | 49.8 us                                                      | 39.6 us: 1.26x faster                                                      |
| pprint_safe_repr         | 1.05 sec                                                     | 843 ms: 1.24x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.76 sec: 1.23x faster                                                     |
| fannkuch                 | 483 ms                                                       | 394 ms: 1.22x faster                                                       |
| sqlglot_normalize        | 144 ms                                                       | 118 ms: 1.22x faster                                                       |
| sympy_sum                | 193 ms                                                       | 159 ms: 1.21x faster                                                       |
| deepcopy                 | 468 us                                                       | 389 us: 1.20x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.35 us: 1.20x faster                                                      |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.25 ms: 1.19x faster                                                      |
| json_loads               | 30.3 us                                                      | 25.5 us: 1.19x faster                                                      |
| sympy_str                | 360 ms                                                       | 302 ms: 1.19x faster                                                       |
| dulwich_log              | 81.1 ms                                                      | 69.1 ms: 1.17x faster                                                      |
| docutils                 | 3.41 sec                                                     | 2.92 sec: 1.17x faster                                                     |
| scimark_sor              | 180 ms                                                       | 155 ms: 1.17x faster                                                       |
| sympy_expand             | 600 ms                                                       | 517 ms: 1.16x faster                                                       |
| nqueens                  | 115 ms                                                       | 99.1 ms: 1.16x faster                                                      |
| bench_thread_pool        | 1.14 ms                                                      | 986 us: 1.16x faster                                                       |
| sympy_integrate          | 28.2 ms                                                      | 24.5 ms: 1.15x faster                                                      |
| mdp                      | 3.01 sec                                                     | 2.62 sec: 1.15x faster                                                     |
| 2to3                     | 350 ms                                                       | 307 ms: 1.14x faster                                                       |
| create_gc_cycles         | 1.76 ms                                                      | 1.56 ms: 1.13x faster                                                      |
| scimark_fft              | 361 ms                                                       | 322 ms: 1.12x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 62.8 ms: 1.12x faster                                                      |
| pathlib                  | 21.4 ms                                                      | 19.2 ms: 1.11x faster                                                      |
| json                     | 5.86 ms                                                      | 5.28 ms: 1.11x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.70 us: 1.11x faster                                                      |
| regex_dna                | 261 ms                                                       | 237 ms: 1.10x faster                                                       |
| xml_etree_parse          | 160 ms                                                       | 146 ms: 1.10x faster                                                       |
| async_generators         | 421 ms                                                       | 385 ms: 1.09x faster                                                       |
| xml_etree_generate       | 92.3 ms                                                      | 84.4 ms: 1.09x faster                                                      |
| xml_etree_iterparse      | 110 ms                                                       | 103 ms: 1.07x faster                                                       |
| regex_v8                 | 27.2 ms                                                      | 25.3 ms: 1.07x faster                                                      |
| meteor_contest           | 138 ms                                                       | 131 ms: 1.06x faster                                                       |
| pidigits                 | 271 ms                                                       | 262 ms: 1.03x faster                                                       |
| gc_traversal             | 3.42 ms                                                      | 3.47 ms: 1.01x slower                                                      |
| unpickle_list            | 4.65 us                                                      | 4.72 us: 1.02x slower                                                      |
| unpack_sequence          | 59.9 ns                                                      | 61.5 ns: 1.03x slower                                                      |
| pickle_dict              | 29.5 us                                                      | 30.5 us: 1.03x slower                                                      |
| pickle_list              | 4.12 us                                                      | 4.28 us: 1.04x slower                                                      |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.04x slower                                                      |
| bench_mp_pool            | 6.37 ms                                                      | 6.86 ms: 1.08x slower                                                      |
| telco                    | 7.23 ms                                                      | 8.06 ms: 1.12x slower                                                      |
| unpickle                 | 13.5 us                                                      | 15.5 us: 1.15x slower                                                      |
| regex_effbot             | 3.09 ms                                                      | 3.63 ms: 1.18x slower                                                      |
| coverage                 | 63.3 ms                                                      | 78.8 ms: 1.24x slower                                                      |
| python_startup           | 11.5 ms                                                      | 15.5 ms: 1.35x slower                                                      |
| python_startup_no_site   | 7.33 ms                                                      | 14.1 ms: 1.92x slower                                                      |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                               |

Benchmark hidden because not significant (2): mypy2, asyncio_websockets
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-594cca3-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_jumps-3.13.0a4+-594cca3.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.19x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.36x