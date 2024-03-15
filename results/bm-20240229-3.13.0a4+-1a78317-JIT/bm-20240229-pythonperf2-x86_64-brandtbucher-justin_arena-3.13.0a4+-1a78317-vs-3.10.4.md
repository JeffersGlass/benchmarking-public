# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_arena
- machine: linux-x86_64
- commit hash: 1a78317
- commit date: 2024-02-29
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.17x faster
- Memory change: 1.35x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 350 ms                                                       | 307 ms: 1.14x faster                                                       |
| chameleon      | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                                      |
| docutils       | 3.41 sec                                                     | 2.91 sec: 1.17x faster                                                     |
| html5lib       | 94.6 ms                                                      | 73.9 ms: 1.28x faster                                                      |
| tornado_http   | 157 ms                                                       | 125 ms: 1.26x faster                                                       |
| Geometric mean | (ref)                                                        | 1.22x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 692 ms                                                       | 445 ms: 1.55x faster                                                       |
| async_tree_memoization  | 819 ms                                                       | 559 ms: 1.47x faster                                                       |
| async_tree_io           | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                     |
| async_tree_cpu_io_mixed | 936 ms                                                       | 710 ms: 1.32x faster                                                       |
| Geometric mean          | (ref)                                                        | 1.45x faster                                                               |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 111 ms                                                       | 78.1 ms: 1.42x faster                                                      |
| nbody          | 134 ms                                                       | 98.5 ms: 1.36x faster                                                      |
| pidigits       | 271 ms                                                       | 261 ms: 1.04x faster                                                       |
| Geometric mean | (ref)                                                        | 1.26x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 190 ms                                                       | 146 ms: 1.30x faster                                                       |
| regex_dna      | 261 ms                                                       | 238 ms: 1.10x faster                                                       |
| regex_v8       | 27.2 ms                                                      | 25.2 ms: 1.08x faster                                                      |
| regex_effbot   | 3.09 ms                                                      | 3.56 ms: 1.15x slower                                                      |
| Geometric mean | (ref)                                                        | 1.07x faster                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|----------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| pickle_pure_python   | 455 us                                                       | 308 us: 1.48x faster                                                       |
| unpickle_pure_python | 312 us                                                       | 230 us: 1.36x faster                                                       |
| json_dumps           | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                      |
| tomli_loads          | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                                     |
| xml_etree_process    | 75.9 ms                                                      | 57.7 ms: 1.31x faster                                                      |
| json_loads           | 30.3 us                                                      | 24.8 us: 1.22x faster                                                      |
| xml_etree_parse      | 160 ms                                                       | 143 ms: 1.12x faster                                                       |
| xml_etree_generate   | 92.3 ms                                                      | 83.2 ms: 1.11x faster                                                      |
| xml_etree_iterparse  | 110 ms                                                       | 102 ms: 1.09x faster                                                       |
| pickle_list          | 4.12 us                                                      | 4.30 us: 1.04x slower                                                      |
| pickle               | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| pickle_dict          | 29.5 us                                                      | 31.0 us: 1.05x slower                                                      |
| unpickle             | 13.5 us                                                      | 15.1 us: 1.12x slower                                                      |
| Geometric mean       | (ref)                                                        | 1.14x faster                                                               |

Benchmark hidden because not significant (1): unpickle_list

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 11.5 ms                                                      | 15.4 ms: 1.34x slower                                                      |
| python_startup_no_site | 7.33 ms                                                      | 13.9 ms: 1.89x slower                                                      |
| Geometric mean         | (ref)                                                        | 1.59x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|-----------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 14.7 ms                                                      | 9.85 ms: 1.49x faster                                                      |
| django_template | 50.2 ms                                                      | 38.9 ms: 1.29x faster                                                      |
| genshi_text     | 31.4 ms                                                      | 29.6 ms: 1.06x faster                                                      |
| genshi_xml      | 63.3 ms                                                      | 60.7 ms: 1.04x faster                                                      |
| Geometric mean  | (ref)                                                        | 1.21x faster                                                               |

All benchmarks:
===============

