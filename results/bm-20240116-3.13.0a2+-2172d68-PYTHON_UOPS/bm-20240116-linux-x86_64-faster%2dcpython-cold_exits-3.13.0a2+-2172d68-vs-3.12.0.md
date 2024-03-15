
# Results vs. 3.12.0

- fork: faster-cpython
- ref: cold_exits
- machine: linux-x86_64
- commit hash: 2172d68
- commit date: 2024-01-16
- overall geometric mean: 1.05x slower
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x slower
- Memory change: 0.93x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| chameleon      | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                  |
| docutils       | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                 |
| tornado_http   | 103 ms                                                 | 97.9 ms: 1.05x faster                                                  |
| Geometric mean | (ref)                                                  | 1.01x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none        | 472 ms                                                 | 451 ms: 1.05x faster                                                   |
| async_tree_memoization | 578 ms                                                 | 570 ms: 1.01x faster                                                   |
| async_tree_none_tg     | 450 ms                                                 | 446 ms: 1.01x faster                                                   |
| async_tree_io_tg       | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| async_tree_io          | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (3): async_tree_cpu_io_mixed, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pidigits       | 187 ms                                                 | 197 ms: 1.05x slower                                                   |
| float          | 84.7 ms                                                | 92.1 ms: 1.09x slower                                                  |
| nbody          | 97.0 ms                                                | 115 ms: 1.19x slower                                                   |
| Geometric mean | (ref)                                                  | 1.11x slower                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                  |
| regex_dna      | 212 ms                                                 | 226 ms: 1.07x slower                                                   |
| regex_v8       | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| regex_compile  | 148 ms                                                 | 170 ms: 1.15x slower                                                   |
| Geometric mean | (ref)                                                  | 1.08x slower                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 324 us                                                 | 300 us: 1.08x faster                                                   |
| unpickle             | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.88 us: 1.04x faster                                                  |
| pickle_dict          | 35.5 us                                                | 34.4 us: 1.03x faster                                                  |
| pickle               | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| xml_etree_parse      | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads           | 28.5 us                                                | 28.4 us: 1.01x faster                                                  |
| xml_etree_generate   | 89.2 ms                                                | 89.9 ms: 1.01x slower                                                  |
| unpickle_pure_python | 230 us                                                 | 233 us: 1.01x slower                                                   |
| unpickle_list        | 5.29 us                                                | 5.36 us: 1.01x slower                                                  |
| json_dumps           | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                  |
| xml_etree_iterparse  | 107 ms                                                 | 112 ms: 1.05x slower                                                   |
| tomli_loads          | 2.33 sec                                               | 2.71 sec: 1.16x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.00x slower                                                           |

