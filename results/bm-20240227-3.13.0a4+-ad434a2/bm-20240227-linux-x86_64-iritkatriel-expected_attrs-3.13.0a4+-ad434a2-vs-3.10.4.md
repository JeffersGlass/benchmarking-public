
# Results vs. 3.10.4

- fork: iritkatriel
- ref: expected_attrs
- machine: linux-x86_64
- commit hash: ad434a2
- commit date: 2024-02-27
- overall geometric mean: 1.38x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.30x faster
- Memory change: 1.06x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 262 ms: 1.33x faster                                                  |
| chameleon      | 9.68 ms                                                | 6.64 ms: 1.46x faster                                                 |
| docutils       | 3.30 sec                                               | 2.57 sec: 1.28x faster                                                |
| tornado_http   | 136 ms                                                 | 94.6 ms: 1.44x faster                                                 |
| Geometric mean | (ref)                                                  | 1.38x faster                                                          |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|-------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 431 ms: 1.69x faster                                                  |
| async_tree_memoization  | 870 ms                                                 | 555 ms: 1.57x faster                                                  |
| async_tree_io           | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 702 ms: 1.45x faster                                                  |
| Geometric mean          | (ref)                                                  | 1.55x faster                                                          |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 88.2 ms: 1.74x faster                                                 |
| float          | 117 ms                                                 | 80.6 ms: 1.45x faster                                                 |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                  |
| Geometric mean | (ref)                                                  | 1.37x faster                                                          |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 131 ms: 1.44x faster                                                  |
| regex_v8       | 27.8 ms                                                | 26.3 ms: 1.05x faster                                                 |
| regex_dna      | 227 ms                                                 | 224 ms: 1.01x faster                                                  |
| regex_effbot   | 3.63 ms                                                | 3.81 ms: 1.05x slower                                                 |
| Geometric mean | (ref)                                                  | 1.10x faster                                                          |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|----------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 292 us: 1.66x faster                                                  |
| unpickle_pure_python | 331 us                                                 | 210 us: 1.58x faster                                                  |
| tomli_loads          | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                |
| xml_etree_process    | 79.1 ms                                                | 57.6 ms: 1.37x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                 |
| xml_etree_generate   | 99.4 ms                                                | 84.0 ms: 1.18x faster                                                 |
| json_loads           | 31.2 us                                                | 27.5 us: 1.13x faster                                                 |
| xml_etree_iterparse  | 115 ms                                                 | 103 ms: 1.12x faster                                                  |
| xml_etree_parse      | 168 ms                                                 | 156 ms: 1.07x faster                                                  |
| unpickle_list        | 5.20 us                                                | 4.90 us: 1.06x faster                                                 |
| pickle_list          | 5.08 us                                                | 4.82 us: 1.05x faster                                                 |
| unpickle             | 14.4 us                                                | 15.0 us: 1.04x slower                                                 |
| pickle               | 10.7 us                                                | 11.4 us: 1.07x slower                                                 |
| pickle_dict          | 29.6 us                                                | 33.6 us: 1.14x slower                                                 |
| Geometric mean       | (ref)                                                  | 1.18x faster                                                          |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                 |
| python_startup_no_site | 5.93 ms                                                | 8.76 ms: 1.48x slower                                                 |
| Geometric mean         | (ref)                                                  | 1.01x slower                                                          |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|-----------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                 |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2 |
|--------------------------|:------------------------------------------------------:|:---------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 109 us: 4.98x faster                                                  |
| generators               | 80.1 ms                                                | 28.7 ms: 2.79x faster                                                 |
| deltablue                | 7.91 ms                                                | 3.14 ms: 2.52x faster                                                 |
| chaos                    | 115 ms                                                 | 58.5 ms: 1.97x faster                                                 |
| raytrace                 | 507 ms                                                 | 257 ms: 1.97x faster                                                  |
| logging_silent           | 190 ns                                                 | 98.1 ns: 1.93x faster                                                 |
| asyncio_tcp              | 922 ms                                                 | 482 ms: 1.91x faster                                                  |
| scimark_sor              | 220 ms                                                 | 116 ms: 1.89x faster                                                  |
| crypto_pyaes             | 128 ms                                                 | 69.0 ms: 1.85x faster                                                 |
| scimark_monte_carlo      | 118 ms                                                 | 66.2 ms: 1.79x faster                                                 |
| go                       | 240 ms                                                 | 135 ms: 1.78x faster                                                  |
| richards_super           | 94.7 ms                                                | 53.2 ms: 1.78x faster                                                 |
| comprehensions           | 28.8 us                                                | 16.3 us: 1.77x faster                                                 |
| hexiom                   | 10.4 ms                                                | 5.89 ms: 1.76x faster                                                 |
| sqlglot_parse            | 2.17 ms                                                | 1.24 ms: 1.75x faster                                                 |
| nbody                    | 154 ms                                                 | 88.2 ms: 1.74x faster                                                 |
| async_tree_none          | 728 ms                                                 | 431 ms: 1.69x faster                                                  |
| richards                 | 79.3 ms                                                | 47.2 ms: 1.68x faster                                                 |
| pickle_pure_python       | 484 us                                                 | 292 us: 1.66x faster                                                  |
| sqlglot_transpile        | 2.57 ms                                                | 1.55 ms: 1.66x faster                                                 |
| pyflate                  | 716 ms                                                 | 439 ms: 1.63x faster                                                  |
| spectral_norm            | 170 ms                                                 | 105 ms: 1.62x faster                                                  |
| coroutines               | 35.1 ms                                                | 21.9 ms: 1.61x faster                                                 |
| scimark_lu               | 176 ms                                                 | 112 ms: 1.58x faster                                                  |
| unpickle_pure_python     | 331 us                                                 | 210 us: 1.58x faster                                                  |
| deepcopy_memo            | 58.5 us                                                | 37.3 us: 1.57x faster                                                 |
| async_tree_memoization   | 870 ms                                                 | 555 ms: 1.57x faster                                                  |
| async_tree_io            | 1.77 sec                                               | 1.17 sec: 1.51x faster                                                |
| mako                     | 16.3 ms                                                | 10.9 ms: 1.49x faster                                                 |
| tomli_loads              | 3.14 sec                                               | 2.14 sec: 1.47x faster                                                |
| chameleon                | 9.68 ms                                                | 6.64 ms: 1.46x faster                                                 |
| float                    | 117 ms                                                 | 80.6 ms: 1.45x faster                                                 |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 702 ms: 1.45x faster                                                  |
| regex_compile            | 188 ms                                                 | 131 ms: 1.44x faster                                                  |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.78 sec: 1.44x faster                                                |
| tornado_http             | 136 ms                                                 | 94.6 ms: 1.44x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.76 us: 1.44x faster                                                 |
| python_startup           | 14.6 ms                                                | 10.1 ms: 1.44x faster                                                 |
| pprint_pformat           | 2.10 sec                                               | 1.46 sec: 1.44x faster                                                |
| logging_format           | 9.09 us                                                | 6.35 us: 1.43x faster                                                 |
| pprint_safe_repr         | 1.02 sec                                               | 713 ms: 1.43x faster                                                  |
| fannkuch                 | 532 ms                                                 | 376 ms: 1.42x faster                                                  |
| deepcopy                 | 479 us                                                 | 341 us: 1.41x faster                                                  |
| unpack_sequence          | 60.0 ns                                                | 42.9 ns: 1.40x faster                                                 |
| deepcopy_reduce          | 4.17 us                                                | 3.01 us: 1.38x faster                                                 |
| xml_etree_process        | 79.1 ms                                                | 57.6 ms: 1.37x faster                                                 |
| sqlglot_normalize        | 143 ms                                                 | 105 ms: 1.36x faster                                                  |
| pycparser                | 1.58 sec                                               | 1.16 sec: 1.36x faster                                                |
| json_dumps               | 14.2 ms                                                | 10.5 ms: 1.35x faster                                                 |
| sympy_sum                | 196 ms                                                 | 146 ms: 1.34x faster                                                  |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.82 ms: 1.34x faster                                                 |
| sympy_integrate          | 25.8 ms                                                | 19.3 ms: 1.33x faster                                                 |
| 2to3                     | 348 ms                                                 | 262 ms: 1.33x faster                                                  |
| nqueens                  | 106 ms                                                 | 80.3 ms: 1.32x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 52.7 ms: 1.31x faster                                                 |
| sympy_str                | 346 ms                                                 | 264 ms: 1.31x faster                                                  |
| scimark_fft              | 466 ms                                                 | 357 ms: 1.31x faster                                                  |
| dulwich_log              | 84.3 ms                                                | 65.1 ms: 1.30x faster                                                 |
| docutils                 | 3.30 sec                                               | 2.57 sec: 1.28x faster                                                |
| sympy_expand             | 566 ms                                                 | 448 ms: 1.26x faster                                                  |
| bench_thread_pool        | 986 us                                                 | 813 us: 1.21x faster                                                  |
| xml_etree_generate       | 99.4 ms                                                | 84.0 ms: 1.18x faster                                                 |
| pathlib                  | 20.5 ms                                                | 17.9 ms: 1.14x faster                                                 |
| json_loads               | 31.2 us                                                | 27.5 us: 1.13x faster                                                 |
| mdp                      | 2.85 sec                                               | 2.53 sec: 1.13x faster                                                |
| meteor_contest           | 120 ms                                                 | 106 ms: 1.13x faster                                                  |
| json                     | 5.69 ms                                                | 5.08 ms: 1.12x faster                                                 |
| xml_etree_iterparse      | 115 ms                                                 | 103 ms: 1.12x faster                                                  |
| create_gc_cycles         | 1.62 ms                                                | 1.49 ms: 1.09x faster                                                 |
| xml_etree_parse          | 168 ms                                                 | 156 ms: 1.07x faster                                                  |
| sqlite_synth             | 3.02 us                                                | 2.84 us: 1.06x faster                                                 |
| unpickle_list            | 5.20 us                                                | 4.90 us: 1.06x faster                                                 |
| regex_v8                 | 27.8 ms                                                | 26.3 ms: 1.05x faster                                                 |
| pickle_list              | 5.08 us                                                | 4.82 us: 1.05x faster                                                 |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                  |
| asyncio_websockets       | 559 ms                                                 | 551 ms: 1.01x faster                                                  |
| regex_dna                | 227 ms                                                 | 224 ms: 1.01x faster                                                  |
| async_generators         | 444 ms                                                 | 448 ms: 1.01x slower                                                  |
| unpickle                 | 14.4 us                                                | 15.0 us: 1.04x slower                                                 |
| regex_effbot             | 3.63 ms                                                | 3.81 ms: 1.05x slower                                                 |
| gc_traversal             | 3.62 ms                                                | 3.84 ms: 1.06x slower                                                 |
| pickle                   | 10.7 us                                                | 11.4 us: 1.07x slower                                                 |
| telco                    | 7.27 ms                                                | 8.25 ms: 1.14x slower                                                 |
| pickle_dict              | 29.6 us                                                | 33.6 us: 1.14x slower                                                 |
| coverage                 | 79.4 ms                                                | 95.2 ms: 1.20x slower                                                 |
| python_startup_no_site   | 5.93 ms                                                | 8.76 ms: 1.48x slower                                                 |
| Geometric mean           | (ref)                                                  | 1.38x faster                                                          |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (13) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, dask, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240227-3.13.0a4+-ad434a2/bm-20240227-linux-x86_64-iritkatriel-expected_attrs-3.13.0a4+-ad434a2.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.33x
- 95% likely to have a speedup of 1.32x
- 99% likely to have a speedup of 1.30x


# Memory

- memory change: 1.06x