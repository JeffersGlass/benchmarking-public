# Results vs. 3.12.0

- fork: gvanrossum
- ref: kenjin_tier2_inliner
- machine: linux-x86_64
- commit hash: 2f9539b
- commit date: 2024-03-05
- overall geometric mean: 1.00x faster \*
- HPT reliability: 98.99%
- HPT 99th percentile: 1.00x faster
- Memory change: 1.17x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 277 ms: 1.01x slower                                                       |
| chameleon      | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                      |
| docutils       | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                     |
| tornado_http   | 103 ms                                                 | 96.9 ms: 1.06x faster                                                      |
| Geometric mean | (ref)                                                  | 1.04x faster                                                               |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 437 ms: 1.08x faster                                                       |
| async_tree_memoization  | 578 ms                                                 | 562 ms: 1.03x faster                                                       |
| async_tree_cpu_io_mixed | 726 ms                                                 | 707 ms: 1.03x faster                                                       |
| async_tree_none_tg      | 450 ms                                                 | 448 ms: 1.00x faster                                                       |
| async_tree_io_tg        | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                     |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                     |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                               |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| float          | 84.7 ms                                                | 78.2 ms: 1.08x faster                                                      |
| nbody          | 97.0 ms                                                | 95.8 ms: 1.01x faster                                                      |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                       |
| Geometric mean | (ref)                                                  | 1.03x faster                                                               |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 142 ms: 1.04x faster                                                       |
| regex_effbot   | 3.61 ms                                                | 3.73 ms: 1.03x slower                                                      |
| regex_dna      | 212 ms                                                 | 223 ms: 1.05x slower                                                       |
| regex_v8       | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                      |
| Geometric mean | (ref)                                                  | 1.03x slower                                                               |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| tomli_loads          | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                     |
| pickle_pure_python   | 324 us                                                 | 298 us: 1.09x faster                                                       |
| unpickle_list        | 5.29 us                                                | 4.97 us: 1.06x faster                                                      |
| xml_etree_process    | 61.7 ms                                                | 59.0 ms: 1.05x faster                                                      |
| unpickle             | 15.9 us                                                | 15.2 us: 1.04x faster                                                      |
| json_loads           | 28.5 us                                                | 27.5 us: 1.04x faster                                                      |
| pickle_dict          | 35.5 us                                                | 34.6 us: 1.03x faster                                                      |
| xml_etree_generate   | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                      |
| xml_etree_parse      | 159 ms                                                 | 156 ms: 1.02x faster                                                       |
| pickle               | 11.6 us                                                | 11.5 us: 1.01x faster                                                      |
| xml_etree_iterparse  | 107 ms                                                 | 106 ms: 1.01x faster                                                       |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                      |
| unpickle_pure_python | 230 us                                                 | 238 us: 1.03x slower                                                       |
| Geometric mean       | (ref)                                                  | 1.03x faster                                                               |

