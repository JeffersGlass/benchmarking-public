# Results vs. 3.10.4

- fork: python
- ref: e2a3e4b7488aff6fdc70
- machine: linux-x86_64
- commit hash: e2a3e4b
- commit date: 2024-02-28
- overall geometric mean: 1.37x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 261 ms: 1.33x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.82 ms: 1.42x faster                                                  |
| docutils       | 3.30 sec                                               | 2.56 sec: 1.29x faster                                                 |
| tornado_http   | 136 ms                                                 | 94.7 ms: 1.44x faster                                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 431 ms: 1.69x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 555 ms: 1.57x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 699 ms: 1.45x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.56x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 86.5 ms: 1.77x faster                                                  |
| float          | 117 ms                                                 | 79.0 ms: 1.48x faster                                                  |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.39x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.44x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                  |
| regex_dna      | 227 ms                                                 | 219 ms: 1.04x faster                                                   |
| regex_effbot   | 3.63 ms                                                | 3.73 ms: 1.03x slower                                                  |
| Geometric mean | (ref)                                                  | 1.13x faster                                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 292 us: 1.66x faster                                                   |
| unpickle_pure_python | 331 us                                                 | 212 us: 1.56x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 57.8 ms: 1.37x faster                                                  |
| xml_etree_generate   | 99.4 ms                                                | 84.7 ms: 1.17x faster                                                  |
| json_loads           | 31.2 us                                                | 27.1 us: 1.15x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.92 us: 1.06x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| unpickle             | 14.4 us                                                | 15.6 us: 1.09x slower                                                  |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.1 us: 1.19x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 8.81 ms: 1.49x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.0 ms: 1.48x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.93x faster                                                   |
| generators               | 80.1 ms                                                | 29.4 ms: 2.72x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.15 ms: 2.51x faster                                                  |
| logging_silent           | 190 ns                                                 | 95.1 ns: 1.99x faster                                                  |
| raytrace                 | 507 ms                                                 | 260 ms: 1.95x faster                                                   |
| chaos                    | 115 ms                                                 | 59.8 ms: 1.93x faster                                                  |
| asyncio_tcp              | 922 ms                                                 | 483 ms: 1.91x faster                                                   |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.84x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 69.9 ms: 1.83x faster                                                  |
| comprehensions           | 28.8 us                                                | 16.1 us: 1.79x faster                                                  |
| nbody                    | 154 ms                                                 | 86.5 ms: 1.77x faster                                                  |
| go                       | 240 ms                                                 | 135 ms: 1.77x faster                                                   |
| hexiom                   | 10.4 ms                                                | 5.86 ms: 1.77x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.8 ms: 1.76x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 67.5 ms: 1.75x faster                                                  |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.74x faster                                                  |
| async_tree_none          | 728 ms                                                 | 431 ms: 1.69x faster                                                   |
| richards                 | 79.3 ms                                                | 47.5 ms: 1.67x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 292 us: 1.66x faster                                                   |
| sqlglot_transpile        | 2.57 ms                                                | 1.56 ms: 1.65x faster                                                  |
| pyflate                  | 716 ms                                                 | 442 ms: 1.62x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.58x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 555 ms: 1.57x faster                                                   |
| spectral_norm            | 170 ms                                                 | 109 ms: 1.56x faster                                                   |
| unpickle_pure_python     | 331 us                                                 | 212 us: 1.56x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 37.5 us: 1.56x faster                                                  |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                   |
| async_tree_io            | 1.77 sec                                               | 1.16 sec: 1.52x faster                                                 |
| mako                     | 16.3 ms                                                | 11.0 ms: 1.48x faster                                                  |
| float                    | 117 ms                                                 | 79.0 ms: 1.48x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.64 us: 1.47x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.15 sec: 1.46x faster                                                 |
| logging_format           | 9.09 us                                                | 6.24 us: 1.46x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 699 ms: 1.45x faster                                                   |
| regex_compile            | 188 ms                                                 | 131 ms: 1.44x faster                                                   |
| tornado_http             | 136 ms                                                 | 94.7 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.79 sec: 1.44x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.43x faster                                                  |
| pprint_pformat           | 2.10 sec                                               | 1.47 sec: 1.43x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 715 ms: 1.42x faster                                                   |
| chameleon                | 9.68 ms                                                | 6.82 ms: 1.42x faster                                                  |
| fannkuch                 | 532 ms                                                 | 376 ms: 1.41x faster                                                   |
| unpack_sequence          | 60.0 ns                                                | 42.5 ns: 1.41x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.60 ms: 1.41x faster                                                  |
| deepcopy                 | 479 us                                                 | 347 us: 1.38x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.15 sec: 1.38x faster                                                 |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.04 us: 1.37x faster                                                  |
| xml_etree_process        | 79.1 ms                                                | 57.8 ms: 1.37x faster                                                  |
| sqlglot_normalize        | 143 ms                                                 | 104 ms: 1.37x faster                                                   |
| nqueens                  | 106 ms                                                 | 77.5 ms: 1.36x faster                                                  |
| sympy_sum                | 196 ms                                                 | 147 ms: 1.34x faster                                                   |
| 2to3                     | 348 ms                                                 | 261 ms: 1.33x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 19.4 ms: 1.33x faster                                                  |
| scimark_fft              | 466 ms                                                 | 353 ms: 1.32x faster                                                   |
| sqlglot_optimize         | 69.2 ms                                                | 52.8 ms: 1.31x faster                                                  |
| sympy_str                | 346 ms                                                 | 266 ms: 1.30x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 65.0 ms: 1.30x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.56 sec: 1.29x faster                                                 |
| sympy_expand             | 566 ms                                                 | 452 ms: 1.25x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 814 us: 1.21x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 84.7 ms: 1.17x faster                                                  |
| json_loads               | 31.2 us                                                | 27.1 us: 1.15x faster                                                  |
| json                     | 5.69 ms                                                | 4.96 ms: 1.15x faster                                                  |
| pathlib                  | 20.5 ms                                                | 17.9 ms: 1.14x faster                                                  |
| meteor_contest           | 120 ms                                                 | 105 ms: 1.14x faster                                                   |
| regex_v8                 | 27.8 ms                                                | 24.8 ms: 1.12x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 104 ms: 1.11x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.48 ms: 1.09x faster                                                  |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.08x faster                                                   |
| sqlite_synth             | 3.02 us                                                | 2.83 us: 1.07x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.68 sec: 1.06x faster                                                 |
| unpickle_list            | 5.20 us                                                | 4.92 us: 1.06x faster                                                  |
| regex_dna                | 227 ms                                                 | 219 ms: 1.04x faster                                                   |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                   |
| regex_effbot             | 3.63 ms                                                | 3.73 ms: 1.03x slower                                                  |
| pickle_list              | 5.08 us                                                | 5.29 us: 1.04x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.6 us: 1.09x slower                                                  |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 4.00 ms: 1.10x slower                                                  |
| telco                    | 7.27 ms                                                | 8.34 ms: 1.15x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.1 us: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 95.2 ms: 1.20x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 8.81 ms: 1.49x slower                                                  |
| Geometric mean           | (ref)                                                  | 1.37x faster                                                           |

Benchmark hidden because not significant (4): mypy2, bench_mp_pool, asyncio_websockets, async_generators
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240228-3.13.0a4+-e2a3e4b/bm-20240228-linux-x86_64-python-e2a3e4b7488aff6fdc70-3.13.0a4+-e2a3e4b.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.34x
- 95% likely to have a speedup of 1.33x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.06x