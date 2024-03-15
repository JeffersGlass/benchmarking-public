
# Results vs. 3.10.4

- fork: brandtbucher
- ref: justin_relax
- machine: linux-x86_64
- commit hash: d5b3dec
- commit date: 2024-02-14
- overall geometric mean: 1.34x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.26x faster
- Memory change: 1.11x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| 2to3           | 348 ms                                                 | 270 ms: 1.29x faster                                                 |
| chameleon      | 9.68 ms                                                | 6.82 ms: 1.42x faster                                                |
| docutils       | 3.30 sec                                               | 2.63 sec: 1.26x faster                                               |
| tornado_http   | 136 ms                                                 | 95.6 ms: 1.43x faster                                                |
| Geometric mean | (ref)                                                  | 1.35x faster                                                         |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| async_tree_none         | 728 ms                                                 | 438 ms: 1.66x faster                                                 |
| async_tree_memoization  | 870 ms                                                 | 561 ms: 1.55x faster                                                 |
| async_tree_io           | 1.77 sec                                               | 1.18 sec: 1.50x faster                                               |
| async_tree_cpu_io_mixed | 1.02 sec                                               | 709 ms: 1.43x faster                                                 |
| Geometric mean          | (ref)                                                  | 1.53x faster                                                         |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| nbody          | 154 ms                                                 | 99.1 ms: 1.55x faster                                                |
| float          | 117 ms                                                 | 81.8 ms: 1.43x faster                                                |
| pidigits       | 191 ms                                                 | 187 ms: 1.02x faster                                                 |
| Geometric mean | (ref)                                                  | 1.31x faster                                                         |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| regex_compile  | 188 ms                                                 | 134 ms: 1.41x faster                                                 |
| regex_v8       | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                |
| regex_dna      | 227 ms                                                 | 231 ms: 1.02x slower                                                 |
| regex_effbot   | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                |
| Geometric mean | (ref)                                                  | 1.10x faster                                                         |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|----------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| pickle_pure_python   | 484 us                                                 | 293 us: 1.65x faster                                                 |
| tomli_loads          | 3.14 sec                                               | 2.05 sec: 1.53x faster                                               |
| unpickle_pure_python | 331 us                                                 | 219 us: 1.51x faster                                                 |
| json_dumps           | 14.2 ms                                                | 10.3 ms: 1.38x faster                                                |
| xml_etree_process    | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                |
| xml_etree_generate   | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                |
| json_loads           | 31.2 us                                                | 27.3 us: 1.14x faster                                                |
| xml_etree_iterparse  | 115 ms                                                 | 106 ms: 1.09x faster                                                 |
| xml_etree_parse      | 168 ms                                                 | 155 ms: 1.08x faster                                                 |
| unpickle_list        | 5.20 us                                                | 5.09 us: 1.02x faster                                                |
| pickle_list          | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| pickle               | 10.7 us                                                | 11.7 us: 1.10x slower                                                |
| unpickle             | 14.4 us                                                | 16.1 us: 1.12x slower                                                |
| pickle_dict          | 29.6 us                                                | 33.6 us: 1.13x slower                                                |
| Geometric mean       | (ref)                                                  | 1.16x faster                                                         |

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| python_startup         | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                |
| python_startup_no_site | 5.93 ms                                                | 8.80 ms: 1.48x slower                                                |
| Geometric mean         | (ref)                                                  | 1.02x slower                                                         |

Benchmarks with tag 'template':
===============================

| Benchmark | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|-----------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| mako      | 16.3 ms                                                | 11.3 ms: 1.45x faster                                                |

All benchmarks:
===============

