# Results vs. 3.12.0

- fork: brandtbucher
- ref: justin_nops
- machine: linux-x86_64
- commit hash: 640fc6e
- commit date: 2024-02-29
- overall geometric mean: 1.00x faster \*
- HPT reliability: 98.15%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                                |
| chameleon      | 7.41 ms                                                | 6.76 ms: 1.10x faster                                               |
| docutils       | 2.77 sec                                               | 2.70 sec: 1.03x faster                                              |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                               |
| Geometric mean | (ref)                                                  | 1.04x faster                                                        |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 440 ms: 1.07x faster                                                |
| async_tree_cpu_io_mixed | 726 ms                                                 | 707 ms: 1.03x faster                                                |
| async_tree_memoization  | 578 ms                                                 | 566 ms: 1.02x faster                                                |
| async_tree_none_tg      | 450 ms                                                 | 447 ms: 1.00x faster                                                |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.01x slower                                              |
| async_tree_io           | 1.16 sec                                               | 1.18 sec: 1.02x slower                                              |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                        |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 80.0 ms: 1.06x faster                                               |
| nbody          | 97.0 ms                                                | 94.1 ms: 1.03x faster                                               |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x faster                                                        |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                                |
| regex_effbot   | 3.61 ms                                                | 3.73 ms: 1.03x slower                                               |
| regex_v8       | 23.1 ms                                                | 24.7 ms: 1.07x slower                                               |
| regex_dna      | 212 ms                                                 | 229 ms: 1.08x slower                                                |
| Geometric mean | (ref)                                                  | 1.03x slower                                                        |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|----------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.07 sec: 1.13x faster                                              |
| unpickle_list        | 5.29 us                                                | 4.79 us: 1.10x faster                                               |
| unpickle             | 15.9 us                                                | 14.5 us: 1.09x faster                                               |
| pickle_pure_python   | 324 us                                                 | 307 us: 1.06x faster                                                |
| xml_etree_process    | 61.7 ms                                                | 58.5 ms: 1.05x faster                                               |
| pickle_dict          | 35.5 us                                                | 34.2 us: 1.04x faster                                               |
| xml_etree_generate   | 89.2 ms                                                | 86.0 ms: 1.04x faster                                               |
| json_loads           | 28.5 us                                                | 27.7 us: 1.03x faster                                               |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                |
| pickle               | 11.6 us                                                | 11.3 us: 1.02x faster                                               |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                               |
| json_dumps           | 10.4 ms                                                | 10.2 ms: 1.01x faster                                               |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.03x slower                                                |
| Geometric mean       | (ref)                                                  | 1.04x faster                                                        |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.3 ms: 1.29x slower                                               |
| python_startup_no_site | 6.94 ms                                                | 11.0 ms: 1.58x slower                                               |
| Geometric mean         | (ref)                                                  | 1.43x slower                                                        |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|-----------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 11.2 ms: 1.06x faster                                               |
| django_template | 34.6 ms                                                | 34.3 ms: 1.01x faster                                               |
| Geometric mean  | (ref)                                                  | 1.03x faster                                                        |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e |
|--------------------------|:------------------------------------------------------:|:-------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 110 us: 1.44x faster                                                |
| comprehensions           | 21.8 us                                                | 17.1 us: 1.27x faster                                               |
| logging_format           | 7.23 us                                                | 6.28 us: 1.15x faster                                               |
| tomli_loads              | 2.33 sec                                               | 2.07 sec: 1.13x faster                                              |
| logging_simple           | 6.46 us                                                | 5.75 us: 1.12x faster                                               |
| crypto_pyaes             | 81.9 ms                                                | 73.2 ms: 1.12x faster                                               |
| scimark_fft              | 382 ms                                                 | 342 ms: 1.12x faster                                                |
| unpickle_list            | 5.29 us                                                | 4.79 us: 1.10x faster                                               |
| deepcopy_reduce          | 3.35 us                                                | 3.04 us: 1.10x faster                                               |
| chameleon                | 7.41 ms                                                | 6.76 ms: 1.10x faster                                               |
| unpickle                 | 15.9 us                                                | 14.5 us: 1.09x faster                                               |
| deltablue                | 3.72 ms                                                | 3.40 ms: 1.09x faster                                               |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                |
| sympy_str                | 300 ms                                                 | 279 ms: 1.07x faster                                                |
| async_tree_none          | 472 ms                                                 | 440 ms: 1.07x faster                                                |
| raytrace                 | 312 ms                                                 | 292 ms: 1.07x faster                                                |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.75 ms: 1.06x faster                                               |
| generators               | 31.2 ms                                                | 29.3 ms: 1.06x faster                                               |
| deepcopy                 | 371 us                                                 | 349 us: 1.06x faster                                                |
| mako                     | 11.9 ms                                                | 11.2 ms: 1.06x faster                                               |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                               |
| float                    | 84.7 ms                                                | 80.0 ms: 1.06x faster                                               |
| pathlib                  | 19.3 ms                                                | 18.3 ms: 1.06x faster                                               |
| sqlglot_parse            | 1.36 ms                                                | 1.29 ms: 1.06x faster                                               |
| pickle_pure_python       | 324 us                                                 | 307 us: 1.06x faster                                                |
| xml_etree_process        | 61.7 ms                                                | 58.5 ms: 1.05x faster                                               |
| deepcopy_memo            | 40.7 us                                                | 38.6 us: 1.05x faster                                               |
| chaos                    | 67.0 ms                                                | 63.6 ms: 1.05x faster                                               |
| fannkuch                 | 417 ms                                                 | 398 ms: 1.05x faster                                                |
| regex_compile            | 148 ms                                                 | 142 ms: 1.04x faster                                                |
| pickle_dict              | 35.5 us                                                | 34.2 us: 1.04x faster                                               |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                               |
| xml_etree_generate       | 89.2 ms                                                | 86.0 ms: 1.04x faster                                               |
| logging_silent           | 104 ns                                                 | 101 ns: 1.04x faster                                                |
| scimark_monte_carlo      | 75.1 ms                                                | 72.6 ms: 1.03x faster                                               |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                |
| meteor_contest           | 112 ms                                                 | 109 ms: 1.03x faster                                                |
| sympy_integrate          | 21.4 ms                                                | 20.8 ms: 1.03x faster                                               |
| nbody                    | 97.0 ms                                                | 94.1 ms: 1.03x faster                                               |
| json_loads               | 28.5 us                                                | 27.7 us: 1.03x faster                                               |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 707 ms: 1.03x faster                                                |
| docutils                 | 2.77 sec                                               | 2.70 sec: 1.03x faster                                              |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                |
| pickle                   | 11.6 us                                                | 11.3 us: 1.02x faster                                               |
| async_tree_memoization   | 578 ms                                                 | 566 ms: 1.02x faster                                                |
| pickle_list              | 5.08 us                                                | 4.98 us: 1.02x faster                                               |
| mdp                      | 2.63 sec                                               | 2.59 sec: 1.02x faster                                              |
| json_dumps               | 10.4 ms                                                | 10.2 ms: 1.01x faster                                               |
| spectral_norm            | 115 ms                                                 | 113 ms: 1.01x faster                                                |
| sympy_expand             | 478 ms                                                 | 473 ms: 1.01x faster                                                |
| pprint_pformat           | 1.57 sec                                               | 1.55 sec: 1.01x faster                                              |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                |
| asyncio_tcp              | 491 ms                                                 | 485 ms: 1.01x faster                                                |
| coroutines               | 23.2 ms                                                | 23.0 ms: 1.01x faster                                               |
| django_template          | 34.6 ms                                                | 34.3 ms: 1.01x faster                                               |
| async_generators         | 463 ms                                                 | 459 ms: 1.01x faster                                                |
| async_tree_none_tg       | 450 ms                                                 | 447 ms: 1.00x faster                                                |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x slower                                                |
| bench_thread_pool        | 842 us                                                 | 844 us: 1.00x slower                                                |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                              |
| 2to3                     | 274 ms                                                 | 277 ms: 1.01x slower                                                |
| aiohttp                  | 1.15 ms                                                | 1.16 ms: 1.01x slower                                               |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.01x slower                                              |
| pyflate                  | 482 ms                                                 | 490 ms: 1.01x slower                                                |
| richards_super           | 51.5 ms                                                | 52.3 ms: 1.02x slower                                               |
| sqlglot_optimize         | 54.8 ms                                                | 55.8 ms: 1.02x slower                                               |
| gunicorn                 | 1.24 ms                                                | 1.26 ms: 1.02x slower                                               |
| async_tree_io            | 1.16 sec                                               | 1.18 sec: 1.02x slower                                              |
| pycparser                | 1.18 sec                                               | 1.21 sec: 1.02x slower                                              |
| create_gc_cycles         | 1.48 ms                                                | 1.52 ms: 1.03x slower                                               |
| regex_effbot             | 3.61 ms                                                | 3.73 ms: 1.03x slower                                               |
| gc_traversal             | 3.79 ms                                                | 3.92 ms: 1.03x slower                                               |
| unpickle_pure_python     | 230 us                                                 | 238 us: 1.03x slower                                                |
| regex_v8                 | 23.1 ms                                                | 24.7 ms: 1.07x slower                                               |
| regex_dna                | 212 ms                                                 | 229 ms: 1.08x slower                                                |
| nqueens                  | 83.3 ms                                                | 90.2 ms: 1.08x slower                                               |
| hexiom                   | 6.41 ms                                                | 7.08 ms: 1.10x slower                                               |
| go                       | 139 ms                                                 | 155 ms: 1.11x slower                                                |
| scimark_lu               | 118 ms                                                 | 132 ms: 1.12x slower                                                |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                               |
| telco                    | 7.10 ms                                                | 8.29 ms: 1.17x slower                                               |
| python_startup           | 9.55 ms                                                | 12.3 ms: 1.29x slower                                               |
| coverage                 | 72.7 ms                                                | 95.6 ms: 1.32x slower                                               |
| dask                     | 372 ms                                                 | 534 ms: 1.44x slower                                                |
| python_startup_no_site   | 6.94 ms                                                | 11.0 ms: 1.58x slower                                               |
| unpack_sequence          | 54.0 ns                                                | 94.6 ns: 1.75x slower                                               |
| Geometric mean           | (ref)                                                  | 1.00x faster                                                        |

Benchmark hidden because not significant (10): pprint_safe_repr, sqlite_synth, scimark_sor, async_tree_cpu_io_mixed_tg, richards, asyncio_websockets, dulwich_log, async_tree_memoization_tg, json, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240229-3.13.0a4+-640fc6e-JIT/bm-20240229-linux-x86_64-brandtbucher-justin_nops-3.13.0a4+-640fc6e.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.15% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x