Benchmark hidden because not significant (1): xml_etree_process

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| python_startup_no_site | 6.94 ms                                                | 8.78 ms: 1.27x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.16x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                  |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20240116-linux-x86_64-faster%2dcpython-cold_exits-3.13.0a2+-2172d68 |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 158 us                                                 | 119 us: 1.33x faster                                                   |
| pickle_pure_python       | 324 us                                                 | 300 us: 1.08x faster                                                   |
| generators               | 31.2 ms                                                | 29.1 ms: 1.07x faster                                                  |
| unpickle                 | 15.9 us                                                | 14.9 us: 1.06x faster                                                  |
| deepcopy_reduce          | 3.35 us                                                | 3.19 us: 1.05x faster                                                  |
| coroutines               | 23.2 ms                                                | 22.1 ms: 1.05x faster                                                  |
| tornado_http             | 103 ms                                                 | 97.9 ms: 1.05x faster                                                  |
| async_tree_none          | 472 ms                                                 | 451 ms: 1.05x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.88 us: 1.04x faster                                                  |
| sympy_sum                | 169 ms                                                 | 163 ms: 1.03x faster                                                   |
| raytrace                 | 312 ms                                                 | 302 ms: 1.03x faster                                                   |
| pickle_dict              | 35.5 us                                                | 34.4 us: 1.03x faster                                                  |
| deepcopy                 | 371 us                                                 | 361 us: 1.03x faster                                                   |
| comprehensions           | 21.8 us                                                | 21.2 us: 1.03x faster                                                  |
| chameleon                | 7.41 ms                                                | 7.27 ms: 1.02x faster                                                  |
| pickle                   | 11.6 us                                                | 11.4 us: 1.02x faster                                                  |
| async_tree_memoization   | 578 ms                                                 | 570 ms: 1.01x faster                                                   |
| pathlib                  | 19.3 ms                                                | 19.1 ms: 1.01x faster                                                  |
| logging_simple           | 6.46 us                                                | 6.39 us: 1.01x faster                                                  |
| async_generators         | 463 ms                                                 | 459 ms: 1.01x faster                                                   |
| gc_traversal             | 3.79 ms                                                | 3.76 ms: 1.01x faster                                                  |
| async_tree_none_tg       | 450 ms                                                 | 446 ms: 1.01x faster                                                   |
| docutils                 | 2.77 sec                                               | 2.75 sec: 1.01x faster                                                 |
| xml_etree_parse          | 159 ms                                                 | 158 ms: 1.01x faster                                                   |
| json_loads               | 28.5 us                                                | 28.4 us: 1.01x faster                                                  |
| asyncio_tcp              | 491 ms                                                 | 493 ms: 1.00x slower                                                   |
| sqlite_synth             | 2.83 us                                                | 2.85 us: 1.01x slower                                                  |
| asyncio_tcp_ssl          | 1.79 sec                                               | 1.80 sec: 1.01x slower                                                 |
| xml_etree_generate       | 89.2 ms                                                | 89.9 ms: 1.01x slower                                                  |
| unpickle_pure_python     | 230 us                                                 | 233 us: 1.01x slower                                                   |
| sympy_integrate          | 21.4 ms                                                | 21.7 ms: 1.01x slower                                                  |
| unpickle_list            | 5.29 us                                                | 5.36 us: 1.01x slower                                                  |
| bench_thread_pool        | 842 us                                                 | 855 us: 1.02x slower                                                   |
| sqlglot_parse            | 1.36 ms                                                | 1.38 ms: 1.02x slower                                                  |
| sqlglot_transpile        | 1.68 ms                                                | 1.71 ms: 1.02x slower                                                  |
| async_tree_io_tg         | 1.18 sec                                               | 1.20 sec: 1.02x slower                                                 |
| crypto_pyaes             | 81.9 ms                                                | 83.5 ms: 1.02x slower                                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.51 ms: 1.02x slower                                                  |
| deepcopy_memo            | 40.7 us                                                | 41.7 us: 1.02x slower                                                  |
| logging_silent           | 104 ns                                                 | 107 ns: 1.03x slower                                                   |
| pycparser                | 1.18 sec                                               | 1.21 sec: 1.03x slower                                                 |
| json_dumps               | 10.4 ms                                                | 10.7 ms: 1.03x slower                                                  |
| regex_effbot             | 3.61 ms                                                | 3.72 ms: 1.03x slower                                                  |
| meteor_contest           | 112 ms                                                 | 116 ms: 1.03x slower                                                   |
| sympy_expand             | 478 ms                                                 | 500 ms: 1.05x slower                                                   |
| async_tree_io            | 1.16 sec                                               | 1.21 sec: 1.05x slower                                                 |
| dulwich_log              | 68.5 ms                                                | 71.8 ms: 1.05x slower                                                  |
| xml_etree_iterparse      | 107 ms                                                 | 112 ms: 1.05x slower                                                   |
| 2to3                     | 274 ms                                                 | 288 ms: 1.05x slower                                                   |
| pidigits                 | 187 ms                                                 | 197 ms: 1.05x slower                                                   |
| sqlglot_normalize        | 110 ms                                                 | 116 ms: 1.05x slower                                                   |
| mdp                      | 2.63 sec                                               | 2.78 sec: 1.06x slower                                                 |
| python_startup           | 9.55 ms                                                | 10.1 ms: 1.06x slower                                                  |
| unpack_sequence          | 54.0 ns                                                | 57.5 ns: 1.07x slower                                                  |
| regex_dna                | 212 ms                                                 | 226 ms: 1.07x slower                                                   |
| scimark_sor              | 129 ms                                                 | 139 ms: 1.07x slower                                                   |
| float                    | 84.7 ms                                                | 92.1 ms: 1.09x slower                                                  |
| regex_v8                 | 23.1 ms                                                | 25.2 ms: 1.09x slower                                                  |
| richards                 | 45.8 ms                                                | 50.0 ms: 1.09x slower                                                  |
| sqlglot_optimize         | 54.8 ms                                                | 59.9 ms: 1.09x slower                                                  |
| richards_super           | 51.5 ms                                                | 56.5 ms: 1.10x slower                                                  |
| pprint_safe_repr         | 776 ms                                                 | 856 ms: 1.10x slower                                                   |
| chaos                    | 67.0 ms                                                | 74.4 ms: 1.11x slower                                                  |
| pprint_pformat           | 1.57 sec                                               | 1.78 sec: 1.13x slower                                                 |
| mako                     | 11.9 ms                                                | 13.6 ms: 1.14x slower                                                  |
| regex_compile            | 148 ms                                                 | 170 ms: 1.15x slower                                                   |
| tomli_loads              | 2.33 sec                                               | 2.71 sec: 1.16x slower                                                 |
| fannkuch                 | 417 ms                                                 | 487 ms: 1.17x slower                                                   |
| scimark_fft              | 382 ms                                                 | 449 ms: 1.18x slower                                                   |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 5.98 ms: 1.18x slower                                                  |
| nqueens                  | 83.3 ms                                                | 98.8 ms: 1.19x slower                                                  |
| nbody                    | 97.0 ms                                                | 115 ms: 1.19x slower                                                   |
| scimark_monte_carlo      | 75.1 ms                                                | 89.5 ms: 1.19x slower                                                  |
| pyflate                  | 482 ms                                                 | 582 ms: 1.21x slower                                                   |
| telco                    | 7.10 ms                                                | 8.69 ms: 1.22x slower                                                  |
| go                       | 139 ms                                                 | 175 ms: 1.25x slower                                                   |
| spectral_norm            | 115 ms                                                 | 145 ms: 1.26x slower                                                   |
| scimark_lu               | 118 ms                                                 | 149 ms: 1.26x slower                                                   |
| python_startup_no_site   | 6.94 ms                                                | 8.78 ms: 1.27x slower                                                  |
| deltablue                | 3.72 ms                                                | 4.82 ms: 1.30x slower                                                  |
| coverage                 | 72.7 ms                                                | 95.8 ms: 1.32x slower                                                  |
| hexiom                   | 6.41 ms                                                | 9.05 ms: 1.41x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.05x slower                                                           |

Benchmark hidden because not significant (11): dask, async_tree_cpu_io_mixed, sympy_str, json, bench_mp_pool, xml_etree_process, asyncio_websockets, logging_format, async_tree_memoization_tg, async_tree_cpu_io_mixed_tg, mypy2
Ignored benchmarks (5) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: aiohttp, django_template, gunicorn, sqlalchemy_declarative, sqlalchemy_imperative


# HPT report

- Reliability score: 100.00% likely to be slow
- 90% likely to have a slowdown of 1.02x
- 95% likely to have a slowdown of 1.02x
- 99% likely to have a slowdown of 1.01x


# Memory

- memory change: 0.93x