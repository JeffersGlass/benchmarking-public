
# Results vs. 3.10.4

- fork: python
- ref: a2bb8ad14409c7ecb8de
- machine: linux-x86_64
- commit hash: a2bb8ad
- commit date: 2024-02-20
- overall geometric mean: 1.24x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.16x faster
- Memory change: 1.07x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 292 ms: 1.19x faster                                                   |
| chameleon      | 9.68 ms                                                | 7.23 ms: 1.34x faster                                                  |
| docutils       | 3.30 sec                                               | 2.81 sec: 1.17x faster                                                 |
| tornado_http   | 136 ms                                                 | 99.1 ms: 1.38x faster                                                  |
| Geometric mean | (ref)                                                  | 1.27x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 451 ms: 1.61x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 579 ms: 1.50x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 727 ms: 1.40x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.49x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 114 ms: 1.35x faster                                                   |
| float          | 117 ms                                                 | 90.8 ms: 1.29x faster                                                  |
| pidigits       | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.21x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 172 ms: 1.10x faster                                                   |
| regex_v8       | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                  |
| regex_dna      | 227 ms                                                 | 230 ms: 1.01x slower                                                   |
| regex_effbot   | 3.63 ms                                                | 3.85 ms: 1.06x slower                                                  |
| Geometric mean | (ref)                                                  | 1.02x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 301 us: 1.61x faster                                                   |
| json_dumps           | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 60.9 ms: 1.30x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 271 us: 1.22x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.63 sec: 1.19x faster                                                 |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.96 us: 1.05x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| pickle_list          | 5.08 us                                                | 5.23 us: 1.03x slower                                                  |
| unpickle             | 14.4 us                                                | 15.6 us: 1.09x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict          | 29.6 us                                                | 34.6 us: 1.17x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.11x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.85 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 13.0 ms: 1.26x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 113 us: 4.80x faster                                                   |
| generators               | 80.1 ms                                                | 29.7 ms: 2.70x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.70 ms: 2.14x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 493 ms: 1.87x faster                                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.81x faster                                                   |
| async_tree_none          | 728 ms                                                 | 451 ms: 1.61x faster                                                   |
| pickle_pure_python       | 484 us                                                 | 301 us: 1.61x faster                                                   |
| scimark_sor              | 220 ms                                                 | 141 ms: 1.56x faster                                                   |
| chaos                    | 115 ms                                                 | 74.4 ms: 1.55x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.41 ms: 1.54x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 83.8 ms: 1.52x faster                                                  |
| coroutines               | 35.1 ms                                                | 23.1 ms: 1.52x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 579 ms: 1.50x faster                                                   |
| raytrace                 | 507 ms                                                 | 339 ms: 1.49x faster                                                   |
| richards_super           | 94.7 ms                                                | 64.2 ms: 1.48x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.75 ms: 1.47x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.21 sec: 1.46x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 41.0 us: 1.43x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.81 sec: 1.42x faster                                                 |
| scimark_monte_carlo      | 118 ms                                                 | 84.3 ms: 1.40x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 727 ms: 1.40x faster                                                   |
| comprehensions           | 28.8 us                                                | 20.7 us: 1.39x faster                                                  |
| go                       | 240 ms                                                 | 173 ms: 1.38x faster                                                   |
| richards                 | 79.3 ms                                                | 57.6 ms: 1.38x faster                                                  |
| tornado_http             | 136 ms                                                 | 99.1 ms: 1.38x faster                                                  |
| logging_simple           | 8.30 us                                                | 6.16 us: 1.35x faster                                                  |
| deepcopy                 | 479 us                                                 | 356 us: 1.35x faster                                                   |
| nbody                    | 154 ms                                                 | 114 ms: 1.35x faster                                                   |
| chameleon                | 9.68 ms                                                | 7.23 ms: 1.34x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.6 ms: 1.34x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.14 us: 1.33x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 60.9 ms: 1.30x faster                                                  |
| logging_format           | 9.09 us                                                | 7.00 us: 1.30x faster                                                  |
| float                    | 117 ms                                                 | 90.8 ms: 1.29x faster                                                  |
| spectral_norm            | 170 ms                                                 | 132 ms: 1.29x faster                                                   |
| pyflate                  | 716 ms                                                 | 565 ms: 1.27x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 113 ms: 1.26x faster                                                   |
| mako                     | 16.3 ms                                                | 13.0 ms: 1.26x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 21.1 ms: 1.22x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 271 us: 1.22x faster                                                   |
| sympy_sum                | 196 ms                                                 | 163 ms: 1.21x faster                                                   |
| pprint_safe_repr         | 1.02 sec                                               | 844 ms: 1.21x faster                                                   |
| dask                     | 441 ms                                                 | 367 ms: 1.20x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.76 sec: 1.19x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.63 sec: 1.19x faster                                                 |
| 2to3                     | 348 ms                                                 | 292 ms: 1.19x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.32 sec: 1.19x faster                                                 |
| dulwich_log              | 84.3 ms                                                | 72.0 ms: 1.17x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.81 sec: 1.17x faster                                                 |
| sympy_str                | 346 ms                                                 | 297 ms: 1.17x faster                                                   |
| hexiom                   | 10.4 ms                                                | 8.93 ms: 1.16x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 856 us: 1.15x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 60.2 ms: 1.15x faster                                                  |
| scimark_lu               | 176 ms                                                 | 154 ms: 1.14x faster                                                   |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.68 ms: 1.14x faster                                                  |
| fannkuch                 | 532 ms                                                 | 468 ms: 1.14x faster                                                   |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                  |
| sympy_expand             | 566 ms                                                 | 502 ms: 1.13x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 89.1 ms: 1.12x faster                                                  |
| json                     | 5.69 ms                                                | 5.14 ms: 1.11x faster                                                  |
| scimark_fft              | 466 ms                                                 | 424 ms: 1.10x faster                                                   |
| regex_compile            | 188 ms                                                 | 172 ms: 1.10x faster                                                   |
| nqueens                  | 106 ms                                                 | 97.8 ms: 1.08x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.9 ms: 1.08x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 55.8 ns: 1.07x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 25.9 ms: 1.07x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.07x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.52 ms: 1.06x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.88 us: 1.05x faster                                                  |
| unpickle_list            | 5.20 us                                                | 4.96 us: 1.05x faster                                                  |
| meteor_contest           | 120 ms                                                 | 115 ms: 1.04x faster                                                   |
| xml_etree_iterparse      | 115 ms                                                 | 111 ms: 1.04x faster                                                   |
| pidigits                 | 191 ms                                                 | 189 ms: 1.01x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 230 ms: 1.01x slower                                                   |
| pickle_list              | 5.08 us                                                | 5.23 us: 1.03x slower                                                  |
| async_generators         | 444 ms                                                 | 465 ms: 1.05x slower                                                   |
| regex_effbot             | 3.63 ms                                                | 3.85 ms: 1.06x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.87 ms: 1.07x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.6 us: 1.09x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict              | 29.6 us                                                | 34.6 us: 1.17x slower                                                  |
| telco                    | 7.27 ms                                                | 8.72 ms: 1.20x slower                                                  |
| coverage                 | 79.4 ms                                                | 97.0 ms: 1.22x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.85 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.24x faster                                                           |

Benchmark hidden because not significant (3): mdp, bench_mp_pool, mypy2
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240220-3.13.0a4+-a2bb8ad-PYTHON_UOPS/bm-20240220-linux-x86_64-python-a2bb8ad14409c7ecb8de-3.13.0a4+-a2bb8ad.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.18x
- 95% likely to have a speedup of 1.17x
- 99% likely to have a speedup of 1.16x


# Memory

- memory change: 1.07x