| Benchmark                | bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317 |
|--------------------------|:------------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 537 us                                                       | 118 us: 4.54x faster                                                       |
| asyncio_tcp              | 779 ms                                                       | 371 ms: 2.10x faster                                                       |
| deltablue                | 7.50 ms                                                      | 3.81 ms: 1.97x faster                                                      |
| asyncio_tcp_ssl          | 3.10 sec                                                     | 1.58 sec: 1.97x faster                                                     |
| generators               | 57.3 ms                                                      | 33.0 ms: 1.74x faster                                                      |
| logging_silent           | 167 ns                                                       | 97.0 ns: 1.72x faster                                                      |
| chaos                    | 109 ms                                                       | 66.8 ms: 1.63x faster                                                      |
| raytrace                 | 489 ms                                                       | 304 ms: 1.61x faster                                                       |
| sqlglot_parse            | 2.24 ms                                                      | 1.40 ms: 1.60x faster                                                      |
| richards_super           | 90.6 ms                                                      | 56.7 ms: 1.60x faster                                                      |
| pylint                   | 566 ms                                                       | 359 ms: 1.58x faster                                                       |
| crypto_pyaes             | 119 ms                                                       | 76.7 ms: 1.55x faster                                                      |
| async_tree_none          | 692 ms                                                       | 445 ms: 1.55x faster                                                       |
| go                       | 262 ms                                                       | 172 ms: 1.52x faster                                                       |
| richards                 | 75.1 ms                                                      | 49.6 ms: 1.52x faster                                                      |
| spectral_norm            | 139 ms                                                       | 92.6 ms: 1.50x faster                                                      |
| mako                     | 14.7 ms                                                      | 9.85 ms: 1.49x faster                                                      |
| pickle_pure_python       | 455 us                                                       | 308 us: 1.48x faster                                                       |
| async_tree_memoization   | 819 ms                                                       | 559 ms: 1.47x faster                                                       |
| sqlglot_transpile        | 2.68 ms                                                      | 1.83 ms: 1.46x faster                                                      |
| async_tree_io            | 1.60 sec                                                     | 1.09 sec: 1.46x faster                                                     |
| comprehensions           | 26.7 us                                                      | 18.7 us: 1.43x faster                                                      |
| float                    | 111 ms                                                       | 78.1 ms: 1.42x faster                                                      |
| scimark_lu               | 167 ms                                                       | 117 ms: 1.42x faster                                                       |
| scimark_monte_carlo      | 107 ms                                                       | 76.6 ms: 1.40x faster                                                      |
| logging_simple           | 8.88 us                                                      | 6.42 us: 1.38x faster                                                      |
| nbody                    | 134 ms                                                       | 98.5 ms: 1.36x faster                                                      |
| pyflate                  | 733 ms                                                       | 538 ms: 1.36x faster                                                       |
| unpickle_pure_python     | 312 us                                                       | 230 us: 1.36x faster                                                       |
| coroutines               | 30.3 ms                                                      | 22.4 ms: 1.35x faster                                                      |
| thrift                   | 1.18 ms                                                      | 868 us: 1.35x faster                                                       |
| logging_format           | 9.64 us                                                      | 7.12 us: 1.35x faster                                                      |
| json_dumps               | 14.5 ms                                                      | 10.8 ms: 1.35x faster                                                      |
| tomli_loads              | 2.92 sec                                                     | 2.17 sec: 1.34x faster                                                     |
| deepcopy_memo            | 49.8 us                                                      | 37.4 us: 1.33x faster                                                      |
| async_tree_cpu_io_mixed  | 936 ms                                                       | 710 ms: 1.32x faster                                                       |
| xml_etree_process        | 75.9 ms                                                      | 57.7 ms: 1.31x faster                                                      |
| pycparser                | 1.67 sec                                                     | 1.28 sec: 1.30x faster                                                     |
| regex_compile            | 190 ms                                                       | 146 ms: 1.30x faster                                                       |
| hexiom                   | 9.42 ms                                                      | 7.30 ms: 1.29x faster                                                      |
| django_template          | 50.2 ms                                                      | 38.9 ms: 1.29x faster                                                      |
| html5lib                 | 94.6 ms                                                      | 73.9 ms: 1.28x faster                                                      |
| pprint_safe_repr         | 1.05 sec                                                     | 835 ms: 1.26x faster                                                       |
| tornado_http             | 157 ms                                                       | 125 ms: 1.26x faster                                                       |
| pprint_pformat           | 2.15 sec                                                     | 1.72 sec: 1.25x faster                                                     |
| fannkuch                 | 483 ms                                                       | 386 ms: 1.25x faster                                                       |
| deepcopy                 | 468 us                                                       | 375 us: 1.25x faster                                                       |
| chameleon                | 9.44 ms                                                      | 7.60 ms: 1.24x faster                                                      |
| json_loads               | 30.3 us                                                      | 24.8 us: 1.22x faster                                                      |
| scimark_sparse_mat_mult  | 5.08 ms                                                      | 4.16 ms: 1.22x faster                                                      |
| sympy_sum                | 193 ms                                                       | 160 ms: 1.21x faster                                                       |
| deepcopy_reduce          | 4.01 us                                                      | 3.34 us: 1.20x faster                                                      |
| sqlglot_normalize        | 144 ms                                                       | 120 ms: 1.20x faster                                                       |
| sympy_str                | 360 ms                                                       | 301 ms: 1.19x faster                                                       |
| scimark_sor              | 180 ms                                                       | 151 ms: 1.19x faster                                                       |
| dulwich_log              | 81.1 ms                                                      | 68.3 ms: 1.19x faster                                                      |
| docutils                 | 3.41 sec                                                     | 2.91 sec: 1.17x faster                                                     |
| sympy_expand             | 600 ms                                                       | 512 ms: 1.17x faster                                                       |
| mdp                      | 3.01 sec                                                     | 2.58 sec: 1.17x faster                                                     |
| bench_thread_pool        | 1.14 ms                                                      | 991 us: 1.15x faster                                                       |
| sympy_integrate          | 28.2 ms                                                      | 24.5 ms: 1.15x faster                                                      |
| 2to3                     | 350 ms                                                       | 307 ms: 1.14x faster                                                       |
| create_gc_cycles         | 1.76 ms                                                      | 1.55 ms: 1.14x faster                                                      |
| scimark_fft              | 361 ms                                                       | 318 ms: 1.14x faster                                                       |
| nqueens                  | 115 ms                                                       | 101 ms: 1.13x faster                                                       |
| xml_etree_parse          | 160 ms                                                       | 143 ms: 1.12x faster                                                       |
| sqlglot_optimize         | 70.1 ms                                                      | 63.0 ms: 1.11x faster                                                      |
| sqlite_synth             | 2.99 us                                                      | 2.69 us: 1.11x faster                                                      |
| xml_etree_generate       | 92.3 ms                                                      | 83.2 ms: 1.11x faster                                                      |
| pathlib                  | 21.4 ms                                                      | 19.3 ms: 1.11x faster                                                      |
| json                     | 5.86 ms                                                      | 5.35 ms: 1.10x faster                                                      |
| regex_dna                | 261 ms                                                       | 238 ms: 1.10x faster                                                       |
| xml_etree_iterparse      | 110 ms                                                       | 102 ms: 1.09x faster                                                       |
| async_generators         | 421 ms                                                       | 389 ms: 1.08x faster                                                       |
| regex_v8                 | 27.2 ms                                                      | 25.2 ms: 1.08x faster                                                      |
| aiohttp                  | 1.19 ms                                                      | 1.10 ms: 1.08x faster                                                      |
| gunicorn                 | 1.16 ms                                                      | 1.08 ms: 1.07x faster                                                      |
| genshi_text              | 31.4 ms                                                      | 29.6 ms: 1.06x faster                                                      |
| meteor_contest           | 138 ms                                                       | 132 ms: 1.05x faster                                                       |
| genshi_xml               | 63.3 ms                                                      | 60.7 ms: 1.04x faster                                                      |
| pidigits                 | 271 ms                                                       | 261 ms: 1.04x faster                                                       |
| asyncio_websockets       | 390 ms                                                       | 387 ms: 1.01x faster                                                       |
| unpack_sequence          | 59.9 ns                                                      | 60.5 ns: 1.01x slower                                                      |
| gc_traversal             | 3.42 ms                                                      | 3.47 ms: 1.02x slower                                                      |
| pickle_list              | 4.12 us                                                      | 4.30 us: 1.04x slower                                                      |
| pickle                   | 9.89 us                                                      | 10.3 us: 1.05x slower                                                      |
| pickle_dict              | 29.5 us                                                      | 31.0 us: 1.05x slower                                                      |
| telco                    | 7.23 ms                                                      | 7.99 ms: 1.11x slower                                                      |
| bench_mp_pool            | 6.37 ms                                                      | 7.08 ms: 1.11x slower                                                      |
| unpickle                 | 13.5 us                                                      | 15.1 us: 1.12x slower                                                      |
| regex_effbot             | 3.09 ms                                                      | 3.56 ms: 1.15x slower                                                      |
| dask                     | 472 ms                                                       | 588 ms: 1.24x slower                                                       |
| coverage                 | 63.3 ms                                                      | 81.4 ms: 1.29x slower                                                      |
| python_startup           | 11.5 ms                                                      | 15.4 ms: 1.34x slower                                                      |
| python_startup_no_site   | 7.33 ms                                                      | 13.9 ms: 1.89x slower                                                      |
| Geometric mean           | (ref)                                                        | 1.24x faster                                                               |

Benchmark hidden because not significant (2): mypy2, unpickle_list
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-pythonperf2-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-1a78317-JIT/bm-20240229-pythonperf2-x86_64-brandtbucher-justin_arena-3.13.0a4+-1a78317.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.20x
- 95% likely to have a speedup of 1.19x
- 99% likely to have a speedup of 1.17x


# Memory

- memory change: 1.35x