
# Results vs. 3.12.0

- fork: python
- ref: v3.11.5
- machine: linux-x86_64
- commit hash: cce6ba9
- commit date: 2023-08-24
- overall geometric mean: 1.02x faster \*
- HPT reliability: 100.00%
- HPT 99th percentile: 1.01x faster
- Memory change: 0.96x

Benchmarks with tag 'apps':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| 2to3           | 274 ms                                                 | 259 ms: 1.06x faster                                   |
| chameleon      | 7.41 ms                                                | 6.61 ms: 1.12x faster                                  |
| docutils       | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| tornado_http   | 103 ms                                                 | 96.7 ms: 1.06x faster                                  |
| Geometric mean | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'asyncio':
==============================

| Benchmark               | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_tree_cpu_io_mixed | 726 ms                                                 | 740 ms: 1.02x slower                                   |
| async_tree_memoization  | 578 ms                                                 | 641 ms: 1.11x slower                                   |
| async_tree_none         | 472 ms                                                 | 526 ms: 1.11x slower                                   |
| async_tree_io           | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| Geometric mean          | (ref)                                                  | 1.09x slower                                           |

Benchmarks with tag 'math':
===========================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| float          | 84.7 ms                                                | 77.0 ms: 1.10x faster                                  |
| nbody          | 97.0 ms                                                | 95.6 ms: 1.01x faster                                  |
| pidigits       | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| Geometric mean | (ref)                                                  | 1.03x faster                                           |

Benchmarks with tag 'regex':
============================

| Benchmark      | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| regex_effbot   | 3.61 ms                                                | 3.25 ms: 1.11x faster                                  |
| regex_compile  | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| regex_v8       | 23.1 ms                                                | 21.8 ms: 1.06x faster                                  |
| regex_dna      | 212 ms                                                 | 201 ms: 1.06x faster                                   |
| Geometric mean | (ref)                                                  | 1.08x faster                                           |

Benchmarks with tag 'serialize':
================================

| Benchmark            | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|----------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| pickle_list          | 5.08 us                                                | 4.12 us: 1.23x faster                                  |
| unpickle             | 15.9 us                                                | 13.3 us: 1.19x faster                                  |
| xml_etree_generate   | 89.2 ms                                                | 76.2 ms: 1.17x faster                                  |
| pickle               | 11.6 us                                                | 10.0 us: 1.16x faster                                  |
| xml_etree_process    | 61.7 ms                                                | 53.8 ms: 1.15x faster                                  |
| pickle_dict          | 35.5 us                                                | 31.0 us: 1.15x faster                                  |
| json_loads           | 28.5 us                                                | 25.9 us: 1.10x faster                                  |
| pickle_pure_python   | 324 us                                                 | 306 us: 1.06x faster                                   |
| unpickle_list        | 5.29 us                                                | 5.00 us: 1.06x faster                                  |
| tomli_loads          | 2.33 sec                                               | 2.22 sec: 1.05x faster                                 |
| xml_etree_iterparse  | 107 ms                                                 | 105 ms: 1.01x faster                                   |
| unpickle_pure_python | 230 us                                                 | 229 us: 1.01x faster                                   |
| json_dumps           | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| Geometric mean       | (ref)                                                  | 1.08x faster                                           |

Benchmark hidden because not significant (1): xml_etree_parse

Benchmarks with tag 'startup':
==============================

| Benchmark              | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| python_startup_no_site | 6.94 ms                                                | 6.04 ms: 1.15x faster                                  |
| python_startup         | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| Geometric mean         | (ref)                                                  | 1.13x faster                                           |

Benchmarks with tag 'template':
===============================

| Benchmark       | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|-----------------|:------------------------------------------------------:|:------------------------------------------------------:|
| mako            | 11.9 ms                                                | 9.99 ms: 1.19x faster                                  |
| django_template | 34.6 ms                                                | 32.6 ms: 1.06x faster                                  |
| Geometric mean  | (ref)                                                  | 1.12x faster                                           |

All benchmarks:
===============

