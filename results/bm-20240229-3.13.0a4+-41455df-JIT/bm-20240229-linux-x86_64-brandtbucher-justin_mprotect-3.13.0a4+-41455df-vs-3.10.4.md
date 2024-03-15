# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_mprotect
- machine: linux-x86_64
- commit hash: 41455df
- commit date: 2024-02-29
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.21x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 275 ms: 1.27x faster                                                    |
| chameleon      | 9.68 ms                                                | 6.77 ms: 1.43x faster                                                   |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                  |
| tornado_http   | 136 ms                                                 | 96.3 ms: 1.42x faster                                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                                            |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                    |
| async_tree_memoization  | 870 ms                                                 | 564 ms: 1.54x faster                                                    |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                  |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 708 ms: 1.44x faster                                                    |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                            |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 93.1 ms: 1.65x faster                                                   |
| float          | 117 ms                                                 | 78.5 ms: 1.49x faster                                                   |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| Geometric mean | (ref)                                                  | 1.36x faster                                                            |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 141 ms: 1.33x faster                                                    |
| regex_v8       | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                   |
| regex_dna      | 227 ms                                                 | 234 ms: 1.03x slower                                                    |
| regex_effbot   | 3.63 ms                                                | 3.82 ms: 1.05x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x faster                                                            |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|----------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                    |
| tomli_loads          | 3.14 sec                                               | 2.04 sec: 1.54x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                                    |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                   |
| xml_etree_process    | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                   |
| xml_etree_generate   | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                   |
| json_loads           | 31.2 us                                                | 27.6 us: 1.13x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.70 us: 1.11x faster                                                   |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| xml_etree_parse      | 168 ms                                                 | 157 ms: 1.07x faster                                                    |
| unpickle             | 14.4 us                                                | 14.5 us: 1.01x slower                                                   |
| pickle_list          | 5.08 us                                                | 5.14 us: 1.01x slower                                                   |
| pickle               | 10.7 us                                                | 11.8 us: 1.11x slower                                                   |
| pickle_dict          | 29.6 us                                                | 34.4 us: 1.16x slower                                                   |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                            |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 11.2 ms: 1.30x faster                                                   |
| python_startup_no_site | 5.93 ms                                                | 9.85 ms: 1.66x slower                                                   |
| Geometric mean         | (ref)                                                  | 1.13x slower                                                            |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|-----------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                   |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df |
|--------------------------|:------------------------------------------------------:|:-----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.97x faster                                                    |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                                   |
| deltablue                | 7.91 ms                                                | 3.38 ms: 2.34x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 475 ms: 1.94x faster                                                    |
| logging_silent           | 190 ns                                                 | 102 ns: 1.86x faster                                                    |
| chaos                    | 115 ms                                                 | 62.3 ms: 1.85x faster                                                   |
| richards_super           | 94.7 ms                                                | 51.7 ms: 1.83x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 72.8 ms: 1.76x faster                                                   |
| raytrace                 | 507 ms                                                 | 289 ms: 1.75x faster                                                    |
| richards                 | 79.3 ms                                                | 45.5 ms: 1.74x faster                                                   |
| scimark_sor              | 220 ms                                                 | 127 ms: 1.72x faster                                                    |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                                   |
| comprehensions           | 28.8 us                                                | 17.2 us: 1.67x faster                                                   |
| scimark_monte_carlo      | 118 ms                                                 | 70.7 ms: 1.67x faster                                                   |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                    |
| nbody                    | 154 ms                                                 | 93.1 ms: 1.65x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                    |
| sqlglot_transpile        | 2.57 ms                                                | 1.63 ms: 1.58x faster                                                   |
| go                       | 240 ms                                                 | 155 ms: 1.55x faster                                                    |
| coroutines               | 35.1 ms                                                | 22.7 ms: 1.55x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 564 ms: 1.54x faster                                                    |
| tomli_loads              | 3.14 sec                                               | 2.04 sec: 1.54x faster                                                  |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.54x faster                                                    |
| pyflate                  | 716 ms                                                 | 471 ms: 1.52x faster                                                    |
| deepcopy_memo            | 58.5 us                                                | 38.5 us: 1.52x faster                                                   |
| mako                     | 16.3 ms                                                | 10.8 ms: 1.51x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                                  |
| float                    | 117 ms                                                 | 78.5 ms: 1.49x faster                                                   |
| hexiom                   | 10.4 ms                                                | 7.01 ms: 1.48x faster                                                   |
| logging_format           | 9.09 us                                                | 6.16 us: 1.48x faster                                                   |
| logging_simple           | 8.30 us                                                | 5.65 us: 1.47x faster                                                   |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 708 ms: 1.44x faster                                                    |
| chameleon                | 9.68 ms                                                | 6.77 ms: 1.43x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                  |
| tornado_http             | 136 ms                                                 | 96.3 ms: 1.42x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                                    |
| scimark_fft              | 466 ms                                                 | 337 ms: 1.38x faster                                                    |
| deepcopy                 | 479 us                                                 | 348 us: 1.38x faster                                                    |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                                   |
| scimark_lu               | 176 ms                                                 | 129 ms: 1.36x faster                                                    |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                                  |
| fannkuch                 | 532 ms                                                 | 392 ms: 1.36x faster                                                    |
| pprint_safe_repr         | 1.02 sec                                               | 751 ms: 1.36x faster                                                    |
| xml_etree_process        | 79.1 ms                                                | 58.6 ms: 1.35x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                    |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.85 ms: 1.33x faster                                                   |
| regex_compile            | 188 ms                                                 | 141 ms: 1.33x faster                                                    |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.31x faster                                                  |
| python_startup           | 14.6 ms                                                | 11.2 ms: 1.30x faster                                                   |
| 2to3                     | 348 ms                                                 | 275 ms: 1.27x faster                                                    |
| sympy_sum                | 196 ms                                                 | 156 ms: 1.26x faster                                                    |
| sqlglot_optimize         | 69.2 ms                                                | 55.5 ms: 1.25x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                                   |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                                    |
| dulwich_log              | 84.3 ms                                                | 68.7 ms: 1.23x faster                                                   |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                                  |
| sympy_expand             | 566 ms                                                 | 473 ms: 1.19x faster                                                    |
| nqueens                  | 106 ms                                                 | 89.8 ms: 1.18x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 841 us: 1.17x faster                                                    |
| xml_etree_generate       | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                   |
| json_loads               | 31.2 us                                                | 27.6 us: 1.13x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 24.6 ms: 1.13x faster                                                   |
| json                     | 5.69 ms                                                | 5.05 ms: 1.13x faster                                                   |
| meteor_contest           | 120 ms                                                 | 108 ms: 1.11x faster                                                    |
| pathlib                  | 20.5 ms                                                | 18.5 ms: 1.11x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.70 us: 1.11x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                    |
| xml_etree_parse          | 168 ms                                                 | 157 ms: 1.07x faster                                                    |
| create_gc_cycles         | 1.62 ms                                                | 1.51 ms: 1.07x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.85 us: 1.06x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.76 sec: 1.03x faster                                                  |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                    |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                    |
| unpickle                 | 14.4 us                                                | 14.5 us: 1.01x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.14 us: 1.01x slower                                                   |
| regex_dna                | 227 ms                                                 | 234 ms: 1.03x slower                                                    |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                                    |
| gc_traversal             | 3.62 ms                                                | 3.80 ms: 1.05x slower                                                   |
| regex_effbot             | 3.63 ms                                                | 3.82 ms: 1.05x slower                                                   |
| pickle                   | 10.7 us                                                | 11.8 us: 1.11x slower                                                   |
| telco                    | 7.27 ms                                                | 8.36 ms: 1.15x slower                                                   |
| pickle_dict              | 29.6 us                                                | 34.4 us: 1.16x slower                                                   |
| dask                     | 441 ms                                                 | 530 ms: 1.20x slower                                                    |
| coverage                 | 79.4 ms                                                | 96.4 ms: 1.21x slower                                                   |
| unpack_sequence          | 60.0 ns                                                | 96.7 ns: 1.61x slower                                                   |
| python_startup_no_site   | 5.93 ms                                                | 9.85 ms: 1.66x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                            |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-41455df-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_mprotect-3.13.0a4+-41455df.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.21x