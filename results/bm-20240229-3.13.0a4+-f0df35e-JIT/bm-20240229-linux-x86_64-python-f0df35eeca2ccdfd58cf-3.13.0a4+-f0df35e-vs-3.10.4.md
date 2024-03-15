# Results vs. 3.10.4

- fork: python
- ref: f0df35eeca2ccdfd58cf
- machine: linux-x86_64
- commit hash: f0df35e
- commit date: 2024-02-29
- overall geometric mean: 1.29x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.22x faster
- Memory change: 1.34x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 280 ms: 1.25x faster                                                   |
| chameleon      | 9.68 ms                                                | 6.77 ms: 1.43x faster                                                  |
| docutils       | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| tornado_http   | 136 ms                                                 | 97.0 ms: 1.41x faster                                                  |
| Geometric mean | (ref)                                                  | 1.32x faster                                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 439 ms: 1.66x faster                                                   |
| async_tree_memoization  | 870 ms                                                 | 566 ms: 1.54x faster                                                   |
| async_tree_io           | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                 |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 712 ms: 1.43x faster                                                   |
| Geometric mean          | (ref)                                                  | 1.52x faster                                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 95.0 ms: 1.62x faster                                                  |
| float          | 117 ms                                                 | 81.5 ms: 1.44x faster                                                  |
| pidigits       | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| Geometric mean | (ref)                                                  | 1.33x faster                                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 151 ms: 1.25x faster                                                   |
| regex_v8       | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                  |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                   |
| Geometric mean | (ref)                                                  | 1.09x faster                                                           |

