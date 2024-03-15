
# Results vs. 3.10.4

- fork: mdboom
- ref: mdboom_compact_int_s
- machine: linux-x86_64
- commit hash: 344a5aa
- commit date: 2023-12-20
- overall geometric mean: 1.35x faster
- HPT reliability: 100.00%
- HPT 99th percentile: 1.28x faster
- Memory change: 1.05x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.94 ms: 1.40x faster                                                  |
| docutils       | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.8 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.35x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 435 ms: 1.68x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.49x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 715 ms: 1.42x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 91.9 ms: 1.67x faster                                                  |
| float          | 117 ms                                                 | 81.6 ms: 1.43x faster                                                  |
| pidigits       | 191 ms                                                 | 226 ms: 1.18x slower                                                   |
| Geometric mean | (ref)                                                  | 1.27x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 135 ms: 1.40x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.1 ms: 1.15x faster                                                  |
| regex_dna      | 227 ms                                                 | 220 ms: 1.03x faster                                                   |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 304 us: 1.59x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 219 us: 1.51x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.16 sec: 1.46x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.8 ms: 1.35x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 85.4 ms: 1.16x faster                                                  |
| json_loads           | 31.2 us                                                | 27.8 us: 1.12x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.07x faster                                                   |
| unpickle_list        | 5.20 us                                                | 5.05 us: 1.03x faster                                                  |
| pickle_list          | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| unpickle             | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle               | 10.7 us                                                | 11.1 us: 1.04x slower                                                  |
| pickle_dict          | 29.6 us                                                | 33.1 us: 1.12x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.17x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.3 ms: 1.41x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.95 ms: 1.51x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.03x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 117 us: 4.66x faster                                                   |
| generators               | 80.1 ms                                                | 29.7 ms: 2.70x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.37 ms: 2.35x faster                                                  |
| chaos                    | 115 ms                                                 | 60.4 ms: 1.91x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 484 ms: 1.91x faster                                                   |
| raytrace                 | 507 ms                                                 | 275 ms: 1.84x faster                                                   |
| logging_silent           | 190 ns                                                 | 105 ns: 1.80x faster                                                   |
| scimark_sor              | 220 ms                                                 | 123 ms: 1.78x faster                                                   |
| richards_super           | 94.7 ms                                                | 53.7 ms: 1.76x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 72.8 ms: 1.76x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.6 us: 1.74x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 68.5 ms: 1.73x faster                                                  |
| go                       | 240 ms                                                 | 140 ms: 1.71x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.28 ms: 1.70x faster                                                  |
| hexiom                   | 10.4 ms                                                | 6.12 ms: 1.70x faster                                                  |
| async_tree_none          | 728 ms                                                 | 435 ms: 1.68x faster                                                   |
| nbody                    | 154 ms                                                 | 91.9 ms: 1.67x faster                                                  |
| richards                 | 79.3 ms                                                | 48.2 ms: 1.65x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.60 ms: 1.61x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 304 us: 1.59x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.0 ms: 1.59x faster                                                  |
| pyflate                  | 716 ms                                                 | 453 ms: 1.58x faster                                                   |
| async_tree_memoization   | 870 ms                                                 | 559 ms: 1.56x faster                                                   |
| spectral_norm            | 170 ms                                                 | 110 ms: 1.54x faster                                                   |
| scimark_lu               | 176 ms                                                 | 116 ms: 1.51x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 38.8 us: 1.51x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 219 us: 1.51x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.49x faster                                                 |
| mako                     | 16.3 ms                                                | 11.1 ms: 1.47x faster                                                  |
| logging_format           | 9.09 us                                                | 6.20 us: 1.47x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.16 sec: 1.46x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.72 us: 1.45x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| tornado_http             | 136 ms                                                 | 94.8 ms: 1.44x faster                                                  |
| float                    | 117 ms                                                 | 81.6 ms: 1.43x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 715 ms: 1.42x faster                                                   |
| python_startup           | 14.6 ms                                                | 10.3 ms: 1.41x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                                 |
| regex_compile            | 188 ms                                                 | 135 ms: 1.40x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.94 ms: 1.40x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 734 ms: 1.39x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 43.4 ns: 1.38x faster                                                  |
| deepcopy                 | 479 us                                                 | 350 us: 1.37x faster                                                   |
| json_dumps               | 14.2 ms                                                | 10.4 ms: 1.37x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.35x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 58.8 ms: 1.35x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 106 ms: 1.34x faster                                                   |
| fannkuch                 | 532 ms                                                 | 396 ms: 1.34x faster                                                   |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                   |
| deepcopy_reduce          | 4.17 us                                                | 3.13 us: 1.33x faster                                                  |
| sympy_integrate          | 25.8 ms                                                | 19.5 ms: 1.33x faster                                                  |
| 2to3                     | 348 ms                                                 | 264 ms: 1.32x faster                                                   |
| nqueens                  | 106 ms                                                 | 81.6 ms: 1.30x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.02 ms: 1.29x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 53.8 ms: 1.29x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.7 ms: 1.28x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.60 sec: 1.27x faster                                                 |
| scimark_fft              | 466 ms                                                 | 367 ms: 1.27x faster                                                   |
| sympy_str                | 346 ms                                                 | 273 ms: 1.27x faster                                                   |
| sympy_expand             | 566 ms                                                 | 455 ms: 1.24x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 833 us: 1.18x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 85.4 ms: 1.16x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.1 ms: 1.15x faster                                                  |
| json_loads               | 31.2 us                                                | 27.8 us: 1.12x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.3 ms: 1.12x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                  |
| json                     | 5.69 ms                                                | 5.15 ms: 1.10x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 105 ms: 1.10x faster                                                   |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.80 us: 1.08x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.07x faster                                                   |
| mdp                      | 2.85 sec                                               | 2.68 sec: 1.06x faster                                                 |
| unpickle_list            | 5.20 us                                                | 5.05 us: 1.03x faster                                                  |
| regex_dna                | 227 ms                                                 | 220 ms: 1.03x faster                                                   |
| pickle_list              | 5.08 us                                                | 4.98 us: 1.02x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                   |
| gc_traversal             | 3.62 ms                                                | 3.61 ms: 1.00x faster                                                  |
| unpickle                 | 14.4 us                                                | 14.8 us: 1.03x slower                                                  |
| pickle                   | 10.7 us                                                | 11.1 us: 1.04x slower                                                  |
| pickle_dict              | 29.6 us                                                | 33.1 us: 1.12x slower                                                  |
| telco                    | 7.27 ms                                                | 8.27 ms: 1.14x slower                                                  |
| pidigits                 | 191 ms                                                 | 226 ms: 1.18x slower                                                   |
| coverage                 | 79.4 ms                                                | 93.9 ms: 1.18x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.95 ms: 1.51x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.35x faster                                                           |

Benchmark hidden because not significant (4): mypy2, bench_mp_pool, async_generators, regex_effbot
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20231220-3.13.0a2+-344a5aa/bm-20231220-linux-x86_64-mdboom-mdboom_compact_int_s-3.13.0a2+-344a5aa.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.32x
- 95% likely to have a speedup of 1.30x
- 99% likely to have a speedup of 1.28x


# Memory

- memory change: 1.05x