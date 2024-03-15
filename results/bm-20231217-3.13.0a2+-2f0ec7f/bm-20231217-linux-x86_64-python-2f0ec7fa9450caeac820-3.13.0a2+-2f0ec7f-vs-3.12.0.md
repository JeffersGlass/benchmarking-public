
# Results vs. 3.12.0

- fork: python
- ref: 2f0ec7fa9450caeac820
- machine: linux-x86_64
- commit hash: 2f0ec7f
- commit date: 2023-12-17
- overall geometric mean: 1.04x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.02x faster
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 262 ms: 1.05x faster                                                   |
| chameleon      | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                  |
| docutils       | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| tornado_http   | 103 ms                                                 | 93.8 ms: 1.09x faster                                                  |
| Geometric mean | (ref)                                                  | 1.07x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 472 ms                                                 | 438 ms: 1.08x faster                                                   |
| async_tree_memoization  | 578 ms                                                 | 564 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed | 726 ms                                                 | 710 ms: 1.02x faster                                                   |
| async_tree_none_tg      | 450 ms                                                 | 444 ms: 1.01x faster                                                   |
| async_tree_io_tg        | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io           | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| Geometric mean          | (ref)                                                  | 1.01x faster                                                           |

Benchmark hidden because not significant (2): async_tree_cpu_io_mixed_tg, async_tree_memoization_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 97.0 ms                                                | 88.8 ms: 1.09x faster                                                  |
| float          | 84.7 ms                                                | 80.8 ms: 1.05x faster                                                  |
| pidigits       | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| Geometric mean | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| regex_v8       | 23.1 ms                                                | 23.8 ms: 1.03x slower                                                  |
| regex_effbot   | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                  |
| regex_dna      | 212 ms                                                 | 229 ms: 1.08x slower                                                   |
| Geometric mean | (ref)                                                  | 1.00x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 295 us: 1.10x faster                                                   |
| tomli_loads          | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| unpickle             | 15.9 us                                                | 14.6 us: 1.09x faster                                                  |
| unpickle_pure_python | 230 us                                                 | 215 us: 1.07x faster                                                   |
| xml_etree_process    | 61.7 ms                                                | 58.3 ms: 1.06x faster                                                  |
| pickle_dict          | 35.5 us                                                | 33.7 us: 1.05x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                  |
| unpickle_list        | 5.29 us                                                | 5.06 us: 1.05x faster                                                  |
| pickle               | 11.6 us                                                | 11.2 us: 1.03x faster                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| pickle_list          | 5.08 us                                                | 4.96 us: 1.03x faster                                                  |
| json_loads           | 28.5 us                                                | 28.1 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| json_dumps           | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| Geometric mean       | (ref)                                                  | 1.05x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.15x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20231217-linux-x86_64-python-2f0ec7fa9450caeac820-3.13.0a2+-2f0ec7f |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 111 us: 1.42x faster                                                   |
| comprehensions           | 21.8 us                                                | 16.0 us: 1.36x faster                                                  |
| raytrace                 | 312 ms                                                 | 260 ms: 1.20x faster                                                   |
| deltablue                | 3.72 ms                                                | 3.19 ms: 1.17x faster                                                  |
| logging_format           | 7.23 us                                                | 6.20 us: 1.17x faster                                                  |
| logging_simple           | 6.46 us                                                | 5.63 us: 1.15x faster                                                  |
| regex_compile            | 148 ms                                                 | 129 ms: 1.15x faster                                                   |
| crypto_pyaes             | 81.9 ms                                                | 71.9 ms: 1.14x faster                                                  |
| sympy_sum                | 169 ms                                                 | 149 ms: 1.14x faster                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 66.5 ms: 1.13x faster                                                  |
| chaos                    | 67.0 ms                                                | 59.7 ms: 1.12x faster                                                  |
| sympy_str                | 300 ms                                                 | 269 ms: 1.11x faster                                                   |
| generators               | 31.2 ms                                                | 28.3 ms: 1.10x faster                                                  |
| sympy_integrate          | 21.4 ms                                                | 19.5 ms: 1.10x faster                                                  |
| pickle_pure_python       | 324 us                                                 | 295 us: 1.10x faster                                                   |
| sqlglot_parse            | 1.36 ms                                                | 1.24 ms: 1.09x faster                                                  |
| tornado_http             | 103 ms                                                 | 93.8 ms: 1.09x faster                                                  |
| tomli_loads              | 2.33 sec                                               | 2.13 sec: 1.09x faster                                                 |
| nbody                    | 97.0 ms                                                | 88.8 ms: 1.09x faster                                                  |
| unpickle                 | 15.9 us                                                | 14.6 us: 1.09x faster                                                  |
| async_tree_none          | 472 ms                                                 | 438 ms: 1.08x faster                                                   |
| sqlglot_transpile        | 1.68 ms                                                | 1.57 ms: 1.07x faster                                                  |
| gc_traversal             | 3.79 ms                                                | 3.54 ms: 1.07x faster                                                  |
| hexiom                   | 6.41 ms                                                | 6.00 ms: 1.07x faster                                                  |
| unpickle_pure_python     | 230 us                                                 | 215 us: 1.07x faster                                                   |
| scimark_sor              | 129 ms                                                 | 121 ms: 1.07x faster                                                   |
| chameleon                | 7.41 ms                                                | 6.96 ms: 1.06x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.15 us: 1.06x faster                                                  |
| docutils                 | 2.77 sec                                               | 2.61 sec: 1.06x faster                                                 |
| coroutines               | 23.2 ms                                                | 21.8 ms: 1.06x faster                                                  |
| deepcopy_memo            | 40.7 us                                                | 38.4 us: 1.06x faster                                                  |
| xml_etree_process        | 61.7 ms                                                | 58.3 ms: 1.06x faster                                                  |
| deepcopy                 | 371 us                                                 | 351 us: 1.06x faster                                                   |
| scimark_lu               | 118 ms                                                 | 112 ms: 1.05x faster                                                   |
| pyflate                  | 482 ms                                                 | 458 ms: 1.05x faster                                                   |
| pickle_dict              | 35.5 us                                                | 33.7 us: 1.05x faster                                                  |
| fannkuch                 | 417 ms                                                 | 397 ms: 1.05x faster                                                   |
| async_generators         | 463 ms                                                 | 440 ms: 1.05x faster                                                   |
| sympy_expand             | 478 ms                                                 | 455 ms: 1.05x faster                                                   |
| float                    | 84.7 ms                                                | 80.8 ms: 1.05x faster                                                  |
| mako                     | 11.9 ms                                                | 11.4 ms: 1.05x faster                                                  |
| meteor_contest           | 112 ms                                                 | 107 ms: 1.05x faster                                                   |
| xml_etree_generate       | 89.2 ms                                                | 85.2 ms: 1.05x faster                                                  |
| 2to3                     | 274 ms                                                 | 262 ms: 1.05x faster                                                   |
| unpickle_list            | 5.29 us                                                | 5.06 us: 1.05x faster                                                  |
| dulwich_log              | 68.5 ms                                                | 65.5 ms: 1.05x faster                                                  |
| sqlglot_normalize        | 110 ms                                                 | 106 ms: 1.04x faster                                                   |
| pathlib                  | 19.3 ms                                                | 18.5 ms: 1.04x faster                                                  |
| nqueens                  | 83.3 ms                                                | 79.8 ms: 1.04x faster                                                  |
| pprint_safe_repr         | 776 ms                                                 | 744 ms: 1.04x faster                                                   |
| pprint_pformat           | 1.57 sec                                               | 1.51 sec: 1.04x faster                                                 |
| mdp                      | 2.63 sec                                               | 2.53 sec: 1.04x faster                                                 |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.89 ms: 1.03x faster                                                  |
| pickle                   | 11.6 us                                                | 11.2 us: 1.03x faster                                                  |
| spectral_norm            | 115 ms                                                 | 111 ms: 1.03x faster                                                   |
| dask                     | 372 ms                                                 | 361 ms: 1.03x faster                                                   |
| sqlglot_optimize         | 54.8 ms                                                | 53.2 ms: 1.03x faster                                                  |
| scimark_fft              | 382 ms                                                 | 371 ms: 1.03x faster                                                   |
| xml_etree_iterparse      | 107 ms                                                 | 104 ms: 1.03x faster                                                   |
| asyncio_tcp              | 491 ms                                                 | 478 ms: 1.03x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.96 us: 1.03x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 564 ms: 1.02x faster                                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 710 ms: 1.02x faster                                                   |
| bench_thread_pool        | 842 us                                                 | 824 us: 1.02x faster                                                   |
| logging_silent           | 104 ns                                                 | 103 ns: 1.02x faster                                                   |
| unpack_sequence          | 54.0 ns                                                | 53.1 ns: 1.02x faster                                                  |
| json_loads               | 28.5 us                                                | 28.1 us: 1.02x faster                                                  |
| json                     | 5.26 ms                                                | 5.18 ms: 1.01x faster                                                  |
| xml_etree_parse          | 159 ms                                                 | 157 ms: 1.01x faster                                                   |
| async_tree_none_tg       | 450 ms                                                 | 444 ms: 1.01x faster                                                   |
| sqlite_synth             | 2.83 us                                                | 2.80 us: 1.01x faster                                                  |
| json_dumps               | 10.4 ms                                                | 10.3 ms: 1.01x faster                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.78 sec: 1.00x faster                                                 |
| pidigits                 | 187 ms                                                 | 187 ms: 1.00x faster                                                   |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| richards                 | 45.8 ms                                                | 47.0 ms: 1.03x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 23.8 ms: 1.03x slower                                                  |
| async_tree_io            | 1.16 sec                                               | 1.19 sec: 1.03x slower                                                 |
| regex_effbot             | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                  |
| richards_super           | 51.5 ms                                                | 53.2 ms: 1.03x slower                                                  |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.05x slower                                                  |
| regex_dna                | 212 ms                                                 | 229 ms: 1.08x slower                                                   |
| telco                    | 7.10 ms                                                | 8.20 ms: 1.15x slower                                                  |
| python_startup_no_site   | 6.94 ms                                                | 8.70 ms: 1.25x slower                                                  |
| coverage                 | 72.7 ms                                                | 95.2 ms: 1.31x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.04x faster                                                           |

Benchmark hidden because not significant (8): async_tree_cpu_io_mixed_tg, go, bench_mp_pool, asyncio_websockets, create_gc_cycles, pycparser, async_tree_memoization_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.03x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.02x


# Memory

- memory change: 0.93x