Benchmark hidden because not significant (1): regex_effbot

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|----------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 305 us: 1.59x faster                                                   |
| tomli_loads          | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| xml_etree_process    | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 245 us: 1.35x faster                                                   |
| xml_etree_generate   | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| json_loads           | 31.2 us                                                | 27.3 us: 1.14x faster                                                  |
| xml_etree_iterparse  | 115 ms                                                 | 108 ms: 1.07x faster                                                   |
| xml_etree_parse      | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| unpickle_list        | 5.20 us                                                | 4.94 us: 1.05x faster                                                  |
| pickle_list          | 5.08 us                                                | 5.26 us: 1.04x slower                                                  |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| pickle               | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| pickle_dict          | 29.6 us                                                | 35.2 us: 1.19x slower                                                  |
| Geometric mean       | (ref)                                                  | 1.14x faster                                                           |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                  |
| python_startup_no_site | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                  |
| Geometric mean         | (ref)                                                  | 1.25x slower                                                           |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|-----------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.6 ms: 1.41x faster                                                  |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e |
|--------------------------|:------------------------------------------------------:|:----------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 110 us: 4.96x faster                                                   |
| generators               | 80.1 ms                                                | 29.1 ms: 2.75x faster                                                  |
| deltablue                | 7.91 ms                                                | 3.43 ms: 2.31x faster                                                  |
| logging_silent           | 190 ns                                                 | 100 ns: 1.90x faster                                                   |
| asyncio_tcp              | 922 ms                                                 | 487 ms: 1.89x faster                                                   |
| chaos                    | 115 ms                                                 | 64.0 ms: 1.80x faster                                                  |
| richards_super           | 94.7 ms                                                | 52.9 ms: 1.79x faster                                                  |
| raytrace                 | 507 ms                                                 | 293 ms: 1.73x faster                                                   |
| crypto_pyaes             | 128 ms                                                 | 74.9 ms: 1.71x faster                                                  |
| scimark_sor              | 220 ms                                                 | 129 ms: 1.71x faster                                                   |
| richards                 | 79.3 ms                                                | 47.3 ms: 1.68x faster                                                  |
| async_tree_none          | 728 ms                                                 | 439 ms: 1.66x faster                                                   |
| sqlglot_parse            | 2.17 ms                                                | 1.32 ms: 1.64x faster                                                  |
| nbody                    | 154 ms                                                 | 95.0 ms: 1.62x faster                                                  |
| comprehensions           | 28.8 us                                                | 18.0 us: 1.60x faster                                                  |
| pickle_pure_python       | 484 us                                                 | 305 us: 1.59x faster                                                   |
| coroutines               | 35.1 ms                                                | 22.3 ms: 1.57x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.66 ms: 1.55x faster                                                  |
| scimark_monte_carlo      | 118 ms                                                 | 76.2 ms: 1.55x faster                                                  |
| async_tree_memoization   | 870 ms                                                 | 566 ms: 1.54x faster                                                   |
| go                       | 240 ms                                                 | 158 ms: 1.52x faster                                                   |
| deepcopy_memo            | 58.5 us                                                | 39.4 us: 1.49x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.19 sec: 1.48x faster                                                 |
| logging_format           | 9.09 us                                                | 6.25 us: 1.45x faster                                                  |
| logging_simple           | 8.30 us                                                | 5.71 us: 1.45x faster                                                  |
| tomli_loads              | 3.14 sec                                               | 2.18 sec: 1.44x faster                                                 |
| float                    | 117 ms                                                 | 81.5 ms: 1.44x faster                                                  |
| chameleon                | 9.68 ms                                                | 6.77 ms: 1.43x faster                                                  |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 712 ms: 1.43x faster                                                   |
| spectral_norm            | 170 ms                                                 | 119 ms: 1.43x faster                                                   |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                                 |
| mako                     | 16.3 ms                                                | 11.6 ms: 1.41x faster                                                  |
| tornado_http             | 136 ms                                                 | 97.0 ms: 1.41x faster                                                  |
| pyflate                  | 716 ms                                                 | 513 ms: 1.40x faster                                                   |
| hexiom                   | 10.4 ms                                                | 7.53 ms: 1.38x faster                                                  |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.37x faster                                                  |
| deepcopy_reduce          | 4.17 us                                                | 3.05 us: 1.37x faster                                                  |
| deepcopy                 | 479 us                                                 | 352 us: 1.36x faster                                                   |
| xml_etree_process        | 79.1 ms                                                | 58.7 ms: 1.35x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 245 us: 1.35x faster                                                   |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.33x faster                                                   |
| scimark_lu               | 176 ms                                                 | 133 ms: 1.32x faster                                                   |
| scimark_fft              | 466 ms                                                 | 354 ms: 1.31x faster                                                   |
| pycparser                | 1.58 sec                                               | 1.22 sec: 1.30x faster                                                 |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 5.04 ms: 1.28x faster                                                  |
| pprint_safe_repr         | 1.02 sec                                               | 794 ms: 1.28x faster                                                   |
| pprint_pformat           | 2.10 sec                                               | 1.67 sec: 1.26x faster                                                 |
| fannkuch                 | 532 ms                                                 | 423 ms: 1.26x faster                                                   |
| regex_compile            | 188 ms                                                 | 151 ms: 1.25x faster                                                   |
| 2to3                     | 348 ms                                                 | 280 ms: 1.25x faster                                                   |
| sympy_sum                | 196 ms                                                 | 160 ms: 1.23x faster                                                   |
| sympy_integrate          | 25.8 ms                                                | 21.0 ms: 1.23x faster                                                  |
| sympy_str                | 346 ms                                                 | 284 ms: 1.22x faster                                                   |
| dulwich_log              | 84.3 ms                                                | 69.3 ms: 1.22x faster                                                  |
| sqlglot_optimize         | 69.2 ms                                                | 56.9 ms: 1.22x faster                                                  |
| docutils                 | 3.30 sec                                               | 2.72 sec: 1.21x faster                                                 |
| python_startup           | 14.6 ms                                                | 12.3 ms: 1.19x faster                                                  |
| sympy_expand             | 566 ms                                                 | 484 ms: 1.17x faster                                                   |
| bench_thread_pool        | 986 us                                                 | 850 us: 1.16x faster                                                   |
| xml_etree_generate       | 99.4 ms                                                | 86.2 ms: 1.15x faster                                                  |
| nqueens                  | 106 ms                                                 | 92.0 ms: 1.15x faster                                                  |
| json_loads               | 31.2 us                                                | 27.3 us: 1.14x faster                                                  |
| regex_v8                 | 27.8 ms                                                | 24.7 ms: 1.12x faster                                                  |
| json                     | 5.69 ms                                                | 5.08 ms: 1.12x faster                                                  |
| pathlib                  | 20.5 ms                                                | 18.6 ms: 1.10x faster                                                  |
| meteor_contest           | 120 ms                                                 | 110 ms: 1.09x faster                                                   |
| create_gc_cycles         | 1.62 ms                                                | 1.50 ms: 1.08x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                  |
| xml_etree_iterparse      | 115 ms                                                 | 108 ms: 1.07x faster                                                   |
| xml_etree_parse          | 168 ms                                                 | 158 ms: 1.06x faster                                                   |
| unpickle_list            | 5.20 us                                                | 4.94 us: 1.05x faster                                                  |
| mdp                      | 2.85 sec                                               | 2.76 sec: 1.03x faster                                                 |
| pidigits                 | 191 ms                                                 | 188 ms: 1.02x faster                                                   |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                   |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                   |
| pickle_list              | 5.08 us                                                | 5.26 us: 1.04x slower                                                  |
| gc_traversal             | 3.62 ms                                                | 3.77 ms: 1.04x slower                                                  |
| async_generators         | 444 ms                                                 | 462 ms: 1.04x slower                                                   |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                  |
| pickle                   | 10.7 us                                                | 11.6 us: 1.09x slower                                                  |
| bench_mp_pool            | 24.0 ms                                                | 28.0 ms: 1.16x slower                                                  |
| pickle_dict              | 29.6 us                                                | 35.2 us: 1.19x slower                                                  |
| telco                    | 7.27 ms                                                | 8.66 ms: 1.19x slower                                                  |
| coverage                 | 79.4 ms                                                | 96.3 ms: 1.21x slower                                                  |
| python_startup_no_site   | 5.93 ms                                                | 10.9 ms: 1.84x slower                                                  |
| unpack_sequence          | 60.0 ns                                                | 121 ns: 2.02x slower                                                   |
| Geometric mean           | (ref)                                                  | 1.29x faster                                                           |

Benchmark hidden because not significant (2): mypy2, regex_effbot
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240229-3.13.0a4+-f0df35e-JIT/bm-20240229-linux-x86_64-python-f0df35eeca2ccdfd58cf-3.13.0a4+-f0df35e.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.25x
- 95% likely to have a speedup of 1.24x
- 99% likely to have a speedup of 1.22x


# Memory

- memory change: 1.34x