Benchmark hidden because not significant (1): json_dumps

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 12.4 ms: 1.29x slower                                                      |
| python_startup_no_site | 6.94 ms                                                | 11.0 ms: 1.58x slower                                                      |
| Geometric mean         | (ref)                                                  | 1.43x slower                                                               |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|-----------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| mako            | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                      |
| django_template | 34.6 ms                                                | 33.9 ms: 1.02x faster                                                      |
| Geometric mean  | (ref)                                                  | 1.06x faster                                                               |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 112 us: 1.41x faster                                                       |
| comprehensions           | 21.8 us                                                | 17.5 us: 1.25x faster                                                      |
| logging_format           | 7.23 us                                                | 6.23 us: 1.16x faster                                                      |
| tomli_loads              | 2.33 sec                                               | 2.02 sec: 1.15x faster                                                     |
| logging_simple           | 6.46 us                                                | 5.64 us: 1.15x faster                                                      |
| scimark_fft              | 382 ms                                                 | 342 ms: 1.12x faster                                                       |
| crypto_pyaes             | 81.9 ms                                                | 73.3 ms: 1.12x faster                                                      |
| mako                     | 11.9 ms                                                | 10.7 ms: 1.11x faster                                                      |
| deltablue                | 3.72 ms                                                | 3.39 ms: 1.10x faster                                                      |
| pickle_pure_python       | 324 us                                                 | 298 us: 1.09x faster                                                       |
| deepcopy_reduce          | 3.35 us                                                | 3.09 us: 1.08x faster                                                      |
| float                    | 84.7 ms                                                | 78.2 ms: 1.08x faster                                                      |
| raytrace                 | 312 ms                                                 | 288 ms: 1.08x faster                                                       |
| chameleon                | 7.41 ms                                                | 6.86 ms: 1.08x faster                                                      |
| async_tree_none          | 472 ms                                                 | 437 ms: 1.08x faster                                                       |
| sympy_sum                | 169 ms                                                 | 157 ms: 1.08x faster                                                       |
| sympy_str                | 300 ms                                                 | 279 ms: 1.07x faster                                                       |
| chaos                    | 67.0 ms                                                | 62.5 ms: 1.07x faster                                                      |
| sqlglot_parse            | 1.36 ms                                                | 1.28 ms: 1.06x faster                                                      |
| scimark_monte_carlo      | 75.1 ms                                                | 70.6 ms: 1.06x faster                                                      |
| unpickle_list            | 5.29 us                                                | 4.97 us: 1.06x faster                                                      |
| tornado_http             | 103 ms                                                 | 96.9 ms: 1.06x faster                                                      |
| fannkuch                 | 417 ms                                                 | 394 ms: 1.06x faster                                                       |
| generators               | 31.2 ms                                                | 29.5 ms: 1.06x faster                                                      |
| deepcopy                 | 371 us                                                 | 353 us: 1.05x faster                                                       |
| pathlib                  | 19.3 ms                                                | 18.4 ms: 1.05x faster                                                      |
| xml_etree_process        | 61.7 ms                                                | 59.0 ms: 1.05x faster                                                      |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                       |
| unpickle                 | 15.9 us                                                | 15.2 us: 1.04x faster                                                      |
| regex_compile            | 148 ms                                                 | 142 ms: 1.04x faster                                                       |
| logging_silent           | 104 ns                                                 | 100 ns: 1.04x faster                                                       |
| pprint_safe_repr         | 776 ms                                                 | 745 ms: 1.04x faster                                                       |
| sqlglot_transpile        | 1.68 ms                                                | 1.62 ms: 1.04x faster                                                      |
| json_loads               | 28.5 us                                                | 27.5 us: 1.04x faster                                                      |
| deepcopy_memo            | 40.7 us                                                | 39.3 us: 1.04x faster                                                      |
| sqlglot_normalize        | 110 ms                                                 | 107 ms: 1.03x faster                                                       |
| coroutines               | 23.2 ms                                                | 22.5 ms: 1.03x faster                                                      |
| json                     | 5.26 ms                                                | 5.11 ms: 1.03x faster                                                      |
| pickle_dict              | 35.5 us                                                | 34.6 us: 1.03x faster                                                      |
| async_tree_memoization   | 578 ms                                                 | 562 ms: 1.03x faster                                                       |
| xml_etree_generate       | 89.2 ms                                                | 86.8 ms: 1.03x faster                                                      |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 707 ms: 1.03x faster                                                       |
| sympy_integrate          | 21.4 ms                                                | 20.9 ms: 1.03x faster                                                      |
| docutils                 | 2.77 sec                                               | 2.71 sec: 1.02x faster                                                     |
| django_template          | 34.6 ms                                                | 33.9 ms: 1.02x faster                                                      |
| xml_etree_parse          | 159 ms                                                 | 156 ms: 1.02x faster                                                       |
| pprint_pformat           | 1.57 sec                                               | 1.54 sec: 1.02x faster                                                     |
| spectral_norm            | 115 ms                                                 | 113 ms: 1.01x faster                                                       |
| mdp                      | 2.63 sec                                               | 2.60 sec: 1.01x faster                                                     |
| nbody                    | 97.0 ms                                                | 95.8 ms: 1.01x faster                                                      |
| pickle                   | 11.6 us                                                | 11.5 us: 1.01x faster                                                      |
| sympy_expand             | 478 ms                                                 | 474 ms: 1.01x faster                                                       |
| sqlite_synth             | 2.83 us                                                | 2.81 us: 1.01x faster                                                      |
| xml_etree_iterparse      | 107 ms                                                 | 106 ms: 1.01x faster                                                       |
| asyncio_tcp              | 491 ms                                                 | 487 ms: 1.01x faster                                                       |
| richards                 | 45.8 ms                                                | 45.5 ms: 1.01x faster                                                      |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.02 ms: 1.01x faster                                                      |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                       |
| async_tree_none_tg       | 450 ms                                                 | 448 ms: 1.00x faster                                                       |
| bench_thread_pool        | 842 us                                                 | 846 us: 1.01x slower                                                       |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                     |
| richards_super           | 51.5 ms                                                | 51.8 ms: 1.01x slower                                                      |
| dulwich_log              | 68.5 ms                                                | 68.9 ms: 1.01x slower                                                      |
| 2to3                     | 274 ms                                                 | 277 ms: 1.01x slower                                                       |
| aiohttp                  | 1.15 ms                                                | 1.16 ms: 1.01x slower                                                      |
| create_gc_cycles         | 1.48 ms                                                | 1.50 ms: 1.01x slower                                                      |
| sqlglot_optimize         | 54.8 ms                                                | 55.6 ms: 1.01x slower                                                      |
| gunicorn                 | 1.24 ms                                                | 1.27 ms: 1.02x slower                                                      |
| async_tree_io_tg         | 1.18 sec                                               | 1.21 sec: 1.02x slower                                                     |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                     |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                                      |
| pycparser                | 1.18 sec                                               | 1.22 sec: 1.03x slower                                                     |
| regex_effbot             | 3.61 ms                                                | 3.73 ms: 1.03x slower                                                      |
| unpickle_pure_python     | 230 us                                                 | 238 us: 1.03x slower                                                       |
| regex_dna                | 212 ms                                                 | 223 ms: 1.05x slower                                                       |
| gc_traversal             | 3.79 ms                                                | 4.03 ms: 1.06x slower                                                      |
| nqueens                  | 83.3 ms                                                | 89.7 ms: 1.08x slower                                                      |
| hexiom                   | 6.41 ms                                                | 7.00 ms: 1.09x slower                                                      |
| regex_v8                 | 23.1 ms                                                | 25.5 ms: 1.10x slower                                                      |
| scimark_lu               | 118 ms                                                 | 130 ms: 1.10x slower                                                       |
| go                       | 139 ms                                                 | 156 ms: 1.12x slower                                                       |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.17x slower                                                      |
| telco                    | 7.10 ms                                                | 8.48 ms: 1.19x slower                                                      |
| python_startup           | 9.55 ms                                                | 12.4 ms: 1.29x slower                                                      |
| coverage                 | 72.7 ms                                                | 97.1 ms: 1.34x slower                                                      |
| dask                     | 372 ms                                                 | 533 ms: 1.43x slower                                                       |
| python_startup_no_site   | 6.94 ms                                                | 11.0 ms: 1.58x slower                                                      |
| unpack_sequence          | 54.0 ns                                                | 96.7 ns: 1.79x slower                                                      |
| Geometric mean           | (ref)                                                  | 1.00x faster                                                               |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, pyflate, async_tree_memoization_tg, async_generators, asyncio_websockets, json_dumps, scimark_sor, mypy2
Ignored benchmarks (2) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: sqlalchemy_declarative, sqlalchemy_imperative
Ignored benchmarks (6) of results/bm-20240305-3.13.0a4+-2f9539b-JIT/bm-20240305-linux-x86_64-gvanrossum-kenjin_tier2_inliner-3.13.0a4+-2f9539b.json: djangocms, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 98.99% likely to be faster
- 90% likely to have a speedup of 1.00x
- 95% likely to have a speedup of 1.00x
- 99% likely to have a speedup of 1.00x


# Memory

- memory change: 1.17x