| Benchmark                | bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0 | bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9 |
|--------------------------|:------------------------------------------------------:|:------------------------------------------------------:|
| async_generators         | 463 ms                                                 | 361 ms: 1.28x faster                                   |
| pickle_list              | 5.08 us                                                | 4.12 us: 1.23x faster                                  |
| unpack_sequence          | 54.0 ns                                                | 43.9 ns: 1.23x faster                                  |
| unpickle                 | 15.9 us                                                | 13.3 us: 1.19x faster                                  |
| mako                     | 11.9 ms                                                | 9.99 ms: 1.19x faster                                  |
| xml_etree_generate       | 89.2 ms                                                | 76.2 ms: 1.17x faster                                  |
| scimark_fft              | 382 ms                                                 | 329 ms: 1.16x faster                                   |
| pickle                   | 11.6 us                                                | 10.0 us: 1.16x faster                                  |
| pyflate                  | 482 ms                                                 | 419 ms: 1.15x faster                                   |
| python_startup_no_site   | 6.94 ms                                                | 6.04 ms: 1.15x faster                                  |
| xml_etree_process        | 61.7 ms                                                | 53.8 ms: 1.15x faster                                  |
| pickle_dict              | 35.5 us                                                | 31.0 us: 1.15x faster                                  |
| sqlite_synth             | 2.83 us                                                | 2.52 us: 1.12x faster                                  |
| chameleon                | 7.41 ms                                                | 6.61 ms: 1.12x faster                                  |
| deepcopy_reduce          | 3.35 us                                                | 2.99 us: 1.12x faster                                  |
| python_startup           | 9.55 ms                                                | 8.56 ms: 1.12x faster                                  |
| regex_effbot             | 3.61 ms                                                | 3.25 ms: 1.11x faster                                  |
| crypto_pyaes             | 81.9 ms                                                | 73.9 ms: 1.11x faster                                  |
| pprint_safe_repr         | 776 ms                                                 | 700 ms: 1.11x faster                                   |
| spectral_norm            | 115 ms                                                 | 104 ms: 1.10x faster                                   |
| logging_format           | 7.23 us                                                | 6.55 us: 1.10x faster                                  |
| scimark_sor              | 129 ms                                                 | 117 ms: 1.10x faster                                   |
| scimark_lu               | 118 ms                                                 | 107 ms: 1.10x faster                                   |
| json_loads               | 28.5 us                                                | 25.9 us: 1.10x faster                                  |
| float                    | 84.7 ms                                                | 77.0 ms: 1.10x faster                                  |
| deepcopy_memo            | 40.7 us                                                | 37.2 us: 1.09x faster                                  |
| scimark_monte_carlo      | 75.1 ms                                                | 68.8 ms: 1.09x faster                                  |
| json                     | 5.26 ms                                                | 4.83 ms: 1.09x faster                                  |
| fannkuch                 | 417 ms                                                 | 383 ms: 1.09x faster                                   |
| logging_simple           | 6.46 us                                                | 5.93 us: 1.09x faster                                  |
| regex_compile            | 148 ms                                                 | 136 ms: 1.09x faster                                   |
| pprint_pformat           | 1.57 sec                                               | 1.45 sec: 1.08x faster                                 |
| telco                    | 7.10 ms                                                | 6.60 ms: 1.08x faster                                  |
| dulwich_log              | 68.5 ms                                                | 63.8 ms: 1.07x faster                                  |
| scimark_sparse_mat_mult  | 5.06 ms                                                | 4.72 ms: 1.07x faster                                  |
| meteor_contest           | 112 ms                                                 | 105 ms: 1.07x faster                                   |
| pathlib                  | 19.3 ms                                                | 18.1 ms: 1.07x faster                                  |
| docutils                 | 2.77 sec                                               | 2.59 sec: 1.07x faster                                 |
| regex_v8                 | 23.1 ms                                                | 21.8 ms: 1.06x faster                                  |
| django_template          | 34.6 ms                                                | 32.6 ms: 1.06x faster                                  |
| tornado_http             | 103 ms                                                 | 96.7 ms: 1.06x faster                                  |
| 2to3                     | 274 ms                                                 | 259 ms: 1.06x faster                                   |
| logging_silent           | 104 ns                                                 | 98.6 ns: 1.06x faster                                  |
| pickle_pure_python       | 324 us                                                 | 306 us: 1.06x faster                                   |
| raytrace                 | 312 ms                                                 | 295 ms: 1.06x faster                                   |
| deepcopy                 | 371 us                                                 | 351 us: 1.06x faster                                   |
| unpickle_list            | 5.29 us                                                | 5.00 us: 1.06x faster                                  |
| regex_dna                | 212 ms                                                 | 201 ms: 1.06x faster                                   |
| sqlalchemy_declarative   | 147 ms                                                 | 140 ms: 1.05x faster                                   |
| tomli_loads              | 2.33 sec                                               | 2.22 sec: 1.05x faster                                 |
| sqlalchemy_imperative    | 18.7 ms                                                | 17.9 ms: 1.05x faster                                  |
| gc_traversal             | 3.79 ms                                                | 3.64 ms: 1.04x faster                                  |
| aiohttp                  | 1.15 ms                                                | 1.10 ms: 1.04x faster                                  |
| gunicorn                 | 1.24 ms                                                | 1.19 ms: 1.04x faster                                  |
| pycparser                | 1.18 sec                                               | 1.13 sec: 1.04x faster                                 |
| sqlglot_optimize         | 54.8 ms                                                | 53.0 ms: 1.03x faster                                  |
| dask                     | 372 ms                                                 | 360 ms: 1.03x faster                                   |
| sympy_str                | 300 ms                                                 | 291 ms: 1.03x faster                                   |
| bench_thread_pool        | 842 us                                                 | 818 us: 1.03x faster                                   |
| sympy_integrate          | 21.4 ms                                                | 21.1 ms: 1.02x faster                                  |
| sqlglot_normalize        | 110 ms                                                 | 108 ms: 1.02x faster                                   |
| mdp                      | 2.63 sec                                               | 2.59 sec: 1.02x faster                                 |
| xml_etree_iterparse      | 107 ms                                                 | 105 ms: 1.01x faster                                   |
| nbody                    | 97.0 ms                                                | 95.6 ms: 1.01x faster                                  |
| sympy_sum                | 169 ms                                                 | 167 ms: 1.01x faster                                   |
| deltablue                | 3.72 ms                                                | 3.69 ms: 1.01x faster                                  |
| unpickle_pure_python     | 230 us                                                 | 229 us: 1.01x faster                                   |
| hexiom                   | 6.41 ms                                                | 6.39 ms: 1.00x faster                                  |
| create_gc_cycles         | 1.48 ms                                                | 1.48 ms: 1.01x slower                                  |
| go                       | 139 ms                                                 | 141 ms: 1.01x slower                                   |
| sqlglot_parse            | 1.36 ms                                                | 1.37 ms: 1.01x slower                                  |
| nqueens                  | 83.3 ms                                                | 84.2 ms: 1.01x slower                                  |
| pidigits                 | 187 ms                                                 | 190 ms: 1.01x slower                                   |
| async_tree_cpu_io_mixed  | 726 ms                                                 | 740 ms: 1.02x slower                                   |
| chaos                    | 67.0 ms                                                | 68.5 ms: 1.02x slower                                  |
| richards                 | 45.8 ms                                                | 47.1 ms: 1.03x slower                                  |
| comprehensions           | 21.8 us                                                | 22.7 us: 1.04x slower                                  |
| coroutines               | 23.2 ms                                                | 25.4 ms: 1.10x slower                                  |
| async_tree_memoization   | 578 ms                                                 | 641 ms: 1.11x slower                                   |
| async_tree_none          | 472 ms                                                 | 526 ms: 1.11x slower                                   |
| async_tree_io            | 1.16 sec                                               | 1.30 sec: 1.13x slower                                 |
| richards_super           | 51.5 ms                                                | 58.3 ms: 1.13x slower                                  |
| json_dumps               | 10.4 ms                                                | 12.6 ms: 1.21x slower                                  |
| asyncio_tcp              | 491 ms                                                 | 864 ms: 1.76x slower                                   |
| asyncio_tcp_ssl          | 1.79 sec                                               | 3.18 sec: 1.78x slower                                 |
| generators               | 31.2 ms                                                | 73.8 ms: 2.36x slower                                  |
| typing_runtime_protocols | 158 us                                                 | 493 us: 3.12x slower                                   |
| Geometric mean           | (ref)                                                  | 1.02x faster                                           |

Benchmark hidden because not significant (4): sqlglot_transpile, xml_etree_parse, sympy_expand, bench_mp_pool
Ignored benchmarks (7) of results/bm-20231002-3.12.0-0fb18b0/bm-20231002-linux-x86_64-python-v3.12.0-3.12.0-0fb18b0.json: async_tree_cpu_io_mixed_tg, async_tree_io_tg, async_tree_memoization_tg, async_tree_none_tg, asyncio_websockets, coverage, mypy2
Ignored benchmarks (7) of results/bm-20230824-3.11.5-cce6ba9/bm-20230824-linux-x86_64-python-v3.11.5-3.11.5-cce6ba9.json: djangocms, flaskblogging, genshi_text, genshi_xml, html5lib, pylint, thrift


# HPT report

- Reliability score: 100.00% likely to be faster
- 90% likely to have a speedup of 1.02x
- 95% likely to have a speedup of 1.02x
- 99% likely to have a speedup of 1.01x


# Memory

- memory change: 0.96x