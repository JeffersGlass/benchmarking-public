# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.31x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.24x faster
- Memory change: 1.33x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 277 ms: 1.26x faster                                                |
| chameleon      | 9.68 ms                                                | 6.76 ms: 1.43x faster                                               |
| docutils       | 3.30 sec                                               | 2.70 sec: 1.22x faster                                              |
| html5lib       | 88.9 ms                                                | 65.2 ms: 1.36x faster                                               |
| tornado_http   | 136 ms                                                 | 96.9 ms: 1.41x faster                                               |
| Geometric mean | (ref)                                                  | 1.33x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 440 ms: 1.65x faster                                                |
| async_tree_memoization  | 870 ms                                                 | 566 ms: 1.54x faster                                                |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                              |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 707 ms: 1.44x faster                                                |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                        |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 94.1 ms: 1.63x faster                                               |
| float          | 117 ms                                                 | 80.0 ms: 1.46x faster                                               |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                |
| Geometric mean | (ref)                                                  | 1.35x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 142 ms: 1.33x faster                                                |
| regex_v8       | 27.8 ms                                                | 24.7 ms: 1.12x faster                                               |
| regex_dna      | 227 ms                                                 | 229 ms: 1.01x slower                                                |
| regex_effbot   | 3.63 ms                                                | 3.73 ms: 1.03x slower                                               |
| Geometric mean | (ref)                                                  | 1.09x faster                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 307 us: 1.58x faster                                                |
| tomli_loads          | 3.14 sec                                               | 2.07 sec: 1.52x faster                                              |
| unpickle_pure_python | 331 us                                                 | 238 us: 1.39x faster                                                |
| json_dumps           | 14.2 ms                                                | 10.2 ms: 1.38x faster                                               |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                               |
| xml_etree_generate   | 99.4 ms                                                | 86.0 ms: 1.16x faster                                               |
| json_loads           | 31.2 us                                                | 27.7 us: 1.13x faster                                               |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                |
| unpickle_list        | 5.20 us                                                | 4.79 us: 1.08x faster                                               |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                               |
| unpickle             | 14.4 us                                                | 14.5 us: 1.01x slower                                               |
| pickle               | 10.7 us                                                | 11.3 us: 1.06x slower                                               |
| pickle_dict          | 29.6 us                                                | 34.2 us: 1.15x slower                                               |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.18x faster                                               |
| python_startup_no_site | 5.93 ms                                                | 11.0 ms: 1.85x slower                                               |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako            | 16.3 ms                                                | 11.2 ms: 1.46x faster                                               |
| django_template | 48.2 ms                                                | 34.3 ms: 1.40x faster                                               |
| genshi_text     | 31.8 ms                                                | 24.2 ms: 1.31x faster                                               |
| genshi_xml      | 66.0 ms                                                | 54.5 ms: 1.21x faster                                               |
| Geometric mean  | (ref)                                                  | 1.34x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.96x faster                                                |
| generators               | 80.1 ms                                                | 29.3 ms: 2.73x faster                                               |
| deltablue                | 7.91 ms                                                | 3.40 ms: 2.32x faster                                               |
| asyncio_tcp              | 922 ms                                                 | 485 ms: 1.90x faster                                                |
| logging_silent           | 190 ns                                                 | 101 ns: 1.88x faster                                                |
| chaos                    | 115 ms                                                 | 63.6 ms: 1.82x faster                                               |
| richards_super           | 94.7 ms                                                | 52.3 ms: 1.81x faster                                               |
| crypto_pyaes             | 128 ms                                                 | 73.2 ms: 1.75x faster                                               |
| raytrace                 | 507 ms                                                 | 292 ms: 1.73x faster                                                |
| richards                 | 79.3 ms                                                | 45.8 ms: 1.73x faster                                               |
| pylint                   | 551 ms                                                 | 319 ms: 1.73x faster                                                |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.71x faster                                                |
| sqlglot_parse            | 2.17 ms                                                | 1.29 ms: 1.68x faster                                               |
| comprehensions           | 28.8 us                                                | 17.1 us: 1.68x faster                                               |
| async_tree_none          | 728 ms                                                 | 440 ms: 1.65x faster                                                |
| nbody                    | 154 ms                                                 | 94.1 ms: 1.63x faster                                               |
| scimark_monte_carlo      | 118 ms                                                 | 72.6 ms: 1.63x faster                                               |
| sqlglot_transpile        | 2.57 ms                                                | 1.62 ms: 1.59x faster                                               |
| pickle_pure_python       | 484 us                                                 | 307 us: 1.58x faster                                                |
| go                       | 240 ms                                                 | 155 ms: 1.55x faster                                                |
| async_tree_memoization   | 870 ms                                                 | 566 ms: 1.54x faster                                                |
| coroutines               | 35.1 ms                                                | 23.0 ms: 1.53x faster                                               |
| tomli_loads              | 3.14 sec                                               | 2.07 sec: 1.52x faster                                              |
| deepcopy_memo            | 58.5 us                                                | 38.6 us: 1.51x faster                                               |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                              |
| spectral_norm            | 170 ms                                                 | 113 ms: 1.50x faster                                                |
| hexiom                   | 10.4 ms                                                | 7.08 ms: 1.47x faster                                               |
| float                    | 117 ms                                                 | 80.0 ms: 1.46x faster                                               |
| pyflate                  | 716 ms                                                 | 490 ms: 1.46x faster                                                |
| mako                     | 16.3 ms                                                | 11.2 ms: 1.46x faster                                               |
| logging_format           | 9.09 us                                                | 6.28 us: 1.45x faster                                               |
| logging_simple           | 8.30 us                                                | 5.75 us: 1.45x faster                                               |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 707 ms: 1.44x faster                                                |
| chameleon                | 9.68 ms                                                | 6.76 ms: 1.43x faster                                               |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                              |
| tornado_http             | 136 ms                                                 | 96.9 ms: 1.41x faster                                               |
| django_template          | 48.2 ms                                                | 34.3 ms: 1.40x faster                                               |
| unpickle_pure_python     | 331 us                                                 | 238 us: 1.39x faster                                                |
| json_dumps               | 14.2 ms                                                | 10.2 ms: 1.38x faster                                               |
| deepcopy                 | 479 us                                                 | 349 us: 1.37x faster                                                |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                               |
| html5lib                 | 88.9 ms                                                | 65.2 ms: 1.36x faster                                               |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.75 ms: 1.36x faster                                               |
| scimark_fft              | 466 ms                                                 | 342 ms: 1.36x faster                                                |
| pprint_pformat           | 2.10 sec                                               | 1.55 sec: 1.36x faster                                              |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                               |
| thrift                   | 1.07 ms                                                | 800 us: 1.34x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 107 ms: 1.34x faster                                                |
| scimark_lu               | 176 ms                                                 | 132 ms: 1.34x faster                                                |
| fannkuch                 | 532 ms                                                 | 398 ms: 1.33x faster                                                |
| regex_compile            | 188 ms                                                 | 142 ms: 1.33x faster                                                |
| pprint_safe_repr         | 1.02 sec                                               | 772 ms: 1.32x faster                                                |
| genshi_text              | 31.8 ms                                                | 24.2 ms: 1.31x faster                                               |
| pycparser                | 1.58 sec                                               | 1.21 sec: 1.30x faster                                              |
| 2to3                     | 348 ms                                                 | 277 ms: 1.26x faster                                                |
| sympy_sum                | 196 ms                                                 | 157 ms: 1.25x faster                                                |
| sympy_integrate          | 25.8 ms                                                | 20.8 ms: 1.24x faster                                               |
| sqlglot_optimize         | 69.2 ms                                                | 55.8 ms: 1.24x faster                                               |
| sympy_str                | 346 ms                                                 | 279 ms: 1.24x faster                                                |
| aiohttp                  | 1.44 ms                                                | 1.16 ms: 1.24x faster                                               |
| dulwich_log              | 84.3 ms                                                | 68.6 ms: 1.23x faster                                               |
| docutils                 | 3.30 sec                                               | 2.70 sec: 1.22x faster                                              |
| gunicorn                 | 1.53 ms                                                | 1.26 ms: 1.21x faster                                               |
| genshi_xml               | 66.0 ms                                                | 54.5 ms: 1.21x faster                                               |
| sympy_expand             | 566 ms                                                 | 473 ms: 1.20x faster                                                |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.18x faster                                               |
| nqueens                  | 106 ms                                                 | 90.2 ms: 1.17x faster                                               |
| bench_thread_pool        | 986 us                                                 | 844 us: 1.17x faster                                                |
| djangocms                | 38.4 us                                                | 33.0 us: 1.16x faster                                               |
| xml_etree_generate       | 99.4 ms                                                | 86.0 ms: 1.16x faster                                               |
| json_loads               | 31.2 us                                                | 27.7 us: 1.13x faster                                               |
| regex_v8                 | 27.8 ms                                                | 24.7 ms: 1.12x faster                                               |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                               |
| mdp                      | 2.85 sec                                               | 2.59 sec: 1.10x faster                                              |
| meteor_contest           | 120 ms                                                 | 109 ms: 1.10x faster                                                |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                |
| unpickle_list            | 5.20 us                                                | 4.79 us: 1.08x faster                                               |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                |
| json                     | 5.69 ms                                                | 5.30 ms: 1.07x faster                                               |
| sqlite_synth             | 3.02 us                                                | 2.82 us: 1.07x faster                                               |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.07x faster                                               |
| pickle_list              | 5.08 us                                                | 4.98 us: 1.02x faster                                               |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                |
| unpickle                 | 14.4 us                                                | 14.5 us: 1.01x slower                                               |
| regex_dna                | 227 ms                                                 | 229 ms: 1.01x slower                                                |
| regex_effbot             | 3.63 ms                                                | 3.73 ms: 1.03x slower                                               |
| async_generators         | 444 ms                                                 | 459 ms: 1.04x slower                                                |
| pickle                   | 10.7 us                                                | 11.3 us: 1.06x slower                                               |
| gc_traversal             | 3.62 ms                                                | 3.92 ms: 1.08x slower                                               |
| telco                    | 7.27 ms                                                | 8.29 ms: 1.14x slower                                               |
| pickle_dict              | 29.6 us                                                | 34.2 us: 1.15x slower                                               |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                               |
| coverage                 | 79.4 ms                                                | 95.6 ms: 1.20x slower                                               |
| dask                     | 441 ms                                                 | 534 ms: 1.21x slower                                                |
| unpack_sequence          | 60.0 ns                                                | 94.6 ns: 1.58x slower                                               |
| python_startup_no_site   | 5.93 ms                                                | 11.0 ms: 1.85x slower                                               |
| Geometric mean           | (ref)                                                  | 1.31x faster                                                        |

Benchmark hidden because not significant (1): mypy2
Ignored benchmarks (3) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: flaskblogging, sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.27x
- 95% likely to have a speedup of 1.26x
- 99% likely to have a speedup of 1.24x


# Memory

- memory change: 1.33x