| Benchmark                | bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120 | bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec |
|--------------------------|:------------------------------------------------------:|:--------------------------------------------------------------------:|
| typing_runtime_protocols | 544 us                                                 | 111 us: 4.90x faster                                                 |
| generators               | 80.1 ms                                                | 29.2 ms: 2.74x faster                                                |
| deltablue                | 7.91 ms                                                | 3.28 ms: 2.41x faster                                                |
| logging_silent           | 190 ns                                                 | 100 ns: 1.89x faster                                                 |
| raytrace                 | 507 ms                                                 | 269 ms: 1.88x faster                                                 |
| asyncio_tcp              | 922 ms                                                 | 491 ms: 1.88x faster                                                 |
| chaos                    | 115 ms                                                 | 62.5 ms: 1.85x faster                                                |
| scimark_sor              | 220 ms                                                 | 120 ms: 1.83x faster                                                 |
| richards_super           | 94.7 ms                                                | 53.2 ms: 1.78x faster                                                |
| crypto_pyaes             | 128 ms                                                 | 73.7 ms: 1.73x faster                                                |
| sqlglot_parse            | 2.17 ms                                                | 1.26 ms: 1.72x faster                                                |
| scimark_monte_carlo      | 118 ms                                                 | 69.7 ms: 1.70x faster                                                |
| richards                 | 79.3 ms                                                | 47.5 ms: 1.67x faster                                                |
| go                       | 240 ms                                                 | 144 ms: 1.66x faster                                                 |
| async_tree_none          | 728 ms                                                 | 438 ms: 1.66x faster                                                 |
| pickle_pure_python       | 484 us                                                 | 293 us: 1.65x faster                                                 |
| sqlglot_transpile        | 2.57 ms                                                | 1.58 ms: 1.62x faster                                                |
| comprehensions           | 28.8 us                                                | 18.1 us: 1.59x faster                                                |
| spectral_norm            | 170 ms                                                 | 108 ms: 1.57x faster                                                 |
| scimark_lu               | 176 ms                                                 | 113 ms: 1.55x faster                                                 |
| coroutines               | 35.1 ms                                                | 22.6 ms: 1.55x faster                                                |
| async_tree_memoization   | 870 ms                                                 | 561 ms: 1.55x faster                                                 |
| deepcopy_memo            | 58.5 us                                                | 37.7 us: 1.55x faster                                                |
| nbody                    | 154 ms                                                 | 99.1 ms: 1.55x faster                                                |
| tomli_loads              | 3.14 sec                                               | 2.05 sec: 1.53x faster                                               |
| hexiom                   | 10.4 ms                                                | 6.81 ms: 1.53x faster                                                |
| unpickle_pure_python     | 331 us                                                 | 219 us: 1.51x faster                                                 |
| logging_simple           | 8.30 us                                                | 5.53 us: 1.50x faster                                                |
| logging_format           | 9.09 us                                                | 6.06 us: 1.50x faster                                                |
| async_tree_io            | 1.77 sec                                               | 1.18 sec: 1.50x faster                                               |
| pyflate                  | 716 ms                                                 | 478 ms: 1.50x faster                                                 |
| mako                     | 16.3 ms                                                | 11.3 ms: 1.45x faster                                                |
| python_startup           | 14.6 ms                                                | 10.2 ms: 1.44x faster                                                |
| async_tree_cpu_io_mixed  | 1.02 sec                                               | 709 ms: 1.43x faster                                                 |
| float                    | 117 ms                                                 | 81.8 ms: 1.43x faster                                                |
| asyncio_tcp_ssl          | 2.57 sec                                               | 1.80 sec: 1.43x faster                                               |
| tornado_http             | 136 ms                                                 | 95.6 ms: 1.43x faster                                                |
| chameleon                | 9.68 ms                                                | 6.82 ms: 1.42x faster                                                |
| regex_compile            | 188 ms                                                 | 134 ms: 1.41x faster                                                 |
| deepcopy                 | 479 us                                                 | 341 us: 1.41x faster                                                 |
| deepcopy_reduce          | 4.17 us                                                | 2.98 us: 1.40x faster                                                |
| pprint_pformat           | 2.10 sec                                               | 1.50 sec: 1.40x faster                                               |
| pprint_safe_repr         | 1.02 sec                                               | 736 ms: 1.38x faster                                                 |
| json_dumps               | 14.2 ms                                                | 10.3 ms: 1.38x faster                                                |
| xml_etree_process        | 79.1 ms                                                | 58.5 ms: 1.35x faster                                                |
| scimark_sparse_mat_mult  | 6.47 ms                                                | 4.85 ms: 1.33x faster                                                |
| sqlglot_normalize        | 143 ms                                                 | 108 ms: 1.33x faster                                                 |
| pycparser                | 1.58 sec                                               | 1.19 sec: 1.32x faster                                               |
| fannkuch                 | 532 ms                                                 | 403 ms: 1.32x faster                                                 |
| scimark_fft              | 466 ms                                                 | 355 ms: 1.31x faster                                                 |
| unpack_sequence          | 60.0 ns                                                | 46.4 ns: 1.29x faster                                                |
| 2to3                     | 348 ms                                                 | 270 ms: 1.29x faster                                                 |
| sympy_sum                | 196 ms                                                 | 155 ms: 1.27x faster                                                 |
| sqlglot_optimize         | 69.2 ms                                                | 54.5 ms: 1.27x faster                                                |
| dulwich_log              | 84.3 ms                                                | 66.8 ms: 1.26x faster                                                |
| sympy_integrate          | 25.8 ms                                                | 20.5 ms: 1.26x faster                                                |
| docutils                 | 3.30 sec                                               | 2.63 sec: 1.26x faster                                               |
| sympy_str                | 346 ms                                                 | 276 ms: 1.25x faster                                                 |
| nqueens                  | 106 ms                                                 | 85.4 ms: 1.24x faster                                                |
| dask                     | 441 ms                                                 | 361 ms: 1.22x faster                                                 |
| sympy_expand             | 566 ms                                                 | 467 ms: 1.21x faster                                                 |
| bench_thread_pool        | 986 us                                                 | 835 us: 1.18x faster                                                 |
| xml_etree_generate       | 99.4 ms                                                | 85.7 ms: 1.16x faster                                                |
| json_loads               | 31.2 us                                                | 27.3 us: 1.14x faster                                                |
| json                     | 5.69 ms                                                | 5.00 ms: 1.14x faster                                                |
| meteor_contest           | 120 ms                                                 | 107 ms: 1.12x faster                                                 |
| pathlib                  | 20.5 ms                                                | 18.4 ms: 1.11x faster                                                |
| create_gc_cycles         | 1.62 ms                                                | 1.46 ms: 1.11x faster                                                |
| regex_v8                 | 27.8 ms                                                | 25.3 ms: 1.10x faster                                                |
| mdp                      | 2.85 sec                                               | 2.61 sec: 1.09x faster                                               |
| xml_etree_iterparse      | 115 ms                                                 | 106 ms: 1.09x faster                                                 |
| xml_etree_parse          | 168 ms                                                 | 155 ms: 1.08x faster                                                 |
| sqlite_synth             | 3.02 us                                                | 2.81 us: 1.08x faster                                                |
| gc_traversal             | 3.62 ms                                                | 3.50 ms: 1.04x faster                                                |
| unpickle_list            | 5.20 us                                                | 5.09 us: 1.02x faster                                                |
| pidigits                 | 191 ms                                                 | 187 ms: 1.02x faster                                                 |
| pickle_list              | 5.08 us                                                | 4.99 us: 1.02x faster                                                |
| asyncio_websockets       | 559 ms                                                 | 552 ms: 1.01x faster                                                 |
| regex_dna                | 227 ms                                                 | 231 ms: 1.02x slower                                                 |
| regex_effbot             | 3.63 ms                                                | 3.74 ms: 1.03x slower                                                |
| async_generators         | 444 ms                                                 | 460 ms: 1.04x slower                                                 |
| pickle                   | 10.7 us                                                | 11.7 us: 1.10x slower                                                |
| unpickle                 | 14.4 us                                                | 16.1 us: 1.12x slower                                                |
| pickle_dict              | 29.6 us                                                | 33.6 us: 1.13x slower                                                |
| telco                    | 7.27 ms                                                | 8.44 ms: 1.16x slower                                                |
| coverage                 | 79.4 ms                                                | 95.7 ms: 1.20x slower                                                |
| python_startup_no_site   | 5.93 ms                                                | 8.80 ms: 1.48x slower                                                |
| Geometric mean           | (ref)                                                  | 1.34x faster                                                         |

Benchmark hidden because not significant (2): mypy2, bench_mp_pool
Ignored benchmarks (12) of results/bm-20220323-3.10.4-9d38120/bm-20220323-linux-x86_64-python-v3.10.4-3.10.4-9d38120.json: aiohttp, django_template, djangocms, flaskblogging, genshi_text, genshi_xml, gunicorn, html5lib, pylint, sqlalchemy_declarative, sqlalchemy_imperative, thrift
Ignored benchmarks (4) of results/bm-20240214-3.13.0a3+-d5b3dec-JIT/bm-20240214-linux-x86_64-brandtbucher-justin_relax-3.13.0a3+-d5b3dec.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.29x
- 95% likely to have a speedup of 1.28x
- 99% likely to have a speedup of 1.26x


# Memory

- memory change: 1.11x